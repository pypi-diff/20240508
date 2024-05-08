# Comparing `tmp/tool_mapi-2.0.0.tar.gz` & `tmp/tool_mapi-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_mapi-2.0.0.tar", last modified: Wed May  8 08:25:31 2024, max compression
+gzip compressed data, was "tool_mapi-3.0.0.tar", last modified: Wed May  8 08:26:15 2024, max compression
```

## Comparing `tool_mapi-2.0.0.tar` & `tool_mapi-3.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 08:25:31.478987 tool_mapi-2.0.0/
--rw-rw-rw-   0        0        0      188 2024-05-08 08:25:31.473730 tool_mapi-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-08 08:25:31.478987 tool_mapi-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      973 2024-05-08 08:24:28.000000 tool_mapi-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:25:31.406019 tool_mapi-2.0.0/tool_mapi/
--rw-rw-rw-   0        0        0        1 2023-09-12 12:45:39.000000 tool_mapi-2.0.0/tool_mapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:25:31.447954 tool_mapi-2.0.0/tool_mapi/clitools/
--rw-rw-rw-   0        0        0        0 2023-09-12 12:45:39.000000 tool_mapi-2.0.0/tool_mapi/clitools/__init__.py
--rw-rw-rw-   0        0        0      350 2023-09-12 12:45:39.000000 tool_mapi-2.0.0/tool_mapi/clitools/print_hello_worlds.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:25:31.464710 tool_mapi-2.0.0/tool_mapi/helloworld/
--rw-rw-rw-   0        0        0       26 2023-09-12 12:45:39.000000 tool_mapi-2.0.0/tool_mapi/helloworld/__init__.py
--rw-rw-rw-   0        0        0      483 2023-09-12 12:45:39.000000 tool_mapi-2.0.0/tool_mapi/helloworld/helloworld.py
--rw-rw-rw-   0        0        0      431 2023-09-12 12:45:39.000000 tool_mapi-2.0.0/tool_mapi/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:25:31.437031 tool_mapi-2.0.0/tool_mapi.egg-info/
--rw-rw-rw-   0        0        0      188 2024-05-08 08:25:31.000000 tool_mapi-2.0.0/tool_mapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2024-05-08 08:25:31.000000 tool_mapi-2.0.0/tool_mapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 08:25:31.000000 tool_mapi-2.0.0/tool_mapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 08:25:31.000000 tool_mapi-2.0.0/tool_mapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 08:26:15.224137 tool_mapi-3.0.0/
+-rw-rw-rw-   0        0        0      198 2024-05-08 08:26:15.221496 tool_mapi-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-08 08:26:15.224137 tool_mapi-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      971 2024-05-08 08:26:10.000000 tool_mapi-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:26:15.173972 tool_mapi-3.0.0/tool_mapi/
+-rw-rw-rw-   0        0        0        1 2023-09-12 12:45:39.000000 tool_mapi-3.0.0/tool_mapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:26:15.207950 tool_mapi-3.0.0/tool_mapi/clitools/
+-rw-rw-rw-   0        0        0        0 2023-09-12 12:45:39.000000 tool_mapi-3.0.0/tool_mapi/clitools/__init__.py
+-rw-rw-rw-   0        0        0      350 2023-09-12 12:45:39.000000 tool_mapi-3.0.0/tool_mapi/clitools/print_hello_worlds.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:26:15.217453 tool_mapi-3.0.0/tool_mapi/helloworld/
+-rw-rw-rw-   0        0        0       26 2023-09-12 12:45:39.000000 tool_mapi-3.0.0/tool_mapi/helloworld/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-09-12 12:45:39.000000 tool_mapi-3.0.0/tool_mapi/helloworld/helloworld.py
+-rw-rw-rw-   0        0        0      431 2023-09-12 12:45:39.000000 tool_mapi-3.0.0/tool_mapi/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:26:15.201427 tool_mapi-3.0.0/tool_mapi.egg-info/
+-rw-rw-rw-   0        0        0      198 2024-05-08 08:26:15.000000 tool_mapi-3.0.0/tool_mapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2024-05-08 08:26:15.000000 tool_mapi-3.0.0/tool_mapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:26:15.000000 tool_mapi-3.0.0/tool_mapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 08:26:15.000000 tool_mapi-3.0.0/tool_mapi.egg-info/top_level.txt
```

### Comparing `tool_mapi-2.0.0/setup.py` & `tool_mapi-3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_packages, setup
 # !python3 -m pip install wheel
 # !python3 -m  pip install setuptools
 # !python3 -m  pip install twine
 
 
-MAJOR = 2
+MAJOR = 3
 MINOR = 0
 MICRO = 0
 VERSION = '%d.%d.%d'%(MAJOR,MINOR,MICRO)
 
  
 name='tool_mapi'
 def _find_packages(packages , name):
@@ -19,15 +19,15 @@
             return  packages
 packages=[i for i in find_packages() if _find_packages(i , name )  ]
 
 setup(
     name=name,
     packages=packages,
     version=VERSION,
-    # description='tool_mapi library',
+    description='tool_mapi library',
     author='Me',
 )
 
 
 # pip install wheel
 # pip install twine
```

