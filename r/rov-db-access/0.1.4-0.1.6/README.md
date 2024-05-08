# Comparing `tmp/rov_db_access-0.1.4.tar.gz` & `tmp/rov_db_access-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rov_db_access-0.1.4.tar", max compression
+gzip compressed data, was "rov_db_access-0.1.6.tar", max compression
```

## Comparing `rov_db_access-0.1.4.tar` & `rov_db_access-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,17 @@
--rw-r--r--   0        0        0      364 2024-01-19 20:30:36.866533 rov_db_access-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-28 21:38:40.450138 rov_db_access-0.1.4/README.md
--rw-r--r--   0        0        0     3575 2024-01-19 20:27:48.898167 rov_db_access-0.1.4/rov_db_access/__init__.py
--rw-r--r--   0        0        0     1654 2023-12-08 19:09:45.309405 rov_db_access-0.1.4/rov_db_access/models.py
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 rov_db_access-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      453 2024-05-08 20:09:03.117867 rov_db_access-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-28 21:38:40.450138 rov_db_access-0.1.6/README.md
+-rw-r--r--   0        0        0      359 2024-05-07 17:08:16.858586 rov_db_access-0.1.6/rov_db_access/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.778226 rov_db_access-0.1.6/rov_db_access/authentication/__init__.py
+-rw-r--r--   0        0        0     2324 2024-05-07 15:18:49.279026 rov_db_access-0.1.6/rov_db_access/authentication/models.py
+-rw-r--r--   0        0        0     1756 2024-05-07 16:22:22.222344 rov_db_access-0.1.6/rov_db_access/authentication/worker.py
+-rw-r--r--   0        0        0      675 2024-05-07 16:39:33.493938 rov_db_access-0.1.6/rov_db_access/config/db_utils.py
+-rw-r--r--   0        0        0     1122 2024-05-08 20:09:03.118984 rov_db_access-0.1.6/rov_db_access/config/settings.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.782941 rov_db_access-0.1.6/rov_db_access/gis/__init__.py
+-rw-r--r--   0        0        0     7207 2024-05-08 20:09:03.119358 rov_db_access-0.1.6/rov_db_access/gis/models.py
+-rw-r--r--   0        0        0    24897 2024-05-08 20:09:03.119358 rov_db_access-0.1.6/rov_db_access/gis/worker.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.791048 rov_db_access-0.1.6/rov_db_access/sentinel/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-19 20:09:14.792050 rov_db_access-0.1.6/rov_db_access/sentinel/models.py
+-rw-r--r--   0        0        0     2984 2024-05-07 16:21:41.802152 rov_db_access-0.1.6/rov_db_access/sentinel/worker.py
+-rw-r--r--   0        0        0     1531 2024-05-08 20:09:03.120864 rov_db_access-0.1.6/rov_db_access/utils/s3_utils.py
+-rw-r--r--   0        0        0     1155 2024-05-08 20:09:03.120864 rov_db_access-0.1.6/rov_db_access/utils/utils.py
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 rov_db_access-0.1.6/PKG-INFO
```

### Comparing `rov_db_access-0.1.4/PKG-INFO` & `rov_db_access-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: rov-db-access
-Version: 0.1.4
+Version: 0.1.6
 Summary: 
 Author: Pablo Cano
 Author-email: pablo.cano@rovisen.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: boto3 (>=1.34.99,<2.0.0)
 Requires-Dist: geoalchemy2 (>=0.14.2,<0.15.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: pytest (>=8.0.0,<9.0.0)
+Requires-Dist: shapely (>=2.0.4,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.23,<3.0.0)
 Description-Content-Type: text/markdown
```

