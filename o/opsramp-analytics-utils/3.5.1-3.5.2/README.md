# Comparing `tmp/opsramp-analytics-utils-3.5.1.tar.gz` & `tmp/opsramp-analytics-utils-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsramp-analytics-utils-3.5.1.tar", last modified: Mon Apr 29 12:20:31 2024, max compression
+gzip compressed data, was "opsramp-analytics-utils-3.5.2.tar", last modified: Wed May  8 09:02:44 2024, max compression
```

## Comparing `opsramp-analytics-utils-3.5.1.tar` & `opsramp-analytics-utils-3.5.2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.133774 opsramp-analytics-utils-3.5.1/
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1073 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/LICENSE
--rw-r--r--   0 rajumummidi   (502) staff       (20)      186 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/MANIFEST.in
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-04-29 12:20:31.133632 opsramp-analytics-utils-3.5.1/PKG-INFO
--rw-r--r--   0 rajumummidi   (502) staff       (20)      711 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/README.md
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.119335 opsramp-analytics-utils-3.5.1/analytics_sdk/
--rw-r--r--   0 rajumummidi   (502) staff       (20)       30 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/__init__.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.122779 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/
--rw-r--r--   0 rajumummidi   (502) staff       (20)      921 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.js
--rw-r--r--   0 rajumummidi   (502) staff       (20)  3321723 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.wrapper.css
--rw-r--r--   0 rajumummidi   (502) staff       (20)  2628164 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.wrapper.js
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.130369 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/
--rw-r--r--   0 rajumummidi   (502) staff       (20)      320 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)    34172 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
--rw-r--r--   0 rajumummidi   (502) staff       (20)   148200 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)    64440 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
--rw-r--r--   0 rajumummidi   (502) staff       (20)    29136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
--rw-r--r--   0 rajumummidi   (502) staff       (20)    64608 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
--rw-r--r--   0 rajumummidi   (502) staff       (20)      602 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)      861 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1403 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)     7536 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
--rw-r--r--   0 rajumummidi   (502) staff       (20)    11968 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
--rw-r--r--   0 rajumummidi   (502) staff       (20)    12136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
--rw-r--r--   0 rajumummidi   (502) staff       (20)      733 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.130945 opsramp-analytics-utils-3.5.1/analytics_sdk/api/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/api/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17387 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/api/api_client.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     9382 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/api/api_task.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)      992 2024-01-29 06:36:39.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/api/thread_process.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17374 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/api_client.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4100 2024-03-08 08:04:41.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/components.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/constants.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4730 2024-03-08 08:03:00.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/oap_dash.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.132497 opsramp-analytics-utils-3.5.1/analytics_sdk/process/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/process/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     5809 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/process/process.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4692 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/process/querybuilder.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.132871 opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    35159 2024-04-29 12:18:52.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/excel.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     2887 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/pdf.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    44741 2024-04-29 12:18:52.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/utilities.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.133448 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-04-29 12:20:31.000000 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/PKG-INFO
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1698 2024-04-29 12:20:31.000000 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)        1 2024-04-29 12:20:31.000000 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)      130 2024-04-29 12:20:31.000000 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/requires.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)       14 2024-04-29 12:20:31.000000 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/top_level.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)      144 2024-04-26 11:14:56.000000 opsramp-analytics-utils-3.5.1/requires-install.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2024-04-29 12:20:31.133829 opsramp-analytics-utils-3.5.1/setup.cfg
--rw-r--r--   0 rajumummidi   (502) staff       (20)      943 2024-04-29 10:22:13.000000 opsramp-analytics-utils-3.5.1/setup.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.254931 opsramp-analytics-utils-3.5.2/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1073 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/LICENSE
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      186 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/MANIFEST.in
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-05-08 09:02:44.254803 opsramp-analytics-utils-3.5.2/PKG-INFO
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      711 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/README.md
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.246716 opsramp-analytics-utils-3.5.2/analytics_sdk/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       30 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/__init__.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.248934 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      921 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.js
+-rw-r--r--   0 rajumummidi   (502) staff       (20)  3321723 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.wrapper.css
+-rw-r--r--   0 rajumummidi   (502) staff       (20)  2628164 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.wrapper.js
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.252507 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      320 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    34172 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
+-rw-r--r--   0 rajumummidi   (502) staff       (20)   148200 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    64440 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    29136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    64608 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      602 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      861 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1403 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     7536 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    11968 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    12136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      733 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.253022 opsramp-analytics-utils-3.5.2/analytics_sdk/api/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/api/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17480 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/api/api_client.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     9382 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/api/api_task.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      992 2024-01-29 06:36:39.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/api/thread_process.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17467 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/api_client.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4100 2024-03-08 08:04:41.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/components.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/constants.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4730 2024-03-08 08:03:00.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/oap_dash.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.253393 opsramp-analytics-utils-3.5.2/analytics_sdk/process/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/process/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     5809 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/process/process.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4692 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/process/querybuilder.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.253955 opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    35159 2024-04-29 12:18:52.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/excel.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17745 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/excel_writer.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     2887 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/pdf.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    45289 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/analytics_sdk/utilities.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-08 09:02:44.254604 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-05-08 09:02:44.000000 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1737 2024-05-08 09:02:44.000000 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        1 2024-05-08 09:02:44.000000 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      148 2024-05-08 09:02:44.000000 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/requires.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       14 2024-05-08 09:02:44.000000 opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/top_level.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      162 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/requires-install.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2024-05-08 09:02:44.254985 opsramp-analytics-utils-3.5.2/setup.cfg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      943 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.2/setup.py
```

### Comparing `opsramp-analytics-utils-3.5.1/LICENSE` & `opsramp-analytics-utils-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/PKG-INFO` & `opsramp-analytics-utils-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.5.1
+Version: 3.5.2
 Summary: OpsRamp Analytics SDK
 Home-page: UNKNOWN
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.5.1/README.md` & `opsramp-analytics-utils-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.js` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.wrapper.css` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.wrapper.css`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.wrapper.js` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/main.wrapper.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg` & `opsramp-analytics-utils-3.5.2/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/api/api_client.py` & `opsramp-analytics-utils-3.5.2/analytics_sdk/api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,16 @@
                         else:
                             uri = self.add_page_no_page_size_for_url(add_pageNo, url, page_no, page_size)
                             res = self.get_response(uri, type)
                         if res == None or not res.ok:
                             error_message = f'Get {type} API is failed, run_id ::: {self.run_id}, url ::: {url}, response ::: {res}, response_json ::: {res.json()}, API_Retry_Count ::: {retry_count}'
                             logger.error('Get %s API is failed, run_id ::: %s, url ::: %s, response ::: %s, response_json ::: %s, API_Retry_Count ::: %s ', type, self.run_id, url, res, res.json(), retry_count)
                             res = None
