# Comparing `tmp/edgegap_settings-1.7.0.tar.gz` & `tmp/edgegap_settings-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_settings-1.7.0.tar", max compression
+gzip compressed data, was "edgegap_settings-1.7.2.tar", max compression
```

## Comparing `edgegap_settings-1.7.0.tar` & `edgegap_settings-1.7.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1993 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/LICENSE
--rw-r--r--   0        0        0     2182 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/README.md
--rw-r--r--   0        0        0       17 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/BUILD
--rw-r--r--   0        0        0      472 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/__init__.py
--rw-r--r--   0        0        0      531 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_apm.py
--rw-r--r--   0        0        0     1169 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_base.py
--rw-r--r--   0        0        0      119 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_configuration.py
--rw-r--r--   0        0        0     3147 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_factory.py
--rw-r--r--   0        0        0      581 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_fields.py
--rw-r--r--   0        0        0      427 2024-05-07 13:27:48.731497 edgegap_settings-1.7.0/edgegap_settings/_logstash.py
--rw-r--r--   0        0        0      798 2024-05-07 13:29:33.612393 edgegap_settings-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 edgegap_settings-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-08 18:14:27.831252 edgegap_settings-1.7.2/LICENSE
+-rw-r--r--   0        0        0     2182 2024-05-08 18:14:27.831369 edgegap_settings-1.7.2/README.md
+-rw-r--r--   0        0        0      523 2024-05-08 19:19:23.397259 edgegap_settings-1.7.2/edgegap_settings/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-08 18:14:27.831602 edgegap_settings-1.7.2/edgegap_settings/_apm.py
+-rw-r--r--   0        0        0     1169 2024-05-08 18:14:27.831706 edgegap_settings-1.7.2/edgegap_settings/_base.py
+-rw-r--r--   0        0        0      119 2024-05-08 18:14:27.831813 edgegap_settings-1.7.2/edgegap_settings/_configuration.py
+-rw-r--r--   0        0        0     3823 2024-05-08 19:19:23.397414 edgegap_settings-1.7.2/edgegap_settings/_factory.py
+-rw-r--r--   0        0        0      581 2024-05-08 18:14:27.832028 edgegap_settings-1.7.2/edgegap_settings/_fields.py
+-rw-r--r--   0        0        0      427 2024-05-08 18:14:27.832131 edgegap_settings-1.7.2/edgegap_settings/_logstash.py
+-rw-r--r--   0        0        0      675 2024-05-08 19:19:23.397510 edgegap_settings-1.7.2/edgegap_settings/_model.py
+-rw-r--r--   0        0        0      820 2024-05-08 19:20:21.398668 edgegap_settings-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 edgegap_settings-1.7.2/PKG-INFO
```

### Comparing `edgegap_settings-1.7.0/LICENSE` & `edgegap_settings-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.7.0/README.md` & `edgegap_settings-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.7.0/edgegap_settings/_apm.py` & `edgegap_settings-1.7.2/edgegap_settings/_apm.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.7.0/edgegap_settings/_base.py` & `edgegap_settings-1.7.2/edgegap_settings/_base.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.7.0/edgegap_settings/_fields.py` & `edgegap_settings-1.7.2/edgegap_settings/_fields.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-1.7.0/pyproject.toml` & `edgegap_settings-1.7.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-settings"
-version = "1.7.0"
+version = "1.7.2"
 description = "The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic-settings = "^2.2.1"
@@ -16,14 +16,15 @@
 elastic-apm = "^6.22.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 pytest-mock = "^3.14.0"
 pytest-cov = "^5.0.0"
 ruff = "^0.4.2"
+starlette = "^0.37.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 extend = "../../../3rdparty/ruff/ruff.toml"
```

### Comparing `edgegap_settings-1.7.0/PKG-INFO` & `edgegap_settings-1.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: edgegap-settings
-Version: 1.7.0
+Version: 1.7.2
 Summary: The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: edgegap-consul (>=1.0.0,<2.0.0)
 Requires-Dist: edgegap-logging (>=1.0.0,<2.0.0)
 Requires-Dist: elastic-apm (>=6.22.0,<7.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-logstash-async (>=3.0.0,<4.0.0)
```

