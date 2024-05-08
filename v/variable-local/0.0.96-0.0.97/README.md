# Comparing `tmp/variable_local-0.0.96.tar.gz` & `tmp/variable_local-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variable_local-0.0.96.tar", last modified: Wed May  8 01:15:37 2024, max compression
+gzip compressed data, was "variable_local-0.0.97.tar", last modified: Wed May  8 01:29:45 2024, max compression
```

## Comparing `variable_local-0.0.96.tar` & `variable_local-0.0.97.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:15:37.173658 variable_local-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 01:15:37.173658 variable_local-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-08 01:15:00.000000 variable_local-0.0.96/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-08 01:15:00.000000 variable_local-0.0.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:15:37.173658 variable_local-0.0.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 01:15:00.000000 variable_local-0.0.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:15:37.169658 variable_local-0.0.96/variable_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:15:37.169658 variable_local-0.0.96/variable_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:15:00.000000 variable_local-0.0.96/variable_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-08 01:15:00.000000 variable_local-0.0.96/variable_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-08 01:15:00.000000 variable_local-0.0.96/variable_local/src/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-08 01:15:00.000000 variable_local-0.0.96/variable_local/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-08 01:15:00.000000 variable_local-0.0.96/variable_local/src/variables_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:15:37.169658 variable_local-0.0.96/variable_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 01:15:37.000000 variable_local-0.0.96/variable_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-08 01:15:37.000000 variable_local-0.0.96/variable_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:15:37.000000 variable_local-0.0.96/variable_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-08 01:15:37.000000 variable_local-0.0.96/variable_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 01:15:37.000000 variable_local-0.0.96/variable_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:29:45.740237 variable_local-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 01:29:45.736237 variable_local-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-08 01:29:21.000000 variable_local-0.0.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-08 01:29:21.000000 variable_local-0.0.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:29:45.740237 variable_local-0.0.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 01:29:21.000000 variable_local-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:29:45.736237 variable_local-0.0.97/variable_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:29:45.736237 variable_local-0.0.97/variable_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:29:21.000000 variable_local-0.0.97/variable_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-08 01:29:21.000000 variable_local-0.0.97/variable_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-08 01:29:21.000000 variable_local-0.0.97/variable_local/src/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-08 01:29:21.000000 variable_local-0.0.97/variable_local/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-08 01:29:21.000000 variable_local-0.0.97/variable_local/src/variables_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:29:45.736237 variable_local-0.0.97/variable_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 01:29:45.000000 variable_local-0.0.97/variable_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-08 01:29:45.000000 variable_local-0.0.97/variable_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:29:45.000000 variable_local-0.0.97/variable_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-08 01:29:45.000000 variable_local-0.0.97/variable_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 01:29:45.000000 variable_local-0.0.97/variable_local.egg-info/top_level.txt
```

### Comparing `variable_local-0.0.96/PKG-INFO` & `variable_local-0.0.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.96
+Version: 0.0.97
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `variable_local-0.0.96/README.md` & `variable_local-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.96/pyproject.toml` & `variable_local-0.0.97/pyproject.toml`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.96/setup.py` & `variable_local-0.0.97/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = 'variable-local'
 package_dir = PACKAGE_NAME.replace('-', '_')
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.96',  # https://pypi.org/project/variable-local
+    version='0.0.97',  # https://pypi.org/project/variable-local
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles variable Local/Remote Python",
     long_description="PyPI Package for Circles variable Local/Remote Python",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
```

### Comparing `variable_local-0.0.96/variable_local/src/constants.py` & `variable_local-0.0.97/variable_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.96/variable_local/src/template.py` & `variable_local-0.0.97/variable_local/src/template.py`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.96/variable_local/src/variables_local.py` & `variable_local-0.0.97/variable_local/src/variables_local.py`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.96/variable_local.egg-info/PKG-INFO` & `variable_local-0.0.97/variable_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.96
+Version: 0.0.97
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

