# Comparing `tmp/wowotou-1.0.0.tar.gz` & `tmp/wowotou-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wowotou-1.0.0.tar", last modified: Sun May  5 04:43:50 2024, max compression
+gzip compressed data, was "wowotou-1.0.1.tar", last modified: Wed May  8 01:30:09 2024, max compression
```

## Comparing `wowotou-1.0.0.tar` & `wowotou-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 04:43:50.388405 wowotou-1.0.0/
--rw-rw-rw-   0        0        0     1093 2024-05-04 17:10:41.000000 wowotou-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      449 2024-05-05 04:43:50.386405 wowotou-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       60 2024-05-05 04:43:26.000000 wowotou-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 04:43:50.388405 wowotou-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      678 2024-05-04 17:17:47.000000 wowotou-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 04:43:50.372407 wowotou-1.0.0/wowotou/
--rw-rw-rw-   0        0        0        0 2024-05-04 17:17:06.000000 wowotou-1.0.0/wowotou/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 04:43:50.384407 wowotou-1.0.0/wowotou/devtools/
--rw-rw-rw-   0        0        0     1043 2024-05-05 04:39:41.000000 wowotou-1.0.0/wowotou/devtools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 04:43:50.381404 wowotou-1.0.0/wowotou.egg-info/
--rw-rw-rw-   0        0        0      449 2024-05-05 04:43:49.000000 wowotou-1.0.0/wowotou.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2024-05-05 04:43:49.000000 wowotou-1.0.0/wowotou.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 04:43:49.000000 wowotou-1.0.0/wowotou.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-05 04:43:49.000000 wowotou-1.0.0/wowotou.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 01:30:09.931953 wowotou-1.0.1/
+-rw-rw-rw-   0        0        0     1093 2024-05-04 17:10:41.000000 wowotou-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      449 2024-05-08 01:30:09.930953 wowotou-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2024-05-05 04:43:26.000000 wowotou-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 01:30:09.932954 wowotou-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      678 2024-05-08 01:30:05.000000 wowotou-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 01:30:09.921954 wowotou-1.0.1/wowotou/
+-rw-rw-rw-   0        0        0        0 2024-05-04 17:17:06.000000 wowotou-1.0.1/wowotou/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 01:30:09.928955 wowotou-1.0.1/wowotou/devtools/
+-rw-rw-rw-   0        0        0     4184 2024-05-07 17:05:49.000000 wowotou-1.0.1/wowotou/devtools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 01:30:09.926954 wowotou-1.0.1/wowotou.egg-info/
+-rw-rw-rw-   0        0        0      449 2024-05-08 01:30:09.000000 wowotou-1.0.1/wowotou.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2024-05-08 01:30:09.000000 wowotou-1.0.1/wowotou.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 01:30:09.000000 wowotou-1.0.1/wowotou.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-08 01:30:09.000000 wowotou-1.0.1/wowotou.egg-info/top_level.txt
```

### Comparing `wowotou-1.0.0/LICENSE` & `wowotou-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wowotou-1.0.0/setup.py` & `wowotou-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wowotou",
-    version="1.0.0",
+    version="1.0.1",
     author="HisAtri",
     author_email="yz@ghacg.com",
     description="Some useful tools",
     install_requires=[],
     long_description=open(r'README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/HisAtri/wowotou",
```

