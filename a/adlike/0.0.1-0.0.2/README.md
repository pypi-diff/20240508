# Comparing `tmp/adlike-0.0.1.tar.gz` & `tmp/adlike-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adlike-0.0.1.tar", last modified: Thu Apr 25 09:28:22 2024, max compression
+gzip compressed data, was "adlike-0.0.2.tar", last modified: Wed May  8 13:40:16 2024, max compression
```

## Comparing `adlike-0.0.1.tar` & `adlike-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-04-25 09:28:22.393245 adlike-0.0.1/
--rw-r--r--   0 reeteshmukul   (501) staff       (20)     1098 2024-04-25 09:28:22.392891 adlike-0.0.1/PKG-INFO
--rw-r--r--   0 reeteshmukul   (501) staff       (20)      580 2024-04-25 09:08:50.000000 adlike-0.0.1/README.md
--rw-r--r--   0 reeteshmukul   (501) staff       (20)      609 2024-04-23 15:34:18.000000 adlike-0.0.1/pyproject.toml
--rw-r--r--   0 reeteshmukul   (501) staff       (20)       38 2024-04-25 09:28:22.393321 adlike-0.0.1/setup.cfg
-drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-04-25 09:28:22.389574 adlike-0.0.1/src/
--rw-r--r--   0 reeteshmukul   (501) staff       (20)        0 2024-04-17 12:03:13.000000 adlike-0.0.1/src/__init__.py
-drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-04-25 09:28:22.390598 adlike-0.0.1/src/adlike/
--rw-r--r--   0 reeteshmukul   (501) staff       (20)       21 2024-04-17 12:03:08.000000 adlike-0.0.1/src/adlike/__init__.py
--rw-r--r--   0 reeteshmukul   (501) staff       (20)     4583 2024-04-25 09:07:37.000000 adlike-0.0.1/src/adlike/adlike.py
-drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-04-25 09:28:22.392540 adlike-0.0.1/src/adlike.egg-info/
--rw-r--r--   0 reeteshmukul   (501) staff       (20)     1098 2024-04-25 09:28:22.000000 adlike-0.0.1/src/adlike.egg-info/PKG-INFO
--rw-r--r--   0 reeteshmukul   (501) staff       (20)      220 2024-04-25 09:28:22.000000 adlike-0.0.1/src/adlike.egg-info/SOURCES.txt
--rw-r--r--   0 reeteshmukul   (501) staff       (20)        1 2024-04-25 09:28:22.000000 adlike-0.0.1/src/adlike.egg-info/dependency_links.txt
--rw-r--r--   0 reeteshmukul   (501) staff       (20)       16 2024-04-25 09:28:22.000000 adlike-0.0.1/src/adlike.egg-info/top_level.txt
+drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-08 13:40:16.535626 adlike-0.0.2/
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)     1098 2024-05-08 13:40:16.535196 adlike-0.0.2/PKG-INFO
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)      580 2024-04-25 09:08:50.000000 adlike-0.0.2/README.md
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)      609 2024-05-08 13:40:07.000000 adlike-0.0.2/pyproject.toml
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)       38 2024-05-08 13:40:16.535929 adlike-0.0.2/setup.cfg
+drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-08 13:40:16.530960 adlike-0.0.2/src/
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)        0 2024-04-17 12:03:13.000000 adlike-0.0.2/src/__init__.py
+drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-08 13:40:16.531659 adlike-0.0.2/src/adlike/
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)       21 2024-04-17 12:03:08.000000 adlike-0.0.2/src/adlike/__init__.py
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)     4583 2024-04-25 09:07:37.000000 adlike-0.0.2/src/adlike/adlike.py
+drwxr-xr-x   0 reeteshmukul   (501) staff       (20)        0 2024-05-08 13:40:16.534718 adlike-0.0.2/src/adlike.egg-info/
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)     1098 2024-05-08 13:40:16.000000 adlike-0.0.2/src/adlike.egg-info/PKG-INFO
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)      220 2024-05-08 13:40:16.000000 adlike-0.0.2/src/adlike.egg-info/SOURCES.txt
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)        1 2024-05-08 13:40:16.000000 adlike-0.0.2/src/adlike.egg-info/dependency_links.txt
+-rw-r--r--   0 reeteshmukul   (501) staff       (20)       16 2024-05-08 13:40:16.000000 adlike-0.0.2/src/adlike.egg-info/top_level.txt
```

### Comparing `adlike-0.0.1/PKG-INFO` & `adlike-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adlike
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package to determine if an Image is an Advertisement
 Author-email: Chitra Vyanjan <chitra.vyanjan@gmail.com>
 Project-URL: Homepage, https://github.com/chitravyanjan/adlike
 Project-URL: Issues, https://github.com/chitravyanjan/adlike/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `adlike-0.0.1/README.md` & `adlike-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `adlike-0.0.1/pyproject.toml` & `adlike-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adlike"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Chitra Vyanjan", email="chitra.vyanjan@gmail.com" },
 ]
 description = "A python package to determine if an Image is an Advertisement"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `adlike-0.0.1/src/adlike/adlike.py` & `adlike-0.0.2/src/adlike/adlike.py`

 * *Files identical despite different names*

### Comparing `adlike-0.0.1/src/adlike.egg-info/PKG-INFO` & `adlike-0.0.2/src/adlike.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adlike
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package to determine if an Image is an Advertisement
 Author-email: Chitra Vyanjan <chitra.vyanjan@gmail.com>
 Project-URL: Homepage, https://github.com/chitravyanjan/adlike
 Project-URL: Issues, https://github.com/chitravyanjan/adlike/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

