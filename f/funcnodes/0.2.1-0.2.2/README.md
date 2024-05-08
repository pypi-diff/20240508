# Comparing `tmp/funcnodes-0.2.1.tar.gz` & `tmp/funcnodes-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes-0.2.1.tar", max compression
+gzip compressed data, was "funcnodes-0.2.2.tar", max compression
```

## Comparing `funcnodes-0.2.1.tar` & `funcnodes-0.2.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     1680 2024-05-08 12:53:16.958919 funcnodes-0.2.1/funcnodes/__init__.py
--rw-r--r--   0        0        0     6499 2024-05-07 08:28:48.305494 funcnodes-0.2.1/funcnodes/__main__.py
--rw-r--r--   0        0        0     2032 2024-05-06 20:07:59.075924 funcnodes-0.2.1/funcnodes/_logging.py
--rw-r--r--   0        0        0      313 2024-04-11 20:53:13.157950 funcnodes-0.2.1/funcnodes/basic_nodes/__init__.py
--rw-r--r--   0        0        0     4391 2024-05-07 07:50:51.041520 funcnodes-0.2.1/funcnodes/basic_nodes/files.py
--rw-r--r--   0        0        0     3474 2024-05-07 07:39:01.326392 funcnodes-0.2.1/funcnodes/basic_nodes/logic.py
--rw-r--r--   0        0        0    11280 2024-05-05 22:02:37.701451 funcnodes-0.2.1/funcnodes/basic_nodes/math.py
--rw-r--r--   0        0        0     3593 2024-05-06 20:07:58.990311 funcnodes-0.2.1/funcnodes/config.py
--rw-r--r--   0        0        0    22123 2024-05-07 08:27:31.506589 funcnodes-0.2.1/funcnodes/eventmanager.py
--rw-r--r--   0        0        0      125 2024-05-06 20:08:00.654935 funcnodes-0.2.1/funcnodes/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.2.1/funcnodes/frontends/__init__.py
--rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/__init__.py
--rw-r--r--   0        0        0      965 2024-04-25 08:06:56.551013 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/asset-manifest.json
--rw-r--r--   0        0        0    28362 2024-04-25 08:34:16.885037 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/css/style.css
--rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/favicon.ico
--rw-r--r--   0        0        0      658 2024-04-25 08:27:16.808142 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/index.html
--rw-r--r--   0        0        0  4138461 2024-04-25 08:27:16.808142 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/424.js
--rw-r--r--   0        0        0     3258 2024-04-25 08:27:16.808142 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt
--rw-r--r--   0        0        0   246139 2024-04-25 08:34:16.885037 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/main.js
--rw-r--r--   0        0        0    11348 2024-04-25 08:27:16.808142 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt
--rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/logo192.png
--rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/logo512.png
--rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/manifest.json
--rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/robots.txt
--rw-r--r--   0        0        0     2952 2024-04-25 08:14:13.637341 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/run.py
--rw-r--r--   0        0        0    27882 2024-05-06 04:17:35.134204 funcnodes-0.2.1/funcnodes/io.py
--rw-r--r--   0        0        0      421 2024-04-12 04:01:45.484336 funcnodes-0.2.1/funcnodes/lib/__init__.py
--rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.2.1/funcnodes/lib/lib.py
--rw-r--r--   0        0        0     7107 2024-05-08 11:06:44.923372 funcnodes-0.2.1/funcnodes/lib/libfinder.py
--rw-r--r--   0        0        0     1792 2024-04-16 04:49:07.183174 funcnodes-0.2.1/funcnodes/lib/libparser.py
--rw-r--r--   0        0        0    31452 2024-05-07 15:29:57.471965 funcnodes-0.2.1/funcnodes/node.py
--rw-r--r--   0        0        0    19738 2024-05-07 08:39:11.933956 funcnodes-0.2.1/funcnodes/nodemaker.py
--rw-r--r--   0        0        0    11850 2024-05-07 03:17:09.186518 funcnodes-0.2.1/funcnodes/nodespace.py
--rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.2.1/funcnodes/triggerstack.py
--rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.2.1/funcnodes/utils/__init__.py
--rw-r--r--   0        0        0     3189 2024-04-11 08:37:44.578407 funcnodes-0.2.1/funcnodes/utils/data.py
--rw-r--r--   0        0        0     2744 2024-02-23 07:11:27.812331 funcnodes-0.2.1/funcnodes/utils/nodeutils.py
--rw-r--r--   0        0        0     5271 2024-05-07 08:22:20.139829 funcnodes-0.2.1/funcnodes/utils/serialization.py
--rw-r--r--   0        0        0      444 2024-05-07 13:05:54.019733 funcnodes-0.2.1/funcnodes/worker/__init__.py
--rw-r--r--   0        0        0     1808 2024-05-07 08:35:08.888378 funcnodes-0.2.1/funcnodes/worker/external_worker.py
--rw-r--r--   0        0        0     3736 2024-03-26 07:43:19.651903 funcnodes-0.2.1/funcnodes/worker/loop.py
--rw-r--r--   0        0        0     3293 2024-05-07 08:43:41.552734 funcnodes-0.2.1/funcnodes/worker/remote_worker.py
--rw-r--r--   0        0        0     8270 2024-05-07 08:43:38.346889 funcnodes-0.2.1/funcnodes/worker/websocket.py
--rw-r--r--   0        0        0    37914 2024-05-07 08:42:49.613686 funcnodes-0.2.1/funcnodes/worker/worker.py
--rw-r--r--   0        0        0    30152 2024-05-06 20:08:11.694569 funcnodes-0.2.1/funcnodes/worker/worker_manager.py
--rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.2.1/LICENSE
--rw-r--r--   0        0        0      666 2024-05-08 12:53:01.277391 funcnodes-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    13174 2024-05-07 11:03:57.250582 funcnodes-0.2.1/README.md
--rw-r--r--   0        0        0    13528 1970-01-01 00:00:00.000000 funcnodes-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1725 2024-05-08 14:07:34.465134 funcnodes-0.2.2/funcnodes/__init__.py
+-rw-r--r--   0        0        0     6499 2024-05-07 08:28:48.305494 funcnodes-0.2.2/funcnodes/__main__.py
+-rw-r--r--   0        0        0     2032 2024-05-06 20:07:59.075924 funcnodes-0.2.2/funcnodes/_logging.py
+-rw-r--r--   0        0        0      313 2024-04-11 20:53:13.157950 funcnodes-0.2.2/funcnodes/basic_nodes/__init__.py
+-rw-r--r--   0        0        0     4391 2024-05-07 07:50:51.041520 funcnodes-0.2.2/funcnodes/basic_nodes/files.py
+-rw-r--r--   0        0        0     3474 2024-05-07 07:39:01.326392 funcnodes-0.2.2/funcnodes/basic_nodes/logic.py
+-rw-r--r--   0        0        0    11280 2024-05-05 22:02:37.701451 funcnodes-0.2.2/funcnodes/basic_nodes/math.py
+-rw-r--r--   0        0        0     3593 2024-05-06 20:07:58.990311 funcnodes-0.2.2/funcnodes/config.py
+-rw-r--r--   0        0        0     1270 2024-05-08 14:07:13.608817 funcnodes-0.2.2/funcnodes/data.py
+-rw-r--r--   0        0        0    22123 2024-05-07 08:27:31.506589 funcnodes-0.2.2/funcnodes/eventmanager.py
+-rw-r--r--   0        0        0      125 2024-05-06 20:08:00.654935 funcnodes-0.2.2/funcnodes/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.2.2/funcnodes/frontends/__init__.py
+-rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-25 08:06:56.551013 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/asset-manifest.json
+-rw-r--r--   0        0        0    28362 2024-04-25 08:34:16.885037 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/css/style.css
+-rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/favicon.ico
+-rw-r--r--   0        0        0      658 2024-04-25 08:27:16.808142 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/index.html
+-rw-r--r--   0        0        0  4138461 2024-04-25 08:27:16.808142 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/js/424.js
+-rw-r--r--   0        0        0     3258 2024-04-25 08:27:16.808142 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt
+-rw-r--r--   0        0        0   246139 2024-04-25 08:34:16.885037 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/js/main.js
+-rw-r--r--   0        0        0    11348 2024-04-25 08:27:16.808142 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt
+-rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/logo192.png
+-rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/logo512.png
+-rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/manifest.json
+-rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/robots.txt
+-rw-r--r--   0        0        0     2952 2024-04-25 08:14:13.637341 funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/run.py
+-rw-r--r--   0        0        0    27882 2024-05-06 04:17:35.134204 funcnodes-0.2.2/funcnodes/io.py
+-rw-r--r--   0        0        0      421 2024-04-12 04:01:45.484336 funcnodes-0.2.2/funcnodes/lib/__init__.py
+-rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.2.2/funcnodes/lib/lib.py
+-rw-r--r--   0        0        0     7107 2024-05-08 11:06:44.923372 funcnodes-0.2.2/funcnodes/lib/libfinder.py
+-rw-r--r--   0        0        0     1792 2024-04-16 04:49:07.183174 funcnodes-0.2.2/funcnodes/lib/libparser.py
+-rw-r--r--   0        0        0    31452 2024-05-07 15:29:57.471965 funcnodes-0.2.2/funcnodes/node.py
+-rw-r--r--   0        0        0    19738 2024-05-07 08:39:11.933956 funcnodes-0.2.2/funcnodes/nodemaker.py
+-rw-r--r--   0        0        0    11850 2024-05-07 03:17:09.186518 funcnodes-0.2.2/funcnodes/nodespace.py
+-rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.2.2/funcnodes/triggerstack.py
+-rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.2.2/funcnodes/utils/__init__.py
+-rw-r--r--   0        0        0     3189 2024-04-11 08:37:44.578407 funcnodes-0.2.2/funcnodes/utils/data.py
+-rw-r--r--   0        0        0     2744 2024-02-23 07:11:27.812331 funcnodes-0.2.2/funcnodes/utils/nodeutils.py
+-rw-r--r--   0        0        0     5271 2024-05-07 08:22:20.139829 funcnodes-0.2.2/funcnodes/utils/serialization.py
+-rw-r--r--   0        0        0      444 2024-05-07 13:05:54.019733 funcnodes-0.2.2/funcnodes/worker/__init__.py
+-rw-r--r--   0        0        0     1808 2024-05-07 08:35:08.888378 funcnodes-0.2.2/funcnodes/worker/external_worker.py
+-rw-r--r--   0        0        0     3736 2024-03-26 07:43:19.651903 funcnodes-0.2.2/funcnodes/worker/loop.py
+-rw-r--r--   0        0        0     3293 2024-05-07 08:43:41.552734 funcnodes-0.2.2/funcnodes/worker/remote_worker.py
+-rw-r--r--   0        0        0     8270 2024-05-07 08:43:38.346889 funcnodes-0.2.2/funcnodes/worker/websocket.py
+-rw-r--r--   0        0        0    37914 2024-05-07 08:42:49.613686 funcnodes-0.2.2/funcnodes/worker/worker.py
+-rw-r--r--   0        0        0    30152 2024-05-06 20:08:11.694569 funcnodes-0.2.2/funcnodes/worker/worker_manager.py
+-rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.2.2/LICENSE
+-rw-r--r--   0        0        0      666 2024-05-08 14:07:43.612879 funcnodes-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    13174 2024-05-07 11:03:57.250582 funcnodes-0.2.2/README.md
+-rw-r--r--   0        0        0    13528 1970-01-01 00:00:00.000000 funcnodes-0.2.2/PKG-INFO
```

### Comparing `funcnodes-0.2.1/funcnodes/__init__.py` & `funcnodes-0.2.2/funcnodes/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .worker import (
     FuncNodesExternalWorker,
     RemoteWorker,
     WSWorker,
     WorkerManager,
     assert_worker_manager_running,
 )
