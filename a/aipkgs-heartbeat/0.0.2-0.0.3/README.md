# Comparing `tmp/aipkgs_heartbeat-0.0.2.tar.gz` & `tmp/aipkgs_heartbeat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_heartbeat-0.0.2.tar", max compression
+gzip compressed data, was "aipkgs_heartbeat-0.0.3.tar", max compression
```

## Comparing `aipkgs_heartbeat-0.0.2.tar` & `aipkgs_heartbeat-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.932000 aipkgs_heartbeat-0.0.2/LICENSE.md
--rw-r--r--   0        0        0        0 2022-09-03 18:02:41.168273 aipkgs_heartbeat-0.0.2/README.rst
--rw-r--r--   0        0        0        0 2023-12-14 16:32:45.512642 aipkgs_heartbeat-0.0.2/aipkgs_heartbeat/__init__.py
--rw-r--r--   0        0        0     4051 2022-07-30 18:17:14.119000 aipkgs_heartbeat-0.0.2/aipkgs_heartbeat/ai_heartbeat.py
--rw-r--r--   0        0        0      578 2023-12-14 16:33:03.304710 aipkgs_heartbeat-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 aipkgs_heartbeat-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.932000 aipkgs_heartbeat-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0        0 2022-09-03 18:02:41.168273 aipkgs_heartbeat-0.0.3/README.rst
+-rw-r--r--   0        0        0        0 2023-12-14 16:32:45.512642 aipkgs_heartbeat-0.0.3/aipkgs_heartbeat/__init__.py
+-rw-r--r--   0        0        0     4051 2022-07-30 18:17:14.119000 aipkgs_heartbeat-0.0.3/aipkgs_heartbeat/ai_heartbeat.py
+-rw-r--r--   0        0        0      582 2024-05-08 14:37:16.185559 aipkgs_heartbeat-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 aipkgs_heartbeat-0.0.3/PKG-INFO
```

### Comparing `aipkgs_heartbeat-0.0.2/LICENSE.md` & `aipkgs_heartbeat-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_heartbeat-0.0.2/aipkgs_heartbeat/ai_heartbeat.py` & `aipkgs_heartbeat-0.0.3/aipkgs_heartbeat/ai_heartbeat.py`

 * *Files identical despite different names*

### Comparing `aipkgs_heartbeat-0.0.2/pyproject.toml` & `aipkgs_heartbeat-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aipkgs-heartbeat"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Alexy <alexy.ib@outlook.com>"]
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
-APScheduler = "^3.9.1"
-Flask-APScheduler = "^1.12.4"
+python = "^3.11.3"
+APScheduler = "^3.10.4"
+Flask-APScheduler = "^1.13.1"
 
 [tool.poetry.extras]
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
```

### Comparing `aipkgs_heartbeat-0.0.2/PKG-INFO` & `aipkgs_heartbeat-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: aipkgs-heartbeat
-Version: 0.0.2
+Version: 0.0.3
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
-Requires-Dist: APScheduler (>=3.9.1,<4.0.0)
-Requires-Dist: Flask-APScheduler (>=1.12.4,<2.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: APScheduler (>=3.10.4,<4.0.0)
+Requires-Dist: Flask-APScheduler (>=1.13.1,<2.0.0)
 Project-URL: Repository, https://gitlab.com/aipy/public/packages.git
 Description-Content-Type: text/x-rst
```

