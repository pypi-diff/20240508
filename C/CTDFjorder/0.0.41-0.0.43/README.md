# Comparing `tmp/ctdfjorder-0.0.41.tar.gz` & `tmp/ctdfjorder-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctdfjorder-0.0.41.tar", last modified: Tue May  7 22:40:12 2024, max compression
+gzip compressed data, was "ctdfjorder-0.0.43.tar", last modified: Tue May  7 23:07:57 2024, max compression
```

## Comparing `ctdfjorder-0.0.41.tar` & `ctdfjorder-0.0.43.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:40:12.815406 ctdfjorder-0.0.41/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:40:12.815406 ctdfjorder-0.0.41/CTDFjorder/
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-07 22:40:09.000000 ctdfjorder-0.0.41/CTDFjorder/CTDFjorder.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 22:40:09.000000 ctdfjorder-0.0.41/CTDFjorder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:40:12.815406 ctdfjorder-0.0.41/CTDFjorder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 22:40:12.000000 ctdfjorder-0.0.41/CTDFjorder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-07 22:40:12.815406 ctdfjorder-0.0.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-07 22:40:09.000000 ctdfjorder-0.0.41/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:40:12.815406 ctdfjorder-0.0.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 22:40:09.000000 ctdfjorder-0.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:07:57.175495 ctdfjorder-0.0.43/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:07:57.175495 ctdfjorder-0.0.43/CTDFjorder/
+-rw-r--r--   0 runner    (1001) docker     (127)    62074 2024-05-07 23:07:52.000000 ctdfjorder-0.0.43/CTDFjorder/CTDFjorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 23:07:52.000000 ctdfjorder-0.0.43/CTDFjorder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:07:57.175495 ctdfjorder-0.0.43/CTDFjorder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-07 23:07:57.000000 ctdfjorder-0.0.43/CTDFjorder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 23:07:57.000000 ctdfjorder-0.0.43/CTDFjorder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:07:57.000000 ctdfjorder-0.0.43/CTDFjorder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 23:07:57.000000 ctdfjorder-0.0.43/CTDFjorder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 23:07:57.000000 ctdfjorder-0.0.43/CTDFjorder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 23:07:57.000000 ctdfjorder-0.0.43/CTDFjorder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-07 23:07:57.175495 ctdfjorder-0.0.43/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-07 23:07:52.000000 ctdfjorder-0.0.43/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:07:57.175495 ctdfjorder-0.0.43/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 23:07:52.000000 ctdfjorder-0.0.43/setup.py
```

### Comparing `ctdfjorder-0.0.41/CTDFjorder/CTDFjorder.py` & `ctdfjorder-0.0.43/CTDFjorder/CTDFjorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1424,15 +1424,14 @@
     if not os.path.isdir("./plots"):
         os.mkdir("./plots")
     if not os.path.isdir("./plots/gif"):
         os.mkdir("./plots/gif")
 
 
 def main():
-    run_default(True)
     if len(sys.argv) < 2:
         print("Usage: ctdfjorder <command> [arguments]")
         print("Commands:")
         print("  process <file>          Process a single RSK file")
         print("  merge                   Merge all RSK files in the current folder")
         print("  default                 Run the default processing pipeline")
         sys.exit(1)
```

### Comparing `ctdfjorder-0.0.41/CTDFjorder.egg-info/PKG-INFO` & `ctdfjorder-0.0.43/CTDFjorder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.41
+Version: 0.0.43
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.41/PKG-INFO` & `ctdfjorder-0.0.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTDFjorder
-Version: 0.0.41
+Version: 0.0.43
 Summary: A package for processing and analyzing CTD data.
 Home-page: https://github.com/nikothomas/CTDFjorder
 Author: Nikolas Yanek-Chrones
 Author-email: nikojb1001@gmail.com
 Project-URL: Homepage, https://github.com/nikothomas/CTDFjorder
 Project-URL: Issues, https://github.com/nikothomas/CTDFjorder/issues
 Keywords: CTD
```

### Comparing `ctdfjorder-0.0.41/README.md` & `ctdfjorder-0.0.43/README.md`

 * *Files identical despite different names*

### Comparing `ctdfjorder-0.0.41/setup.py` & `ctdfjorder-0.0.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="CTDFjorder",
-    version="0.0.41",
+    version="0.0.43",
     author="Nikolas Yanek-Chrones",
     author_email="nikojb1001@gmail.com",
     description="A package for processing and analyzing CTD data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/nikothomas/CTDFjorder",
     project_urls={
```