+from .data import DataEnum
 
 from . import config
 from .config import RenderOptions
 
 __all__ = [
     "NodeInput",
     "NodeOutput",
@@ -58,12 +59,13 @@
     "RemoteWorker",
     "WSWorker",
     "WorkerManager",
     "assert_worker_manager_running",
     "config",
     "RenderOptions",
     "NoValue",
+    "DataEnum",
 ]
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 DEBUG = True
```

### Comparing `funcnodes-0.2.1/funcnodes/__main__.py` & `funcnodes-0.2.2/funcnodes/__main__.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/_logging.py` & `funcnodes-0.2.2/funcnodes/_logging.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/basic_nodes/files.py` & `funcnodes-0.2.2/funcnodes/basic_nodes/files.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/basic_nodes/logic.py` & `funcnodes-0.2.2/funcnodes/basic_nodes/logic.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/basic_nodes/math.py` & `funcnodes-0.2.2/funcnodes/basic_nodes/math.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/config.py` & `funcnodes-0.2.2/funcnodes/config.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/eventmanager.py` & `funcnodes-0.2.2/funcnodes/eventmanager.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/asset-manifest.json` & `funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/css/style.css` & `funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/css/style.css`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/favicon.ico` & `funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/favicon.ico`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/index.html` & `funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/index.html`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/424.js` & `funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/js/424.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt` & `funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/main.js` & `funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/js/main.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt` & `funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/logo192.png` & `funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/logo192.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/logo512.png` & `funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/logo512.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/run.py` & `funcnodes-0.2.2/funcnodes/frontends/funcnodes_react/run.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/io.py` & `funcnodes-0.2.2/funcnodes/io.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/lib/lib.py` & `funcnodes-0.2.2/funcnodes/lib/lib.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/lib/libfinder.py` & `funcnodes-0.2.2/funcnodes/lib/libfinder.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/lib/libparser.py` & `funcnodes-0.2.2/funcnodes/lib/libparser.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/node.py` & `funcnodes-0.2.2/funcnodes/node.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/nodemaker.py` & `funcnodes-0.2.2/funcnodes/nodemaker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/nodespace.py` & `funcnodes-0.2.2/funcnodes/nodespace.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/triggerstack.py` & `funcnodes-0.2.2/funcnodes/triggerstack.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/utils/data.py` & `funcnodes-0.2.2/funcnodes/utils/data.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/utils/nodeutils.py` & `funcnodes-0.2.2/funcnodes/utils/nodeutils.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/utils/serialization.py` & `funcnodes-0.2.2/funcnodes/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/worker/external_worker.py` & `funcnodes-0.2.2/funcnodes/worker/external_worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/worker/loop.py` & `funcnodes-0.2.2/funcnodes/worker/loop.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/worker/remote_worker.py` & `funcnodes-0.2.2/funcnodes/worker/remote_worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/worker/websocket.py` & `funcnodes-0.2.2/funcnodes/worker/websocket.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/worker/worker.py` & `funcnodes-0.2.2/funcnodes/worker/worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/funcnodes/worker/worker_manager.py` & `funcnodes-0.2.2/funcnodes/worker/worker_manager.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/LICENSE` & `funcnodes-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/pyproject.toml` & `funcnodes-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcnodes"
-version = "0.2.1"
+version = "0.2.2"
 description = "funcnodes"
 authors = ["Julian Kimmig <julian.kimmig@linkdlab.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 exposedfunctionality = "^0.3.6"
```

### Comparing `funcnodes-0.2.1/README.md` & `funcnodes-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.1/PKG-INFO` & `funcnodes-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcnodes
-Version: 0.2.1
+Version: 0.2.2
 Summary: funcnodes
 Author: Julian Kimmig
 Author-email: julian.kimmig@linkdlab.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

