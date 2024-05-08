# Comparing `tmp/modelmerge-0.1.5.tar.gz` & `tmp/modelmerge-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.1.5.tar", last modified: Wed May  8 17:24:33 2024, max compression
+gzip compressed data, was "modelmerge-0.1.6.tar", last modified: Wed May  8 18:28:59 2024, max compression
```

## Comparing `modelmerge-0.1.5.tar` & `modelmerge-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:24:33.408787 modelmerge-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 17:24:24.000000 modelmerge-0.1.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:24:33.408787 modelmerge-0.1.5/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 17:24:33.000000 modelmerge-0.1.5/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 17:24:33.000000 modelmerge-0.1.5/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:24:33.000000 modelmerge-0.1.5/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 17:24:33.000000 modelmerge-0.1.5/ModelMerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:24:33.000000 modelmerge-0.1.5/ModelMerge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 17:24:33.408787 modelmerge-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 17:24:24.000000 modelmerge-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:24:33.408787 modelmerge-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 17:24:24.000000 modelmerge-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:24:33.408787 modelmerge-0.1.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-08 17:24:24.000000 modelmerge-0.1.5/test/test_google_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:28:59.064345 modelmerge-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 18:28:43.000000 modelmerge-0.1.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:28:59.064345 modelmerge-0.1.6/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:28:59.000000 modelmerge-0.1.6/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 18:28:59.000000 modelmerge-0.1.6/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:28:59.000000 modelmerge-0.1.6/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 18:28:59.000000 modelmerge-0.1.6/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:28:59.000000 modelmerge-0.1.6/ModelMerge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:28:59.064345 modelmerge-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 18:28:43.000000 modelmerge-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:28:59.064345 modelmerge-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-08 18:28:43.000000 modelmerge-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:28:59.064345 modelmerge-0.1.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-08 18:28:43.000000 modelmerge-0.1.6/test/test_google_search.py
```

### Comparing `modelmerge-0.1.5/LICENSE` & `modelmerge-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.5/setup.py` & `modelmerge-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
 setup(
     name="ModelMerge",
-    version="0.1.5",
+    version="0.1.6",
     description="ModelMerge is a multi-large language model API aggregator.",
     long_description=Path.open(Path("README.md"), encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(where=["models", "tools", "utils"]),
-    package_dir={"": "."},
+    # package_dir={"": "."},
     install_requires=Path.open(Path("requirements.txt"), encoding="utf-8").read().splitlines(),
     # py_modules=["LLM-Hub"]
 )
```

### Comparing `modelmerge-0.1.5/test/test_google_search.py` & `modelmerge-0.1.6/test/test_google_search.py`

 * *Files identical despite different names*

