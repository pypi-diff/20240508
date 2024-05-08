# Comparing `tmp/amos_api-1.0.0.tar.gz` & `tmp/amos_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amos_api-1.0.0.tar", last modified: Wed May  8 06:29:51 2024, max compression
+gzip compressed data, was "amos_api-1.0.1.tar", last modified: Wed May  8 08:02:36 2024, max compression
```

## Comparing `amos_api-1.0.0.tar` & `amos_api-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 06:29:51.968680 amos_api-1.0.0/
--rw-rw-rw-   0        0        0      178 2024-05-08 06:29:51.968680 amos_api-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1222 2024-05-08 06:19:41.000000 amos_api-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 06:29:51.967675 amos_api-1.0.0/amos_api.egg-info/
--rw-rw-rw-   0        0        0      178 2024-05-08 06:29:51.000000 amos_api-1.0.0/amos_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-05-08 06:29:51.000000 amos_api-1.0.0/amos_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 06:29:51.000000 amos_api-1.0.0/amos_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 06:29:51.000000 amos_api-1.0.0/amos_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 06:29:51.968680 amos_api-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      302 2024-05-08 06:25:55.000000 amos_api-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:02:36.012926 amos_api-1.0.1/
+-rw-rw-rw-   0        0        0        4 2024-05-08 07:51:35.000000 amos_api-1.0.1/.gitignore
+-rw-rw-rw-   0        0        0       40 2024-05-08 07:40:55.000000 amos_api-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      178 2024-05-08 08:02:36.011930 amos_api-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1222 2024-05-08 06:19:41.000000 amos_api-1.0.1/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-08 07:53:03.000000 amos_api-1.0.1/_descr.md
+drwxrwxrwx   0        0        0        0 2024-05-08 08:02:36.010934 amos_api-1.0.1/amos_api.egg-info/
+-rw-rw-rw-   0        0        0      178 2024-05-08 08:02:35.000000 amos_api-1.0.1/amos_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-05-08 08:02:35.000000 amos_api-1.0.1/amos_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:02:35.000000 amos_api-1.0.1/amos_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-08 08:02:35.000000 amos_api-1.0.1/amos_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 08:02:36.012926 amos_api-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      392 2024-05-08 08:02:24.000000 amos_api-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:02:36.010934 amos_api-1.0.1/src/
+-rw-rw-rw-   0        0        0        0 2024-01-17 05:54:47.000000 amos_api-1.0.1/src/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-08 07:57:12.000000 amos_api-1.0.1/src/amos_api.py
+-rw-rw-rw-   0        0        0      571 2024-05-08 06:11:21.000000 amos_api-1.0.1/src/utils.py
```

### Comparing `amos_api-1.0.0/README.md` & `amos_api-1.0.1/README.md`

 * *Files identical despite different names*

