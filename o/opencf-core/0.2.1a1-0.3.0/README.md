# Comparing `tmp/opencf_core-0.2.1a1.tar.gz` & `tmp/opencf_core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencf_core-0.2.1a1.tar", max compression
+gzip compressed data, was "opencf_core-0.3.0.tar", max compression
```

## Comparing `opencf_core-0.2.1a1.tar` & `opencf_core-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7078 2024-05-03 17:07:50.871608 opencf_core-0.2.1a1/README.md
--rw-r--r--   0        0        0        0 2024-05-03 17:07:50.875608 opencf_core-0.2.1a1/opencf_core/__init__.py
--rw-r--r--   0        0        0    19442 2024-05-03 17:31:07.238604 opencf_core-0.2.1a1/opencf_core/base_converter.py
--rw-r--r--   0        0        0     6210 2024-05-03 17:33:26.276403 opencf_core-0.2.1a1/opencf_core/converter_app.py
--rw-r--r--   0        0        0    15473 2024-05-03 17:07:50.879608 opencf_core-0.2.1a1/opencf_core/filetypes.py
--rw-r--r--   0        0        0     5891 2024-05-03 17:07:50.879608 opencf_core-0.2.1a1/opencf_core/io_handler.py
--rw-r--r--   0        0        0     3441 2024-05-03 17:07:50.879608 opencf_core-0.2.1a1/opencf_core/logging_config.py
--rw-r--r--   0        0        0     2014 2024-05-03 17:07:50.879608 opencf_core-0.2.1a1/opencf_core/mimes.py
--rw-r--r--   0        0        0     1110 2024-05-03 17:51:52.829523 opencf_core-0.2.1a1/pyproject.toml
--rw-r--r--   0        0        0     8275 1970-01-01 00:00:00.000000 opencf_core-0.2.1a1/PKG-INFO
+-rw-r--r--   0        0        0     7078 2024-05-03 17:07:50.871608 opencf_core-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 17:07:50.875608 opencf_core-0.3.0/opencf_core/__init__.py
+-rw-r--r--   0        0        0    19442 2024-05-03 17:31:07.238604 opencf_core-0.3.0/opencf_core/base_converter.py
+-rw-r--r--   0        0        0     6210 2024-05-03 17:33:26.276403 opencf_core-0.3.0/opencf_core/converter_app.py
+-rw-r--r--   0        0        0    15473 2024-05-03 17:07:50.879608 opencf_core-0.3.0/opencf_core/filetypes.py
+-rw-r--r--   0        0        0     5891 2024-05-03 17:07:50.879608 opencf_core-0.3.0/opencf_core/io_handler.py
+-rw-r--r--   0        0        0     3441 2024-05-03 17:07:50.879608 opencf_core-0.3.0/opencf_core/logging_config.py
+-rw-r--r--   0        0        0     2014 2024-05-03 17:07:50.879608 opencf_core-0.3.0/opencf_core/mimes.py
+-rw-r--r--   0        0        0     1108 2024-05-08 08:25:59.106994 opencf_core-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8273 1970-01-01 00:00:00.000000 opencf_core-0.3.0/PKG-INFO
```

### Comparing `opencf_core-0.2.1a1/README.md` & `opencf_core-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `opencf_core-0.2.1a1/opencf_core/base_converter.py` & `opencf_core-0.3.0/opencf_core/base_converter.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.2.1a1/opencf_core/converter_app.py` & `opencf_core-0.3.0/opencf_core/converter_app.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.2.1a1/opencf_core/filetypes.py` & `opencf_core-0.3.0/opencf_core/filetypes.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.2.1a1/opencf_core/io_handler.py` & `opencf_core-0.3.0/opencf_core/io_handler.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.2.1a1/opencf_core/logging_config.py` & `opencf_core-0.3.0/opencf_core/logging_config.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.2.1a1/opencf_core/mimes.py` & `opencf_core-0.3.0/opencf_core/mimes.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.2.1a1/pyproject.toml` & `opencf_core-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "opencf-core"
 packages = [
     {include = "opencf_core"}
 ]
-version = "0.2.1a1"
+version = "0.3.0"
 description = "A robust framework for handling file conversion tasks in Python"
 authors = ["Hermann Agossou <agossouhermann7@gmail.com>"]
 readme = "README.md"
 maintainers = [
     "Hermann Agossou <agossouhermann7@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `opencf_core-0.2.1a1/PKG-INFO` & `opencf_core-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencf-core
-Version: 0.2.1a1
+Version: 0.3.0
 Summary: A robust framework for handling file conversion tasks in Python
 Home-page: https://github.com/Hermann-web/opencf-core
 License: MIT
 Keywords: file conversion,data processing,file formats
 Author: Hermann Agossou
 Author-email: agossouhermann7@gmail.com
 Maintainer: Hermann Agossou
```

