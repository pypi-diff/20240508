# Comparing `tmp/charzr_lib-1.0.1.tar.gz` & `tmp/charzr_lib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charzr_lib-1.0.1.tar", last modified: Wed May  8 00:53:36 2024, max compression
+gzip compressed data, was "charzr_lib-1.0.2.tar", last modified: Wed May  8 01:07:33 2024, max compression
```

## Comparing `charzr_lib-1.0.1.tar` & `charzr_lib-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 00:53:36.774624 charzr_lib-1.0.1/
--rw-rw-rw-   0        0        0      346 2024-05-08 00:53:36.771695 charzr_lib-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 00:53:36.399729 charzr_lib-1.0.1/charzr_lib/
--rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.1/charzr_lib/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.1/charzr_lib/pokemon.csv
--rw-rw-rw-   0        0        0      743 2024-05-08 00:26:00.000000 charzr_lib-1.0.1/charzr_lib/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-08 00:53:36.769743 charzr_lib-1.0.1/charzr_lib.egg-info/
--rw-rw-rw-   0        0        0      346 2024-05-08 00:53:34.000000 charzr_lib-1.0.1/charzr_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-08 00:53:34.000000 charzr_lib-1.0.1/charzr_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 00:53:34.000000 charzr_lib-1.0.1/charzr_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-08 00:53:34.000000 charzr_lib-1.0.1/charzr_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 00:53:34.000000 charzr_lib-1.0.1/charzr_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 00:53:36.774624 charzr_lib-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      474 2024-05-08 00:49:10.000000 charzr_lib-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 01:07:33.141656 charzr_lib-1.0.2/
+-rw-rw-rw-   0        0        0      316 2024-05-08 01:07:33.136775 charzr_lib-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 01:07:33.044027 charzr_lib-1.0.2/charzr_lib/
+-rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.2/charzr_lib/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.2/charzr_lib/pokemon.csv
+-rw-rw-rw-   0        0        0      743 2024-05-08 00:26:00.000000 charzr_lib-1.0.2/charzr_lib/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-08 01:07:33.133847 charzr_lib-1.0.2/charzr_lib.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-05-08 01:07:32.000000 charzr_lib-1.0.2/charzr_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-08 01:07:32.000000 charzr_lib-1.0.2/charzr_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 01:07:32.000000 charzr_lib-1.0.2/charzr_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 01:07:32.000000 charzr_lib-1.0.2/charzr_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 01:07:32.000000 charzr_lib-1.0.2/charzr_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 01:07:33.141656 charzr_lib-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      454 2024-05-08 01:06:42.000000 charzr_lib-1.0.2/setup.py
```

### Comparing `charzr_lib-1.0.1/README.md` & `charzr_lib-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.1/charzr_lib/pokemon.csv` & `charzr_lib-1.0.2/charzr_lib/pokemon.csv`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.1/charzr_lib/random_pokemon.py` & `charzr_lib-1.0.2/charzr_lib/random_pokemon.py`

 * *Files identical despite different names*

