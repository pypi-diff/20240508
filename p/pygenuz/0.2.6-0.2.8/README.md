# Comparing `tmp/pygenuz-0.2.6.tar.gz` & `tmp/pygenuz-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenuz-0.2.6.tar", last modified: Wed May  8 10:53:22 2024, max compression
+gzip compressed data, was "pygenuz-0.2.8.tar", last modified: Wed May  8 10:58:08 2024, max compression
```

## Comparing `pygenuz-0.2.6.tar` & `pygenuz-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 10:53:22.023335 pygenuz-0.2.6/
--rw-r--r--   0 khezozbek   (501) staff       (20)     7042 2024-05-08 10:53:22.023204 pygenuz-0.2.6/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)     6411 2024-05-07 17:58:23.000000 pygenuz-0.2.6/README.md
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 10:53:22.022070 pygenuz-0.2.6/pygenuz/
--rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.2.6/pygenuz/__init__.py
--rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.2.6/pygenuz/app.py
--rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.2.6/pygenuz/configs.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.2.6/pygenuz/db.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.2.6/pygenuz/middelware.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.2.6/pygenuz/response.py
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 10:53:22.022997 pygenuz-0.2.6/pygenuz.egg-info/
--rw-r--r--   0 khezozbek   (501) staff       (20)     7042 2024-05-08 10:53:21.000000 pygenuz-0.2.6/pygenuz.egg-info/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-08 10:53:21.000000 pygenuz-0.2.6/pygenuz.egg-info/SOURCES.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-08 10:53:21.000000 pygenuz-0.2.6/pygenuz.egg-info/dependency_links.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-08 10:53:21.000000 pygenuz-0.2.6/pygenuz.egg-info/requires.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-08 10:53:21.000000 pygenuz-0.2.6/pygenuz.egg-info/top_level.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-08 10:53:22.023388 pygenuz-0.2.6/setup.cfg
--rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-08 10:53:14.000000 pygenuz-0.2.6/setup.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 10:58:08.827525 pygenuz-0.2.8/
+-rw-r--r--   0 khezozbek   (501) staff       (20)     7042 2024-05-08 10:58:08.827398 pygenuz-0.2.8/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)     6411 2024-05-07 17:58:23.000000 pygenuz-0.2.8/README.md
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 10:58:08.826289 pygenuz-0.2.8/pygenuz/
+-rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.2.8/pygenuz/__init__.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.2.8/pygenuz/app.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.2.8/pygenuz/configs.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.2.8/pygenuz/db.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.2.8/pygenuz/middelware.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.2.8/pygenuz/response.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 10:58:08.827160 pygenuz-0.2.8/pygenuz.egg-info/
+-rw-r--r--   0 khezozbek   (501) staff       (20)     7042 2024-05-08 10:58:08.000000 pygenuz-0.2.8/pygenuz.egg-info/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-08 10:58:08.000000 pygenuz-0.2.8/pygenuz.egg-info/SOURCES.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-08 10:58:08.000000 pygenuz-0.2.8/pygenuz.egg-info/dependency_links.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-08 10:58:08.000000 pygenuz-0.2.8/pygenuz.egg-info/requires.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-08 10:58:08.000000 pygenuz-0.2.8/pygenuz.egg-info/top_level.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-08 10:58:08.827577 pygenuz-0.2.8/setup.cfg
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-08 10:57:32.000000 pygenuz-0.2.8/setup.py
```

### Comparing `pygenuz-0.2.6/PKG-INFO` & `pygenuz-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.2.6
+Version: 0.2.8
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygenuz-0.2.6/README.md` & `pygenuz-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.6/pygenuz/app.py` & `pygenuz-0.2.8/pygenuz/app.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.6/pygenuz/middelware.py` & `pygenuz-0.2.8/pygenuz/middelware.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.6/pygenuz/response.py` & `pygenuz-0.2.8/pygenuz/response.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.6/pygenuz.egg-info/PKG-INFO` & `pygenuz-0.2.8/pygenuz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.2.6
+Version: 0.2.8
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygenuz-0.2.6/setup.py` & `pygenuz-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pygenuz'
 DESCRIPTION = 'My first Python web framework.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'cssezozbel@gmail.com'
 AUTHOR = "E'zozbek Kholbutayev"
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.2.6'
+VERSION = '0.2.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

