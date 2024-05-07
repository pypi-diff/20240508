# Comparing `tmp/hugg-0.2.8.tar.gz` & `tmp/hugg-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.2.8.tar", last modified: Fri Nov  3 15:51:54 2023, max compression
+gzip compressed data, was "hugg-0.2.9.tar", last modified: Fri Nov  3 16:50:50 2023, max compression
```

## Comparing `hugg-0.2.8.tar` & `hugg-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 15:51:54.990458 hugg-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-03 15:51:46.000000 hugg-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-03 15:51:54.986458 hugg-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-03 15:51:46.000000 hugg-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 15:51:54.986458 hugg-0.2.8/hugg/
--rw-r--r--   0 runner    (1001) docker     (127)    56239 2023-11-03 15:51:46.000000 hugg-0.2.8/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 15:51:54.986458 hugg-0.2.8/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-03 15:51:54.000000 hugg-0.2.8/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-03 15:51:54.000000 hugg-0.2.8/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 15:51:54.000000 hugg-0.2.8/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-11-03 15:51:54.000000 hugg-0.2.8/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-03 15:51:54.000000 hugg-0.2.8/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 15:51:54.990458 hugg-0.2.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3810 2023-11-03 15:51:46.000000 hugg-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:50:50.189997 hugg-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-03 16:50:37.000000 hugg-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-03 16:50:50.189997 hugg-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-03 16:50:37.000000 hugg-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:50:50.189997 hugg-0.2.9/hugg/
+-rw-r--r--   0 runner    (1001) docker     (127)    56239 2023-11-03 16:50:37.000000 hugg-0.2.9/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 16:50:50.189997 hugg-0.2.9/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-03 16:50:50.000000 hugg-0.2.9/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-03 16:50:50.000000 hugg-0.2.9/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 16:50:50.000000 hugg-0.2.9/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2023-11-03 16:50:50.000000 hugg-0.2.9/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-03 16:50:50.000000 hugg-0.2.9/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 16:50:50.189997 hugg-0.2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3810 2023-11-03 16:50:37.000000 hugg-0.2.9/setup.py
```

### Comparing `hugg-0.2.8/LICENSE` & `hugg-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.2.8/PKG-INFO` & `hugg-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugg
-Version: 0.2.8
+Version: 0.2.9
 Summary: My short description for my project.
 Home-page: https://github.com/franceme/hugg
 Author: Miles Frantz
 Author-email: frantzme@vt.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `hugg-0.2.8/hugg/__init__.py` & `hugg-0.2.9/hugg/__init__.py`

 * *Files identical despite different names*

### Comparing `hugg-0.2.8/hugg.egg-info/PKG-INFO` & `hugg-0.2.9/hugg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugg
-Version: 0.2.8
+Version: 0.2.9
 Summary: My short description for my project.
 Home-page: https://github.com/franceme/hugg
 Author: Miles Frantz
 Author-email: frantzme@vt.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `hugg-0.2.8/setup.py` & `hugg-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

