# Comparing `tmp/pg_sync_roles-0.0.4.tar.gz` & `tmp/pg_sync_roles-0.0.5.tar.gz`

## Comparing `pg_sync_roles-0.0.4.tar` & `pg_sync_roles-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/pg_sync_roles.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/LICENSE
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/README.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/pg_sync_roles.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/README.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.5/PKG-INFO
```

### Comparing `pg_sync_roles-0.0.4/.gitignore` & `pg_sync_roles-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.4/LICENSE` & `pg_sync_roles-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.4/README.md` & `pg_sync_roles-0.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -23,56 +23,72 @@
 
 
 ## Usage
 
 To give a user CONNECT privileges on a database, as well as membership of role:
 
 ```python
-from pg_sync_roles import DatabaseConnect, RoleMembership, pg_sync_roles
+from pg_sync_roles import DatabaseConnect, RoleMembership, sync_roles
 
 # For example purposes, PostgreSQL can be run locally using this...
 # docker run --rm -it -e POSTGRES_HOST_AUTH_METHOD=trust -p 5432:5432 postgres
 
 # ... which should work with this engine
 engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
 
 with engine.begin() as conn:
-    pg_sync_roles(
+    sync_roles(
         conn,
         'my_user_name',
         grants=(
             DatabaseConnect('my_database_name'),
             RoleMembership('my_role_name'),
         ),
     )
 ```
 
-A more complex example:
+A more complex example, where permissions and memberships are granted, but also any existing permissions not passed are revoked:
 
 ```python
 from pg_sync_roles import (
     RoleMembership,
     SchemaUsage,
     SchemaOwnership,
     TableSelect,
-    pg_sync_roles,
+    sync_roles,
 )
 
 engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
 
 with engine.begin() as conn:
-    pg_sync_roles(
+    sync_roles(
         conn,
         'my_role_name',
         grants=(
             TableSelect('my_schema', 'my_table'),
             SchemaUsage('my_schema'),
             RoleMembership('my_other_role'),
             SchemaOwnership('my_other_schema', create_if_not_exists=True),
         ),
+        # Revokes all table select, schema usage, and role memberships
+        # that are not not passed via the grants parameter
         revokes=(
             TableSelect,
             SchemaUsage,
             RoleMembership,
         ),
     )
 ```
+
+
+## Compatibility
+
+pg-sync-role aims to be compatible with a wide range of Python and other dependencies:
+
+- Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
+- psycopg2 >= 2.9.2 and Psycopg 3 >= 3.1.4
+- SQLAlchemy >= 1.4.24 (tested on 1.4.24 and 2.0.0)
+- PostgreSQL >= 9.6 (tested on 9.6, 10.0, 11.0, 12.0, 13.0, 14.0, 15.0, and 16.0)
+
+Note that SQLAlchemy < 2 does not support Psycopg 3, and for SQLAlchemy < 2 `future=True` must be passed to its create_engine function.
+
+There are no plans to drop support for any of the above.
```

### Comparing `pg_sync_roles-0.0.4/pyproject.toml` & `pg_sync_roles-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-sync-roles"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Department for Business and Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "sqlalchemy>=1.4.24",
+]
 
 [project.urls]
 "Source" = "https://github.com/uktrade/pg-sync-roles"
 
 [project.optional-dependencies]
 dev = [
   "pytest>=7.4.4",
 ]
 ci = [
   "pytest==7.4.4",
   "pytest-cov",
 ]
+ci-psycopg2-sqlalchemy1 = [
+    "psycopg2==2.9.2",
+    "sqlalchemy==1.4.24",
+]
+ci-psycopg2-sqlalchemy2 = [
+    "psycopg2==2.9.2",
+    "sqlalchemy==2.0.0",
+]
+ci-psycopg3-sqlalchemy2 = [
+    "psycopg==3.1.4",
+    "sqlalchemy==2.0.0",
+]
 
 [tool.hatch.build]
 include = [
   "pg_sync_roles.py"
 ]
```

### Comparing `pg_sync_roles-0.0.4/PKG-INFO` & `pg_sync_roles-0.0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.3
 Name: pg-sync-roles
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships
 Project-URL: Source, https://github.com/uktrade/pg-sync-roles
 Author-email: Department for Business and Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: sqlalchemy>=1.4.24
 Provides-Extra: ci
 Requires-Dist: pytest-cov; extra == 'ci'
 Requires-Dist: pytest==7.4.4; extra == 'ci'
