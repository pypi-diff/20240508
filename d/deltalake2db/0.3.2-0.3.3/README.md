# Comparing `tmp/deltalake2db-0.3.2.tar.gz` & `tmp/deltalake2db-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltalake2db-0.3.2.tar", max compression
+gzip compressed data, was "deltalake2db-0.3.3.tar", max compression
```

## Comparing `deltalake2db-0.3.2.tar` & `deltalake2db-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2066 2024-04-17 07:37:40.689949 deltalake2db-0.3.2/README.md
--rw-r--r--   0        0        0      343 2024-04-17 07:37:40.689949 deltalake2db-0.3.2/deltalake2db/__init__.py
--rw-r--r--   0        0        0     1189 2024-04-17 07:37:40.689949 deltalake2db-0.3.2/deltalake2db/azure_helper.py
--rw-r--r--   0        0        0    15056 2024-04-17 07:37:40.693949 deltalake2db-0.3.2/deltalake2db/duckdb.py
--rw-r--r--   0        0        0      891 2024-04-17 07:37:40.693949 deltalake2db-0.3.2/deltalake2db/filter_by_meta.py
--rw-r--r--   0        0        0     7641 2024-04-17 07:37:40.693949 deltalake2db-0.3.2/deltalake2db/polars.py
--rw-r--r--   0        0        0      963 2024-04-17 07:37:40.693949 deltalake2db-0.3.2/deltalake2db/protocol_check.py
--rw-r--r--   0        0        0     2608 2024-04-17 07:37:40.693949 deltalake2db-0.3.2/deltalake2db/sql_utils.py
--rw-r--r--   0        0        0      784 2024-04-17 07:37:40.693949 deltalake2db-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2587 1970-01-01 00:00:00.000000 deltalake2db-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2066 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/README.md
+-rw-r--r--   0        0        0      343 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/__init__.py
+-rw-r--r--   0        0        0     1225 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/azure_helper.py
+-rw-r--r--   0        0        0    15196 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/duckdb.py
+-rw-r--r--   0        0        0      889 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/filter_by_meta.py
+-rw-r--r--   0        0        0     7614 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/polars.py
+-rw-r--r--   0        0        0      963 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/protocol_check.py
+-rw-r--r--   0        0        0     2666 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/deltalake2db/sql_utils.py
+-rw-r--r--   0        0        0      885 2024-05-08 13:34:51.098398 deltalake2db-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 deltalake2db-0.3.3/PKG-INFO
```

### Comparing `deltalake2db-0.3.2/README.md` & `deltalake2db-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.2/deltalake2db/azure_helper.py` & `deltalake2db-0.3.3/deltalake2db/azure_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-def apply_azure_chain(storage_options: dict | None):
+from typing import Optional
+
+
+def apply_azure_chain(storage_options: Optional[dict]):
     # support for "Chain" as in duckdb: https://duckdb.org/docs/extensions/azure#credential_chain-provider
     if storage_options is None:
         return None
     chain = storage_options.get("chain", None)
     if chain is not None:
         from azure.identity import (
             ChainedTokenCredential,
```

### Comparing `deltalake2db-0.3.2/deltalake2db/duckdb.py` & `deltalake2db-0.3.3/deltalake2db/duckdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from collections.abc import Sequence
-import os
 from pathlib import Path
-from typing import TYPE_CHECKING, Callable
+from typing import TYPE_CHECKING, Callable, Optional, Union
 from deltalake import DataType, Field
 from deltalake.schema import StructType, ArrayType, PrimitiveType, MapType
 import sqlglot.expressions as ex
 from deltalake2db.azure_helper import apply_azure_chain
 from deltalake2db.filter_by_meta import _can_filter
 import deltalake2db.sql_utils as squ
 
 if TYPE_CHECKING:
     from deltalake import DeltaTable
     import duckdb
 
 
-def _cast(s: ex.Expression, t: ex.DataType.Type | None):
+def _cast(s: ex.Expression, t: Optional[ex.DataType.Type]):
     if t is None:
         return s
     return ex.cast(s, t)
 
 
 def _dummy_expr(
     field_type: "PrimitiveType | StructType | ArrayType | MapType",
@@ -52,15 +51,15 @@
         )
     raise ValueError(f"Unsupported type {field_type}")
 
 
 def _get_expr(
     base_expr: "ex.Expression|None",
     dtype: "DataType",
-    meta: Field | None,
+    meta: Optional[Field],
     alias=True,
     *,
     counter: int = 0,
 ) -> "ex.Expression":
     pn = (
         meta.metadata.get("delta.columnMapping.physicalName", meta.name)
         if meta
@@ -97,15 +96,14 @@
                 )
             )
         )
         if alias and meta is not None:
             return struct_expr.as_(meta.name)
         return struct_expr
     elif isinstance(dtype, ArrayType):
