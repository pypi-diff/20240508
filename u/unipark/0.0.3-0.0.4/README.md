# Comparing `tmp/unipark-0.0.3.tar.gz` & `tmp/unipark-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/parklam/workspace/python/common/dist/tmphqvp_5o9/unipark-0.0.3.tar", last modified: Tue Jan  2 15:02:23 2024, max compression
+gzip compressed data, was "unipark-0.0.4.tar", last modified: Wed May  8 16:41:32 2024, max compression
```

## Comparing `unipark-0.0.3.tar` & `unipark-0.0.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-01-02 15:02:23.429907 unipark-0.0.3/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      131 2023-10-12 11:57:58.000000 unipark-0.0.3/MANIFEST.in
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      334 2024-01-02 15:02:23.429907 unipark-0.0.3/PKG-INFO
--rw-rw-r--   0 parklam   (1000) parklam   (1000)       83 2023-10-07 03:22:37.000000 unipark-0.0.3/README.md
--rw-rw-r--   0 parklam   (1000) parklam   (1000)        6 2024-01-02 15:01:43.000000 unipark-0.0.3/VERSION
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      138 2023-10-17 06:13:44.000000 unipark-0.0.3/pyproject.toml
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-01-02 15:02:23.421908 unipark-0.0.3/requirements/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      113 2023-10-11 19:05:16.000000 unipark-0.0.3/requirements/runtime.txt
--rw-rw-r--   0 parklam   (1000) parklam   (1000)       38 2024-01-02 15:02:23.429907 unipark-0.0.3/setup.cfg
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     1722 2023-10-13 05:37:26.000000 unipark-0.0.3/setup.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-01-02 15:02:23.425907 unipark-0.0.3/tests/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      144 2023-10-31 19:27:19.000000 unipark-0.0.3/tests/__init__.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      609 2023-10-16 05:05:16.000000 unipark-0.0.3/tests/test_cli.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     2808 2023-10-13 07:00:36.000000 unipark-0.0.3/tests/test_config.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     9632 2023-10-30 12:15:00.000000 unipark-0.0.3/tests/test_mvc.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      630 2023-10-13 05:15:16.000000 unipark-0.0.3/tests/test_requests.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     1093 2023-10-13 05:34:55.000000 unipark-0.0.3/tests/test_utils.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-01-02 15:02:23.425907 unipark-0.0.3/unipark/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      795 2023-10-17 06:21:08.000000 unipark-0.0.3/unipark/__init__.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-01-02 15:02:23.425907 unipark-0.0.3/unipark/cli/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      545 2023-10-13 07:10:19.000000 unipark-0.0.3/unipark/cli/__init__.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      963 2023-10-12 08:17:57.000000 unipark-0.0.3/unipark/config.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-01-02 15:02:23.429907 unipark-0.0.3/unipark/mvc/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     5808 2023-10-31 05:02:40.000000 unipark-0.0.3/unipark/mvc/__init__.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      824 2023-10-31 19:27:19.000000 unipark-0.0.3/unipark/mvc/command.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     2329 2023-10-16 03:57:36.000000 unipark-0.0.3/unipark/mvc/facade.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     1237 2023-10-31 19:29:36.000000 unipark-0.0.3/unipark/mvc/mediator.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     1672 2023-10-31 19:27:19.000000 unipark-0.0.3/unipark/mvc/observer.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      737 2023-10-31 19:27:19.000000 unipark-0.0.3/unipark/mvc/proxy.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     4363 2023-10-13 05:13:35.000000 unipark-0.0.3/unipark/requests.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-01-02 15:02:23.429907 unipark-0.0.3/unipark/utils/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     2863 2023-10-31 19:27:19.000000 unipark-0.0.3/unipark/utils/__init__.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     6364 2023-10-07 10:19:42.000000 unipark-0.0.3/unipark/utils/log.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     1381 2023-12-03 06:41:23.000000 unipark-0.0.3/unipark/utils/translation.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)       47 2024-01-02 15:02:20.000000 unipark-0.0.3/unipark/version.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-01-02 15:02:23.425907 unipark-0.0.3/unipark.egg-info/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      334 2024-01-02 15:02:22.000000 unipark-0.0.3/unipark.egg-info/PKG-INFO
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      699 2024-01-02 15:02:23.000000 unipark-0.0.3/unipark.egg-info/SOURCES.txt
--rw-rw-r--   0 parklam   (1000) parklam   (1000)        1 2024-01-02 15:02:22.000000 unipark-0.0.3/unipark.egg-info/dependency_links.txt
--rw-rw-r--   0 parklam   (1000) parklam   (1000)       41 2024-01-02 15:02:22.000000 unipark-0.0.3/unipark.egg-info/entry_points.txt
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      113 2024-01-02 15:02:23.000000 unipark-0.0.3/unipark.egg-info/requires.txt
--rw-rw-r--   0 parklam   (1000) parklam   (1000)        8 2024-01-02 15:02:23.000000 unipark-0.0.3/unipark.egg-info/top_level.txt
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.039103 unipark-0.0.4/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      131 2023-10-12 11:57:58.000000 unipark-0.0.4/MANIFEST.in
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      334 2024-05-08 16:41:32.035103 unipark-0.0.4/PKG-INFO
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)       83 2023-10-07 03:22:37.000000 unipark-0.0.4/README.md
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)        6 2024-05-08 14:10:40.000000 unipark-0.0.4/VERSION
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      138 2023-10-17 06:13:44.000000 unipark-0.0.4/pyproject.toml
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.027103 unipark-0.0.4/requirements/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      113 2023-10-11 19:05:16.000000 unipark-0.0.4/requirements/runtime.txt
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)       38 2024-05-08 16:41:32.039103 unipark-0.0.4/setup.cfg
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1722 2023-10-13 05:37:26.000000 unipark-0.0.4/setup.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.031103 unipark-0.0.4/tests/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      144 2023-10-31 19:27:19.000000 unipark-0.0.4/tests/__init__.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      609 2023-10-16 05:05:16.000000 unipark-0.0.4/tests/test_cli.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     2796 2024-05-08 14:04:13.000000 unipark-0.0.4/tests/test_config.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     9632 2023-10-30 12:15:00.000000 unipark-0.0.4/tests/test_mvc.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      630 2023-10-13 05:15:16.000000 unipark-0.0.4/tests/test_requests.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1093 2023-10-13 05:34:55.000000 unipark-0.0.4/tests/test_utils.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.031103 unipark-0.0.4/unipark/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      795 2023-10-17 06:21:08.000000 unipark-0.0.4/unipark/__init__.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.035103 unipark-0.0.4/unipark/cli/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      545 2023-10-13 07:10:19.000000 unipark-0.0.4/unipark/cli/__init__.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1334 2024-05-08 14:01:37.000000 unipark-0.0.4/unipark/config.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.035103 unipark-0.0.4/unipark/mvc/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     5808 2023-10-31 05:02:40.000000 unipark-0.0.4/unipark/mvc/__init__.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      824 2023-10-31 19:27:19.000000 unipark-0.0.4/unipark/mvc/command.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     2329 2023-10-16 03:57:36.000000 unipark-0.0.4/unipark/mvc/facade.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1237 2023-10-31 19:29:36.000000 unipark-0.0.4/unipark/mvc/mediator.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1672 2023-10-31 19:27:19.000000 unipark-0.0.4/unipark/mvc/observer.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      737 2023-10-31 19:27:19.000000 unipark-0.0.4/unipark/mvc/proxy.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     4363 2023-10-13 05:13:35.000000 unipark-0.0.4/unipark/requests.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.035103 unipark-0.0.4/unipark/utils/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     2863 2023-10-31 19:27:19.000000 unipark-0.0.4/unipark/utils/__init__.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     6364 2023-10-07 10:19:42.000000 unipark-0.0.4/unipark/utils/log.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1381 2023-12-03 06:41:23.000000 unipark-0.0.4/unipark/utils/translation.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)       47 2024-05-08 16:41:29.000000 unipark-0.0.4/unipark/version.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.035103 unipark-0.0.4/unipark.egg-info/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      334 2024-05-08 16:41:30.000000 unipark-0.0.4/unipark.egg-info/PKG-INFO
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      699 2024-05-08 16:41:32.000000 unipark-0.0.4/unipark.egg-info/SOURCES.txt
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)        1 2024-05-08 16:41:30.000000 unipark-0.0.4/unipark.egg-info/dependency_links.txt
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)       41 2024-05-08 16:41:31.000000 unipark-0.0.4/unipark.egg-info/entry_points.txt
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      113 2024-05-08 16:41:31.000000 unipark-0.0.4/unipark.egg-info/requires.txt
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)        8 2024-05-08 16:41:31.000000 unipark-0.0.4/unipark.egg-info/top_level.txt
```

### Comparing `unipark-0.0.3/setup.py` & `unipark-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/tests/test_cli.py` & `unipark-0.0.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/tests/test_config.py` & `unipark-0.0.4/tests/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     def tearDown(self):
         pass
 
     def test_001_retrieve_option_by_attribute(self):
         init_dotenv()
 
         self.assertEqual(settings.DEBUG, True)
