# Comparing `tmp/pg_sync_roles-0.0.2.tar.gz` & `tmp/pg_sync_roles-0.0.3.tar.gz`

## Comparing `pg_sync_roles-0.0.2.tar` & `pg_sync_roles-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/pg_sync_roles.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/LICENSE
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/pg_sync_roles.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/PKG-INFO
```

### Comparing `pg_sync_roles-0.0.2/.gitignore` & `pg_sync_roles-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.2/LICENSE` & `pg_sync_roles-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.2/README.md` & `pg_sync_roles-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -40,7 +40,37 @@
         conn,
         'my_user_name',
         grants=(
             DatabaseConnect('my_database_name'),
             RoleMembership('my_role_name'),
         ),
     )
+```
+
+A more complex example:
+
+```python
+from pg_sync_roles import (
+    RoleMembership,
+    SchemaUsage,
+    SchemaOwnership,
+    TableSelect,
+    pg_sync_roles,
+)
+
+engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
+
+with engine.begin() as conn:
+    pg_sync_roles(
+        conn,
+        'my_role_name',
+        grants=(
+            TableSelect('my_schema', 'my_table'),
+            SchemaUsage('my_schema'),
+            RoleMembership('my_other_role'),
+            SchemaOwnership('my_other_schema', create_if_not_exists=True),
+        ),
+        revoke_other_role_memberships=True,
+        revoke_other_table_selects=True,
+        revoke_other_schema_usage=True,
+    )
+```
```

### Comparing `pg_sync_roles-0.0.2/pyproject.toml` & `pg_sync_roles-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-sync-roles"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Department for Business and Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_sync_roles-0.0.2/PKG-INFO` & `pg_sync_roles-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pg-sync-roles
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships
 Project-URL: Source, https://github.com/uktrade/pg-sync-roles
 Author-email: Department for Business and Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -53,7 +53,37 @@
         conn,
         'my_user_name',
         grants=(
             DatabaseConnect('my_database_name'),
             RoleMembership('my_role_name'),
         ),
     )
+```
+
+A more complex example:
+
+```python
+from pg_sync_roles import (
+    RoleMembership,
+    SchemaUsage,
+    SchemaOwnership,
+    TableSelect,
+    pg_sync_roles,
+)
+
+engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
+
+with engine.begin() as conn:
+    pg_sync_roles(
+        conn,
+        'my_role_name',
+        grants=(
+            TableSelect('my_schema', 'my_table'),
+            SchemaUsage('my_schema'),
+            RoleMembership('my_other_role'),
+            SchemaOwnership('my_other_schema', create_if_not_exists=True),
+        ),
+        revoke_other_role_memberships=True,
+        revoke_other_table_selects=True,
+        revoke_other_schema_usage=True,
+    )
+```
```

