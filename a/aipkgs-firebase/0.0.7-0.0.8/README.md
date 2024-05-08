# Comparing `tmp/aipkgs_firebase-0.0.7.tar.gz` & `tmp/aipkgs_firebase-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_firebase-0.0.7.tar", max compression
+gzip compressed data, was "aipkgs_firebase-0.0.8.tar", max compression
```

## Comparing `aipkgs_firebase-0.0.7.tar` & `aipkgs_firebase-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.928787 aipkgs_firebase-0.0.7/LICENSE.md
--rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-0.0.7/README.rst
--rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-0.0.7/aipkgs_firebase/__init__.py
--rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-0.0.7/aipkgs_firebase/helpers.py
--rw-r--r--   0        0        0      136 2023-11-26 12:53:12.992955 aipkgs_firebase-0.0.7/aipkgs_firebase/messaging/__init__.py
--rw-r--r--   0        0        0     5155 2022-03-08 13:06:48.928493 aipkgs_firebase-0.0.7/aipkgs_firebase/messaging/core.py
--rw-r--r--   0        0        0       74 2022-03-08 13:06:48.928579 aipkgs_firebase-0.0.7/aipkgs_firebase/messaging/enums.py
--rw-r--r--   0        0        0     2474 2022-03-08 13:06:48.928861 aipkgs_firebase-0.0.7/aipkgs_firebase/messaging/helpers.py
--rw-r--r--   0        0        0     4215 2023-11-26 13:02:21.871322 aipkgs_firebase-0.0.7/aipkgs_firebase/storage/core.py
--rw-r--r--   0        0        0     2501 2023-11-26 12:59:30.711356 aipkgs_firebase-0.0.7/aipkgs_firebase/storage/helpers.py
--rw-r--r--   0        0        0     2511 2023-11-26 12:59:11.574625 aipkgs_firebase-0.0.7/aipkgs_firebase/storage/root.py
--rw-r--r--   0        0        0      568 2023-11-26 13:03:59.073290 aipkgs_firebase-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 aipkgs_firebase-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.928787 aipkgs_firebase-0.0.8/LICENSE.md
+-rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-0.0.8/README.rst
+-rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-0.0.8/aipkgs_firebase/__init__.py
+-rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-0.0.8/aipkgs_firebase/helpers.py
+-rw-r--r--   0        0        0      136 2023-11-26 12:53:12.992955 aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/__init__.py
+-rw-r--r--   0        0        0     5155 2022-03-08 13:06:48.928493 aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/core.py
+-rw-r--r--   0        0        0       74 2022-03-08 13:06:48.928579 aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/enums.py
+-rw-r--r--   0        0        0     2474 2022-03-08 13:06:48.928861 aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/helpers.py
+-rw-r--r--   0        0        0     4215 2023-11-26 13:02:21.871322 aipkgs_firebase-0.0.8/aipkgs_firebase/storage/core.py
+-rw-r--r--   0        0        0     2501 2023-11-26 12:59:30.711356 aipkgs_firebase-0.0.8/aipkgs_firebase/storage/helpers.py
+-rw-r--r--   0        0        0     2511 2023-11-26 12:59:11.574625 aipkgs_firebase-0.0.8/aipkgs_firebase/storage/root.py
+-rw-r--r--   0        0        0      571 2024-05-08 14:08:14.528442 aipkgs_firebase-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 aipkgs_firebase-0.0.8/PKG-INFO
```

### Comparing `aipkgs_firebase-0.0.7/LICENSE.md` & `aipkgs_firebase-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.7/aipkgs_firebase/helpers.py` & `aipkgs_firebase-0.0.8/aipkgs_firebase/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.7/aipkgs_firebase/messaging/core.py` & `aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.7/aipkgs_firebase/messaging/helpers.py` & `aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.7/aipkgs_firebase/storage/core.py` & `aipkgs_firebase-0.0.8/aipkgs_firebase/storage/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.7/aipkgs_firebase/storage/helpers.py` & `aipkgs_firebase-0.0.8/aipkgs_firebase/storage/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.7/aipkgs_firebase/storage/root.py` & `aipkgs_firebase-0.0.8/aipkgs_firebase/storage/root.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.7/pyproject.toml` & `aipkgs_firebase-0.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aipkgs-firebase"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["Alexy <alexy.ib@outlook.com>"]
 # New attributes
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/aipy/public/packages.git"
 repository = "https://gitlab.com/aipy/public/packages.git"
 keywords = ["ai"]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-firebase-admin = "^5.2.0"
-aipkgs-core = "^0.3.6"
+python = "^3.11.3"
+firebase-admin = "^6.5.0"
+aipkgs-core = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
```

### Comparing `aipkgs_firebase-0.0.7/PKG-INFO` & `aipkgs_firebase-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: aipkgs-firebase
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Home-page: https://gitlab.com/aipy/public/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aipkgs-core (>=0.3.6,<0.4.0)
-Requires-Dist: firebase-admin (>=5.2.0,<6.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aipkgs-core (>=0.4.0,<0.5.0)
+Requires-Dist: firebase-admin (>=6.5.0,<7.0.0)
 Project-URL: Repository, https://gitlab.com/aipy/public/packages.git
 Description-Content-Type: text/x-rst
 
 AI's package
```

