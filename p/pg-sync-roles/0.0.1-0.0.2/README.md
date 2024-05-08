# Comparing `tmp/pg_sync_roles-0.0.1.tar.gz` & `tmp/pg_sync_roles-0.0.2.tar.gz`

## Comparing `pg_sync_roles-0.0.1.tar` & `pg_sync_roles-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.1/pg_sync_roles.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.1/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.1/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.1/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/pg_sync_roles.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/PKG-INFO
```

### Comparing `pg_sync_roles-0.0.1/.gitignore` & `pg_sync_roles-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.1/LICENSE` & `pg_sync_roles-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.1/pyproject.toml` & `pg_sync_roles-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-sync-roles"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Department for Business and Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

