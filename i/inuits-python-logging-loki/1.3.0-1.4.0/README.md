# Comparing `tmp/inuits_python_logging_loki-1.3.0.tar.gz` & `tmp/inuits_python_logging_loki-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inuits_python_logging_loki-1.3.0.tar", last modified: Wed May  8 12:06:43 2024, max compression
+gzip compressed data, was "inuits_python_logging_loki-1.4.0.tar", last modified: Wed May  8 12:59:15 2024, max compression
```

## Comparing `inuits_python_logging_loki-1.3.0.tar` & `inuits_python_logging_loki-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:06:43.670477 inuits_python_logging_loki-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-08 12:06:43.670477 inuits_python_logging_loki-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:06:43.670477 inuits_python_logging_loki-1.3.0/inuits_python_logging_loki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-08 12:06:43.000000 inuits_python_logging_loki-1.3.0/inuits_python_logging_loki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 12:06:43.000000 inuits_python_logging_loki-1.3.0/inuits_python_logging_loki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:06:43.000000 inuits_python_logging_loki-1.3.0/inuits_python_logging_loki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 12:06:43.000000 inuits_python_logging_loki-1.3.0/inuits_python_logging_loki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 12:06:43.000000 inuits_python_logging_loki-1.3.0/inuits_python_logging_loki.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:06:43.670477 inuits_python_logging_loki-1.3.0/logging_loki/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/logging_loki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/logging_loki/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/logging_loki/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/logging_loki/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/logging_loki/json_loki_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/logging_loki/log_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/logging_loki/loki_context_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/logging_loki/loki_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:06:43.670477 inuits_python_logging_loki-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:06:43.670477 inuits_python_logging_loki-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-08 12:06:38.000000 inuits_python_logging_loki-1.3.0/tests/test_emitter_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:59:15.641526 inuits_python_logging_loki-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-08 12:59:15.641526 inuits_python_logging_loki-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:59:15.641526 inuits_python_logging_loki-1.4.0/inuits_python_logging_loki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-08 12:59:15.000000 inuits_python_logging_loki-1.4.0/inuits_python_logging_loki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 12:59:15.000000 inuits_python_logging_loki-1.4.0/inuits_python_logging_loki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:59:15.000000 inuits_python_logging_loki-1.4.0/inuits_python_logging_loki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 12:59:15.000000 inuits_python_logging_loki-1.4.0/inuits_python_logging_loki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 12:59:15.000000 inuits_python_logging_loki-1.4.0/inuits_python_logging_loki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:59:15.641526 inuits_python_logging_loki-1.4.0/logging_loki/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/logging_loki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/logging_loki/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/logging_loki/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/logging_loki/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/logging_loki/json_loki_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/logging_loki/log_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/logging_loki/loki_context_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/logging_loki/loki_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:59:15.641526 inuits_python_logging_loki-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:59:15.641526 inuits_python_logging_loki-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-08 12:59:10.000000 inuits_python_logging_loki-1.4.0/tests/test_emitter_v1.py
```

### Comparing `inuits_python_logging_loki-1.3.0/LICENSE` & `inuits_python_logging_loki-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.3.0/PKG-INFO` & `inuits_python_logging_loki-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-python-logging-loki
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python logging handler for Grafana Loki.
 Author-email: Inuits <developers@inuits.eu>, Andrey Maslov <greyzmeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Andrey Maslov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `inuits_python_logging_loki-1.3.0/README.md` & `inuits_python_logging_loki-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.3.0/inuits_python_logging_loki.egg-info/PKG-INFO` & `inuits_python_logging_loki-1.4.0/inuits_python_logging_loki.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-python-logging-loki
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python logging handler for Grafana Loki.
 Author-email: Inuits <developers@inuits.eu>, Andrey Maslov <greyzmeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Andrey Maslov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `inuits_python_logging_loki-1.3.0/inuits_python_logging_loki.egg-info/SOURCES.txt` & `inuits_python_logging_loki-1.4.0/inuits_python_logging_loki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.3.0/logging_loki/const.py` & `inuits_python_logging_loki-1.4.0/logging_loki/const.py`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.3.0/logging_loki/emitter.py` & `inuits_python_logging_loki-1.4.0/logging_loki/emitter.py`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.3.0/logging_loki/handlers.py` & `inuits_python_logging_loki-1.4.0/logging_loki/handlers.py`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.3.0/logging_loki/json_loki_logger.py` & `inuits_python_logging_loki-1.4.0/logging_loki/json_loki_logger.py`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.3.0/logging_loki/loki_context_logger.py` & `inuits_python_logging_loki-1.4.0/logging_loki/loki_context_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,24 +12,24 @@
         tags.update(log_context.get_tags())
         log_func = getattr(self.logger, level)
         if level == "exception":
             log_func(log_context.to_string(), tags, exc_info=exc_info)
         else:
             log_func(log_context.to_string(), tags)
 
-    def debug(self, message, code=None, log_context=None):
+    def debug(self, message, log_context=None, code=None):
         self._log('debug', message, code, log_context)
 
-    def info(self, message, code=None, log_context=None):
+    def info(self, message, log_context=None, code=None):
         self._log('info', message, code, log_context)
 
-    def warning(self, message, code=None, log_context=None):
+    def warning(self, message, log_context=None, code=None):
         self._log('warning', message, code, log_context)
 
-    def error(self, message, code=None, log_context=None):
+    def error(self, message, log_context=None, code=None):
         self._log('error', message, code, log_context)
 
-    def critical(self, message, code=None, log_context=None):
+    def critical(self, message, log_context=None, code=None):
         self._log('critical', message, code, log_context)
 
-    def exception(self, message, exc_info=None, code=None, log_context=None):
+    def exception(self, message, exc_info=None, log_context=None, code=None):
         self._log('exception', message, code, log_context, exc_info)
```

### Comparing `inuits_python_logging_loki-1.3.0/logging_loki/loki_logger.py` & `inuits_python_logging_loki-1.4.0/logging_loki/loki_logger.py`

 * *Files identical despite different names*

### Comparing `inuits_python_logging_loki-1.3.0/pyproject.toml` & `inuits_python_logging_loki-1.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=59.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inuits-python-logging-loki"
-version = "1.3.0"
+version = "1.4.0"
 description = "Python logging handler for Grafana Loki."
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }, {name="Andrey Maslov", email="greyzmeem@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

### Comparing `inuits_python_logging_loki-1.3.0/tests/test_emitter_v1.py` & `inuits_python_logging_loki-1.4.0/tests/test_emitter_v1.py`

 * *Files identical despite different names*

