# Comparing `tmp/ctdfjorder-0.0.40.tar.gz` & `tmp/ctdfjorder-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdfjorder-0.0.40.tar", last modified: Tue May  7 22:11:45 2024, max compression
+gzip compressed data, was "ctdfjorder-0.0.41.tar", last modified: Tue May  7 22:40:12 2024, max compression
```

## Comparing `ctdfjorder-0.0.40.tar` & `ctdfjorder-0.0.41.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:11:45.204559 ctdfjorder-0.0.40/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:11:45.200559 ctdfjorder-0.0.40/CTDFjorder/
--rw-r--r--   0 runner    (1001) docker     (127)    62118 2024-05-07 22:11:40.000000 ctdfjorder-0.0.40/CTDFjorder/CTDFjorder.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 22:11:40.000000 ctdfjorder-0.0.40/CTDFjorder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:11:45.204559 ctdfjorder-0.0.40/CTDFjorder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 22:11:45.000000 ctdfjorder-0.0.40/CTDFjorder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-07 22:11:45.204559 ctdfjorder-0.0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-07 22:11:40.000000 ctdfjorder-0.0.40/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:11:45.204559 ctdfjorder-0.0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 22:11:40.000000 ctdfjorder-0.0.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:40:12.815406 ctdfjorder-0.0.41/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:40:12.815406 ctdfjorder-0.0.41/CTDFjorder/
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-07 22:40:09.000000 ctdfjorder-0.0.41/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 22:40:09.000000 ctdfjorder-0.0.41/CTDFjorder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:40:12.815406 ctdfjorder-0.0.41/CTDFjorder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-07 22:40:12.815406 ctdfjorder-0.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-07 22:40:09.000000 ctdfjorder-0.0.41/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:40:12.815406 ctdfjorder-0.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 22:40:09.000000 ctdfjorder-0.0.41/setup.py
```

### Comparing `ctdfjorder-0.0.40/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.41/CTDFjorder/CTDFjorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1484,9 +1484,8 @@
         print("  default                 Run the default processing pipeline")
         print("  defaultplotall          Run the default processing pipeline and create plots")
         print("CWD:")
         print(_get_cwd())
         sys.exit(1)
 
 if __name__ == "__main__":
-    run_default(True)
     main()
```

### Comparing `ctdfjorder-0.0.40/CTDFjorder.egg-info/PKG-INFO` & `ctdfjorder-0.0.41/CTDFjorder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.40
+Version: 0.0.41
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.40/PKG-INFO` & `ctdfjorder-0.0.41/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.40
+Version: 0.0.41
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.40/README.md` & `ctdfjorder-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.40/setup.py` & `ctdfjorder-0.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CTDFjorder",
-    version="0.0.40",
+    version="0.0.41",
     author="Nikolas Yanek-Chrones",
     author_email="nikojb1001@gmail.com",
     description="A package for processing and analyzing CTD data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nikothomas/CTDFjorder",
     project_urls={
```

