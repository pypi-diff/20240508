# Comparing `tmp/lyyddmsg-1.1.tar.gz` & `tmp/lyyddmsg-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyyddmsg-1.1.tar", last modified: Tue Apr 30 00:48:23 2024, max compression
+gzip compressed data, was "lyyddmsg-1.2.tar", last modified: Wed May  8 13:11:39 2024, max compression
```

## Comparing `lyyddmsg-1.1.tar` & `lyyddmsg-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 00:48:23.650228 lyyddmsg-1.1/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyddmsg-1.1/LICENSE
--rw-rw-rw-   0        0        0      159 2024-04-30 00:48:23.650228 lyyddmsg-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyddmsg-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 00:48:23.648215 lyyddmsg-1.1/lyyddmsg.egg-info/
--rw-rw-rw-   0        0        0      159 2024-04-30 00:48:23.000000 lyyddmsg-1.1/lyyddmsg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2024-04-30 00:48:23.000000 lyyddmsg-1.1/lyyddmsg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 00:48:23.000000 lyyddmsg-1.1/lyyddmsg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 00:48:23.000000 lyyddmsg-1.1/lyyddmsg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    25075 2024-03-02 00:08:57.000000 lyyddmsg-1.1/lyyddmsg.py
--rw-rw-rw-   0        0        0       42 2024-04-30 00:48:23.650228 lyyddmsg-1.1/setup.cfg
--rw-rw-rw-   0        0        0      262 2024-04-30 00:48:22.000000 lyyddmsg-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 13:11:39.547817 lyyddmsg-1.2/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyddmsg-1.2/LICENSE
+-rw-rw-rw-   0        0        0      159 2024-05-08 13:11:39.546811 lyyddmsg-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyddmsg-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 13:11:39.545809 lyyddmsg-1.2/lyyddmsg.egg-info/
+-rw-rw-rw-   0        0        0      159 2024-05-08 13:11:39.000000 lyyddmsg-1.2/lyyddmsg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2024-05-08 13:11:39.000000 lyyddmsg-1.2/lyyddmsg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 13:11:39.000000 lyyddmsg-1.2/lyyddmsg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 13:11:39.000000 lyyddmsg-1.2/lyyddmsg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17479 2024-05-08 13:11:35.000000 lyyddmsg-1.2/lyyddmsg.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 13:11:39.547817 lyyddmsg-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      262 2024-05-08 13:11:38.000000 lyyddmsg-1.2/setup.py
```

### Comparing `lyyddmsg-1.1/LICENSE` & `lyyddmsg-1.2/LICENSE`

 * *Files identical despite different names*

