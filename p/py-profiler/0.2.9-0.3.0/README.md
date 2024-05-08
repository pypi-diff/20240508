# Comparing `tmp/py_profiler-0.2.9.tar.gz` & `tmp/py_profiler-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_profiler-0.2.9.tar", last modified: Wed May  8 17:57:10 2024, max compression
+gzip compressed data, was "py_profiler-0.3.0.tar", last modified: Wed May  8 18:11:39 2024, max compression
```

## Comparing `py_profiler-0.2.9.tar` & `py_profiler-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 17:57:10.635984 py_profiler-0.2.9/
--rw-r--r--   0 andy       (501) staff       (20)     1073 2023-02-02 15:54:28.000000 py_profiler-0.2.9/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)       50 2023-02-02 15:54:28.000000 py_profiler-0.2.9/MANIFEST.in
--rw-r--r--   0 andy       (501) staff       (20)     3725 2024-05-08 17:57:10.635669 py_profiler-0.2.9/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     3120 2024-03-14 09:41:54.000000 py_profiler-0.2.9/README.md
--rw-r--r--   0 andy       (501) staff       (20)      141 2024-05-08 17:44:24.000000 py_profiler-0.2.9/pyproject.toml
--rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-08 17:57:10.636079 py_profiler-0.2.9/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)      922 2024-05-08 17:44:52.000000 py_profiler-0.2.9/setup.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 17:57:10.629814 py_profiler-0.2.9/src/
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 17:57:10.633175 py_profiler-0.2.9/src/py_profiler/
--rw-r--r--   0 andy       (501) staff       (20)       79 2023-02-02 15:54:28.000000 py_profiler-0.2.9/src/py_profiler/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1487 2024-05-08 17:55:54.000000 py_profiler-0.2.9/src/py_profiler/decorator.py
--rw-r--r--   0 andy       (501) staff       (20)      330 2024-03-15 15:55:53.000000 py_profiler-0.2.9/src/py_profiler/fastapi_profiler_controller.py
--rw-r--r--   0 andy       (501) staff       (20)      522 2023-02-02 15:54:28.000000 py_profiler-0.2.9/src/py_profiler/long_adder.py
--rw-r--r--   0 andy       (501) staff       (20)     5555 2024-03-14 09:41:54.000000 py_profiler-0.2.9/src/py_profiler/measure_service.py
--rw-r--r--   0 andy       (501) staff       (20)      260 2024-03-14 09:41:54.000000 py_profiler-0.2.9/src/py_profiler/profiler_controller.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 17:57:10.634513 py_profiler-0.2.9/src/py_profiler/templates/
--rw-r--r--   0 andy       (501) staff       (20)     3337 2024-05-06 07:17:48.000000 py_profiler-0.2.9/src/py_profiler/templates/profiler.html
--rw-r--r--   0 andy       (501) staff       (20)      743 2023-02-02 15:54:28.000000 py_profiler-0.2.9/src/py_profiler/utils.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 17:57:10.635160 py_profiler-0.2.9/src/py_profiler.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)     3725 2024-05-08 17:57:10.000000 py_profiler-0.2.9/src/py_profiler.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      520 2024-05-08 17:57:10.000000 py_profiler-0.2.9/src/py_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-08 17:57:10.000000 py_profiler-0.2.9/src/py_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       30 2024-05-08 17:57:10.000000 py_profiler-0.2.9/src/py_profiler.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)       12 2024-05-08 17:57:10.000000 py_profiler-0.2.9/src/py_profiler.egg-info/top_level.txt
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 18:11:39.898991 py_profiler-0.3.0/
+-rw-r--r--   0 andy       (501) staff       (20)     1073 2023-02-02 15:54:28.000000 py_profiler-0.3.0/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)       50 2023-02-02 15:54:28.000000 py_profiler-0.3.0/MANIFEST.in
+-rw-r--r--   0 andy       (501) staff       (20)     3725 2024-05-08 18:11:39.898700 py_profiler-0.3.0/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     3120 2024-03-14 09:41:54.000000 py_profiler-0.3.0/README.md
+-rw-r--r--   0 andy       (501) staff       (20)      141 2024-05-08 17:44:24.000000 py_profiler-0.3.0/pyproject.toml
+-rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-08 18:11:39.899058 py_profiler-0.3.0/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)      922 2024-05-08 18:11:06.000000 py_profiler-0.3.0/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 18:11:39.893853 py_profiler-0.3.0/src/
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 18:11:39.897213 py_profiler-0.3.0/src/py_profiler/
+-rw-r--r--   0 andy       (501) staff       (20)       79 2023-02-02 15:54:28.000000 py_profiler-0.3.0/src/py_profiler/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     1456 2024-05-08 18:09:42.000000 py_profiler-0.3.0/src/py_profiler/decorator.py
+-rw-r--r--   0 andy       (501) staff       (20)      330 2024-03-15 15:55:53.000000 py_profiler-0.3.0/src/py_profiler/fastapi_profiler_controller.py
+-rw-r--r--   0 andy       (501) staff       (20)      522 2023-02-02 15:54:28.000000 py_profiler-0.3.0/src/py_profiler/long_adder.py
+-rw-r--r--   0 andy       (501) staff       (20)     5555 2024-03-14 09:41:54.000000 py_profiler-0.3.0/src/py_profiler/measure_service.py
+-rw-r--r--   0 andy       (501) staff       (20)      260 2024-03-14 09:41:54.000000 py_profiler-0.3.0/src/py_profiler/profiler_controller.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 18:11:39.898075 py_profiler-0.3.0/src/py_profiler/templates/
+-rw-r--r--   0 andy       (501) staff       (20)     3337 2024-05-06 07:17:48.000000 py_profiler-0.3.0/src/py_profiler/templates/profiler.html
+-rw-r--r--   0 andy       (501) staff       (20)      743 2023-02-02 15:54:28.000000 py_profiler-0.3.0/src/py_profiler/utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 18:11:39.898395 py_profiler-0.3.0/src/py_profiler.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)     3725 2024-05-08 18:11:39.000000 py_profiler-0.3.0/src/py_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      520 2024-05-08 18:11:39.000000 py_profiler-0.3.0/src/py_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-08 18:11:39.000000 py_profiler-0.3.0/src/py_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       30 2024-05-08 18:11:39.000000 py_profiler-0.3.0/src/py_profiler.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)       12 2024-05-08 18:11:39.000000 py_profiler-0.3.0/src/py_profiler.egg-info/top_level.txt
```

### Comparing `py_profiler-0.2.9/LICENSE` & `py_profiler-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.9/PKG-INFO` & `py_profiler-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_profiler
-Version: 0.2.9
+Version: 0.3.0
 Summary: A library to measure your method, function execution time.
 Home-page: https://github.com/andy1xx8/py-profiler
 Author: Andy Le
 Author-email: tauit.dnmd@gmail.com
 Project-URL: Bug Tracker, https://github.com/andy1xx8/py-profiler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py_profiler-0.2.9/README.md` & `py_profiler-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.9/setup.py` & `py_profiler-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_profiler",
