# Comparing `tmp/pypomes_db-0.5.3.tar.gz` & `tmp/pypomes_db-0.5.4.tar.gz`

## Comparing `pypomes_db-0.5.3.tar` & `pypomes_db-0.5.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    29559 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    13749 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    29559 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    15840 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    13750 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/PKG-INFO
```

### Comparing `pypomes_db-0.5.3/src/pypomes_db/__init__.py` & `pypomes_db-0.5.4/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.3/src/pypomes_db/db_common.py` & `pypomes_db-0.5.4/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.3/src/pypomes_db/db_pomes.py` & `pypomes_db-0.5.4/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.3/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.5.4/src/pypomes_db/oracle_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,17 +207,17 @@
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
-        with (curr_conn.cursor() as cursor):
+        # noinspection DuplicatedCode
+        with curr_conn.cursor() as cursor:
 
-            # noinspection DuplicatedCode
             # execute the query
             cursor.execute(statement=sel_stmt,
                            parameters=where_vals)
 
             # fetch rows in batches/all rows
             result = 0
             op_errors: list[str] = []
@@ -228,15 +228,15 @@
                 rows = cursor.fetchall()
             while rows:
                 result += db_bulk_insert_to(errors=op_errors,
                                             insert_stmt=insert_stmt,
                                             insert_vals=rows,
                                             engine=target_engine,
                                             conn=target_conn,
-                                            logger=logger)
+                                            logger=logger) or 0
                 # errors ?
                 if op_errors:
                     # yes, register them and abort the operation
                     errors.extend(op_errors)
                     break
                 if not batch_size:
                     break
```

### Comparing `pypomes_db-0.5.3/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.5.4/src/pypomes_db/postgres_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,17 +207,17 @@
 
     # make sure to have a connection
     curr_conn: connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
+        # noinspection DuplicatedCode
         with curr_conn.cursor() as cursor:
 
-            # noinspection DuplicatedCode
             # execute the query
             cursor.execute(statement=sel_stmt,
                            parameters=where_vals)
 
             # fetch rows in batches/all rows
             result = 0
             op_errors: list[str] = []
@@ -228,15 +228,15 @@
                 rows = cursor.fetchall()
             while rows:
                 result += db_bulk_insert_to(errors=op_errors,
                                             insert_stmt=insert_stmt,
                                             insert_vals=rows,
                                             engine=target_engine,
                                             conn=target_conn,
-                                            logger=logger)
+                                            logger=logger) or 0
                 # errors ?
                 if op_errors:
                     # yes, register them and abort the operation
                     errors.extend(op_errors)
                     break
                 if not batch_size:
                     break
```

### Comparing `pypomes_db-0.5.3/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.5.4/src/pypomes_db/sqlserver_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,17 +205,17 @@
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
+        # noinspection DuplicatedCode
         with curr_conn.cursor() as cursor:
 
-            # noinspection DuplicatedCode
             # execute the query
             cursor.execute(sel_stmt, where_vals)
 
             # fetch rows in batches/all rows
             result = 0
             op_errors: list[str] = []
             rows: list[Row]
@@ -226,15 +226,15 @@
             while rows:
                 tuples: list[tuple] = [tuple(row) for row in rows]
                 result += db_bulk_insert_to(errors=op_errors,
                                             insert_stmt=insert_stmt,
                                             insert_vals=tuples,
                                             engine=target_engine,
                                             conn=target_conn,
-                                            logger=logger)
+                                            logger=logger) or 0
                 # errors ?
                 if op_errors:
                     # yes, register them and abort the operation
                     errors.extend(op_errors)
                     break
                 if not batch_size:
                     break
```

### Comparing `pypomes_db-0.5.3/LICENSE` & `pypomes_db-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.3/pyproject.toml` & `pypomes_db-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.5.3"
+version = "0.5.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.5.3/PKG-INFO` & `pypomes_db-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.5.3
+Version: 0.5.4
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

