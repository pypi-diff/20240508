# Comparing `tmp/pytrivialsql-0.1.6.tar.gz` & `tmp/pytrivialsql-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrivialsql-0.1.6.tar", last modified: Tue May  7 14:57:02 2024, max compression
+gzip compressed data, was "pytrivialsql-0.1.7.tar", last modified: Wed May  8 20:46:08 2024, max compression
```

## Comparing `pytrivialsql-0.1.6.tar` & `pytrivialsql-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:02.012923 pytrivialsql-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-07 14:57:02.012923 pytrivialsql-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:57:02.012923 pytrivialsql-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:02.008923 pytrivialsql-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:02.008923 pytrivialsql-0.1.6/src/pytrivialsql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/src/pytrivialsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/src/pytrivialsql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/src/pytrivialsql/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/src/pytrivialsql/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:02.012923 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-07 14:57:02.000000 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 14:57:02.000000 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:57:02.000000 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 14:57:02.000000 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 14:57:02.000000 pytrivialsql-0.1.6/src/pytrivialsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:02.012923 pytrivialsql-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/tests/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 14:56:43.000000 pytrivialsql-0.1.6/tests/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/src/pytrivialsql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/src/pytrivialsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/src/pytrivialsql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/src/pytrivialsql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/src/pytrivialsql/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-08 20:46:08.000000 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-08 20:46:08.000000 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:46:08.000000 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 20:46:08.000000 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 20:46:08.000000 pytrivialsql-0.1.7/src/pytrivialsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:46:08.426672 pytrivialsql-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/tests/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-08 20:45:53.000000 pytrivialsql-0.1.7/tests/test_sqlite.py
```

### Comparing `pytrivialsql-0.1.6/LICENSE` & `pytrivialsql-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.6/PKG-INFO` & `pytrivialsql-0.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.6
+Version: 0.1.7
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.6/pyproject.toml` & `pytrivialsql-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytrivialsql"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="inaimathi", email="leo.zovic@gmail.com" },
 ]
 description = "A trivial set of QOL bindings for SQL in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pytrivialsql-0.1.6/src/pytrivialsql/postgres.py` & `pytrivialsql-0.1.7/src/pytrivialsql/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def select(
         self, table_name, columns, where=None, order_by=None, limit=None, transform=None
     ):
         try:
             with self._conn.cursor() as cur:
                 if columns is None:
                     columns = "*"
-                if isinstance(columns, str):
+                if type(columns) is str:
                     columns = [columns]
                 query, args = sql.select_q(
                     table_name,
                     columns,
                     where=where,
                     order_by=order_by,
                     limit=limit,
```

### Comparing `pytrivialsql-0.1.6/src/pytrivialsql/sql.py` & `pytrivialsql-0.1.7/src/pytrivialsql/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,30 +131,35 @@
 def select_q(
     table_name,
     columns,
     where=None,
     join=None,
     order_by=None,
     limit=None,
+    offset=None,
     placeholder=None,
 ):
     if placeholder is None:
         placeholder = "?"
+    if type(columns) is str:
+        columns = [columns]
     query = f"SELECT {', '.join(columns)} FROM {table_name}"
     args = ()
     if join is not None:
         query += join_to_string(join)
     if where is not None:
         where_str, where_args = where_to_string(where, placeholder)
         query += where_str
         args = where_args
     if order_by is not None:
         query += f" ORDER BY {order_by}"
     if limit is not None:
         query += f" LIMIT {limit}"
+    if offset is not None:
+        query += f" OFFSET {offset}"
     return (query, args)
 
 
 def update_q(table_name, **kwargs):
     placeholder = kwargs.get("placeholder", "?")
     if "placeholder" in kwargs:
         del kwargs["placeholder"]
@@ -170,8 +175,8 @@
     return query + where_str, tuple(kwargs.values()) + where_args
 
 
 def delete_q(table_name, where, placeholder=None):
     if placeholder is None:
         placeholder = "?"
     where_str, where_args = where_to_string(where, placeholder)
-    return f"DELETE FROM {table_name} {where_str}", where_args
+    return f"DELETE FROM {table_name}{where_str}", where_args
```

### Comparing `pytrivialsql-0.1.6/src/pytrivialsql/sqlite.py` & `pytrivialsql-0.1.7/src/pytrivialsql/sqlite.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.6/src/pytrivialsql.egg-info/PKG-INFO` & `pytrivialsql-0.1.7/src/pytrivialsql.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.6
+Version: 0.1.7
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.6/tests/test_postgres.py` & `pytrivialsql-0.1.7/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.6/tests/test_sql.py` & `pytrivialsql-0.1.7/tests/test_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,21 +141,21 @@
             ("INSERT INTO table_name (prop, propb) VALUES (%s, %s)", ("Blah!", 12)),
         )
 
 
 class TestDelete_q(unittest.TestCase):
     def test_string_rep(self):
         self.assertEqual(
-            ("DELETE FROM table_name  WHERE id=?", (1,)),
+            ("DELETE FROM table_name WHERE id=?", (1,)),
             sql.delete_q("table_name", where={"id": 1}),
         )
 
     def test_placeholder_change(self):
         self.assertEqual(
-            ("DELETE FROM table_name  WHERE id=%s", (1,)),
+            ("DELETE FROM table_name WHERE id=%s", (1,)),
             sql.delete_q("table_name", where={"id": 1}, placeholder="%s"),
         )
 
 
 class TestUpdate_q(unittest.TestCase):
     def test_string_rep(self):
         self.assertEqual(
```

### Comparing `pytrivialsql-0.1.6/tests/test_sqlite.py` & `pytrivialsql-0.1.7/tests/test_sqlite.py`

 * *Files identical despite different names*

