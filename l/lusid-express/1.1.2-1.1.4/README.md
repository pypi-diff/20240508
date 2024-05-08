# Comparing `tmp/lusid_express-1.1.2.tar.gz` & `tmp/lusid_express-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-1.1.2.tar", last modified: Wed May  8 12:56:33 2024, max compression
+gzip compressed data, was "lusid_express-1.1.4.tar", last modified: Wed May  8 16:24:02 2024, max compression
```

## Comparing `lusid_express-1.1.2.tar` & `lusid_express-1.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.276624 lusid_express-1.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-08 12:55:44.000000 lusid_express-1.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-08 12:55:44.000000 lusid_express-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8202 2024-05-08 12:56:33.276624 lusid_express-1.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7562 2024-05-08 12:55:44.000000 lusid_express-1.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 12:56:33.276624 lusid_express-1.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-08 12:55:44.000000 lusid_express-1.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.270624 lusid_express-1.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.272624 lusid_express-1.1.2/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5913 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.273624 lusid_express-1.1.2/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-05-08 12:56:32.000000 lusid_express-1.1.2/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.275624 lusid_express-1.1.2/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.275624 lusid_express-1.1.2/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)    11360 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3156 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.275624 lusid_express-1.1.2/src/lusid_express/utils/
--rw-rw-rw-   0 root         (0) root         (0)     2172 2024-05-08 12:55:44.000000 lusid_express-1.1.2/src/lusid_express/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 12:56:33.273624 lusid_express-1.1.2/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8202 2024-05-08 12:56:33.000000 lusid_express-1.1.2/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      518 2024-05-08 12:56:33.000000 lusid_express-1.1.2/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 12:56:33.000000 lusid_express-1.1.2/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-08 12:56:33.000000 lusid_express-1.1.2/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-08 12:56:33.000000 lusid_express-1.1.2/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:24:02.338680 lusid_express-1.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-08 16:23:17.000000 lusid_express-1.1.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-08 16:23:17.000000 lusid_express-1.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8202 2024-05-08 16:24:02.338680 lusid_express-1.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7562 2024-05-08 16:23:17.000000 lusid_express-1.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 16:24:02.338680 lusid_express-1.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-08 16:23:17.000000 lusid_express-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:24:02.333680 lusid_express-1.1.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:24:02.334680 lusid_express-1.1.4/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-08 16:23:17.000000 lusid_express-1.1.4/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5913 2024-05-08 16:23:17.000000 lusid_express-1.1.4/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:24:02.335680 lusid_express-1.1.4/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-05-08 16:24:01.000000 lusid_express-1.1.4/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:24:02.337680 lusid_express-1.1.4/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-08 16:23:17.000000 lusid_express-1.1.4/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:24:02.338680 lusid_express-1.1.4/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-08 16:23:17.000000 lusid_express-1.1.4/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2024-05-08 16:23:17.000000 lusid_express-1.1.4/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3157 2024-05-08 16:23:17.000000 lusid_express-1.1.4/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:24:02.338680 lusid_express-1.1.4/src/lusid_express/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2172 2024-05-08 16:23:17.000000 lusid_express-1.1.4/src/lusid_express/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 16:24:02.335680 lusid_express-1.1.4/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8202 2024-05-08 16:24:02.000000 lusid_express-1.1.4/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      518 2024-05-08 16:24:02.000000 lusid_express-1.1.4/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 16:24:02.000000 lusid_express-1.1.4/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-08 16:24:02.000000 lusid_express-1.1.4/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-08 16:24:02.000000 lusid_express-1.1.4/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-1.1.2/LICENSE` & `lusid_express-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.2/PKG-INFO` & `lusid_express-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 1.1.2
+Version: 1.1.4
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.1.2/README.md` & `lusid_express-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.2/setup.py` & `lusid_express-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 # List of requirements
 requirements = [
     'pyyaml',
 'luminesce-sdk-preview==1.14.758',
 'lusid-jam==0.1.2',
-'lusid-sdk-preview==1.1.220',
+'lusid-sdk-preview==1.1.420',
 'fbnlab-preview==0.1.108',
 'finbourne-access-sdk==0.0.3751',
 'finbourne-identity-sdk==0.0.2834',
 'finbourne-insights-sdk-preview==0.0.763',
 'finbourne-sdk-utilities==0.0.10',
 'lusid-configuration-sdk-preview==0.1.514',
 'lusid-drive-sdk-preview==0.1.617',
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='1.1.2',
+    version='1.1.4',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-1.1.2/src/lusid_express/__main__.py` & `lusid_express-1.1.4/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.2/src/lusid_express/apis/__init__.py` & `lusid_express-1.1.4/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.2/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-1.1.4/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.2/src/lusid_express/display/__init__.py` & `lusid_express-1.1.4/src/lusid_express/display/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.2/src/lusid_express/load.le` & `lusid_express-1.1.4/src/lusid_express/load.le`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, List
 import uuid
 import os as __os
 
 def load_environment(FBN_SECRETS_PATH:str):
-    """_summary_
+    """_summary_ 
 
     Args:
         FBN_SECRETS_PATH (str): _description_
     """
     __os.environ['FBN_SECRETS_PATH'] =  FBN_SECRETS_PATH
     D = __os.environ.get('FBN_SECRETS_PATH')
     from IPython import get_ipython
```

### Comparing `lusid_express-1.1.2/src/lusid_express/utils/__init__.py` & `lusid_express-1.1.4/src/lusid_express/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.2/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-1.1.4/src/lusid_express.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 1.1.2
+Version: 1.1.4
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.1.2/src/lusid_express.egg-info/SOURCES.txt` & `lusid_express-1.1.4/src/lusid_express.egg-info/SOURCES.txt`

 * *Files identical despite different names*

