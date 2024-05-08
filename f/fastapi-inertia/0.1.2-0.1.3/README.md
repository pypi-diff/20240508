# Comparing `tmp/fastapi_inertia-0.1.2.tar.gz` & `tmp/fastapi_inertia-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_inertia-0.1.2.tar", max compression
+gzip compressed data, was "fastapi_inertia-0.1.3.tar", max compression
```

## Comparing `fastapi_inertia-0.1.2.tar` & `fastapi_inertia-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1075 2024-04-21 18:04:08.142429 fastapi_inertia-0.1.2/LICENSE
--rw-r--r--   0        0        0    16710 2024-04-23 16:11:11.035698 fastapi_inertia-0.1.2/README.md
--rw-r--r--   0        0        0      556 2024-04-21 18:04:08.143798 fastapi_inertia-0.1.2/inertia/__init__.py
--rw-r--r--   0        0        0      704 2024-04-21 18:04:08.144132 fastapi_inertia-0.1.2/inertia/config.py
--rw-r--r--   0        0        0     2215 2024-04-21 18:04:08.144480 fastapi_inertia-0.1.2/inertia/exceptions.py
--rw-r--r--   0        0        0    12335 2024-04-23 15:17:26.663599 fastapi_inertia-0.1.2/inertia/inertia.py
--rw-r--r--   0        0        0        0 2024-04-23 15:27:17.449490 fastapi_inertia-0.1.2/inertia/py.typed
--rw-r--r--   0        0        0     1481 2024-04-23 15:17:26.663934 fastapi_inertia-0.1.2/inertia/utils.py
--rw-r--r--   0        0        0     1154 2024-04-23 16:11:11.037505 fastapi_inertia-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    17644 1970-01-01 00:00:00.000000 fastapi_inertia-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-21 18:04:08.142429 fastapi_inertia-0.1.3/LICENSE
+-rw-r--r--   0        0        0    16710 2024-04-23 16:11:11.035698 fastapi_inertia-0.1.3/README.md
+-rw-r--r--   0        0        0      556 2024-04-21 18:04:08.143798 fastapi_inertia-0.1.3/inertia/__init__.py
+-rw-r--r--   0        0        0      704 2024-04-21 18:04:08.144132 fastapi_inertia-0.1.3/inertia/config.py
+-rw-r--r--   0        0        0     2215 2024-04-21 18:04:08.144480 fastapi_inertia-0.1.3/inertia/exceptions.py
+-rw-r--r--   0        0        0    12335 2024-04-23 15:17:26.663599 fastapi_inertia-0.1.3/inertia/inertia.py
+-rw-r--r--   0        0        0        0 2024-04-23 15:27:17.449490 fastapi_inertia-0.1.3/inertia/py.typed
+-rw-r--r--   0        0        0     1481 2024-04-23 15:17:26.663934 fastapi_inertia-0.1.3/inertia/utils.py
+-rw-r--r--   0        0        0     1154 2024-05-08 15:09:54.434001 fastapi_inertia-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    17644 1970-01-01 00:00:00.000000 fastapi_inertia-0.1.3/PKG-INFO
```

### Comparing `fastapi_inertia-0.1.2/LICENSE` & `fastapi_inertia-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.2/README.md` & `fastapi_inertia-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.2/inertia/__init__.py` & `fastapi_inertia-0.1.3/inertia/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.2/inertia/config.py` & `fastapi_inertia-0.1.3/inertia/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.2/inertia/exceptions.py` & `fastapi_inertia-0.1.3/inertia/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.2/inertia/inertia.py` & `fastapi_inertia-0.1.3/inertia/inertia.py`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.2/inertia/utils.py` & `fastapi_inertia-0.1.3/inertia/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_inertia-0.1.2/pyproject.toml` & `fastapi_inertia-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-inertia"
-version = "0.1.2"
+version = "0.1.3"
 description = "An implementation of the Inertia protocol for FastAPI."
 authors = ["Hugo Mortreux <70602545+hxjo@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hxjo/fastapi-inertia"
 homepage = "https://github.com/hxjo/fastapi-inertia"
 keywords = ["inertia", "inertiajs", "fastapi", "python"]
@@ -19,15 +19,15 @@
 packages = [
     { include = "inertia"}
 ]
 exclude = ["inertia/tests/**/*"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
-fastapi = "^0.110.2"
+fastapi = "^0.111.0"
 
 [tool.poetry.group.dev.dependencies]
 uvicorn = "^0.29.0"
 mypy = "^1.9.0"
 ruff = "^0.4.1"
 pytest = "^8.1.1"
 httpx = "^0.27.0"
```

### Comparing `fastapi_inertia-0.1.2/PKG-INFO` & `fastapi_inertia-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-inertia
-Version: 0.1.2
+Version: 0.1.3
 Summary: An implementation of the Inertia protocol for FastAPI.
 Home-page: https://github.com/hxjo/fastapi-inertia
 License: MIT
 Keywords: inertia,inertiajs,fastapi,python
 Author: Hugo Mortreux
 Author-email: 70602545+hxjo@users.noreply.github.com
 Requires-Python: >=3.9
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: fastapi (>=0.110.2,<0.111.0)
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Project-URL: Repository, https://github.com/hxjo/fastapi-inertia
 Description-Content-Type: text/markdown
 
 # Inertia.js FastAPI Adapter
 <!-- TOC -->
 * [Inertia.js FastAPI Adapter](#inertiajs-fastapi-adapter)
   * [Installation](#installation)
```

