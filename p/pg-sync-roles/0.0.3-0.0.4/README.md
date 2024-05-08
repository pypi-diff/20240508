# Comparing `tmp/pg_sync_roles-0.0.3.tar.gz` & `tmp/pg_sync_roles-0.0.4.tar.gz`

## Comparing `pg_sync_roles-0.0.3.tar` & `pg_sync_roles-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/pg_sync_roles.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/LICENSE
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/pg_sync_roles.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/README.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/PKG-INFO
```

### Comparing `pg_sync_roles-0.0.3/.gitignore` & `pg_sync_roles-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.3/LICENSE` & `pg_sync_roles-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.3/README.md` & `pg_sync_roles-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pg-sync-roles
+# pg-sync-roles [![PyPI package](https://img.shields.io/pypi/v/pg-sync-roles?label=PyPI%20package)](https://pypi.org/project/pg-sync-roles/) [![Test suite](https://img.shields.io/github/actions/workflow/status/uktrade/pg-sync-roles/test.yaml?label=Test%20suite)](https://github.com/uktrade/pg-sync-roles/actions/workflows/test.yaml) [![Code coverage](https://img.shields.io/codecov/c/github/uktrade/pg-sync-roles?label=Code%20coverage)](https://app.codecov.io/gh/uktrade/pg-sync-roles)
 
 Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships
 
 > [!WARNING]  
 > Work in progress. This README serves as a rough design spec.
 
 ## Features
@@ -65,12 +65,14 @@
         'my_role_name',
         grants=(
             TableSelect('my_schema', 'my_table'),
             SchemaUsage('my_schema'),
             RoleMembership('my_other_role'),
             SchemaOwnership('my_other_schema', create_if_not_exists=True),
         ),
-        revoke_other_role_memberships=True,
-        revoke_other_table_selects=True,
-        revoke_other_schema_usage=True,
+        revokes=(
+            TableSelect,
+            SchemaUsage,
+            RoleMembership,
+        ),
     )
 ```
```

