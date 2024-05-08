# Comparing `tmp/modelmerge-0.2.0.tar.gz` & `tmp/modelmerge-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.2.0.tar", last modified: Wed May  8 19:06:28 2024, max compression
+gzip compressed data, was "modelmerge-0.2.1.tar", last modified: Wed May  8 19:12:13 2024, max compression
```

## Comparing `modelmerge-0.2.0.tar` & `modelmerge-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.552159 modelmerge-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 19:06:20.000000 modelmerge-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 19:06:28.552159 modelmerge-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 19:06:20.000000 modelmerge-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:06:28.552159 modelmerge-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-08 19:06:20.000000 modelmerge-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.548159 modelmerge-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.548159 modelmerge-0.2.0/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.552159 modelmerge-0.2.0/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28525 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.552159 modelmerge-0.2.0/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.552159 modelmerge-0.2.0/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18685 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/utils/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-08 19:06:20.000000 modelmerge-0.2.0/src/ModelMerge/utils/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:06:28.552159 modelmerge-0.2.0/src/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 19:06:28.000000 modelmerge-0.2.0/src/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-08 19:06:28.000000 modelmerge-0.2.0/src/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:06:28.000000 modelmerge-0.2.0/src/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 19:06:28.000000 modelmerge-0.2.0/src/ModelMerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:06:28.000000 modelmerge-0.2.0/src/ModelMerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.303237 modelmerge-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 19:12:04.000000 modelmerge-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 19:12:13.303237 modelmerge-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 19:12:04.000000 modelmerge-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:12:13.303237 modelmerge-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 19:12:04.000000 modelmerge-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.299237 modelmerge-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.299237 modelmerge-0.2.1/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.303237 modelmerge-0.2.1/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28525 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.303237 modelmerge-0.2.1/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.303237 modelmerge-0.2.1/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18685 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/utils/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-08 19:12:04.000000 modelmerge-0.2.1/src/ModelMerge/utils/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:12:13.303237 modelmerge-0.2.1/src/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 19:12:13.000000 modelmerge-0.2.1/src/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-08 19:12:13.000000 modelmerge-0.2.1/src/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:12:13.000000 modelmerge-0.2.1/src/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 19:12:13.000000 modelmerge-0.2.1/src/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:12:13.000000 modelmerge-0.2.1/src/ModelMerge.egg-info/top_level.txt
```

### Comparing `modelmerge-0.2.0/LICENSE` & `modelmerge-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.0/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.2.1/src/ModelMerge/models/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.0/src/ModelMerge/models/claude.py` & `modelmerge-0.2.1/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.0/src/ModelMerge/models/config.py` & `modelmerge-0.2.1/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.0/src/ModelMerge/models/dalle.py` & `modelmerge-0.2.1/src/ModelMerge/models/dalle.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.0/src/ModelMerge/models/genimi.py` & `modelmerge-0.2.1/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.0/src/ModelMerge/models/groq.py` & `modelmerge-0.2.1/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.0/src/ModelMerge/tools/function_call.py` & `modelmerge-0.2.1/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.0/src/ModelMerge/utils/plugins.py` & `modelmerge-0.2.1/src/ModelMerge/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.0/src/ModelMerge/utils/prompt.py` & `modelmerge-0.2.1/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.2.0/src/ModelMerge.egg-info/SOURCES.txt` & `modelmerge-0.2.1/src/ModelMerge.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 src/ModelMerge/__init__.py
+src/ModelMerge/config.py
 src/ModelMerge.egg-info/PKG-INFO
 src/ModelMerge.egg-info/SOURCES.txt
 src/ModelMerge.egg-info/dependency_links.txt
 src/ModelMerge.egg-info/requires.txt
 src/ModelMerge.egg-info/top_level.txt
 src/ModelMerge/models/__init__.py
 src/ModelMerge/models/chatgpt.py
```

