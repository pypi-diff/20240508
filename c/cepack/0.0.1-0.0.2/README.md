# Comparing `tmp/cepack-0.0.1.tar.gz` & `tmp/cepack-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cepack-0.0.1.tar", last modified: Tue May  7 03:08:03 2024, max compression
+gzip compressed data, was "cepack-0.0.2.tar", last modified: Wed May  8 08:10:21 2024, max compression
```

## Comparing `cepack-0.0.1.tar` & `cepack-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 03:08:03.251375 cepack-0.0.1/
--rw-rw-rw-   0        0        0    35821 2024-05-03 11:30:29.000000 cepack-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       18 2024-05-03 11:30:29.000000 cepack-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      607 2024-05-07 03:08:03.251375 cepack-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2024-05-03 11:31:02.000000 cepack-0.0.1/README.md
--rw-rw-rw-   0        0        0      706 2024-05-07 03:05:41.000000 cepack-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 03:08:03.251375 cepack-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 03:08:03.229279 cepack-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 03:08:03.240137 cepack-0.0.1/src/cepack/
--rw-rw-rw-   0        0        0      199 2024-05-07 03:05:41.000000 cepack-0.0.1/src/cepack/__init__.py
--rw-rw-rw-   0        0        0     1491 2024-05-07 03:05:41.000000 cepack-0.0.1/src/cepack/main.py
--rw-rw-rw-   0        0        0     3084 2024-05-07 03:05:41.000000 cepack-0.0.1/src/cepack/utility.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:08:03.251375 cepack-0.0.1/src/cepack.egg-info/
--rw-rw-rw-   0        0        0      607 2024-05-07 03:08:03.000000 cepack-0.0.1/src/cepack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-05-07 03:08:03.000000 cepack-0.0.1/src/cepack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 03:08:03.000000 cepack-0.0.1/src/cepack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-07 03:08:03.000000 cepack-0.0.1/src/cepack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2024-05-07 03:08:03.000000 cepack-0.0.1/src/cepack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-07 03:08:03.000000 cepack-0.0.1/src/cepack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 03:08:03.249477 cepack-0.0.1/test/
--rw-rw-rw-   0        0        0      275 2024-05-07 03:05:41.000000 cepack-0.0.1/test/test.py
--rw-rw-rw-   0        0        0      670 2024-05-07 03:05:41.000000 cepack-0.0.1/test/test_download_repo.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:10:21.673040 cepack-0.0.2/
+-rw-rw-rw-   0        0        0    35821 2024-05-03 11:30:29.000000 cepack-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       18 2024-05-03 11:30:29.000000 cepack-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      607 2024-05-08 08:10:21.673040 cepack-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2024-05-03 11:31:02.000000 cepack-0.0.2/README.md
+-rw-rw-rw-   0        0        0      706 2024-05-08 08:07:16.000000 cepack-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 08:10:21.673040 cepack-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 08:10:21.655167 cepack-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 08:10:21.665359 cepack-0.0.2/src/cepack/
+-rw-rw-rw-   0        0        0      229 2024-05-08 06:42:57.000000 cepack-0.0.2/src/cepack/__init__.py
+-rw-rw-rw-   0        0        0     1637 2024-05-08 07:15:03.000000 cepack-0.0.2/src/cepack/main.py
+-rw-rw-rw-   0        0        0     3084 2024-05-07 15:52:58.000000 cepack-0.0.2/src/cepack/utility.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:10:21.673040 cepack-0.0.2/src/cepack.egg-info/
+-rw-rw-rw-   0        0        0      607 2024-05-08 08:10:21.000000 cepack-0.0.2/src/cepack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-05-08 08:10:21.000000 cepack-0.0.2/src/cepack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:10:21.000000 cepack-0.0.2/src/cepack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-08 08:10:21.000000 cepack-0.0.2/src/cepack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2024-05-08 08:10:21.000000 cepack-0.0.2/src/cepack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 08:10:21.000000 cepack-0.0.2/src/cepack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 08:10:21.673040 cepack-0.0.2/test/
+-rw-rw-rw-   0        0        0     1462 2024-05-08 08:04:18.000000 cepack-0.0.2/test/test_ci.py
+-rw-rw-rw-   0        0        0      678 2024-05-08 01:05:34.000000 cepack-0.0.2/test/test_utility.py
```

### Comparing `cepack-0.0.1/LICENSE` & `cepack-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cepack-0.0.1/PKG-INFO` & `cepack-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cepack
-Version: 0.0.1
+Version: 0.0.2
 Summary: embedded pack manage
 Author-email: paopaozhi <paopaozhi@hotmail.com>
 Project-URL: Homepage, https://github.com/paopaozhi/cepack
 Project-URL: Bug Tracker, https://github.com/paopaozhi/cepack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cepack-0.0.1/pyproject.toml` & `cepack-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cepack"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "paopaozhi", email = "paopaozhi@hotmail.com" }]
 dependencies = ["typer","toml","requests"]
 description = "embedded pack manage"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `cepack-0.0.1/src/cepack/main.py` & `cepack-0.0.2/src/cepack/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import typer
 import logging
 import toml
-from .utility import download_release,get_repo_info
+from .utility import download_repo,download_release,get_repo_info
 import requests
 import sys
+from pathlib import Path
 
 log = logging.getLogger("rich")
-log.setLevel(logging.INFO)
 
 app = typer.Typer()
 
-@app.callback(invoke_without_command=True)
+@app.command()
 def install():
     base_url = "https://api.github.com"
     
     try:
         cfg_file = toml.load("./depend.toml")
     except:
         log.error("none depend.toml!")
         sys.exit()
 
     depend_lib = cfg_file["depend"]
     
     for lib_name in depend_lib:
+        if Path(f"lib/{lib_name}").exists():
+            log.info(f"{lib_name}: {depend_lib[lib_name]}")
+            continue
+        
         log.debug(lib_name)
         # 获取url
         lib_url = depend_lib[lib_name]["url"]
 
         lib_info =get_repo_info(lib_url)
 
         owner = lib_info["owner"]
@@ -37,15 +41,15 @@
 
         ret = requests.get(list_releases)
         try:
             # print(ret.json()["zipball_url"])
             release_url = ret.json()["zipball_url"]
             download_release(release_url,repo)
         except KeyError:
-            pass
+            download_repo(lib_url,repo)
     
 @app.command()
 def goodbye(name: str, formal: bool = False):
     if formal:
         print(f"Goodbye Ms. {name}. Have a good day.")
     else:
         print(f"Bye {name}!")
```

### Comparing `cepack-0.0.1/src/cepack/utility.py` & `cepack-0.0.2/src/cepack/utility.py`

 * *Files identical despite different names*

### Comparing `cepack-0.0.1/src/cepack.egg-info/PKG-INFO` & `cepack-0.0.2/src/cepack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cepack
-Version: 0.0.1
+Version: 0.0.2
 Summary: embedded pack manage
 Author-email: paopaozhi <paopaozhi@hotmail.com>
 Project-URL: Homepage, https://github.com/paopaozhi/cepack
 Project-URL: Bug Tracker, https://github.com/paopaozhi/cepack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

