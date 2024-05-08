# Comparing `tmp/fastapi_storage_helper-0.0.4.tar.gz` & `tmp/fastapi_storage_helper-0.0.5.tar.gz`

## Comparing `fastapi_storage_helper-0.0.4.tar` & `fastapi_storage_helper-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/build_and_publish.sh
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/build_and_test.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/pytest.ini
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/readme.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/requirements.txt
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/startup.sh
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/tox.ini
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/.github/workflows/publish.yaml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/fastapi_storage_helper/__init__.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/fastapi_storage_helper/storage.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/README.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/build_and_publish.sh
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/build_and_test.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/pytest.ini
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/readme.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/requirements.txt
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/startup.sh
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/tox.ini
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/fastapi_storage_helper/__init__.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/fastapi_storage_helper/storage.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/.gitignore
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/README.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi_storage_helper-0.0.5/PKG-INFO
```

### Comparing `fastapi_storage_helper-0.0.4/.github/workflows/publish.yaml` & `fastapi_storage_helper-0.0.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_storage_helper-0.0.4/.gitignore` & `fastapi_storage_helper-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_storage_helper-0.0.4/pyproject.toml` & `fastapi_storage_helper-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_storage_helper"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Dzung Nguyen", email="dung@megatron-solutions.com" },
 ]
 description = "FastAPI Storage Helper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fastapi_storage_helper-0.0.4/PKG-INFO` & `fastapi_storage_helper-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fastapi_storage_helper
-Version: 0.0.4
+Version: 0.0.5
 Summary: FastAPI Storage Helper
 Project-URL: Homepage, https://github.com/megatron-global/fastapi-queue
 Project-URL: Bug Tracker, https://github.com/megatron-global/fastapi-queue/issues
 Author-email: Dzung Nguyen <dung@megatron-solutions.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

