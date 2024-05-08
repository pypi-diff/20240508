# Comparing `tmp/langevals_google_cloud-0.1.2.tar.gz` & `tmp/langevals_google_cloud-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_google_cloud-0.1.2.tar", max compression
+gzip compressed data, was "langevals_google_cloud-0.1.3.tar", max compression
```

## Comparing `langevals_google_cloud-0.1.2.tar` & `langevals_google_cloud-0.1.3.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     4443 2024-04-28 13:24:54.116394 langevals_google_cloud-0.1.2/langevals_google_cloud/dlp_pii_detection.py
--rw-r--r--   0        0        0      540 2024-04-28 13:25:35.780510 langevals_google_cloud-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 langevals_google_cloud-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4443 2024-05-07 14:19:44.470403 langevals_google_cloud-0.1.3/langevals_google_cloud/dlp_pii_detection.py
+-rw-r--r--   0        0        0      540 2024-05-07 14:20:36.722759 langevals_google_cloud-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 langevals_google_cloud-0.1.3/PKG-INFO
```

### Comparing `langevals_google_cloud-0.1.2/langevals_google_cloud/dlp_pii_detection.py` & `langevals_google_cloud-0.1.3/langevals_google_cloud/dlp_pii_detection.py`

 * *Files identical despite different names*

### Comparing `langevals_google_cloud-0.1.2/pyproject.toml` & `langevals_google_cloud-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "langevals-google-cloud"
-version = "0.1.2"
+version = "0.1.3"
 description = "LangEvals integration for Google Cloud APIs evaluators"
 authors = [ "Rogerio Chaves <rogerio@langwatch.ai>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-langevals-core = "^0.1.2"
+langevals-core = "^0.1.3"
 google-cloud-dlp = "^3.16.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.2"
 python-dotenv = "1.0.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `langevals_google_cloud-0.1.2/PKG-INFO` & `langevals_google_cloud-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: langevals-google-cloud
-Version: 0.1.2
+Version: 0.1.3
 Summary: LangEvals integration for Google Cloud APIs evaluators
 License: MIT
 Author: Rogerio Chaves
 Author-email: rogerio@langwatch.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: google-cloud-dlp (>=3.16.0,<4.0.0)
-Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
+Requires-Dist: langevals-core (>=0.1.3,<0.2.0)
```