-
         vl = squ.list_transform(
             "x_" + str(counter),
             base_expr,
             _get_expr(
                 ex.Identifier(this="x_" + str(counter), quoted=False),
                 dtype.element_type,
                 meta=meta,
@@ -117,15 +115,14 @@
             return vl.as_(meta.name)
         return vl
 
     return base_expr.as_(meta.name) if meta is not None and alias else base_expr
 
 
 def load_install_azure(con: "duckdb.DuckDBPyConnection"):
-
     with con.cursor() as cur:
         cur.execute(
             "select loaded, installed from duckdb_extensions() where extension_name='azure' "
         )
         res = cur.fetchone()
         loaded = res[0] if res else False
         installed = res[0] if res else False
@@ -232,20 +229,20 @@
     "timestampNtz": ex.DataType.Type.TIMESTAMP,
     "decimal": ex.DataType.Type.DECIMAL,
 }
 
 
 def create_view_for_delta(
     con: "duckdb.DuckDBPyConnection",
-    delta_table: "DeltaTable | Path | str",
+    delta_table: "Union[DeltaTable , Path , str]",
     view_name: str,
     overwrite=True,
     *,
-    conditions: dict | None = None,
-    storage_options: dict | None = None,
+    conditions: Optional[dict] = None,
+    storage_options: Optional[dict] = None,
 ):
     sql = get_sql_for_delta(
         delta_table,
         duck_con=con,
         conditions=conditions,
         storage_options=storage_options,
     )
@@ -253,24 +250,24 @@
     if overwrite:
         con.execute(f'create or replace view "{view_name}" as {sql}')
     else:
         con.execute(f'create view "{view_name}" as {sql}')
 
 
 def get_sql_for_delta_expr(
-    dt: "DeltaTable | Path | str",
-    conditions: dict | None | Sequence[ex.Expression] | ex.Expression = None,
-    select: Sequence[str | ex.Expression] | None = None,
+    dt: "Union[DeltaTable,Path , str]",
+    conditions: Union[Optional[dict], Sequence[ex.Expression], ex.Expression] = None,
+    select: Union[Sequence[Union[str, ex.Expression]], None] = None,
     distinct=False,
-    cte_wrap_name: str | None = None,
-    action_filter: Callable[[dict], bool] | None = None,
+    cte_wrap_name: Union[str, None] = None,
+    action_filter: Union[Callable[[dict], bool], None] = None,
     sql_prefix="delta",
-    delta_table_cte_name: str | None = None,
-    duck_con: "duckdb.DuckDBPyConnection | None" = None,
-    storage_options: dict | None = None,
+    delta_table_cte_name: Union[str, None] = None,
+    duck_con: "Union[duckdb.DuckDBPyConnection, None]" = None,
+    storage_options: Optional[dict] = None,
 ) -> ex.Select:
     from .sql_utils import read_parquet, union, filter_via_dict
 
     if isinstance(dt, Path) or isinstance(dt, str):
         from deltalake import DeltaTable
 
         storage_options_for_delta = apply_azure_chain(storage_options)
@@ -289,18 +286,19 @@
     owns_con = False
     if duck_con is None:
         import duckdb
 
         duck_con = duckdb.connect()
         owns_con = True
     if dt.table_uri.startswith("az://") or dt.table_uri.startswith("abfss://"):
-        apply_storage_options(duck_con, storage_options or dt._storage_options, type="azure")  # type: ignore
+        apply_storage_options(
+            duck_con, storage_options or dt._storage_options or {}, type="azure"
+        )  # type: ignore
 
     try:
-
         for ac in dt.get_add_actions(flatten=True).to_pylist():
             if (
                 conditions is not None
                 and isinstance(conditions, dict)
                 and _can_filter(ac, conditions)
             ):
                 continue
@@ -341,15 +339,14 @@
                 elif "partition." + field.name in ac:
                     cols_sql.append(
                         _cast(ex.convert(ac["partition." + field.name]), cast_as).as_(
                             field_name
                         )
                     )
                 elif phys_name in cols:
-
                     cols_sql.append(
                         _get_expr(ex.column(phys_name, quoted=True), field.type, field)
                     )
                 else:
                     cols_sql.append(ex.Null().as_(field_name))
 
             select_pq = ex.select(*cols_sql).from_(
@@ -392,23 +389,23 @@
             return se
     finally:
         if owns_con:
             duck_con.close()
 
 
 def get_sql_for_delta(
-    dt: "DeltaTable | Path",
-    conditions: dict | None = None,
-    select: list[str] | None = None,
+    dt: "Union[DeltaTable, Path, str]",
+    conditions: Optional[dict] = None,
+    select: Union[list[str], None] = None,
     distinct=False,
-    action_filter: Callable[[dict], bool] | None = None,
-    cte_wrap_name: str | None = None,
+    action_filter: Union[Callable[[dict], bool], None] = None,
+    cte_wrap_name: Union[str, None] = None,
     sql_prefix="delta",
-    duck_con: "duckdb.DuckDBPyConnection | None" = None,
-    storage_options: dict | None = None,
+    duck_con: "Union[duckdb.DuckDBPyConnection, None]" = None,
+    storage_options: Optional[dict] = None,
 ) -> str:
     expr = get_sql_for_delta_expr(
         dt=dt,
         conditions=conditions,
         select=select,
         distinct=distinct,
         action_filter=action_filter,
```

### Comparing `deltalake2db-0.3.2/deltalake2db/filter_by_meta.py` & `deltalake2db-0.3.3/deltalake2db/filter_by_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 
 def _can_filter(action: dict, conditions: dict):
     # partition.COLNAME
     # min.COLNAME
     # max.COLNAME
     try:
-
         for key, value in conditions.items():
             part_vl = action.get("partition." + key, None)
             if part_vl is not None and part_vl != value:
                 return True
             min_vl = action.get("min." + key, None)
             max_vl = action.get("max." + key, None)
             if isinstance(min_vl, str):
```

### Comparing `deltalake2db-0.3.2/deltalake2db/polars.py` & `deltalake2db-0.3.3/deltalake2db/polars.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from pathlib import Path
-from typing import TYPE_CHECKING, cast
+from typing import TYPE_CHECKING, cast, Union, Optional
 
 from deltalake2db.azure_helper import apply_azure_chain
 from deltalake2db.filter_by_meta import _can_filter
 
 if TYPE_CHECKING:
     import polars as pl
 from deltalake import DeltaTable, Field, DataType
-from deltalake.exceptions import DeltaProtocolError
-from deltalake.schema import StructType, ArrayType, PrimitiveType, MapType
+from deltalake.schema import StructType, ArrayType, MapType
 import os
 
 
 def _get_expr(
-    base_expr: "pl.Expr|None",
+    base_expr: "Union[pl.Expr,None]",
     dtype: "DataType",
-    meta: Field | None,
-    parquet_field: "pl.PolarsDataType | None",
+    meta: Optional[Field],
+    parquet_field: "Optional[pl.PolarsDataType]",
 ) -> "pl.Expr":
     import polars as pl
 
     if parquet_field is None:
         return (
             pl.lit(None, _get_type(dtype)).alias(meta.name)
             if meta
@@ -134,17 +133,17 @@
 
 
 def _filter_cond(f: "pl.LazyFrame", conditions: dict) -> "pl.LazyFrame":
     return f.filter(**conditions)
 
 
 def scan_delta_union(
-    delta_table: DeltaTable | Path | str,
-    conditions: dict | None = None,
-    storage_options: dict | None = None,
+    delta_table: Union[DeltaTable, Path, str],
+    conditions: Optional[dict] = None,
+    storage_options: Optional[dict] = None,
 ) -> "pl.LazyFrame":
     import polars as pl
     from .protocol_check import check_is_supported
 
     if isinstance(delta_table, Path) or isinstance(delta_table, str):
         storage_options_for_delta = apply_azure_chain(storage_options)
         delta_table = DeltaTable(delta_table, storage_options=storage_options_for_delta)
```

### Comparing `deltalake2db-0.3.2/deltalake2db/protocol_check.py` & `deltalake2db-0.3.3/deltalake2db/protocol_check.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.2/deltalake2db/sql_utils.py` & `deltalake2db-0.3.3/deltalake2db/sql_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
-from typing import Sequence, Any, TypeVar
+from typing import Optional, Sequence, Any, TypeVar
 import sqlglot.expressions as ex
+from typing import Union
 
 
 def read_parquet(
-    path: str | Path | list[Path] | list[str] | ex.Expression | list[ex.Expression],
+    path: Union[str, Path, list[Path], list[str], ex.Expression, list[ex.Expression]],
 ) -> ex.Expression:
     if isinstance(path, list):
         return ex.func(
             "read_parquet",
             ex.array(
                 *[
                     ex.Literal.string(str(p)) if isinstance(p, (str, Path)) else p
@@ -35,15 +36,15 @@
         return ex.union(selects[0], selects[1], distinct=distinct)
     else:
         return ex.union(
             selects[0], union(selects[1:], distinct=distinct), distinct=distinct
         )
 
 
-def filter_via_dict(conditions: dict[str, Any] | None):
+def filter_via_dict(conditions: Optional[dict[str, Any]]):
     if not conditions or len(conditions) == 0:
         return None
     return [
         (
             ex.EQ(this=ex.column(k, quoted=True), expression=ex.convert(v))
             if v is not None
             else ex.Is(this=ex.column(k, quoted=True), expression=ex.Null())
@@ -68,15 +69,17 @@
             ex.PropertyEQ(this=ex.Identifier(this=k, quoted=True), expression=v)
             for k, v in items.items()
         ]
     )
 
 
 def list_transform(
-    param_names: list[str] | str, list_expr: ex.Expression, value_expr: ex.Expression
+    param_names: Union[list[str], str],
+    list_expr: ex.Expression,
+    value_expr: ex.Expression,
 ) -> ex.Expression:
     if isinstance(param_names, str):
         param_names = [param_names]
     return ex.func(
         "list_transform",
         list_expr,
         ex.Lambda(
```

### Comparing `deltalake2db-0.3.2/pyproject.toml` & `deltalake2db-0.3.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 [tool.poetry]
 name = "deltalake2db"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 deltalake = ">=0.16.1"
 sqlglot = ">=22.2.1"
 azure-identity = { version = "^1.16.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.352"
-black = "^24.2.0"
 polars = "^0.20.16"
 duckdb = "^0.10.1"
+ruff = "^0.4.3"
 
 [tool.poetry.group.test.dependencies]
 pytest-cov = "^4.1.0"
 pytest = "^8.1.0"
 polars = "^0.20.13"
 duckdb = "^0.10.0"
 docker = "^7.0.0"
 azure-storage-blob = "^12.19.1"
 python-dotenv = "^1.0.1"
-pandas = "^2.2.1"
+pandas = ">=1.4.2"
 azure-identity = "^1.16.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+
+[tool.pyright]
+venv = ".venv"
+venvPath = "."
+pythonVersion = "3.9"
+typeCheckingMode = "basic"
```

### Comparing `deltalake2db-0.3.2/PKG-INFO` & `deltalake2db-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: deltalake2db
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: azure-identity (>=1.16.0,<2.0.0)
 Requires-Dist: deltalake (>=0.16.1)
 Requires-Dist: sqlglot (>=22.2.1)
 Description-Content-Type: text/markdown
```

