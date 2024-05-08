# Comparing `tmp/md2tgmd-0.1.7.tar.gz` & `tmp/md2tgmd-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2tgmd-0.1.7.tar", last modified: Tue May  7 09:29:49 2024, max compression
+gzip compressed data, was "md2tgmd-0.1.8.tar", last modified: Wed May  8 17:31:29 2024, max compression
```

## Comparing `md2tgmd-0.1.7.tar` & `md2tgmd-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:29:49.025808 md2tgmd-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-07 09:29:41.000000 md2tgmd-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 09:29:49.021808 md2tgmd-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-07 09:29:41.000000 md2tgmd-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:29:49.025808 md2tgmd-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-07 09:29:41.000000 md2tgmd-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:29:49.021808 md2tgmd-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:29:49.021808 md2tgmd-0.1.7/src/md2tgmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-07 09:29:48.000000 md2tgmd-0.1.7/src/md2tgmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 09:29:48.000000 md2tgmd-0.1.7/src/md2tgmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:29:48.000000 md2tgmd-0.1.7/src/md2tgmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 09:29:48.000000 md2tgmd-0.1.7/src/md2tgmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-07 09:29:41.000000 md2tgmd-0.1.7/src/md2tgmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:31:29.440477 md2tgmd-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-08 17:31:21.000000 md2tgmd-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-08 17:31:29.440477 md2tgmd-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-08 17:31:21.000000 md2tgmd-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:31:29.440477 md2tgmd-0.1.8/md2tgmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-08 17:31:29.000000 md2tgmd-0.1.8/md2tgmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-08 17:31:29.000000 md2tgmd-0.1.8/md2tgmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:31:29.000000 md2tgmd-0.1.8/md2tgmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 17:31:29.000000 md2tgmd-0.1.8/md2tgmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:31:29.440477 md2tgmd-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-08 17:31:21.000000 md2tgmd-0.1.8/setup.py
```

### Comparing `md2tgmd-0.1.7/LICENSE` & `md2tgmd-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `md2tgmd-0.1.7/PKG-INFO` & `md2tgmd-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2tgmd
-Version: 0.1.7
+Version: 0.1.8
 Summary: md2tgmd is a Markdown to Telegram-specific-markdown converter.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # md2tgmd
 
 md2tgmd is a Markdown to [Telegram-specific-markdown](https://core.telegram.org/bots/api#formatting-options) converter.
```

### Comparing `md2tgmd-0.1.7/README.md` & `md2tgmd-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `md2tgmd-0.1.7/src/md2tgmd.egg-info/PKG-INFO` & `md2tgmd-0.1.8/md2tgmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2tgmd
-Version: 0.1.7
+Version: 0.1.8
 Summary: md2tgmd is a Markdown to Telegram-specific-markdown converter.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # md2tgmd
 
 md2tgmd is a Markdown to [Telegram-specific-markdown](https://core.telegram.org/bots/api#formatting-options) converter.
```

