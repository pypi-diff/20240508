# Comparing `tmp/modelmerge-0.1.6.tar.gz` & `tmp/modelmerge-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.1.6.tar", last modified: Wed May  8 18:28:59 2024, max compression
+gzip compressed data, was "modelmerge-0.1.7.tar", last modified: Wed May  8 18:41:42 2024, max compression
```

## Comparing `modelmerge-0.1.6.tar` & `modelmerge-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:28:59.064345 modelmerge-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 18:28:43.000000 modelmerge-0.1.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:28:59.064345 modelmerge-0.1.6/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:28:59.000000 modelmerge-0.1.6/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 18:28:59.000000 modelmerge-0.1.6/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:28:59.000000 modelmerge-0.1.6/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 18:28:59.000000 modelmerge-0.1.6/ModelMerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:28:59.000000 modelmerge-0.1.6/ModelMerge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:28:59.064345 modelmerge-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 18:28:43.000000 modelmerge-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:28:59.064345 modelmerge-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-08 18:28:43.000000 modelmerge-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:28:59.064345 modelmerge-0.1.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-08 18:28:43.000000 modelmerge-0.1.6/test/test_google_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:41:42.581050 modelmerge-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 18:41:34.000000 modelmerge-0.1.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:41:42.581050 modelmerge-0.1.7/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:41:42.000000 modelmerge-0.1.7/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-08 18:41:42.000000 modelmerge-0.1.7/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:41:42.000000 modelmerge-0.1.7/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 18:41:42.000000 modelmerge-0.1.7/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 18:41:42.000000 modelmerge-0.1.7/ModelMerge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 18:41:42.581050 modelmerge-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 18:41:34.000000 modelmerge-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:41:42.581050 modelmerge-0.1.7/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 18:41:34.000000 modelmerge-0.1.7/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28521 2024-05-08 18:41:34.000000 modelmerge-0.1.7/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-08 18:41:34.000000 modelmerge-0.1.7/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-05-08 18:41:34.000000 modelmerge-0.1.7/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 18:41:34.000000 modelmerge-0.1.7/models/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-08 18:41:34.000000 modelmerge-0.1.7/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 18:41:34.000000 modelmerge-0.1.7/models/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:41:42.581050 modelmerge-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-08 18:41:34.000000 modelmerge-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:41:42.581050 modelmerge-0.1.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-08 18:41:34.000000 modelmerge-0.1.7/test/test_google_search.py
```

### Comparing `modelmerge-0.1.6/LICENSE` & `modelmerge-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.1.6/test/test_google_search.py` & `modelmerge-0.1.7/test/test_google_search.py`

 * *Files identical despite different names*