+                            if res.status_code == 410:
+                                break
                             if retry_count > 3:
                                 raise Exception(error_message)
                         elif res.json() is not None and "results" not in res.json():
                             error_message = f"Get {type} results keyword is missing in API response, run_id ::: {self.run_id}, url ::: {url}, response ::: {res}, response_json ::: {res.json()}, API_Retry_Count ::: {retry_count}"
                             logger.error('Get %s results keyword is missing in API response, run_id ::: %s, url ::: %s, response : %s, response_json ::: %s, API_Retry_Count ::: %s ', type, self.run_id, url, res, res.json(), retry_count)
                             res = None
                             if retry_count > 3:
```

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/api/api_task.py` & `opsramp-analytics-utils-3.5.2/analytics_sdk/api/api_task.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/api/thread_process.py` & `opsramp-analytics-utils-3.5.2/analytics_sdk/api/thread_process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/api_client.py` & `opsramp-analytics-utils-3.5.2/analytics_sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,16 @@
                         else:
                             uri = self.add_page_no_page_size_for_url(add_pageNo, url, page_no, page_size)
                             res = self.get_response(uri, type)
                         if res == None or not res.ok:
                             error_message = f'Get {type} API is failed, run_id ::: {self.run_id}, url ::: {url}, response ::: {res}, response_json ::: {res.json()}, API_Retry_Count ::: {retry_count}'
                             logger.error('Get %s API is failed, run_id ::: %s, url ::: %s, response ::: %s, response_json ::: %s, API_Retry_Count ::: %s ', type, self.run_id, url, res, res.json(), retry_count)
                             res = None
+                            if res.status_code == 410:
+                                break
                             if retry_count > 3:
                                 raise Exception(error_message)
                         elif res.json() is not None and "results" not in res.json():
                             error_message = f"Get {type} results keyword is missing in API response, run_id ::: {self.run_id}, url ::: {url}, response ::: {res}, response_json ::: {res.json()}, API_Retry_Count ::: {retry_count}"
                             logger.error('Get %s results keyword is missing in API response, run_id ::: %s, url ::: %s, response : %s, response_json ::: %s, API_Retry_Count ::: %s ', type, self.run_id, url, res, res.json(), retry_count)
                             res = None
                             if retry_count > 3:
```

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/components.py` & `opsramp-analytics-utils-3.5.2/analytics_sdk/components.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/oap_dash.py` & `opsramp-analytics-utils-3.5.2/analytics_sdk/oap_dash.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/process/process.py` & `opsramp-analytics-utils-3.5.2/analytics_sdk/process/process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/process/querybuilder.py` & `opsramp-analytics-utils-3.5.2/analytics_sdk/process/querybuilder.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/excel.py` & `opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/excel.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/pdf.py` & `opsramp-analytics-utils-3.5.2/analytics_sdk/renderer/pdf.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.1/analytics_sdk/utilities.py` & `opsramp-analytics-utils-3.5.2/analytics_sdk/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,14 +519,28 @@
     api_proce_before_time = time.time()
     res = call_put_requests(url , data=json.dumps(data), verify=False);
     api_proce_after_time = time.time()
     api_proce_diff = diff_sec(api_proce_before_time, api_proce_after_time)
     if api_proce_diff > API_TIME_STACKS:
         logging.info('Database update response took %d (greater than %d) seconds', api_proce_diff, API_TIME_STACKS)
     logger.info('Database update response is %s', res)