-    version="0.2.9",
+    version="0.3.0",
     author="Andy Le",
     author_email="tauit.dnmd@gmail.com",
     description="A library to measure your method, function execution time.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andy1xx8/py-profiler",
     project_urls={
```

### Comparing `py_profiler-0.2.9/src/py_profiler/decorator.py` & `py_profiler-0.3.0/src/py_profiler/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
             finally:
                 profiling_service.stop_measure(
                     func_name,
                     time.time() * 1000_000_000 - begin_time,
                     is_error=is_error
                 )
 
-        @functools.wraps(func)
         def wrapper(*args, **kwargs):
             if name is None:
                 try:
                     func_name = func.__func__.__qualname__
                 except:
                     func_name = func.__qualname__
             else:
```

### Comparing `py_profiler-0.2.9/src/py_profiler/long_adder.py` & `py_profiler-0.3.0/src/py_profiler/long_adder.py`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.9/src/py_profiler/measure_service.py` & `py_profiler-0.3.0/src/py_profiler/measure_service.py`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.9/src/py_profiler/templates/profiler.html` & `py_profiler-0.3.0/src/py_profiler/templates/profiler.html`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.9/src/py_profiler/utils.py` & `py_profiler-0.3.0/src/py_profiler/utils.py`

 * *Files identical despite different names*

### Comparing `py_profiler-0.2.9/src/py_profiler.egg-info/PKG-INFO` & `py_profiler-0.3.0/src/py_profiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_profiler
-Version: 0.2.9
+Version: 0.3.0
 Summary: A library to measure your method, function execution time.
 Home-page: https://github.com/andy1xx8/py-profiler
 Author: Andy Le
 Author-email: tauit.dnmd@gmail.com
 Project-URL: Bug Tracker, https://github.com/andy1xx8/py-profiler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py_profiler-0.2.9/src/py_profiler.egg-info/SOURCES.txt` & `py_profiler-0.3.0/src/py_profiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

