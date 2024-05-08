# Comparing `tmp/airbyte_source_mixpanel-2.2.0.tar.gz` & `tmp/airbyte_source_mixpanel-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_mixpanel-2.2.0.tar", max compression
+gzip compressed data, was "airbyte_source_mixpanel-2.2.2.tar", max compression
```

## Comparing `airbyte_source_mixpanel-2.2.0.tar` & `airbyte_source_mixpanel-2.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     4532 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/README.md
--rw-r--r--   0        0        0      749 2024-03-21 02:02:44.234918 airbyte_source_mixpanel-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     1138 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/__init__.py
--rw-r--r--   0        0        0     3363 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/config_migrations.py
--rw-r--r--   0        0        0     1505 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/property_transformation.py
--rw-r--r--   0        0        0      350 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/run.py
--rw-r--r--   0        0        0      641 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/schemas/annotations.json
--rw-r--r--   0        0        0     1001 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/schemas/cohort_members.json
--rw-r--r--   0        0        0      629 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/schemas/cohorts.json
--rw-r--r--   0        0        0      941 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/schemas/engage.json
--rw-r--r--   0        0        0     5299 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/schemas/export.json
--rw-r--r--   0        0        0     3229 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/schemas/funnels.json
--rw-r--r--   0        0        0      466 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/schemas/revenue.json
--rw-r--r--   0        0        0     7834 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/source.py
--rw-r--r--   0        0        0     5361 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/spec.json
--rw-r--r--   0        0        0      603 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/__init__.py
--rw-r--r--   0        0        0     1343 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/annotations.py
--rw-r--r--   0        0        0     9920 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/base.py
--rw-r--r--   0        0        0     1496 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/cohort_members.py
--rw-r--r--   0        0        0     1519 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/cohorts.py
--rw-r--r--   0        0        0     8610 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/engage.py
--rw-r--r--   0        0        0     8023 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/export.py
--rw-r--r--   0        0        0     6250 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/funnels.py
--rw-r--r--   0        0        0     1649 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/revenue.py
--rw-r--r--   0        0        0     1624 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/testing.py
--rw-r--r--   0        0        0     1965 2024-03-21 01:47:20.577994 airbyte_source_mixpanel-2.2.0/source_mixpanel/utils.py
--rw-r--r--   0        0        0     5240 1970-01-01 00:00:00.000000 airbyte_source_mixpanel-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4537 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/README.md
+-rw-r--r--   0        0        0      753 2024-05-07 13:32:21.808242 airbyte_source_mixpanel-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1138 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/__init__.py
+-rw-r--r--   0        0        0     3363 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/config_migrations.py
+-rw-r--r--   0        0        0     1505 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/property_transformation.py
+-rw-r--r--   0        0        0      350 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/run.py
+-rw-r--r--   0        0        0     1208 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/schemas/annotations.json
+-rw-r--r--   0        0        0     2050 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/schemas/cohort_members.json
+-rw-r--r--   0        0        0     1249 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/schemas/cohorts.json
+-rw-r--r--   0        0        0     1796 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/schemas/engage.json
+-rw-r--r--   0        0        0     9765 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/schemas/export.json
+-rw-r--r--   0        0        0     5384 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/schemas/funnels.json
+-rw-r--r--   0        0        0      843 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/schemas/revenue.json
+-rw-r--r--   0        0        0     7834 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/source.py
+-rw-r--r--   0        0        0     5361 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/spec.json
+-rw-r--r--   0        0        0      603 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/annotations.py
+-rw-r--r--   0        0        0     9920 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/base.py
+-rw-r--r--   0        0        0     1496 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/cohort_members.py
+-rw-r--r--   0        0        0     1519 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/cohorts.py
+-rw-r--r--   0        0        0     8610 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/engage.py
+-rw-r--r--   0        0        0     8023 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/export.py
+-rw-r--r--   0        0        0     6250 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/funnels.py
+-rw-r--r--   0        0        0     1649 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/revenue.py
+-rw-r--r--   0        0        0     1624 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/testing.py
+-rw-r--r--   0        0        0     1965 2024-05-07 10:45:34.000000 airbyte_source_mixpanel-2.2.2/source_mixpanel/utils.py
+-rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 airbyte_source_mixpanel-2.2.2/PKG-INFO
```

### Comparing `airbyte_source_mixpanel-2.2.0/README.md` & `airbyte_source_mixpanel-2.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-mixpanel spec
 poetry run source-mixpanel check --config secrets/config.json
 poetry run source-mixpanel discover --config secrets/config.json
-poetry run source-mixpanel read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-mixpanel read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

### Comparing `airbyte_source_mixpanel-2.2.0/pyproject.toml` & `airbyte_source_mixpanel-2.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.2.0"
+version = "2.2.2"
 name = "airbyte-source-mixpanel"
 description = "Source implementation for Mixpanel."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_mixpanel" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 
 [tool.poetry.scripts]
 source-mixpanel = "source_mixpanel.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
 pytest-mock = "^3.6"
```

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/__init__.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/config_migrations.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/property_transformation.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/property_transformation.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/schemas/cohort_members.json` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/schemas/revenue.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('date', OrderedDict([('description', 'Date for which the "*

 * *                 "revenue data is recorded'), ('type', ['null', 'string']), ('format', 'date')])), "*

 * *                 "('datetime', OrderedDict([('description', 'Date and time for which the revenue "*

 * *                 "data is recorded'), ('type', ['null', 'string']), ('format', 'date-time')])), "*

 * *                 "('count', OrderedDict([('description', 'Number of revenue transactions for the "*

 * *               […]*

```diff
@@ -1,97 +1,44 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "browser": {
+        "amount": {
+            "description": "Total revenue amount for the specified date",
+            "multipleOf": 1e-20,
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "browser_version": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "city": {
-            "type": [
-                "null",
-                "string"
+                "number"
             ]
         },
-        "cohort_id": {
+        "count": {
+            "description": "Number of revenue transactions for the specified date",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "country_code": {
+        "date": {
+            "description": "Date for which the revenue data is recorded",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "distinct_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "email": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "first_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "last_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "last_seen": {
+        "datetime": {
+            "description": "Date and time for which the revenue data is recorded",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "region": {
+        "paid_count": {
+            "description": "Number of successful paid transactions for the specified date",
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "timezone": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "unblocked": {
-            "type": [
-                "null",
-                "string"
+                "integer"
             ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/source.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/spec.json` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/__init__.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/annotations.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/annotations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/base.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/base.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/cohort_members.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/cohort_members.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/cohorts.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/cohorts.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/engage.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/engage.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/export.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/export.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/funnels.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/funnels.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/streams/revenue.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/streams/revenue.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/testing.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/testing.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/source_mixpanel/utils.py` & `airbyte_source_mixpanel-2.2.2/source_mixpanel/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-2.2.0/PKG-INFO` & `airbyte_source_mixpanel-2.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-mixpanel
-Version: 2.2.0
+Version: 2.2.2
 Summary: Source implementation for Mixpanel.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/mixpanel
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Mixpanel source connector
 
 
@@ -45,15 +45,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-mixpanel spec
 poetry run source-mixpanel check --config secrets/config.json
 poetry run source-mixpanel discover --config secrets/config.json
-poetry run source-mixpanel read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-mixpanel read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

