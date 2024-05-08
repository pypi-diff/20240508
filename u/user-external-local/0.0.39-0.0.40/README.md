# Comparing `tmp/user_external_local-0.0.39.tar.gz` & `tmp/user_external_local-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_external_local-0.0.39.tar", last modified: Tue May  7 08:34:17 2024, max compression
+gzip compressed data, was "user_external_local-0.0.40.tar", last modified: Tue May  7 11:24:45 2024, max compression
```

## Comparing `user_external_local-0.0.39.tar` & `user_external_local-0.0.40.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:34:17.582368 user_external_local-0.0.39/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 08:34:17.582368 user_external_local-0.0.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-07 08:33:52.000000 user_external_local-0.0.39/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 08:33:52.000000 user_external_local-0.0.39/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:34:17.582368 user_external_local-0.0.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-07 08:33:52.000000 user_external_local-0.0.39/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:34:17.582368 user_external_local-0.0.39/user_external_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:34:17.582368 user_external_local-0.0.39/user_external_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 08:33:52.000000 user_external_local-0.0.39/user_external_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-05-07 08:33:52.000000 user_external_local-0.0.39/user_external_local/src/user_externals_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:34:17.582368 user_external_local-0.0.39/user_external_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 08:34:17.000000 user_external_local-0.0.39/user_external_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 08:34:17.000000 user_external_local-0.0.39/user_external_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:34:17.000000 user_external_local-0.0.39/user_external_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-07 08:34:17.000000 user_external_local-0.0.39/user_external_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 08:34:17.000000 user_external_local-0.0.39/user_external_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:24:45.719142 user_external_local-0.0.40/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 11:24:45.719142 user_external_local-0.0.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-07 11:24:22.000000 user_external_local-0.0.40/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 11:24:22.000000 user_external_local-0.0.40/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:24:45.719142 user_external_local-0.0.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-07 11:24:22.000000 user_external_local-0.0.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:24:45.715142 user_external_local-0.0.40/user_external_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:24:45.715142 user_external_local-0.0.40/user_external_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 11:24:22.000000 user_external_local-0.0.40/user_external_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-05-07 11:24:22.000000 user_external_local-0.0.40/user_external_local/src/user_externals_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:24:45.719142 user_external_local-0.0.40/user_external_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 11:24:45.000000 user_external_local-0.0.40/user_external_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 11:24:45.000000 user_external_local-0.0.40/user_external_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:24:45.000000 user_external_local-0.0.40/user_external_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-07 11:24:45.000000 user_external_local-0.0.40/user_external_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 11:24:45.000000 user_external_local-0.0.40/user_external_local.egg-info/top_level.txt
```

### Comparing `user_external_local-0.0.39/PKG-INFO` & `user_external_local-0.0.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-external-local
-Version: 0.0.39
+Version: 0.0.40
 Home-page: https://github.com/circles-zone/user-external-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `user_external_local-0.0.39/README.md` & `user_external_local-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `user_external_local-0.0.39/setup.py` & `user_external_local-0.0.40/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-external-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/user-external-local
-    version='0.0.39',
+    version='0.0.40',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="user-external-local",
```

### Comparing `user_external_local-0.0.39/user_external_local/src/user_externals_local.py` & `user_external_local-0.0.40/user_external_local/src/user_externals_local.py`

 * *Files identical despite different names*

### Comparing `user_external_local-0.0.39/user_external_local.egg-info/PKG-INFO` & `user_external_local-0.0.40/user_external_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-external-local
-Version: 0.0.39
+Version: 0.0.40
 Home-page: https://github.com/circles-zone/user-external-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

