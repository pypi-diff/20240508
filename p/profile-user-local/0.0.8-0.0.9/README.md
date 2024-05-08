# Comparing `tmp/profile-user-local-0.0.8.tar.gz` & `tmp/profile-user-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile-user-local-0.0.8.tar", last modified: Thu Dec  7 20:32:50 2023, max compression
+gzip compressed data, was "profile-user-local-0.0.9.tar", last modified: Fri Dec  8 13:19:59 2023, max compression
```

## Comparing `profile-user-local-0.0.8.tar` & `profile-user-local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:32:50.761604 profile-user-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-12-07 20:32:50.757604 profile-user-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-12-07 20:32:18.000000 profile-user-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:32:50.753604 profile-user-local-0.0.8/profile_user_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:32:50.757604 profile-user-local-0.0.8/profile_user_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 20:32:18.000000 profile-user-local-0.0.8/profile_user_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2023-12-07 20:32:18.000000 profile-user-local-0.0.8/profile_user_local/src/profile_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-12-07 20:32:18.000000 profile-user-local-0.0.8/profile_user_local/src/profile_user_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:32:50.757604 profile-user-local-0.0.8/profile_user_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-12-07 20:32:50.000000 profile-user-local-0.0.8/profile_user_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-12-07 20:32:50.000000 profile-user-local-0.0.8/profile_user_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 20:32:50.000000 profile-user-local-0.0.8/profile_user_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-07 20:32:50.000000 profile-user-local-0.0.8/profile_user_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-07 20:32:50.000000 profile-user-local-0.0.8/profile_user_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      745 2023-12-07 20:32:18.000000 profile-user-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 20:32:50.761604 profile-user-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-07 20:32:18.000000 profile-user-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:19:59.030456 profile-user-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-12-08 13:19:59.030456 profile-user-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-12-08 13:19:27.000000 profile-user-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:19:59.026456 profile-user-local-0.0.9/profile_user_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:19:59.026456 profile-user-local-0.0.9/profile_user_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 13:19:27.000000 profile-user-local-0.0.9/profile_user_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2023-12-08 13:19:27.000000 profile-user-local-0.0.9/profile_user_local/src/profile_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-12-08 13:19:27.000000 profile-user-local-0.0.9/profile_user_local/src/profile_user_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 13:19:59.030456 profile-user-local-0.0.9/profile_user_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-12-08 13:19:59.000000 profile-user-local-0.0.9/profile_user_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2023-12-08 13:19:59.000000 profile-user-local-0.0.9/profile_user_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 13:19:59.000000 profile-user-local-0.0.9/profile_user_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-08 13:19:59.000000 profile-user-local-0.0.9/profile_user_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-08 13:19:59.000000 profile-user-local-0.0.9/profile_user_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2023-12-08 13:19:27.000000 profile-user-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 13:19:59.030456 profile-user-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-08 13:19:27.000000 profile-user-local-0.0.9/setup.py
```

### Comparing `profile-user-local-0.0.8/PKG-INFO` & `profile-user-local-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-user-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles profile-user Local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profile-user-local-0.0.8/README.md` & `profile-user-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `profile-user-local-0.0.8/profile_user_local/src/profile_user.py` & `profile-user-local-0.0.9/profile_user_local/src/profile_user.py`

 * *Files identical despite different names*

### Comparing `profile-user-local-0.0.8/profile_user_local/src/profile_user_constants.py` & `profile-user-local-0.0.9/profile_user_local/src/profile_user_constants.py`

 * *Files identical despite different names*

### Comparing `profile-user-local-0.0.8/profile_user_local.egg-info/PKG-INFO` & `profile-user-local-0.0.9/profile_user_local.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-user-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles profile-user Local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profile-user-local-0.0.8/pyproject.toml` & `profile-user-local-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 # TODO: Please update the name, similar to storage-local (suffix -local)
 name = "profile-user-local"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.8" # https://pypi.org/project/profile-user-local/ i.e. https://pypi.org/project/storage-local/
+version = "0.0.9" # https://pypi.org/project/profile-user-local/ i.e. https://pypi.org/project/storage-local/
 description = "profile-user-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

### Comparing `profile-user-local-0.0.8/setup.py` & `profile-user-local-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 with open('README.md') as f:
     readme = f.read()
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # https://pypi.org/project/profile-user-local/
+    version='0.0.9',  # https://pypi.org/project/profile-user-local/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles profile-user Local Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/circles",
     packages=[package_dir],
```

