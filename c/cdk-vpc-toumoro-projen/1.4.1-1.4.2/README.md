# Comparing `tmp/cdk-vpc-toumoro-projen-1.4.1.tar.gz` & `tmp/cdk-vpc-toumoro-projen-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-vpc-toumoro-projen-1.4.1.tar", last modified: Wed May  8 17:50:02 2024, max compression
+gzip compressed data, was "cdk-vpc-toumoro-projen-1.4.2.tar", last modified: Wed May  8 17:52:14 2024, max compression
```

## Comparing `cdk-vpc-toumoro-projen-1.4.1.tar` & `cdk-vpc-toumoro-projen-1.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:50:02.261533 cdk-vpc-toumoro-projen-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-08 17:49:51.000000 cdk-vpc-toumoro-projen-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 17:49:51.000000 cdk-vpc-toumoro-projen-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-08 17:50:02.261533 cdk-vpc-toumoro-projen-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 17:49:51.000000 cdk-vpc-toumoro-projen-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 17:49:51.000000 cdk-vpc-toumoro-projen-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:50:02.261533 cdk-vpc-toumoro-projen-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-08 17:49:51.000000 cdk-vpc-toumoro-projen-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:50:02.257533 cdk-vpc-toumoro-projen-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:50:02.261533 cdk-vpc-toumoro-projen-1.4.1/src/cdk-vpc-toumoro-projen/
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-08 17:49:51.000000 cdk-vpc-toumoro-projen-1.4.1/src/cdk-vpc-toumoro-projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:50:02.261533 cdk-vpc-toumoro-projen-1.4.1/src/cdk-vpc-toumoro-projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-08 17:49:51.000000 cdk-vpc-toumoro-projen-1.4.1/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30612 2024-05-08 17:49:51.000000 cdk-vpc-toumoro-projen-1.4.1/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpc-toumoro-projen@1.4.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:49:51.000000 cdk-vpc-toumoro-projen-1.4.1/src/cdk-vpc-toumoro-projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:50:02.261533 cdk-vpc-toumoro-projen-1.4.1/src/cdk_vpc_toumoro_projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-08 17:50:02.000000 cdk-vpc-toumoro-projen-1.4.1/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-08 17:50:02.000000 cdk-vpc-toumoro-projen-1.4.1/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:50:02.000000 cdk-vpc-toumoro-projen-1.4.1/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-08 17:50:02.000000 cdk-vpc-toumoro-projen-1.4.1/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 17:50:02.000000 cdk-vpc-toumoro-projen-1.4.1/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:52:14.309875 cdk-vpc-toumoro-projen-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-08 17:52:02.000000 cdk-vpc-toumoro-projen-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 17:52:02.000000 cdk-vpc-toumoro-projen-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 17:52:14.309875 cdk-vpc-toumoro-projen-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 17:52:02.000000 cdk-vpc-toumoro-projen-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 17:52:02.000000 cdk-vpc-toumoro-projen-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:52:14.309875 cdk-vpc-toumoro-projen-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-08 17:52:02.000000 cdk-vpc-toumoro-projen-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:52:14.305875 cdk-vpc-toumoro-projen-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:52:14.309875 cdk-vpc-toumoro-projen-1.4.2/src/cdk-vpc-toumoro-projen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-08 17:52:02.000000 cdk-vpc-toumoro-projen-1.4.2/src/cdk-vpc-toumoro-projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:52:14.309875 cdk-vpc-toumoro-projen-1.4.2/src/cdk-vpc-toumoro-projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-08 17:52:02.000000 cdk-vpc-toumoro-projen-1.4.2/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30659 2024-05-08 17:52:02.000000 cdk-vpc-toumoro-projen-1.4.2/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpc-toumoro-projen@1.4.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:52:02.000000 cdk-vpc-toumoro-projen-1.4.2/src/cdk-vpc-toumoro-projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:52:14.309875 cdk-vpc-toumoro-projen-1.4.2/src/cdk_vpc_toumoro_projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 17:52:14.000000 cdk-vpc-toumoro-projen-1.4.2/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-08 17:52:14.000000 cdk-vpc-toumoro-projen-1.4.2/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:52:14.000000 cdk-vpc-toumoro-projen-1.4.2/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-08 17:52:14.000000 cdk-vpc-toumoro-projen-1.4.2/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 17:52:14.000000 cdk-vpc-toumoro-projen-1.4.2/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
```

### Comparing `cdk-vpc-toumoro-projen-1.4.1/LICENSE` & `cdk-vpc-toumoro-projen-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-vpc-toumoro-projen-1.4.1/PKG-INFO` & `cdk-vpc-toumoro-projen-1.4.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 1.4.1
+Version: 1.4.2
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,10 +19,14 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # replace this
 
+# Examples
+
+[Examples](examples/README.md)
+
 # Documentation API
 
 [API](API.md)
```

### Comparing `cdk-vpc-toumoro-projen-1.4.1/setup.py` & `cdk-vpc-toumoro-projen-1.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-vpc-toumoro-projen",
-    "version": "1.4.1",
+    "version": "1.4.2",
     "description": "A CDK construct library to create a VPC with public and private subnets.",
     "license": "GPL-3.0-or-later",
     "url": "https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git",
     "long_description_content_type": "text/markdown",
     "author": "tm-lcarvalho<lucio.carvalho@toumoro.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk-vpc-toumoro-projen",
         "cdk-vpc-toumoro-projen._jsii"
     ],
     "package_data": {
         "cdk-vpc-toumoro-projen._jsii": [
-            "cdk-vpc-toumoro-projen@1.4.1.jsii.tgz"
+            "cdk-vpc-toumoro-projen@1.4.2.jsii.tgz"
         ],
         "cdk-vpc-toumoro-projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-vpc-toumoro-projen-1.4.1/src/cdk-vpc-toumoro-projen/__init__.py` & `cdk-vpc-toumoro-projen-1.4.2/src/cdk-vpc-toumoro-projen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 '''
 # replace this
 
+# Examples
+
+[Examples](examples/README.md)
+
 # Documentation API
 
 [API](API.md)
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
```

### Comparing `cdk-vpc-toumoro-projen-1.4.1/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO` & `cdk-vpc-toumoro-projen-1.4.2/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 1.4.1
+Version: 1.4.2
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -19,10 +19,14 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # replace this
 
+# Examples
+
+[Examples](examples/README.md)
+
 # Documentation API
 
 [API](API.md)
```