+Provides-Extra: ci-psycopg2-sqlalchemy1
+Requires-Dist: psycopg2==2.9.2; extra == 'ci-psycopg2-sqlalchemy1'
+Requires-Dist: sqlalchemy==1.4.24; extra == 'ci-psycopg2-sqlalchemy1'
+Provides-Extra: ci-psycopg2-sqlalchemy2
+Requires-Dist: psycopg2==2.9.2; extra == 'ci-psycopg2-sqlalchemy2'
+Requires-Dist: sqlalchemy==2.0.0; extra == 'ci-psycopg2-sqlalchemy2'
+Provides-Extra: ci-psycopg3-sqlalchemy2
+Requires-Dist: psycopg==3.1.4; extra == 'ci-psycopg3-sqlalchemy2'
+Requires-Dist: sqlalchemy==2.0.0; extra == 'ci-psycopg3-sqlalchemy2'
 Provides-Extra: dev
 Requires-Dist: pytest>=7.4.4; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # pg-sync-roles [![PyPI package](https://img.shields.io/pypi/v/pg-sync-roles?label=PyPI%20package)](https://pypi.org/project/pg-sync-roles/) [![Test suite](https://img.shields.io/github/actions/workflow/status/uktrade/pg-sync-roles/test.yaml?label=Test%20suite)](https://github.com/uktrade/pg-sync-roles/actions/workflows/test.yaml) [![Code coverage](https://img.shields.io/codecov/c/github/uktrade/pg-sync-roles?label=Code%20coverage)](https://app.codecov.io/gh/uktrade/pg-sync-roles)
 
 Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships
@@ -41,56 +51,72 @@
 
 
 ## Usage
 
 To give a user CONNECT privileges on a database, as well as membership of role:
 
 ```python
-from pg_sync_roles import DatabaseConnect, RoleMembership, pg_sync_roles
+from pg_sync_roles import DatabaseConnect, RoleMembership, sync_roles
 
 # For example purposes, PostgreSQL can be run locally using this...
 # docker run --rm -it -e POSTGRES_HOST_AUTH_METHOD=trust -p 5432:5432 postgres
 
 # ... which should work with this engine
 engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
 
 with engine.begin() as conn:
-    pg_sync_roles(
+    sync_roles(
         conn,
         'my_user_name',
         grants=(
             DatabaseConnect('my_database_name'),
             RoleMembership('my_role_name'),
         ),
     )
 ```
 
-A more complex example:
+A more complex example, where permissions and memberships are granted, but also any existing permissions not passed are revoked:
 
 ```python
 from pg_sync_roles import (
     RoleMembership,
     SchemaUsage,
     SchemaOwnership,
     TableSelect,
-    pg_sync_roles,
+    sync_roles,
 )
 
 engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
 
 with engine.begin() as conn:
-    pg_sync_roles(
+    sync_roles(
         conn,
         'my_role_name',
         grants=(
             TableSelect('my_schema', 'my_table'),
             SchemaUsage('my_schema'),
             RoleMembership('my_other_role'),
             SchemaOwnership('my_other_schema', create_if_not_exists=True),
         ),
+        # Revokes all table select, schema usage, and role memberships
+        # that are not not passed via the grants parameter
         revokes=(
             TableSelect,
             SchemaUsage,
             RoleMembership,
         ),
     )
 ```
+
+
+## Compatibility
+
+pg-sync-role aims to be compatible with a wide range of Python and other dependencies:
+
+- Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
+- psycopg2 >= 2.9.2 and Psycopg 3 >= 3.1.4
+- SQLAlchemy >= 1.4.24 (tested on 1.4.24 and 2.0.0)
+- PostgreSQL >= 9.6 (tested on 9.6, 10.0, 11.0, 12.0, 13.0, 14.0, 15.0, and 16.0)
+
+Note that SQLAlchemy < 2 does not support Psycopg 3, and for SQLAlchemy < 2 `future=True` must be passed to its create_engine function.
+
+There are no plans to drop support for any of the above.
```

