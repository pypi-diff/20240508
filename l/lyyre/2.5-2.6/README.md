# Comparing `tmp/lyyre-2.5.tar.gz` & `tmp/lyyre-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyyre-2.5.tar", last modified: Wed May  8 13:23:56 2024, max compression
+gzip compressed data, was "lyyre-2.6.tar", last modified: Wed May  8 13:27:45 2024, max compression
```

## Comparing `lyyre-2.5.tar` & `lyyre-2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:23:56.330300 lyyre-2.5/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyre-2.5/LICENSE
--rw-rw-rw-   0        0        0      156 2024-05-08 13:23:56.330300 lyyre-2.5/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyre-2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 13:23:56.328977 lyyre-2.5/lyyre.egg-info/
--rw-rw-rw-   0        0        0      156 2024-05-08 13:23:56.000000 lyyre-2.5/lyyre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-08 13:23:56.000000 lyyre-2.5/lyyre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:23:56.000000 lyyre-2.5/lyyre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-05-08 13:23:56.000000 lyyre-2.5/lyyre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-08 13:23:56.000000 lyyre-2.5/lyyre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9790 2024-05-08 13:19:36.000000 lyyre-2.5/lyyre.py
--rw-rw-rw-   0        0        0       42 2024-05-08 13:23:56.330300 lyyre-2.5/setup.cfg
--rw-rw-rw-   0        0        0      262 2024-05-08 13:23:55.000000 lyyre-2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:27:45.754865 lyyre-2.6/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyre-2.6/LICENSE
+-rw-rw-rw-   0        0        0      156 2024-05-08 13:27:45.754865 lyyre-2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyre-2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 13:27:45.752855 lyyre-2.6/lyyre.egg-info/
+-rw-rw-rw-   0        0        0      156 2024-05-08 13:27:45.000000 lyyre-2.6/lyyre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-08 13:27:45.000000 lyyre-2.6/lyyre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 13:27:45.000000 lyyre-2.6/lyyre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-05-08 13:27:45.000000 lyyre-2.6/lyyre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-08 13:27:45.000000 lyyre-2.6/lyyre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9790 2024-05-08 13:19:36.000000 lyyre-2.6/lyyre.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 13:27:45.754865 lyyre-2.6/setup.cfg
+-rw-rw-rw-   0        0        0      262 2024-05-08 13:27:44.000000 lyyre-2.6/setup.py
```

### Comparing `lyyre-2.5/LICENSE` & `lyyre-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lyyre-2.5/lyyre.py` & `lyyre-2.6/lyyre.py`

 * *Files identical despite different names*

