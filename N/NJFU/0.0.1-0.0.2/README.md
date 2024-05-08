# Comparing `tmp/NJFU-0.0.1.tar.gz` & `tmp/NJFU-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NJFU-0.0.1.tar", last modified: Tue May  7 09:27:32 2024, max compression
+gzip compressed data, was "NJFU-0.0.2.tar", last modified: Tue May  7 09:33:37 2024, max compression
```

## Comparing `NJFU-0.0.1.tar` & `NJFU-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:27:32.762046 NJFU-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:27:32.751083 NJFU-0.0.1/NJFU/
--rw-rw-rw-   0        0        0       41 2024-05-07 09:26:12.000000 NJFU-0.0.1/NJFU/__init__.py
--rw-rw-rw-   0        0        0       61 2024-05-07 09:27:16.000000 NJFU-0.0.1/NJFU/hello.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:27:32.761049 NJFU-0.0.1/NJFU.egg-info/
--rw-rw-rw-   0        0        0      900 2024-05-07 09:27:32.000000 NJFU-0.0.1/NJFU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      151 2024-05-07 09:27:32.000000 NJFU-0.0.1/NJFU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:27:32.000000 NJFU-0.0.1/NJFU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-07 09:27:32.000000 NJFU-0.0.1/NJFU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      900 2024-05-07 09:27:32.762046 NJFU-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-07 09:27:32.762046 NJFU-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1060 2024-05-07 09:27:16.000000 NJFU-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:33:37.719274 NJFU-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-07 09:33:37.707221 NJFU-0.0.2/NJFU/
+-rw-rw-rw-   0        0        0       82 2024-05-07 09:33:24.000000 NJFU-0.0.2/NJFU/__init__.py
+-rw-rw-rw-   0        0        0       61 2024-05-07 09:27:16.000000 NJFU-0.0.2/NJFU/hello.py
+-rw-rw-rw-   0        0        0     6397 2024-05-07 09:33:24.000000 NJFU-0.0.2/NJFU/txt2xml.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:33:37.718278 NJFU-0.0.2/NJFU.egg-info/
+-rw-rw-rw-   0        0        0      900 2024-05-07 09:33:37.000000 NJFU-0.0.2/NJFU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-05-07 09:33:37.000000 NJFU-0.0.2/NJFU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 09:33:37.000000 NJFU-0.0.2/NJFU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-07 09:33:37.000000 NJFU-0.0.2/NJFU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      900 2024-05-07 09:33:37.719274 NJFU-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-07 09:33:37.719274 NJFU-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1060 2024-05-07 09:33:35.000000 NJFU-0.0.2/setup.py
```

### Comparing `NJFU-0.0.1/NJFU.egg-info/PKG-INFO` & `NJFU-0.0.2/NJFU.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NJFU
-Version: 0.0.1
+Version: 0.0.2
 Summary: NJFU
 Home-page: https://github.com/
 Author: XHF
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
```

### Comparing `NJFU-0.0.1/PKG-INFO` & `NJFU-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NJFU
-Version: 0.0.1
+Version: 0.0.2
 Summary: NJFU
 Home-page: https://github.com/
 Author: XHF
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
```

### Comparing `NJFU-0.0.1/setup.py` & `NJFU-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="NJFU",
-    version="0.0.1",
+    version="0.0.2",
     author="XHF",
 
     description="NJFU",
 
     Long_description_content_type="text/markdown",
     url="https://github.com/",
     packages=setuptools.find_packages(),
```

