# Comparing `tmp/pcTools543-0.1.tar.gz` & `tmp/pcTools543-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcTools543-0.1.tar", last modified: Wed May  8 01:11:47 2024, max compression
+gzip compressed data, was "pcTools543-0.11.tar", last modified: Wed May  8 02:41:41 2024, max compression
```

## Comparing `pcTools543-0.1.tar` & `pcTools543-0.11.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 01:11:47.486515 pcTools543-0.1/
--rw-rw-rw-   0        0        0     1074 2024-05-08 00:53:40.000000 pcTools543-0.1/LICENSE
--rw-rw-rw-   0        0        0      957 2024-05-08 01:11:47.486515 pcTools543-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      556 2024-05-08 00:53:21.000000 pcTools543-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 01:11:47.471007 pcTools543-0.1/pcTools543/
--rw-rw-rw-   0        0        0        0 2024-05-08 00:48:37.000000 pcTools543-0.1/pcTools543/__init__.py
--rw-rw-rw-   0        0        0       56 2024-05-08 01:11:43.000000 pcTools543-0.1/pcTools543/pcTools.py
-drwxrwxrwx   0        0        0        0 2024-05-08 01:11:47.486515 pcTools543-0.1/pcTools543.egg-info/
--rw-rw-rw-   0        0        0      957 2024-05-08 01:11:47.000000 pcTools543-0.1/pcTools543.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-08 01:11:47.000000 pcTools543-0.1/pcTools543.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 01:11:47.000000 pcTools543-0.1/pcTools543.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-08 01:11:47.000000 pcTools543-0.1/pcTools543.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 01:11:47.000000 pcTools543-0.1/pcTools543.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-08 01:11:47.486515 pcTools543-0.1/setup.cfg
--rw-rw-rw-   0        0        0      732 2024-05-08 01:11:20.000000 pcTools543-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 02:41:41.019928 pcTools543-0.11/
+-rw-rw-rw-   0        0        0     1074 2024-05-08 00:53:40.000000 pcTools543-0.11/LICENSE
+-rw-rw-rw-   0        0        0      958 2024-05-08 02:41:41.019928 pcTools543-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2024-05-08 00:53:21.000000 pcTools543-0.11/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 02:41:41.009305 pcTools543-0.11/pcTools543/
+-rw-rw-rw-   0        0        0       74 2024-05-08 02:27:18.000000 pcTools543-0.11/pcTools543/__init__.py
+-rw-rw-rw-   0        0        0       56 2024-05-08 01:15:24.000000 pcTools543-0.11/pcTools543/pcTools.py
+drwxrwxrwx   0        0        0        0 2024-05-08 02:41:41.018971 pcTools543-0.11/pcTools543.egg-info/
+-rw-rw-rw-   0        0        0      958 2024-05-08 02:41:40.000000 pcTools543-0.11/pcTools543.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-08 02:41:40.000000 pcTools543-0.11/pcTools543.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 02:41:40.000000 pcTools543-0.11/pcTools543.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-08 02:41:40.000000 pcTools543-0.11/pcTools543.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 02:41:40.000000 pcTools543-0.11/pcTools543.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-08 02:41:41.020925 pcTools543-0.11/setup.cfg
+-rw-rw-rw-   0        0        0      733 2024-05-08 02:38:40.000000 pcTools543-0.11/setup.py
```

### Comparing `pcTools543-0.1/LICENSE` & `pcTools543-0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `pcTools543-0.1/PKG-INFO` & `pcTools543-0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcTools543
-Version: 0.1
+Version: 0.11
 Summary: Just
 Home-page: https://github.com/
 Author: Su
 Author-email: aaaaaaaa@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pcTools543-0.1/README.md` & `pcTools543-0.11/README.md`

 * *Files identical despite different names*

### Comparing `pcTools543-0.1/pcTools543.egg-info/PKG-INFO` & `pcTools543-0.11/pcTools543.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcTools543
-Version: 0.1
+Version: 0.11
 Summary: Just
 Home-page: https://github.com/
 Author: Su
 Author-email: aaaaaaaa@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pcTools543-0.1/setup.py` & `pcTools543-0.11/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pcTools543",
-    version="0.1",
+    version="0.11",
     author="Su",
     author_email="aaaaaaaa@qq.com",
     description="Just",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     packages=setuptools.find_packages(),
```