+    
+    
+def upload_file(run_id, reportname, filepath):
+    if storage_name == 's3':
+        excel_file_location = f'{PLATFORM_ROUTE}/{run_id}/xls/' + reportname
+        excel_url = upload_excel_s3(filepath, BUCKET_NAME, excel_file_location)
+    elif storage_name == 'ceph':
+        excel_file_location = f'{APP_ID.lower()}/{run_id}/xls/' + reportname
+        excel_url = upload_excel_ceph(filepath, BUCKET_NAME, excel_file_location)
+    else:
+        logger.info("No storages are found")
+    
+    delete_excel_file(filepath)
+    return excel_url
 
 
 #Upload excel file to s3
 def upload_excel_s3(local_file, bucket, s3_file):
     retry = 1
     s3 = get_s3_client()
     while retry <= API_RETRY:
```

### Comparing `opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/PKG-INFO` & `opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.5.1
+Version: 3.5.2
 Summary: OpsRamp Analytics SDK
 Home-page: UNKNOWN
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/SOURCES.txt` & `opsramp-analytics-utils-3.5.2/opsramp_analytics_utils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,13 +30,14 @@
 analytics_sdk/api/api_task.py
 analytics_sdk/api/thread_process.py
 analytics_sdk/process/__init__.py
 analytics_sdk/process/process.py
 analytics_sdk/process/querybuilder.py
 analytics_sdk/renderer/__init__.py
 analytics_sdk/renderer/excel.py
+analytics_sdk/renderer/excel_writer.py
 analytics_sdk/renderer/pdf.py
 opsramp_analytics_utils.egg-info/PKG-INFO
 opsramp_analytics_utils.egg-info/SOURCES.txt
 opsramp_analytics_utils.egg-info/dependency_links.txt
 opsramp_analytics_utils.egg-info/requires.txt
 opsramp_analytics_utils.egg-info/top_level.txt
```

### Comparing `opsramp-analytics-utils-3.5.1/setup.py` & `opsramp-analytics-utils-3.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open("requires-{}.txt".format(req_type)) as fp:
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 
 setuptools.setup(
     name="opsramp-analytics-utils",
-    version="3.5.1",
+    version="3.5.2",
     author="OpsRamp",
     author_email="opsramp@support.com",
     description="OpsRamp Analytics SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=read_req_file("install"),
     # url="https://github.com/opsramp/analytics-sdk",
```

