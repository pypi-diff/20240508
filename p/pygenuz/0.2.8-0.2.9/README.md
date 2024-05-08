# Comparing `tmp/pygenuz-0.2.8.tar.gz` & `tmp/pygenuz-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenuz-0.2.8.tar", last modified: Wed May  8 10:58:08 2024, max compression
+gzip compressed data, was "pygenuz-0.2.9.tar", last modified: Wed May  8 11:01:52 2024, max compression
```

## Comparing `pygenuz-0.2.8.tar` & `pygenuz-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 10:58:08.827525 pygenuz-0.2.8/
--rw-r--r--   0 khezozbek   (501) staff       (20)     7042 2024-05-08 10:58:08.827398 pygenuz-0.2.8/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)     6411 2024-05-07 17:58:23.000000 pygenuz-0.2.8/README.md
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 10:58:08.826289 pygenuz-0.2.8/pygenuz/
--rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.2.8/pygenuz/__init__.py
--rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.2.8/pygenuz/app.py
--rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.2.8/pygenuz/configs.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.2.8/pygenuz/db.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.2.8/pygenuz/middelware.py
--rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.2.8/pygenuz/response.py
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 10:58:08.827160 pygenuz-0.2.8/pygenuz.egg-info/
--rw-r--r--   0 khezozbek   (501) staff       (20)     7042 2024-05-08 10:58:08.000000 pygenuz-0.2.8/pygenuz.egg-info/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-08 10:58:08.000000 pygenuz-0.2.8/pygenuz.egg-info/SOURCES.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-08 10:58:08.000000 pygenuz-0.2.8/pygenuz.egg-info/dependency_links.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-08 10:58:08.000000 pygenuz-0.2.8/pygenuz.egg-info/requires.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-08 10:58:08.000000 pygenuz-0.2.8/pygenuz.egg-info/top_level.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-08 10:58:08.827577 pygenuz-0.2.8/setup.cfg
--rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-08 10:57:32.000000 pygenuz-0.2.8/setup.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 11:01:52.267016 pygenuz-0.2.9/
+-rw-r--r--   0 khezozbek   (501) staff       (20)     7069 2024-05-08 11:01:52.266852 pygenuz-0.2.9/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)     6438 2024-05-08 11:00:23.000000 pygenuz-0.2.9/README.md
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 11:01:52.265672 pygenuz-0.2.9/pygenuz/
+-rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-07 07:34:41.000000 pygenuz-0.2.9/pygenuz/__init__.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3787 2024-05-07 15:58:04.000000 pygenuz-0.2.9/pygenuz/app.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)       86 2024-05-07 16:18:44.000000 pygenuz-0.2.9/pygenuz/configs.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      201 2024-05-07 16:08:54.000000 pygenuz-0.2.9/pygenuz/db.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.2.9/pygenuz/middelware.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.2.9/pygenuz/response.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-08 11:01:52.266595 pygenuz-0.2.9/pygenuz.egg-info/
+-rw-r--r--   0 khezozbek   (501) staff       (20)     7069 2024-05-08 11:01:52.000000 pygenuz-0.2.9/pygenuz.egg-info/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)      282 2024-05-08 11:01:52.000000 pygenuz-0.2.9/pygenuz.egg-info/SOURCES.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-08 11:01:52.000000 pygenuz-0.2.9/pygenuz.egg-info/dependency_links.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)      116 2024-05-08 11:01:52.000000 pygenuz-0.2.9/pygenuz.egg-info/requires.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-08 11:01:52.000000 pygenuz-0.2.9/pygenuz.egg-info/top_level.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-08 11:01:52.267074 pygenuz-0.2.9/setup.cfg
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3912 2024-05-08 11:01:47.000000 pygenuz-0.2.9/setup.py
```

### Comparing `pygenuz-0.2.8/PKG-INFO` & `pygenuz-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.2.8
+Version: 0.2.9
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 
 
 # PyGenUz: Python Web Framewrok build for learning purposes
 
-![purpose](https://img.shields.io/badge/purpose-learning-green)
+![purpose](https://img.shields.io/badge/purpose-learning-and-building-green)
 ![PyPI Version](https://img.shields.io/pypi/v/pygenuz)
 
-PyGenUz is a Python web framewrok built for learning purposes.
+PyGenUz is a Python web framewrok built for learning and building purposes.
 
 It's a WSGI framework and can be used with any WSGI aplication server such as Gunicorn.
 
 ## Installation
 ```shell
 pip install pygenuz
 ```
@@ -262,7 +262,8 @@
     session.delete(book)
     session.commit()
     response.text = "Book deleted successfully"
 ```
 
 # EVERY MONDAY YOU WILL SEE A NEW BIG UPDATE UNTIL V1.0.0 
 
+
```

### Comparing `pygenuz-0.2.8/README.md` & `pygenuz-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PyGenUz: Python Web Framewrok build for learning purposes
 
-![purpose](https://img.shields.io/badge/purpose-learning-green)
+![purpose](https://img.shields.io/badge/purpose-learning-and-building-green)
 ![PyPI Version](https://img.shields.io/pypi/v/pygenuz)
 
-PyGenUz is a Python web framewrok built for learning purposes.
+PyGenUz is a Python web framewrok built for learning and building purposes.
 
 It's a WSGI framework and can be used with any WSGI aplication server such as Gunicorn.
 
 ## Installation
 ```shell
 pip install pygenuz
 ```
@@ -241,8 +241,8 @@
         response.status_code = 404
         return
     session.delete(book)
     session.commit()
     response.text = "Book deleted successfully"
 ```
 
-# EVERY MONDAY YOU WILL SEE A NEW BIG UPDATE UNTIL V1.0.0 
+# EVERY MONDAY YOU WILL SEE A NEW BIG UPDATE UNTIL V1.0.0
```

### Comparing `pygenuz-0.2.8/pygenuz/app.py` & `pygenuz-0.2.9/pygenuz/app.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.8/pygenuz/middelware.py` & `pygenuz-0.2.9/pygenuz/middelware.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.8/pygenuz/response.py` & `pygenuz-0.2.9/pygenuz/response.py`

 * *Files identical despite different names*

### Comparing `pygenuz-0.2.8/pygenuz.egg-info/PKG-INFO` & `pygenuz-0.2.9/pygenuz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.2.8
+Version: 0.2.9
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 
 
 # PyGenUz: Python Web Framewrok build for learning purposes
 
-![purpose](https://img.shields.io/badge/purpose-learning-green)
+![purpose](https://img.shields.io/badge/purpose-learning-and-building-green)
 ![PyPI Version](https://img.shields.io/pypi/v/pygenuz)
 
-PyGenUz is a Python web framewrok built for learning purposes.
+PyGenUz is a Python web framewrok built for learning and building purposes.
 
 It's a WSGI framework and can be used with any WSGI aplication server such as Gunicorn.
 
 ## Installation
 ```shell
 pip install pygenuz
 ```
@@ -262,7 +262,8 @@
     session.delete(book)
     session.commit()
     response.text = "Book deleted successfully"
 ```
 
 # EVERY MONDAY YOU WILL SEE A NEW BIG UPDATE UNTIL V1.0.0 
 
+
```

### Comparing `pygenuz-0.2.8/setup.py` & `pygenuz-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pygenuz'
 DESCRIPTION = 'My first Python web framework.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'cssezozbel@gmail.com'
 AUTHOR = "E'zozbek Kholbutayev"
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.2.8'
+VERSION = '0.2.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

