# Comparing `tmp/tool_mapi-4.0.0.tar.gz` & `tmp/tool_mapi-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_mapi-4.0.0.tar", last modified: Wed May  8 08:26:44 2024, max compression
+gzip compressed data, was "tool_mapi-5.0.0.tar", last modified: Wed May  8 08:30:33 2024, max compression
```

## Comparing `tool_mapi-4.0.0.tar` & `tool_mapi-5.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 08:26:44.901024 tool_mapi-4.0.0/
--rw-rw-rw-   0        0        0      203 2024-05-08 08:26:44.896238 tool_mapi-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-08 08:26:44.901024 tool_mapi-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0      973 2024-05-08 08:26:42.000000 tool_mapi-4.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:26:44.838508 tool_mapi-4.0.0/tool_mapi/
--rw-rw-rw-   0        0        0        1 2023-09-12 12:45:39.000000 tool_mapi-4.0.0/tool_mapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:26:44.879621 tool_mapi-4.0.0/tool_mapi/clitools/
--rw-rw-rw-   0        0        0        0 2023-09-12 12:45:39.000000 tool_mapi-4.0.0/tool_mapi/clitools/__init__.py
--rw-rw-rw-   0        0        0      350 2023-09-12 12:45:39.000000 tool_mapi-4.0.0/tool_mapi/clitools/print_hello_worlds.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:26:44.891513 tool_mapi-4.0.0/tool_mapi/helloworld/
--rw-rw-rw-   0        0        0       26 2023-09-12 12:45:39.000000 tool_mapi-4.0.0/tool_mapi/helloworld/__init__.py
--rw-rw-rw-   0        0        0      483 2023-09-12 12:45:39.000000 tool_mapi-4.0.0/tool_mapi/helloworld/helloworld.py
--rw-rw-rw-   0        0        0      431 2023-09-12 12:45:39.000000 tool_mapi-4.0.0/tool_mapi/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:26:44.867286 tool_mapi-4.0.0/tool_mapi.egg-info/
--rw-rw-rw-   0        0        0      203 2024-05-08 08:26:44.000000 tool_mapi-4.0.0/tool_mapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2024-05-08 08:26:44.000000 tool_mapi-4.0.0/tool_mapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 08:26:44.000000 tool_mapi-4.0.0/tool_mapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 08:26:44.000000 tool_mapi-4.0.0/tool_mapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 08:30:33.431615 tool_mapi-5.0.0/
+-rw-rw-rw-   0        0        0      203 2024-05-08 08:30:33.423860 tool_mapi-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-08 08:30:33.433070 tool_mapi-5.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      973 2024-05-08 08:27:49.000000 tool_mapi-5.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:30:33.352618 tool_mapi-5.0.0/tool_mapi/
+-rw-rw-rw-   0        0        0        1 2023-09-12 12:45:39.000000 tool_mapi-5.0.0/tool_mapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:30:33.400096 tool_mapi-5.0.0/tool_mapi/clitools/
+-rw-rw-rw-   0        0        0        0 2023-09-12 12:45:39.000000 tool_mapi-5.0.0/tool_mapi/clitools/__init__.py
+-rw-rw-rw-   0        0        0      350 2023-09-12 12:45:39.000000 tool_mapi-5.0.0/tool_mapi/clitools/print_hello_worlds.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:30:33.416258 tool_mapi-5.0.0/tool_mapi/helloworld/
+-rw-rw-rw-   0        0        0       26 2023-09-12 12:45:39.000000 tool_mapi-5.0.0/tool_mapi/helloworld/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-09-12 12:45:39.000000 tool_mapi-5.0.0/tool_mapi/helloworld/helloworld.py
+-rw-rw-rw-   0        0        0      431 2023-09-12 12:45:39.000000 tool_mapi-5.0.0/tool_mapi/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:30:33.388923 tool_mapi-5.0.0/tool_mapi.egg-info/
+-rw-rw-rw-   0        0        0      203 2024-05-08 08:30:33.000000 tool_mapi-5.0.0/tool_mapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2024-05-08 08:30:33.000000 tool_mapi-5.0.0/tool_mapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:30:33.000000 tool_mapi-5.0.0/tool_mapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 08:30:33.000000 tool_mapi-5.0.0/tool_mapi.egg-info/top_level.txt
```

### Comparing `tool_mapi-4.0.0/setup.py` & `tool_mapi-5.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_packages, setup
 # !python3 -m pip install wheel
 # !python3 -m  pip install setuptools
 # !python3 -m  pip install twine
 
 
-MAJOR = 4
+MAJOR = 5
 MINOR = 0
 MICRO = 0
 VERSION = '%d.%d.%d'%(MAJOR,MINOR,MICRO)
 
  
 name='tool_mapi'
 def _find_packages(packages , name):
```

