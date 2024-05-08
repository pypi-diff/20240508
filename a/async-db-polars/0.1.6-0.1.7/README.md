# Comparing `tmp/async_db_polars-0.1.6.tar.gz` & `tmp/async_db_polars-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_db_polars-0.1.6.tar", max compression
+gzip compressed data, was "async_db_polars-0.1.7.tar", max compression
```

## Comparing `async_db_polars-0.1.6.tar` & `async_db_polars-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       73 2024-01-03 01:48:08.386767 async_db_polars-0.1.6/README.md
--rw-r--r--   0        0        0     7693 2024-01-13 18:28:13.809815 async_db_polars-0.1.6/async_db_polars/db.py
--rw-r--r--   0        0        0     3742 2024-03-06 04:15:03.269311 async_db_polars-0.1.6/async_db_polars/pgdb.py
--rw-r--r--   0        0        0      548 2024-03-06 04:15:11.513344 async_db_polars-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 async_db_polars-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       73 2024-01-03 01:48:08.386767 async_db_polars-0.1.7/README.md
+-rw-r--r--   0        0        0     7693 2024-01-13 18:28:13.809815 async_db_polars-0.1.7/async_db_polars/db.py
+-rw-r--r--   0        0        0     4356 2024-05-05 14:46:08.222478 async_db_polars-0.1.7/async_db_polars/pgdb.py
+-rw-r--r--   0        0        0      484 2024-05-08 00:40:59.084772 async_db_polars-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 async_db_polars-0.1.7/PKG-INFO
```

### Comparing `async_db_polars-0.1.6/async_db_polars/db.py` & `async_db_polars-0.1.7/async_db_polars/db.py`

 * *Files identical despite different names*

### Comparing `async_db_polars-0.1.6/async_db_polars/pgdb.py` & `async_db_polars-0.1.7/async_db_polars/pgdb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import reduce
-from typing import Optional
+from typing import Awaitable, Callable, Optional
 
 import asyncpg
 import polars as pl
 from polars.type_aliases import SchemaDict
 
 from async_db_polars.db import DB
 
@@ -58,37 +58,50 @@
     str(pl.Utf8): "TEXT",
     str(pl.String): "TEXT",
 }
 
 
 def map_to_postgres_type(polars_type: str):
     try:
-        return filter(
-            lambda x: x[0] in polars_type, POLARS_TO_POSTGRES_TYPE_MAP.items()
-        ).__next__()[1]
+        return next(
+            filter(lambda x: x[0] in polars_type, POLARS_TO_POSTGRES_TYPE_MAP.items())
+        )[1]
     except StopIteration:
         raise ValueError(f"Polars type {polars_type} is not supported by Postgres.")
 
 
 class PGDB(DB):
-    pool: asyncpg.Pool
+    pool: Optional[asyncpg.Pool] = None
+    init_func: Optional[Callable[[], Awaitable[asyncpg.Pool]]] = None
 
-    def init(self, pool: asyncpg.Pool):
-        self.pool = pool
+    def __init__(
+        self,
+        pool_or_pool_factory: asyncpg.Pool | Callable[[], Awaitable[asyncpg.Pool]],
+    ):
+        if isinstance(pool_or_pool_factory, asyncpg.Pool):
+            self.pool = pool_or_pool_factory
+        else:
+            self.init_func = pool_or_pool_factory
+
+    async def close(self):
+        if self.pool is not None:
+            await self.pool.close()
 
     async def fetch(
         self,
         query: str,
         *,
         schema_overrides: Optional[SchemaDict] = None,
         timeout: Optional[float] = None,
         **kwargs,
     ):
-        numbered_args_query = kwargs_to_sql(query, **kwargs)
+        if self.pool is None:
+            self.pool = await self.init_func()  # type: ignore
 
+        numbered_args_query = kwargs_to_sql(query, **kwargs)
         res = await self.pool.fetch(
             numbered_args_query, *kwargs.values(), timeout=timeout
         )
         return res_to_df(res, schema_overrides)
 
     async def insert(
         self,
@@ -96,14 +109,17 @@
         table_name: str,
         *,
         pkey_cols: Optional[set[str]] = None,
         return_cols: Optional[set[str]] = None,
         return_schema_overrides: Optional[SchemaDict] = None,
         timeout: Optional[float] = None,
     ):
+        if self.pool is None:
+            self.pool = await self.init_func()  # type: ignore
+
         cols_sql = ", ".join(df.columns)
 
         placeholder_fillers = ", ".join(
             map(
                 lambda x: f"${x[0]}::{map_to_postgres_type(str(x[1][1]))}[]",
                 enumerate(df.schema.items(), 1),
             )
```

### Comparing `async_db_polars-0.1.6/PKG-INFO` & `async_db_polars-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: async-db-polars
-Version: 0.1.6
+Version: 0.1.7
 Summary: High level DB abstraction that uses polars to represent tables in memory.
 License: MIT
 Author: WolfEYc
 Author-email: wolfeycode@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: pg
-Requires-Dist: asyncpg (>=0.29.0,<0.30.0) ; extra == "pg"
+Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: polars (>=0.20.3,<0.21.0)
 Description-Content-Type: text/markdown
 
 High level DB abstraction that uses polars to represent tables in memory.
```

