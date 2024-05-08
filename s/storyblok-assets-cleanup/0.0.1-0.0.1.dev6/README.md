# Comparing `tmp/storyblok-assets-cleanup-0.0.1.tar.gz` & `tmp/storyblok-assets-cleanup-0.0.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storyblok-assets-cleanup-0.0.1.tar", last modified: Tue Sep 26 09:08:36 2023, max compression
+gzip compressed data, was "storyblok-assets-cleanup-0.0.1.dev6.tar", last modified: Wed May  8 11:03:07 2024, max compression
```

## Comparing `storyblok-assets-cleanup-0.0.1.tar` & `storyblok-assets-cleanup-0.0.1.dev6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 09:08:36.579865 storyblok-assets-cleanup-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-26 09:08:25.000000 storyblok-assets-cleanup-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2023-09-26 09:08:36.579865 storyblok-assets-cleanup-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-09-26 09:08:25.000000 storyblok-assets-cleanup-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-09-26 09:08:36.579865 storyblok-assets-cleanup-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-09-26 09:08:25.000000 storyblok-assets-cleanup-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 09:08:36.579865 storyblok-assets-cleanup-0.0.1/storyblok_assets_cleanup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2023-09-26 09:08:36.000000 storyblok-assets-cleanup-0.0.1/storyblok_assets_cleanup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-09-26 09:08:36.000000 storyblok-assets-cleanup-0.0.1/storyblok_assets_cleanup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 09:08:36.000000 storyblok-assets-cleanup-0.0.1/storyblok_assets_cleanup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-09-26 09:08:36.000000 storyblok-assets-cleanup-0.0.1/storyblok_assets_cleanup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-26 09:08:36.000000 storyblok-assets-cleanup-0.0.1/storyblok_assets_cleanup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-26 09:08:36.000000 storyblok-assets-cleanup-0.0.1/storyblok_assets_cleanup.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    12154 2023-09-26 09:08:25.000000 storyblok-assets-cleanup-0.0.1/storyblok_assets_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:03:07.650562 storyblok-assets-cleanup-0.0.1.dev6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 11:02:56.000000 storyblok-assets-cleanup-0.0.1.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-08 11:03:07.650562 storyblok-assets-cleanup-0.0.1.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-08 11:02:56.000000 storyblok-assets-cleanup-0.0.1.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-08 11:03:07.650562 storyblok-assets-cleanup-0.0.1.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-08 11:02:56.000000 storyblok-assets-cleanup-0.0.1.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:03:07.650562 storyblok-assets-cleanup-0.0.1.dev6/storyblok_assets_cleanup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-08 11:03:07.000000 storyblok-assets-cleanup-0.0.1.dev6/storyblok_assets_cleanup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-08 11:03:07.000000 storyblok-assets-cleanup-0.0.1.dev6/storyblok_assets_cleanup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:03:07.000000 storyblok-assets-cleanup-0.0.1.dev6/storyblok_assets_cleanup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 11:03:07.000000 storyblok-assets-cleanup-0.0.1.dev6/storyblok_assets_cleanup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 11:03:07.000000 storyblok-assets-cleanup-0.0.1.dev6/storyblok_assets_cleanup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 11:03:07.000000 storyblok-assets-cleanup-0.0.1.dev6/storyblok_assets_cleanup.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12154 2024-05-08 11:02:56.000000 storyblok-assets-cleanup-0.0.1.dev6/storyblok_assets_cleanup.py
```

### Comparing `storyblok-assets-cleanup-0.0.1/LICENSE` & `storyblok-assets-cleanup-0.0.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `storyblok-assets-cleanup-0.0.1/PKG-INFO` & `storyblok-assets-cleanup-0.0.1.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storyblok-assets-cleanup
-Version: 0.0.1
+Version: 0.0.1.dev6
 Summary: Utility to clean unused storyblok assets.
 Home-page: https://github.com/significa/storyblok-assets-cleanup
 Author: Significa
 License: MIT
 Keywords: storyblok
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `storyblok-assets-cleanup-0.0.1/README.md` & `storyblok-assets-cleanup-0.0.1.dev6/README.md`

 * *Files identical despite different names*

### Comparing `storyblok-assets-cleanup-0.0.1/setup.py` & `storyblok-assets-cleanup-0.0.1.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `storyblok-assets-cleanup-0.0.1/storyblok_assets_cleanup.egg-info/PKG-INFO` & `storyblok-assets-cleanup-0.0.1.dev6/storyblok_assets_cleanup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storyblok-assets-cleanup
-Version: 0.0.1
+Version: 0.0.1.dev6
 Summary: Utility to clean unused storyblok assets.
 Home-page: https://github.com/significa/storyblok-assets-cleanup
 Author: Significa
 License: MIT
 Keywords: storyblok
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `storyblok-assets-cleanup-0.0.1/storyblok_assets_cleanup.py` & `storyblok-assets-cleanup-0.0.1.dev6/storyblok_assets_cleanup.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
             to_be_deleted_count,
             path_name,
         ])
 
     print()
 
     if should_delete_images:
-        should_delete_images = input('Do you really want to delete the assets? (y/n): ') != 'y'
+        should_delete_images = input('Do you really want to delete the assets? (y/n): ') == 'y'
     elif backup_assets:
         input('Images will not be deleted but will perform backup. Press any key to continue: ')
     else:
         input('Dry run mode: nothing will be done. Press any key to continue: ')
 
     for asset in assets_not_in_use:
         id = asset["id"]
```

