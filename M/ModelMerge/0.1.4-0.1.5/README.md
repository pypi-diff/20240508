# Comparing `tmp/modelmerge-0.1.4.tar.gz` & `tmp/modelmerge-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.1.4.tar", last modified: Wed May  8 10:12:11 2024, max compression
+gzip compressed data, was "modelmerge-0.1.5.tar", last modified: Wed May  8 17:24:33 2024, max compression
```

## Comparing `modelmerge-0.1.4.tar` & `modelmerge-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:12:11.099353 modelmerge-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 10:12:02.000000 modelmerge-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-08 10:12:11.099353 modelmerge-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 10:12:02.000000 modelmerge-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:12:11.099353 modelmerge-0.1.4/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:12:11.099353 modelmerge-0.1.4/models/ModelMerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-08 10:12:11.000000 modelmerge-0.1.4/models/ModelMerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-08 10:12:11.000000 modelmerge-0.1.4/models/ModelMerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:12:11.000000 modelmerge-0.1.4/models/ModelMerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:12:11.000000 modelmerge-0.1.4/models/ModelMerge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:12:11.099353 modelmerge-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-08 10:12:02.000000 modelmerge-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:24:33.408787 modelmerge-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 17:24:24.000000 modelmerge-0.1.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:24:33.408787 modelmerge-0.1.5/ModelMerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 17:24:33.000000 modelmerge-0.1.5/ModelMerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 17:24:33.000000 modelmerge-0.1.5/ModelMerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:24:33.000000 modelmerge-0.1.5/ModelMerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 17:24:33.000000 modelmerge-0.1.5/ModelMerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:24:33.000000 modelmerge-0.1.5/ModelMerge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-08 17:24:33.408787 modelmerge-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 17:24:24.000000 modelmerge-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:24:33.408787 modelmerge-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 17:24:24.000000 modelmerge-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:24:33.408787 modelmerge-0.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-08 17:24:24.000000 modelmerge-0.1.5/test/test_google_search.py
```

### Comparing `modelmerge-0.1.4/LICENSE` & `modelmerge-0.1.5/LICENSE`

 * *Files identical despite different names*

