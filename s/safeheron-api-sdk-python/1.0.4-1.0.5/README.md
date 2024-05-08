# Comparing `tmp/safeheron_api_sdk_python-1.0.4.tar.gz` & `tmp/safeheron_api_sdk_python-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeheron_api_sdk_python-1.0.4.tar", last modified: Wed May  8 10:19:05 2024, max compression
+gzip compressed data, was "safeheron_api_sdk_python-1.0.5.tar", last modified: Wed May  8 10:41:50 2024, max compression
```

## Comparing `safeheron_api_sdk_python-1.0.4.tar` & `safeheron_api_sdk_python-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:19:05.479512 safeheron_api_sdk_python-1.0.4/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.0.4/LICENSE
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:19:05.478812 safeheron_api_sdk_python-1.0.4/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     4109 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.4/README.md
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.4/README.rst
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:19:05.457304 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1166 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python/client.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     8494 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python/tools.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:19:05.477659 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python.egg-info/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:19:05.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      298 2024-05-08 10:19:05.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 10:19:05.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       25 2024-05-08 10:19:05.000000 safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-08 10:19:05.479659 safeheron_api_sdk_python-1.0.4/setup.cfg
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      681 2024-05-08 10:16:18.000000 safeheron_api_sdk_python-1.0.4/setup.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:41:50.615317 safeheron_api_sdk_python-1.0.5/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.0.5/LICENSE
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:41:50.614349 safeheron_api_sdk_python-1.0.5/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     4109 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.5/README.md
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.5/README.rst
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:41:50.608642 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1166 2024-05-08 10:39:36.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python/client.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     8494 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python/tools.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-08 10:41:50.612756 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python.egg-info/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      405 2024-05-08 10:41:50.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      298 2024-05-08 10:41:50.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 10:41:50.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-08 10:41:50.000000 safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-08 10:41:50.615513 safeheron_api_sdk_python-1.0.5/setup.cfg
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      734 2024-05-08 10:41:16.000000 safeheron_api_sdk_python-1.0.5/setup.py
```

### Comparing `safeheron_api_sdk_python-1.0.4/LICENSE` & `safeheron_api_sdk_python-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.4/README.md` & `safeheron_api_sdk_python-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python/client.py` & `safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python/client.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.0.4/safeheron_api_sdk_python/tools.py` & `safeheron_api_sdk_python-1.0.5/safeheron_api_sdk_python/tools.py`

 * *Files identical despite different names*

