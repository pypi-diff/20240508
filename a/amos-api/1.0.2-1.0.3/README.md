# Comparing `tmp/amos_api-1.0.2.tar.gz` & `tmp/amos_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amos_api-1.0.2.tar", last modified: Wed May  8 08:07:54 2024, max compression
+gzip compressed data, was "amos_api-1.0.3.tar", last modified: Wed May  8 08:21:31 2024, max compression
```

## Comparing `amos_api-1.0.2.tar` & `amos_api-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 08:07:54.410423 amos_api-1.0.2/
--rw-rw-rw-   0        0        0        4 2024-05-08 07:51:35.000000 amos_api-1.0.2/.gitignore
--rw-rw-rw-   0        0        0       40 2024-05-08 07:40:55.000000 amos_api-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      178 2024-05-08 08:07:54.409425 amos_api-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1222 2024-05-08 06:19:41.000000 amos_api-1.0.2/README.md
--rw-rw-rw-   0        0        0       86 2024-05-08 07:53:03.000000 amos_api-1.0.2/_descr.md
-drwxrwxrwx   0        0        0        0 2024-05-08 08:07:54.409425 amos_api-1.0.2/amos_api.egg-info/
--rw-rw-rw-   0        0        0      178 2024-05-08 08:07:54.000000 amos_api-1.0.2/amos_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-05-08 08:07:54.000000 amos_api-1.0.2/amos_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 08:07:54.000000 amos_api-1.0.2/amos_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-08 08:07:54.000000 amos_api-1.0.2/amos_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 08:07:54.410423 amos_api-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      392 2024-05-08 08:07:37.000000 amos_api-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:07:54.408426 amos_api-1.0.2/src/
--rw-rw-rw-   0        0        0       82 2024-05-08 08:07:22.000000 amos_api-1.0.2/src/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-08 08:07:24.000000 amos_api-1.0.2/src/amos_api.py
--rw-rw-rw-   0        0        0      571 2024-05-08 06:11:21.000000 amos_api-1.0.2/src/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:21:31.338693 amos_api-1.0.3/
+-rw-rw-rw-   0        0        0        4 2024-05-08 07:51:35.000000 amos_api-1.0.3/.gitignore
+-rw-rw-rw-   0        0        0       40 2024-05-08 07:40:55.000000 amos_api-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1674 2024-05-08 08:21:31.338693 amos_api-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1222 2024-05-08 06:19:41.000000 amos_api-1.0.3/README.md
+-rw-rw-rw-   0        0        0       82 2024-05-08 08:07:22.000000 amos_api-1.0.3/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-05-08 07:53:03.000000 amos_api-1.0.3/_descr.md
+-rw-rw-rw-   0        0        0      565 2024-05-08 08:21:16.000000 amos_api-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 08:21:31.338693 amos_api-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 08:21:31.333709 amos_api-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 08:21:31.337696 amos_api-1.0.3/src/amos_api.egg-info/
+-rw-rw-rw-   0        0        0     1674 2024-05-08 08:21:31.000000 amos_api-1.0.3/src/amos_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-08 08:21:31.000000 amos_api-1.0.3/src/amos_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:21:31.000000 amos_api-1.0.3/src/amos_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 08:21:31.000000 amos_api-1.0.3/src/amos_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 08:21:31.000000 amos_api-1.0.3/src/amos_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-08 08:07:24.000000 amos_api-1.0.3/src/amos_api.py
+-rw-rw-rw-   0        0        0      571 2024-05-08 06:11:21.000000 amos_api-1.0.3/utils.py
```

### Comparing `amos_api-1.0.2/README.md` & `amos_api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `amos_api-1.0.2/src/utils.py` & `amos_api-1.0.3/utils.py`

 * *Files identical despite different names*

