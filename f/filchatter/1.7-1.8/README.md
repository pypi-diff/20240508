# Comparing `tmp/filchatter-1.7.tar.gz` & `tmp/filchatter-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filchatter-1.7.tar", last modified: Tue May  7 09:45:22 2024, max compression
+gzip compressed data, was "filchatter-1.8.tar", last modified: Wed May  8 10:59:52 2024, max compression
```

## Comparing `filchatter-1.7.tar` & `filchatter-1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:45:22.108937 filchatter-1.7/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:45:22.087992 filchatter-1.7/Filchatter/
--rw-rw-rw-   0        0        0       62 2024-05-04 06:42:16.000000 filchatter-1.7/Filchatter/__init__.py
--rw-rw-rw-   0        0        0     1035 2024-05-07 09:44:39.000000 filchatter-1.7/Filchatter/filchatter.py
--rw-rw-rw-   0        0        0     1070 2024-05-04 05:07:58.000000 filchatter-1.7/LICENSE.md
--rw-rw-rw-   0        0        0      106 2024-05-07 09:45:22.106941 filchatter-1.7/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-04 05:10:02.000000 filchatter-1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 09:45:22.105944 filchatter-1.7/filchatter.egg-info/
--rw-rw-rw-   0        0        0      106 2024-05-07 09:45:21.000000 filchatter-1.7/filchatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-05-07 09:45:22.000000 filchatter-1.7/filchatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:45:21.000000 filchatter-1.7/filchatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-07 09:45:21.000000 filchatter-1.7/filchatter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 09:45:21.000000 filchatter-1.7/filchatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-07 09:45:21.000000 filchatter-1.7/filchatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 09:45:22.108937 filchatter-1.7/setup.cfg
--rw-rw-rw-   0        0        0      278 2024-05-07 09:45:15.000000 filchatter-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:59:52.045936 filchatter-1.8/
+drwxrwxrwx   0        0        0        0 2024-05-08 10:59:52.010472 filchatter-1.8/Filchatter/
+-rw-rw-rw-   0        0        0       62 2024-05-04 06:42:16.000000 filchatter-1.8/Filchatter/__init__.py
+-rw-rw-rw-   0        0        0     1035 2024-05-08 10:59:20.000000 filchatter-1.8/Filchatter/filchatter.py
+-rw-rw-rw-   0        0        0     1070 2024-05-04 05:07:58.000000 filchatter-1.8/LICENSE.md
+-rw-rw-rw-   0        0        0      106 2024-05-08 10:59:52.044938 filchatter-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-04 05:10:02.000000 filchatter-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 10:59:52.042944 filchatter-1.8/filchatter.egg-info/
+-rw-rw-rw-   0        0        0      106 2024-05-08 10:59:51.000000 filchatter-1.8/filchatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-08 10:59:51.000000 filchatter-1.8/filchatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 10:59:51.000000 filchatter-1.8/filchatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-08 10:59:51.000000 filchatter-1.8/filchatter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 10:59:51.000000 filchatter-1.8/filchatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 10:59:51.000000 filchatter-1.8/filchatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 10:59:52.046933 filchatter-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      278 2024-05-08 10:59:25.000000 filchatter-1.8/setup.py
```

### Comparing `filchatter-1.7/Filchatter/filchatter.py` & `filchatter-1.8/Filchatter/filchatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
 class Filchatter:
-    url = "http://210.113.121.214:4440"
+    url = "http://218.239.229.119:4440"
 
     def __init__(self, api_key= None):
         self.session = requests.Session()
         self.set_api_key(api_key)
         
     def set_api_key(self, key):
         self.api_key = key
```

### Comparing `filchatter-1.7/LICENSE.md` & `filchatter-1.8/LICENSE.md`

 * *Files identical despite different names*

