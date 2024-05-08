# Comparing `tmp/new_dt_algorithm-0.7.tar.gz` & `tmp/new_dt_algorithm-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_dt_algorithm-0.7.tar", last modified: Tue May  7 12:18:49 2024, max compression
+gzip compressed data, was "new_dt_algorithm-0.8.tar", last modified: Tue May  7 20:27:47 2024, max compression
```

## Comparing `new_dt_algorithm-0.7.tar` & `new_dt_algorithm-0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 12:18:49.632838 new_dt_algorithm-0.7/
--rw-rw-rw-   0        0        0      214 2024-05-07 12:18:49.632838 new_dt_algorithm-0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-07 11:26:56.000000 new_dt_algorithm-0.7/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 12:18:49.632838 new_dt_algorithm-0.7/new_dt_algorithm.egg-info/
--rw-rw-rw-   0        0        0      214 2024-05-07 12:18:49.000000 new_dt_algorithm-0.7/new_dt_algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-07 12:18:49.000000 new_dt_algorithm-0.7/new_dt_algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 12:18:49.000000 new_dt_algorithm-0.7/new_dt_algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-07 12:18:49.000000 new_dt_algorithm-0.7/new_dt_algorithm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    21851 2024-05-07 12:18:08.000000 new_dt_algorithm-0.7/new_dt_algorithm.py
--rw-rw-rw-   0        0        0       42 2024-05-07 12:18:49.632838 new_dt_algorithm-0.7/setup.cfg
--rw-rw-rw-   0        0        0      443 2024-05-07 12:18:41.000000 new_dt_algorithm-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:27:47.235164 new_dt_algorithm-0.8/
+-rw-rw-rw-   0        0        0      214 2024-05-07 20:27:47.235164 new_dt_algorithm-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:26:56.000000 new_dt_algorithm-0.8/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 20:27:47.219552 new_dt_algorithm-0.8/new_dt_algorithm.egg-info/
+-rw-rw-rw-   0        0        0      214 2024-05-07 20:27:47.000000 new_dt_algorithm-0.8/new_dt_algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-07 20:27:47.000000 new_dt_algorithm-0.8/new_dt_algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 20:27:47.000000 new_dt_algorithm-0.8/new_dt_algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 20:27:47.000000 new_dt_algorithm-0.8/new_dt_algorithm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    55797 2024-05-07 20:26:29.000000 new_dt_algorithm-0.8/new_dt_algorithm.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 20:27:47.235164 new_dt_algorithm-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      443 2024-05-07 20:07:48.000000 new_dt_algorithm-0.8/setup.py
```

