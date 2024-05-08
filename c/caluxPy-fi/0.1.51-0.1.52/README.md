# Comparing `tmp/caluxpy_fi-0.1.51.tar.gz` & `tmp/caluxpy_fi-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluxpy_fi-0.1.51.tar", last modified: Mon May  6 20:54:12 2024, max compression
+gzip compressed data, was "caluxpy_fi-0.1.52.tar", last modified: Wed May  8 17:53:13 2024, max compression
```

## Comparing `caluxpy_fi-0.1.51.tar` & `caluxpy_fi-0.1.52.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 20:54:12.273790 caluxpy_fi-0.1.51/
--rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.51/LICENSE.txt
--rw-rw-rw-   0        0        0     4738 2024-05-06 20:54:12.273790 caluxpy_fi-0.1.51/PKG-INFO
--rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.51/README.md
--rw-rw-rw-   0        0        0      824 2024-05-06 20:51:40.000000 caluxpy_fi-0.1.51/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 20:54:12.273790 caluxpy_fi-0.1.51/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 20:54:12.209385 caluxpy_fi-0.1.51/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 20:54:12.256335 caluxpy_fi-0.1.51/src/caluxPy_fi/
--rw-rw-rw-   0        0        0    10586 2024-05-06 20:51:18.000000 caluxpy_fi-0.1.51/src/caluxPy_fi/Convexity.py
--rw-rw-rw-   0        0        0     1189 2024-05-06 14:57:42.000000 caluxpy_fi-0.1.51/src/caluxPy_fi/DataBase.py
--rw-rw-rw-   0        0        0     4215 2024-05-06 14:57:19.000000 caluxpy_fi-0.1.51/src/caluxPy_fi/ExternalImport.py
--rw-rw-rw-   0        0        0    10568 2024-05-06 14:54:58.000000 caluxpy_fi-0.1.51/src/caluxPy_fi/ExternalImport2.py
--rw-rw-rw-   0        0        0    58790 2024-05-06 14:47:32.000000 caluxpy_fi-0.1.51/src/caluxPy_fi/FixedIncome.py
--rw-rw-rw-   0        0        0     5781 2024-05-06 14:55:12.000000 caluxpy_fi-0.1.51/src/caluxPy_fi/Multiple.py
--rw-rw-rw-   0        0        0    13098 2024-05-06 14:51:25.000000 caluxpy_fi-0.1.51/src/caluxPy_fi/Portfolio.py
--rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.51/src/caluxPy_fi/Support.py
--rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.51/src/caluxPy_fi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:54:12.272671 caluxpy_fi-0.1.51/src/caluxPy_fi.egg-info/
--rw-rw-rw-   0        0        0     4738 2024-05-06 20:54:12.000000 caluxpy_fi-0.1.51/src/caluxPy_fi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2024-05-06 20:54:12.000000 caluxpy_fi-0.1.51/src/caluxPy_fi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 20:54:12.000000 caluxpy_fi-0.1.51/src/caluxPy_fi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-05-06 20:54:12.000000 caluxpy_fi-0.1.51/src/caluxPy_fi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-06 20:54:12.000000 caluxpy_fi-0.1.51/src/caluxPy_fi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 17:53:12.997747 caluxpy_fi-0.1.52/
+-rw-rw-rw-   0        0        0     1106 2024-03-18 20:26:44.000000 caluxpy_fi-0.1.52/LICENSE.txt
+-rw-rw-rw-   0        0        0     4738 2024-05-08 17:53:12.994976 caluxpy_fi-0.1.52/PKG-INFO
+-rw-rw-rw-   0        0        0     2724 2024-01-12 17:32:24.000000 caluxpy_fi-0.1.52/README.md
+-rw-rw-rw-   0        0        0      824 2024-05-08 17:51:47.000000 caluxpy_fi-0.1.52/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 17:53:12.997747 caluxpy_fi-0.1.52/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 17:53:12.870833 caluxpy_fi-0.1.52/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 17:53:12.980121 caluxpy_fi-0.1.52/src/caluxPy_fi/
+-rw-rw-rw-   0        0        0    10586 2024-05-08 17:51:33.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/Convexity.py
+-rw-rw-rw-   0        0        0     1189 2024-05-06 14:57:42.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/DataBase.py
+-rw-rw-rw-   0        0        0     4215 2024-05-06 14:57:19.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/ExternalImport.py
+-rw-rw-rw-   0        0        0    10568 2024-05-06 14:54:58.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/ExternalImport2.py
+-rw-rw-rw-   0        0        0    58790 2024-05-06 14:47:32.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/FixedIncome.py
+-rw-rw-rw-   0        0        0     5781 2024-05-06 14:55:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/Multiple.py
+-rw-rw-rw-   0        0        0    13098 2024-05-06 14:51:25.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/Portfolio.py
+-rw-rw-rw-   0        0        0    12223 2024-03-21 21:17:02.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/Support.py
+-rw-rw-rw-   0        0        0       28 2024-01-11 15:43:14.000000 caluxpy_fi-0.1.52/src/caluxPy_fi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 17:53:12.982473 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/
+-rw-rw-rw-   0        0        0     4738 2024-05-08 17:53:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2024-05-08 17:53:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 17:53:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-05-08 17:53:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 17:53:12.000000 caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/top_level.txt
```

### Comparing `caluxpy_fi-0.1.51/LICENSE.txt` & `caluxpy_fi-0.1.52/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.51/PKG-INFO` & `caluxpy_fi-0.1.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.51
+Version: 0.1.52
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

### Comparing `caluxpy_fi-0.1.51/README.md` & `caluxpy_fi-0.1.52/README.md`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.51/pyproject.toml` & `caluxpy_fi-0.1.52/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caluxPy_fi"
-version = "0.1.51"
+version = "0.1.52"
 authors = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 maintainers = [
   { name = "Luis Manuel Tavarez Valenzuela", email = "luima2494@gmail.com" }
 ]
 description = "Fixed Income Valuation and Analysis"
```

### Comparing `caluxpy_fi-0.1.51/src/caluxPy_fi/Convexity.py` & `caluxpy_fi-0.1.52/src/caluxPy_fi/Convexity.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.51/src/caluxPy_fi/DataBase.py` & `caluxpy_fi-0.1.52/src/caluxPy_fi/DataBase.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.51/src/caluxPy_fi/ExternalImport.py` & `caluxpy_fi-0.1.52/src/caluxPy_fi/ExternalImport.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.51/src/caluxPy_fi/ExternalImport2.py` & `caluxpy_fi-0.1.52/src/caluxPy_fi/ExternalImport2.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.51/src/caluxPy_fi/FixedIncome.py` & `caluxpy_fi-0.1.52/src/caluxPy_fi/FixedIncome.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.51/src/caluxPy_fi/Multiple.py` & `caluxpy_fi-0.1.52/src/caluxPy_fi/Multiple.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.51/src/caluxPy_fi/Portfolio.py` & `caluxpy_fi-0.1.52/src/caluxPy_fi/Portfolio.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.51/src/caluxPy_fi/Support.py` & `caluxpy_fi-0.1.52/src/caluxPy_fi/Support.py`

 * *Files identical despite different names*

### Comparing `caluxpy_fi-0.1.51/src/caluxPy_fi.egg-info/PKG-INFO` & `caluxpy_fi-0.1.52/src/caluxPy_fi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluxPy_fi
-Version: 0.1.51
+Version: 0.1.52
 Summary: Fixed Income Valuation and Analysis
 Author-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 Maintainer-email: Luis Manuel Tavarez Valenzuela <luima2494@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Luis Manuel Tavarez Valenzuela
```

