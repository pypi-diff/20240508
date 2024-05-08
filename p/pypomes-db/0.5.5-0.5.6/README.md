# Comparing `tmp/pypomes_db-0.5.5.tar.gz` & `tmp/pypomes_db-0.5.6.tar.gz`

## Comparing `pypomes_db-0.5.5.tar` & `pypomes_db-0.5.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38002 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    24057 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    21898 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    21948 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38002 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    24057 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    21898 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    21948 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/PKG-INFO
```

### Comparing `pypomes_db-0.5.5/src/pypomes_db/__init__.py` & `pypomes_db-0.5.6/src/pypomes_db/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from .db_pomes import (
     db_setup, db_get_engines, db_get_params,
     db_assert_connection, db_connect, db_exists,
     db_select_one, db_select_all, db_update,
     db_delete, db_insert, db_bulk_insert, db_bulk_copy,
-    db_execute, db_call_function, db_call_procedure,
+    db_copy_lobs, db_update_lob, db_execute,
+    db_call_function, db_call_procedure,
 )
 
 __all__ = [
     # db_pomes
     "db_setup", "db_get_engines", "db_get_params",
     "db_assert_connection", "db_connect", "db_exists",
     "db_select_one", "db_select_all", "db_update",
     "db_delete", "db_insert", "db_bulk_insert", "db_bulk_copy",
-    "db_execute", "db_call_function", "db_call_procedure",
+    "db_copy_lobs", "db_update_lob", "db_execute",
+    "db_call_function", "db_call_procedure",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_db")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_db-0.5.5/src/pypomes_db/db_common.py` & `pypomes_db-0.5.6/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.5/src/pypomes_db/db_pomes.py` & `pypomes_db-0.5.6/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.5/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.5.6/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.5/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.5.6/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.5/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.5.6/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.5/LICENSE` & `pypomes_db-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.5/pyproject.toml` & `pypomes_db-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.5.5"
+version = "0.5.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.5.5/PKG-INFO` & `pypomes_db-0.5.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.5.5
+Version: 0.5.6
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