-        self.assertEqual(settings.VAR_INTEGER, '8')
-        self.assertEqual(settings.VAR_FLOAT, '8.88')
+        self.assertEqual(settings.VAR_INTEGER, 8)
+        self.assertEqual(settings.VAR_FLOAT, 8.88)
         self.assertEqual(settings.VAR_STRING, 'string from ".env"')
 
     def test_002_retrieve_option_by_get(self):
         init_dotenv()
 
         self.assertEqual(settings('DEBUG', cast=bool), True)
         self.assertEqual(settings('VAR_INTEGER', cast=int), 8)
@@ -77,17 +77,17 @@
         self.assertEqual(settings('VAR_INTEGER', cast=int), 6)
         self.assertEqual(settings('VAR_FLOAT', cast=float), 6.66)
         self.assertEqual(settings('VAR_STRING'), 'string from "os.environ"')
 
     def test_004_reload_dotenv(self):
         init_dotenv()
         self.assertEqual(settings.DEBUG, True)
-        self.assertEqual(settings.VAR_INTEGER, '8')
-        self.assertEqual(settings.VAR_FLOAT, '8.88')
+        self.assertEqual(settings.VAR_INTEGER, 8)
+        self.assertEqual(settings.VAR_FLOAT, 8.88)
         self.assertEqual(settings.VAR_STRING, 'string from ".env"')
 
         override_dotenv()
         settings.reload()
         self.assertEqual(settings.DEBUG, False)
