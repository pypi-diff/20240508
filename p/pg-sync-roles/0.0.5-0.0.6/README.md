# Comparing `tmp/pg_sync_roles-0.0.5.tar.gz` & `tmp/pg_sync_roles-0.0.6.tar.gz`

## Comparing `pg_sync_roles-0.0.5.tar` & `pg_sync_roles-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/pg_sync_roles.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/LICENSE
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/README.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/pg_sync_roles.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/README.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/PKG-INFO
```

### Comparing `pg_sync_roles-0.0.5/.gitignore` & `pg_sync_roles-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.5/LICENSE` & `pg_sync_roles-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.5/README.md` & `pg_sync_roles-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         ),
     )
 ```
 
 
 ## Compatibility
 
-pg-sync-role aims to be compatible with a wide range of Python and other dependencies:
+pg-sync-roles aims to be compatible with a wide range of Python and other dependencies:
 
 - Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
 - psycopg2 >= 2.9.2 and Psycopg 3 >= 3.1.4
 - SQLAlchemy >= 1.4.24 (tested on 1.4.24 and 2.0.0)
 - PostgreSQL >= 9.6 (tested on 9.6, 10.0, 11.0, 12.0, 13.0, 14.0, 15.0, and 16.0)
 
 Note that SQLAlchemy < 2 does not support Psycopg 3, and for SQLAlchemy < 2 `future=True` must be passed to its create_engine function.
```

### Comparing `pg_sync_roles-0.0.5/pyproject.toml` & `pg_sync_roles-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-sync-roles"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Department for Business and Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_sync_roles-0.0.5/PKG-INFO` & `pg_sync_roles-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pg-sync-roles
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships
 Project-URL: Source, https://github.com/uktrade/pg-sync-roles
 Author-email: Department for Business and Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -106,15 +106,15 @@
         ),
     )
 ```
 
 
 ## Compatibility
 
-pg-sync-role aims to be compatible with a wide range of Python and other dependencies:
+pg-sync-roles aims to be compatible with a wide range of Python and other dependencies:
 
 - Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
 - psycopg2 >= 2.9.2 and Psycopg 3 >= 3.1.4
 - SQLAlchemy >= 1.4.24 (tested on 1.4.24 and 2.0.0)
 - PostgreSQL >= 9.6 (tested on 9.6, 10.0, 11.0, 12.0, 13.0, 14.0, 15.0, and 16.0)
 
 Note that SQLAlchemy < 2 does not support Psycopg 3, and for SQLAlchemy < 2 `future=True` must be passed to its create_engine function.
```

