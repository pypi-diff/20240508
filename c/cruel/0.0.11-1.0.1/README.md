# Comparing `tmp/cruel-0.0.11.tar.gz` & `tmp/cruel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cruel-0.0.11.tar", last modified: Wed May  8 13:18:22 2024, max compression
+gzip compressed data, was "cruel-1.0.1.tar", last modified: Wed May  8 12:59:19 2024, max compression
```

## Comparing `cruel-0.0.11.tar` & `cruel-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 13:18:22.354735 cruel-0.0.11/
--rw-r--r--   0 codie     (1000) codie     (1000)    35148 2024-04-09 16:46:37.000000 cruel-0.0.11/LICENCE
--rw-r--r--   0 codie     (1000) codie     (1000)     2389 2024-05-08 13:18:22.354735 cruel-0.0.11/PKG-INFO
--rw-r--r--   0 codie     (1000) codie     (1000)     1468 2024-05-08 12:59:00.000000 cruel-0.0.11/README.md
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 13:18:22.353735 cruel-0.0.11/cruel/
--rw-r--r--   0 codie     (1000) codie     (1000)       31 2024-05-08 12:42:21.000000 cruel-0.0.11/cruel/__init__.py
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 13:18:22.353735 cruel-0.0.11/cruel/utils/
--rw-r--r--   0 codie     (1000) codie     (1000)        0 2024-04-09 16:46:37.000000 cruel-0.0.11/cruel/utils/__init__.py
--rw-r--r--   0 codie     (1000) codie     (1000)     1790 2024-05-08 13:17:36.000000 cruel-0.0.11/cruel/utils/req.py
-drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 13:18:22.353735 cruel-0.0.11/cruel.egg-info/
--rw-r--r--   0 codie     (1000) codie     (1000)     2389 2024-05-08 13:18:22.000000 cruel-0.0.11/cruel.egg-info/PKG-INFO
--rw-r--r--   0 codie     (1000) codie     (1000)      231 2024-05-08 13:18:22.000000 cruel-0.0.11/cruel.egg-info/SOURCES.txt
--rw-r--r--   0 codie     (1000) codie     (1000)        1 2024-05-08 13:18:22.000000 cruel-0.0.11/cruel.egg-info/dependency_links.txt
--rw-r--r--   0 codie     (1000) codie     (1000)      173 2024-05-08 13:18:22.000000 cruel-0.0.11/cruel.egg-info/requires.txt
--rw-r--r--   0 codie     (1000) codie     (1000)        6 2024-05-08 13:18:22.000000 cruel-0.0.11/cruel.egg-info/top_level.txt
--rw-r--r--   0 codie     (1000) codie     (1000)       38 2024-05-08 13:18:22.354735 cruel-0.0.11/setup.cfg
--rw-r--r--   0 codie     (1000) codie     (1000)     1164 2024-05-08 13:18:19.000000 cruel-0.0.11/setup.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 12:59:19.094668 cruel-1.0.1/
+-rw-r--r--   0 codie     (1000) codie     (1000)    35148 2024-04-09 16:46:37.000000 cruel-1.0.1/LICENCE
+-rw-r--r--   0 codie     (1000) codie     (1000)     2388 2024-05-08 12:59:19.094668 cruel-1.0.1/PKG-INFO
+-rw-r--r--   0 codie     (1000) codie     (1000)     1468 2024-05-08 12:59:00.000000 cruel-1.0.1/README.md
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 12:59:19.093668 cruel-1.0.1/cruel/
+-rw-r--r--   0 codie     (1000) codie     (1000)       31 2024-05-08 12:42:21.000000 cruel-1.0.1/cruel/__init__.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 12:59:19.093668 cruel-1.0.1/cruel/utils/
+-rw-r--r--   0 codie     (1000) codie     (1000)        0 2024-04-09 16:46:37.000000 cruel-1.0.1/cruel/utils/__init__.py
+-rw-r--r--   0 codie     (1000) codie     (1000)     1801 2024-05-08 12:45:33.000000 cruel-1.0.1/cruel/utils/req.py
+drwxr-xr-x   0 codie     (1000) codie     (1000)        0 2024-05-08 12:59:19.093668 cruel-1.0.1/cruel.egg-info/
+-rw-r--r--   0 codie     (1000) codie     (1000)     2388 2024-05-08 12:59:19.000000 cruel-1.0.1/cruel.egg-info/PKG-INFO
+-rw-r--r--   0 codie     (1000) codie     (1000)      231 2024-05-08 12:59:19.000000 cruel-1.0.1/cruel.egg-info/SOURCES.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)        1 2024-05-08 12:59:19.000000 cruel-1.0.1/cruel.egg-info/dependency_links.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)      173 2024-05-08 12:59:19.000000 cruel-1.0.1/cruel.egg-info/requires.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)        6 2024-05-08 12:59:19.000000 cruel-1.0.1/cruel.egg-info/top_level.txt
+-rw-r--r--   0 codie     (1000) codie     (1000)       38 2024-05-08 12:59:19.094668 cruel-1.0.1/setup.cfg
+-rw-r--r--   0 codie     (1000) codie     (1000)     1164 2024-05-08 12:59:00.000000 cruel-1.0.1/setup.py
```

### Comparing `cruel-0.0.11/LICENCE` & `cruel-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `cruel-0.0.11/PKG-INFO` & `cruel-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cruel
-Version: 0.0.11
+Version: 1.0.1
 Summary: Cruel - Scrape everything or anything from the web.
 Home-page: https://github.com/Bishwas-py/cruel
 Author: Bishwas Bhandari
 Author-email: yo@bishwas.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cruel-0.0.11/README.md` & `cruel-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cruel-0.0.11/cruel/utils/req.py` & `cruel-1.0.1/cruel/utils/req.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,21 +22,19 @@
         self.session_number = 1
 
     def request(
             self,
             method,
             url: str = '',
             self_: 'Session' = None,
+            use_scraper_api: bool = True,
             *args,
             **kwargs,
     ) -> Response:
-        if self_ is None:
-            self_ = self
-
-        if self_.USE_SCRAPER_API and not self_.SCRAPER_API_KEY:
+        if (use_scraper_api or self_.USE_SCRAPER_API) and not self_.SCRAPER_API_KEY:
             raise ValueError(
                 f"No Scraper API key found, please get one from {SCRAPER_API_REF}, and "
                 f"use `set_scraper_api_key(` to set it.")
         if self_.SCRAPER_API_KEY and self_.USE_SCRAPER_API:
             kwargs["params"] = {
                 "api_key": self_.SCRAPER_API_KEY,
                 "url": url,
```

### Comparing `cruel-0.0.11/cruel.egg-info/PKG-INFO` & `cruel-1.0.1/cruel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cruel
-Version: 0.0.11
+Version: 1.0.1
 Summary: Cruel - Scrape everything or anything from the web.
 Home-page: https://github.com/Bishwas-py/cruel
 Author: Bishwas Bhandari
 Author-email: yo@bishwas.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cruel-0.0.11/setup.py` & `cruel-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cruel",
-    version="0.0.11",
+    version="1.0.01",
     description="Cruel - Scrape everything or anything from the web.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bishwas-py/cruel",
     author="Bishwas Bhandari",
     author_email="yo@bishwas.net",
     py_modules=["cruel"],
```