-        self.assertEqual(settings.VAR_INTEGER, '6')
-        self.assertEqual(settings.VAR_FLOAT, '6.66')
+        self.assertEqual(settings.VAR_INTEGER, 6)
+        self.assertEqual(settings.VAR_FLOAT, 6.66)
         self.assertEqual(settings.VAR_STRING, 'string from ".env(override)"')
```

### Comparing `unipark-0.0.3/tests/test_mvc.py` & `unipark-0.0.4/tests/test_mvc.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/tests/test_requests.py` & `unipark-0.0.4/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/tests/test_utils.py` & `unipark-0.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/__init__.py` & `unipark-0.0.4/unipark/__init__.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/cli/__init__.py` & `unipark-0.0.4/unipark/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/config.py` & `unipark-0.0.4/unipark/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,24 +10,36 @@
 class Settings(object):
     auto_cast = True
 
     def __getattr__(self, item):
         if item in dir(self):
             return super().__getattr__(item)
         else:
-            return self._retrieve_option_from_config(item)
+            try:
+                return self._retrieve_option_from_config(item)
+            except decouple.UndefinedValueError as e:
+                raise AttributeError(str(e))
 
     def _retrieve_option_from_config(self, *args, **kwargs):
         option = decouple.config(*args, **kwargs)
         if self.auto_cast and \
-                isinstance(option, str) and \
-                option.upper() in ( 'TRUE', 'FALSE', ):
-            return option.upper() == 'TRUE'
-        else:
-            return option
+                isinstance(option, str):
+            if option.upper() in ( 'TRUE', 'FALSE', ):
+                return option.upper() == 'TRUE'
+            else:
+                try:
+                    return int(option)
+                except ValueError as e:
+                    pass
+                try:
+                    return float(option)
+                except ValueError as e:
+                    pass
+        return option
+
 
     def __call__(self, *args, **kwargs):
         if kwargs.get('force_reload', False):
             self.reload()
         return self._retrieve_option_from_config(*args, **kwargs)
 
     def reload(self):
```

### Comparing `unipark-0.0.3/unipark/mvc/__init__.py` & `unipark-0.0.4/unipark/mvc/__init__.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/mvc/command.py` & `unipark-0.0.4/unipark/mvc/command.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/mvc/facade.py` & `unipark-0.0.4/unipark/mvc/facade.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/mvc/mediator.py` & `unipark-0.0.4/unipark/mvc/mediator.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/mvc/observer.py` & `unipark-0.0.4/unipark/mvc/observer.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/mvc/proxy.py` & `unipark-0.0.4/unipark/mvc/proxy.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/requests.py` & `unipark-0.0.4/unipark/requests.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/utils/__init__.py` & `unipark-0.0.4/unipark/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/utils/log.py` & `unipark-0.0.4/unipark/utils/log.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark/utils/translation.py` & `unipark-0.0.4/unipark/utils/translation.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.3/unipark.egg-info/SOURCES.txt` & `unipark-0.0.4/unipark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

