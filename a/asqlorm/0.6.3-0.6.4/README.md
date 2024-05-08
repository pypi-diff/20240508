# Comparing `tmp/asqlorm-0.6.3.tar.gz` & `tmp/asqlorm-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asqlorm-0.6.3.tar", max compression
+gzip compressed data, was "asqlorm-0.6.4.tar", max compression
```

## Comparing `asqlorm-0.6.3.tar` & `asqlorm-0.6.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.3/README.md
--rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.3/asqlorm/__init__.py
--rw-r--r--   0        0        0    30571 2024-02-24 23:55:25.233638 asqlorm-0.6.3/asqlorm/generator/main.py
--rw-r--r--   0        0        0    44542 2024-04-25 00:06:52.855343 asqlorm-0.6.3/asqlorm/models.py
--rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.3/asqlorm/sql/sql_alchemy.py
--rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.3/asqlorm/utils.py
--rw-r--r--   0        0        0      655 2024-04-25 00:07:03.209829 asqlorm-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 asqlorm-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.4/README.md
+-rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.4/asqlorm/__init__.py
+-rw-r--r--   0        0        0    30525 2024-05-08 17:40:16.365136 asqlorm-0.6.4/asqlorm/generator/main.py
+-rw-r--r--   0        0        0    44542 2024-04-25 00:06:52.855343 asqlorm-0.6.4/asqlorm/models.py
+-rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.4/asqlorm/sql/sql_alchemy.py
+-rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.4/asqlorm/utils.py
+-rw-r--r--   0        0        0      655 2024-05-08 17:40:19.668975 asqlorm-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 asqlorm-0.6.4/PKG-INFO
```

### Comparing `asqlorm-0.6.3/asqlorm/generator/main.py` & `asqlorm-0.6.4/asqlorm/generator/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,15 +512,15 @@
             resolver_func_strs.append(
                 f"""
     def {link_name}(self, resolver: T.Optional["{target_rez_name}"] = None, key: str = "{link_name}"{kwargs_str}) -> "{safe_table_name}Resolver":
         self.add_child(
             key=key,
             resolver = resolver or {target_rez_name}(),
             cardinality={'Cardinality.ONE' if link.cardinality == Cardinality.ONE else 'Cardinality.MANY'},
-            from_='{link.from_}',
+            from_=\"\"\"{link.from_}\"\"\",
             is_required={'False' if link.is_nullable else 'True'}
         )
         {update_qb_str}
         return self
             """
             )
             target_node_name = (
@@ -569,62 +569,62 @@
             )
 
         if get_params:
             joined_get_params = ", ".join(sorted(get_params))
             get_strs = f"""
     async def get(self, conn: AsyncConnection | None = None, *, {joined_get_params}) -> {safe_table_name} | None:
         return await self._get(conn=conn, {get_inner_params})
-    
+
     async def gerror(self, conn: AsyncConnection | None = None, *, {joined_get_params}) -> {safe_table_name}:
         return await self._gerror(conn=conn, {get_inner_params})
-    
+
     async def query(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> list[{safe_table_name}]:
         return await self._query(conn=conn, format_sql=format_sql, log_query=log_query)
-    
+
     async def first_or_none(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {safe_table_name} | None:
         return await super().first_or_none(conn=conn, format_sql=format_sql, log_query=log_query)
-    
+
     async def first(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {safe_table_name}:
         return await super().first(conn=conn, format_sql=format_sql, log_query=log_query)
-    
+
     async def one_or_none(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {safe_table_name} | None:
         return await super().one_or_none(conn=conn, format_sql=format_sql, log_query=log_query)
 
     async def one(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {safe_table_name}:
         return await super().one(conn=conn, format_sql=format_sql, log_query=log_query)
-    
+
     def filter_by(self, *, {filter_by_params_str}) -> "{safe_table_name}Resolver":
         return self._filter_by({filter_by_inner_params})
-    
+
     def filter_in(self, *, {filter_in_params_str}) -> "{safe_table_name}Resolver":
         return self._filter_in({filter_in_inner_params})
-    
+
     async def insert_one(self, insert: {safe_table_name}Insert, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_insert: bool = False, force_refresh: bool = False, conflict: Conflict | None = None) -> {safe_table_name}:
         return await super().insert_one(insert=insert, format_sql=format_sql, log_query=log_query, conn=conn, commit_after_insert=commit_after_insert, force_refresh=force_refresh, conflict=conflict)
-    
+
     async def insert_one_or_none(self, insert: {safe_table_name}Insert, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_insert: bool = False, force_refresh: bool = False, conflict: Conflict | None = None) -> T.Optional[{safe_table_name}]:
         return await super().insert_one_or_none(insert=insert, format_sql=format_sql, log_query=log_query, conn=conn, commit_after_insert=commit_after_insert, force_refresh=force_refresh, conflict=conflict)
 
     async def insert_many(self, inserts: list[{safe_table_name}Insert], conflict: Conflict | None = None, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_insert: bool = False, force_refresh: bool = False) -> list[{safe_table_name}]:
         return await super().insert_many(inserts=inserts, conflict=conflict, format_sql=format_sql, log_query=log_query, conn=conn, commit_after_insert=commit_after_insert, force_refresh=force_refresh)
-    
+
     async def delete_one_or_none(self, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_delete: bool = False) -> T.Optional[{safe_table_name}]:
         return await super().delete_one_or_none(format_sql=format_sql, log_query=log_query, conn=conn, commit_after_delete=commit_after_delete)
-    
+
     async def delete_one(self, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_delete: bool = False) -> {safe_table_name}:
         return await super().delete_one(format_sql=format_sql, log_query=log_query, conn=conn, commit_after_delete=commit_after_delete)
-    
+
     async def delete_many(self, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_delete: bool = False, delete_all: bool = False) -> list[{safe_table_name}]:
         return await super().delete_many(format_sql=format_sql, log_query=log_query, conn=conn, commit_after_delete=commit_after_delete, delete_all=delete_all)
             """
             if patch_fields_strs:
                 patch_one_str = f"""
     async def patch_one(self, patch: {safe_table_name}Patch, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_patch: bool = False, force_refresh: bool = False) -> {safe_table_name}:
         return await super().patch_one(patch=patch, format_sql=format_sql, log_query=log_query, conn=conn, commit_after_patch=commit_after_patch, force_refresh=force_refresh)
-    
+
     async def patch_many(self, patch: {safe_table_name}Patch, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_patch: bool = False, force_refresh: bool = False, patch_all: bool = False) -> list[{safe_table_name}]:
         return await super().patch_many(patch=patch, format_sql=format_sql, log_query=log_query, conn=conn, commit_after_patch=commit_after_patch, force_refresh=force_refresh, patch_all=patch_all)
                 """
                 get_strs = f"{get_strs}\n{patch_one_str}"
         else:
             get_strs = ""
 
@@ -649,15 +649,15 @@
         else:
             include_func_str = ""
 
         resolver_strs.append(
             f"""
 class {safe_table_name}Resolver({base_resolver_import_name or base_resolver_name}):
     _node = {safe_table_name}
-    
+
 {get_strs}
 {resolver_func_str}
     {include_func_str}
         """
         )
     all_strs = [
         "import typing as T",
```

### Comparing `asqlorm-0.6.3/asqlorm/models.py` & `asqlorm-0.6.4/asqlorm/models.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.3/asqlorm/sql/sql_alchemy.py` & `asqlorm-0.6.4/asqlorm/sql/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.3/asqlorm/utils.py` & `asqlorm-0.6.4/asqlorm/utils.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.3/pyproject.toml` & `asqlorm-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asqlorm"
-version = "0.6.3"
+version = "0.6.4"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = 'asqlorm' }]
 exclude = ["tests/**/*"]
```

### Comparing `asqlorm-0.6.3/PKG-INFO` & `asqlorm-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asqlorm
-Version: 0.6.3
+Version: 0.6.4
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
```

