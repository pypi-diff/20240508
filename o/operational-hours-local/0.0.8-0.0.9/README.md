# Comparing `tmp/operational-hours-local-0.0.8.tar.gz` & `tmp/operational-hours-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operational-hours-local-0.0.8.tar", last modified: Mon Aug 21 07:56:33 2023, max compression
+gzip compressed data, was "operational-hours-local-0.0.9.tar", last modified: Mon Aug 21 13:08:25 2023, max compression
```

## Comparing `operational-hours-local-0.0.8.tar` & `operational-hours-local-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:56:33.811525 operational-hours-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-21 07:56:33.811525 operational-hours-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-21 07:56:09.000000 operational-hours-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:56:33.811525 operational-hours-local-0.0.8/operational_hours_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-21 07:56:33.000000 operational-hours-local-0.0.8/operational_hours_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-21 07:56:33.000000 operational-hours-local-0.0.8/operational_hours_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 07:56:33.000000 operational-hours-local-0.0.8/operational_hours_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 07:56:33.000000 operational-hours-local-0.0.8/operational_hours_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-21 07:56:09.000000 operational-hours-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 07:56:33.811525 operational-hours-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-21 07:56:09.000000 operational-hours-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:08:25.111866 operational-hours-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-21 13:08:25.111866 operational-hours-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-21 13:07:55.000000 operational-hours-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:08:25.111866 operational-hours-local-0.0.9/operational_hours_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-21 13:08:25.000000 operational-hours-local-0.0.9/operational_hours_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-21 13:08:25.000000 operational-hours-local-0.0.9/operational_hours_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 13:08:25.000000 operational-hours-local-0.0.9/operational_hours_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 13:08:25.000000 operational-hours-local-0.0.9/operational_hours_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-21 13:07:55.000000 operational-hours-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 13:08:25.111866 operational-hours-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-21 13:07:55.000000 operational-hours-local-0.0.9/setup.py
```

### Comparing `operational-hours-local-0.0.8/PKG-INFO` & `operational-hours-local-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operational-hours-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles operational-hours-local Local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `operational-hours-local-0.0.8/README.md` & `operational-hours-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `operational-hours-local-0.0.8/operational_hours_local.egg-info/PKG-INFO` & `operational-hours-local-0.0.9/operational_hours_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operational-hours-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles operational-hours-local Local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `operational-hours-local-0.0.8/pyproject.toml` & `operational-hours-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `operational-hours-local-0.0.8/setup.py` & `operational-hours-local-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Each Python project should have pyproject.toml or setup.py
 # TODO: Please create pyproject.toml instead of setup.py (delete the setup.py)
 # used by python -m build
 # ```python -m build``` needs pyproject.toml or setup.py
 # The need for setup.py is changing as of poetry 1.1.0 (including current pre-release) as we have moved away from needing to generate a setup.py file to enable editable installs - We might able to delete this file in the near future
 setuptools.setup(
      name='operational-hours-local',  
-     version='0.0.8', # https://pypi.org/project/operational-hours-local/
+     version='0.0.9', # https://pypi.org/project/operational-hours-local/
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles operational-hours-local Local Python", 
      long_description="This is a package for sharing common functions of operational hours CRUD used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/circles",
      packages=setuptools.find_packages(),
```

