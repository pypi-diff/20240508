# Comparing `tmp/lyyre-2.3.tar.gz` & `tmp/lyyre-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyyre-2.3.tar", last modified: Tue Jan  2 05:24:16 2024, max compression
+gzip compressed data, was "lyyre-2.4.tar", last modified: Wed May  8 13:19:41 2024, max compression
```

## Comparing `lyyre-2.3.tar` & `lyyre-2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-01-02 05:24:16.778689 lyyre-2.3/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyre-2.3/LICENSE
--rw-rw-rw-   0        0        0      175 2024-01-02 05:24:16.776688 lyyre-2.3/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyre-2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-02 05:24:16.775689 lyyre-2.3/lyyre.egg-info/
--rw-rw-rw-   0        0        0      175 2024-01-02 05:24:16.000000 lyyre-2.3/lyyre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-01-02 05:24:16.000000 lyyre-2.3/lyyre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-02 05:24:16.000000 lyyre-2.3/lyyre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-01-02 05:24:16.000000 lyyre-2.3/lyyre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-02 05:24:16.000000 lyyre-2.3/lyyre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1546 2023-10-26 22:17:47.000000 lyyre-2.3/lyyre.py
--rw-rw-rw-   0        0        0       42 2024-01-02 05:24:16.778689 lyyre-2.3/setup.cfg
--rw-rw-rw-   0        0        0      262 2024-01-02 05:24:16.000000 lyyre-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:19:41.591094 lyyre-2.4/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyre-2.4/LICENSE
+-rw-rw-rw-   0        0        0      156 2024-05-08 13:19:41.591094 lyyre-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyre-2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 13:19:41.590094 lyyre-2.4/lyyre.egg-info/
+-rw-rw-rw-   0        0        0      156 2024-05-08 13:19:41.000000 lyyre-2.4/lyyre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-08 13:19:41.000000 lyyre-2.4/lyyre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 13:19:41.000000 lyyre-2.4/lyyre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-05-08 13:19:41.000000 lyyre-2.4/lyyre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-08 13:19:41.000000 lyyre-2.4/lyyre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9790 2024-05-08 13:19:36.000000 lyyre-2.4/lyyre.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 13:19:41.591094 lyyre-2.4/setup.cfg
+-rw-rw-rw-   0        0        0      262 2024-05-08 13:19:40.000000 lyyre-2.4/setup.py
```

### Comparing `lyyre-2.3/LICENSE` & `lyyre-2.4/LICENSE`

 * *Files identical despite different names*

