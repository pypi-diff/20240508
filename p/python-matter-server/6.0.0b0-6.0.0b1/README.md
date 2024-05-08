# Comparing `tmp/python_matter_server-6.0.0b0.tar.gz` & `tmp/python_matter_server-6.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_matter_server-6.0.0b0.tar", last modified: Wed May  1 13:07:34 2024, max compression
+gzip compressed data, was "python_matter_server-6.0.0b1.tar", last modified: Wed May  8 20:06:09 2024, max compression
```

## Comparing `python_matter_server-6.0.0b0.tar` & `python_matter_server-6.0.0b1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:34.862515 python_matter_server-6.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-05-01 13:07:34.862515 python_matter_server-6.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:34.850515 python_matter_server-6.0.0b0/matter_server/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:34.850515 python_matter_server-6.0.0b0/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:34.854515 python_matter_server-6.0.0b0/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/client/models/clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21263 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15188 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:34.854515 python_matter_server-6.0.0b0/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:34.854515 python_matter_server-6.0.0b0/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/common/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:34.854515 python_matter_server-6.0.0b0/matter_server/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-01 13:07:32.000000 python_matter_server-6.0.0b0/matter_server/dashboard/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:34.854515 python_matter_server-6.0.0b0/matter_server/dashboard/js/
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-01 13:07:32.000000 python_matter_server-6.0.0b0/matter_server/dashboard/js/dialog-box-ztARVrB9.js
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-01 13:07:32.000000 python_matter_server-6.0.0b0/matter_server/dashboard/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)   230455 2024-05-01 13:07:32.000000 python_matter_server-6.0.0b0/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:34.858515 python_matter_server-6.0.0b0/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    62442 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:34.858515 python_matter_server-6.0.0b0/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/helpers/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/helpers/custom_web_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-01 13:07:16.000000 python_matter_server-6.0.0b0/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-01 13:07:21.000000 python_matter_server-6.0.0b0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:07:34.858515 python_matter_server-6.0.0b0/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-05-01 13:07:34.000000 python_matter_server-6.0.0b0/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-01 13:07:34.000000 python_matter_server-6.0.0b0/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:07:34.000000 python_matter_server-6.0.0b0/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 13:07:34.000000 python_matter_server-6.0.0b0/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:07:34.000000 python_matter_server-6.0.0b0/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-01 13:07:34.000000 python_matter_server-6.0.0b0/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 13:07:34.000000 python_matter_server-6.0.0b0/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:07:34.862515 python_matter_server-6.0.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.816553 python_matter_server-6.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-05-08 20:06:09.816553 python_matter_server-6.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.804553 python_matter_server-6.0.0b1/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.804553 python_matter_server-6.0.0b1/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29900 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.804553 python_matter_server-6.0.0b1/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/models/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21263 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.808553 python_matter_server-6.0.0b1/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.808553 python_matter_server-6.0.0b1/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/common/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.808553 python_matter_server-6.0.0b1/matter_server/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 20:06:06.000000 python_matter_server-6.0.0b1/matter_server/dashboard/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.808553 python_matter_server-6.0.0b1/matter_server/dashboard/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-08 20:06:06.000000 python_matter_server-6.0.0b1/matter_server/dashboard/js/dialog-box-ztARVrB9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-08 20:06:06.000000 python_matter_server-6.0.0b1/matter_server/dashboard/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)   230455 2024-05-08 20:06:06.000000 python_matter_server-6.0.0b1/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.808553 python_matter_server-6.0.0b1/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62667 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.812553 python_matter_server-6.0.0b1/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/helpers/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/helpers/custom_web_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-08 20:05:42.000000 python_matter_server-6.0.0b1/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-08 20:05:52.000000 python_matter_server-6.0.0b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:06:09.812553 python_matter_server-6.0.0b1/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 20:06:09.000000 python_matter_server-6.0.0b1/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:06:09.816553 python_matter_server-6.0.0b1/setup.cfg
```

### Comparing `python_matter_server-6.0.0b0/LICENSE` & `python_matter_server-6.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/PKG-INFO` & `python_matter_server-6.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 6.0.0b0
+Version: 6.0.0b1
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -14,33 +14,37 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: aiorun
 Requires-Dist: async-timeout
 Requires-Dist: coloredlogs
-Requires-Dist: dacite
 Requires-Dist: orjson
 Requires-Dist: home-assistant-chip-clusters==2024.4.1
 Provides-Extra: server
-Requires-Dist: home-assistant-chip-core==2024.4.1; extra == "server"
-Requires-Dist: cryptography==42.0.5; extra == "server"
+Requires-Dist: aiohttp==3.9.5; extra == "server"
+Requires-Dist: aiorun==2023.7.2; extra == "server"
+Requires-Dist: async-timeout==4.0.3; extra == "server"
+Requires-Dist: coloredlogs==15.0.1; extra == "server"
+Requires-Dist: cryptography==42.0.6; extra == "server"
+Requires-Dist: orjson==3.9.15; extra == "server"
 Requires-Dist: zeroconf==0.132.2; extra == "server"
+Requires-Dist: home-assistant-chip-core==2024.4.1; extra == "server"
 Provides-Extra: test
 Requires-Dist: codespell==2.2.6; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
 Requires-Dist: pre-commit==3.7.0; extra == "test"
 Requires-Dist: pre-commit-hooks==4.6.0; extra == "test"
 Requires-Dist: pylint==3.1.0; extra == "test"
 Requires-Dist: pytest==8.2.0; extra == "test"
 Requires-Dist: pytest-asyncio==0.23.6; extra == "test"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "test"
 Requires-Dist: pytest-cov==5.0.0; extra == "test"
-Requires-Dist: ruff==0.4.2; extra == "test"
+Requires-Dist: ruff==0.4.3; extra == "test"
 Requires-Dist: tomli==2.0.1; extra == "test"
 
 # Python Matter Server
 
 This project implements a Matter Controller Server over WebSockets using the
 [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip)
 as a base and provides both a server and client implementation.
```

### Comparing `python_matter_server-6.0.0b0/README.md` & `python_matter_server-6.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/client/client.py` & `python_matter_server-6.0.0b1/matter_server/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """Matter Client implementation."""
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Callable
 import logging
-from types import TracebackType
 from typing import TYPE_CHECKING, Any, Final, Optional, cast
 import uuid
 
-from aiohttp import ClientSession
 from chip.clusters import Objects as Clusters
 from chip.clusters.Types import NullValue
 
 from matter_server.common.errors import ERROR_MAP, NodeNotExists
 
 from ..common.helpers.util import (
     convert_ip_address,
@@ -46,14 +43,18 @@
     MatterNode,
     NetworkType,
     NodeDiagnostics,
     NodeType,
 )
 
 if TYPE_CHECKING:
+    from collections.abc import Callable
+    from types import TracebackType
+
+    from aiohttp import ClientSession
     from chip.clusters.Objects import ClusterCommand
 
 SUB_WILDCARD: Final = "*"
 
 # pylint: disable=too-many-public-methods,too-many-locals,too-many-branches
```

### Comparing `python_matter_server-6.0.0b0/matter_server/client/connection.py` & `python_matter_server-6.0.0b1/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/client/exceptions.py` & `python_matter_server-6.0.0b1/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/client/models/clusters.py` & `python_matter_server-6.0.0b1/matter_server/client/models/clusters.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/client/models/device_types.py` & `python_matter_server-6.0.0b1/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/client/models/node.py` & `python_matter_server-6.0.0b1/matter_server/client/models/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """Matter node."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum
 import logging
-from typing import Any, TypeVar, cast
+from typing import TYPE_CHECKING, Any, TypeVar, cast
 
 from chip.clusters import Objects as Clusters
 from chip.clusters.ClusterObjects import ALL_ATTRIBUTES, ALL_CLUSTERS
 
 from matter_server.common.helpers.util import (
     create_attribute_path,
     parse_attribute_path,
     parse_value,
 )
-from matter_server.common.models import MatterNodeData
 
 from .device_types import (
     ALL_TYPES as DEVICE_TYPES,
     Aggregator,
     BridgedDevice,
     DeviceType,
     RootNode,
 )
 
+if TYPE_CHECKING:
+    from matter_server.common.models import MatterNodeData
+
 LOGGER = logging.getLogger(__name__)
 
 # pylint: disable=invalid-name
 _CLUSTER_T = TypeVar("_CLUSTER_T", bound=Clusters.Cluster)
 _ATTRIBUTE_T = TypeVar("_ATTRIBUTE_T", bound=Clusters.ClusterAttributeDescriptor)
 # pylint: enable=invalid-name
```

### Comparing `python_matter_server-6.0.0b0/matter_server/common/errors.py` & `python_matter_server-6.0.0b1/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/common/helpers/api.py` & `python_matter_server-6.0.0b1/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/common/helpers/json.py` & `python_matter_server-6.0.0b1/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/common/helpers/util.py` & `python_matter_server-6.0.0b1/matter_server/common/helpers/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     Union,
     cast,
     get_args,
     get_origin,
     get_type_hints,
 )
 
-from chip.clusters.ClusterObjects import (
-    ClusterAttributeDescriptor,
-    ClusterObjectDescriptor,
-)
 from chip.clusters.Types import Nullable
 from chip.tlv import float32, uint
 
 if TYPE_CHECKING:
     from _typeshed import DataclassInstance
+    from chip.clusters.ClusterObjects import (
+        ClusterAttributeDescriptor,
+        ClusterObjectDescriptor,
+    )
 
     _T = TypeVar("_T", bound=DataclassInstance)
 
 CHIP_CLUSTERS_PKG_NAME = "home-assistant-chip-clusters"
 CHIP_CORE_PKG_NAME = "home-assistant-chip-core"
 
 cached_fields = cache(fields)
```

### Comparing `python_matter_server-6.0.0b0/matter_server/common/models.py` & `python_matter_server-6.0.0b1/matter_server/common/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Models that are (serializeable) shared between server and client."""
 
 from __future__ import annotations
 
 from collections.abc import Callable
 from dataclasses import dataclass, field
-from datetime import datetime
+from datetime import datetime  # noqa: TCH003
 from enum import Enum
 from typing import Any
 
 # Enums and constants
 
 
 class EventType(Enum):
```

### Comparing `python_matter_server-6.0.0b0/matter_server/dashboard/index.html` & `python_matter_server-6.0.0b1/matter_server/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/dashboard/js/dialog-box-ztARVrB9.js` & `python_matter_server-6.0.0b1/matter_server/dashboard/js/dialog-box-ztARVrB9.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/dashboard/js/main.js` & `python_matter_server-6.0.0b1/matter_server/dashboard/js/main.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js` & `python_matter_server-6.0.0b1/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/server/__main__.py` & `python_matter_server-6.0.0b1/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/server/client_handler.py` & `python_matter_server-6.0.0b1/matter_server/server/client_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """Logic to handle a client connected over WebSockets."""
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Callable
 from concurrent import futures
 from contextlib import suppress
 import logging
 from typing import TYPE_CHECKING, Any, Final
 
 from aiohttp import WSMsgType, web
 import async_timeout
 from chip.exceptions import ChipStackError
 
 from matter_server.common.const import VERBOSE_LOG_LEVEL
 from matter_server.common.helpers.json import json_dumps, json_loads
-from matter_server.common.models import EventType
 
 from ..common.errors import InvalidArguments, InvalidCommand, MatterError
 from ..common.helpers.api import parse_arguments
 from ..common.helpers.util import dataclass_from_dict
 from ..common.models import (
     APICommand,
     CommandMessage,
     ErrorResultMessage,
     EventMessage,
     MessageType,
     SuccessResultMessage,
 )
 
 if TYPE_CHECKING:
+    from collections.abc import Callable
+
+    from matter_server.common.models import EventType
+
     from ..common.helpers.api import APICommandHandler
     from .server import MatterServer
 
 MAX_PENDING_MSG = 512
 CANCELLATION_ERRORS: Final = (asyncio.CancelledError, futures.CancelledError)
 
 LOGGER = logging.getLogger(__name__)
```

### Comparing `python_matter_server-6.0.0b0/matter_server/server/const.py` & `python_matter_server-6.0.0b1/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/server/device_controller.py` & `python_matter_server-6.0.0b1/matter_server/server/device_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,26 @@
 
 # pylint: disable=too-many-lines
 
 from __future__ import annotations
 
 import asyncio
 from collections import deque
-from collections.abc import Callable, Iterable
 from datetime import datetime
 from functools import partial
 import logging
-from pathlib import Path
 from random import randint
 import time
 from typing import TYPE_CHECKING, Any, TypeVar, cast
 
-from chip.ChipDeviceCtrl import DeviceProxyWrapper
 from chip.clusters import Attribute, Objects as Clusters
 from chip.clusters.Attribute import ValueDecodeFailure
 from chip.clusters.ClusterObjects import ALL_ATTRIBUTES, ALL_CLUSTERS, Cluster
 from chip.discovery import DiscoveryType
 from chip.exceptions import ChipStackError
-from chip.native import PyChipError
 from zeroconf import BadTypeInNameException, IPVersion, ServiceStateChange, Zeroconf
 from zeroconf.asyncio import AsyncServiceBrowser, AsyncServiceInfo, AsyncZeroconf
 
 from matter_server.common.const import VERBOSE_LOG_LEVEL
 from matter_server.common.models import CommissionableNodeData, CommissioningParameters
 from matter_server.server.helpers.attributes import parse_attributes_from_read_result
 from matter_server.server.helpers.utils import ping_ip
@@ -53,15 +49,19 @@
     MatterNodeEvent,
     NodePingResult,
 )
 from .const import DATA_MODEL_SCHEMA_VERSION
 from .helpers.paa_certificates import fetch_certificates
 
 if TYPE_CHECKING:
-    from chip.ChipDeviceCtrl import ChipDeviceController
+    from collections.abc import Callable, Iterable
+    from pathlib import Path
+
+    from chip.ChipDeviceCtrl import ChipDeviceController, DeviceProxyWrapper
+    from chip.native import PyChipError
 
     from .server import MatterServer
 
 _T = TypeVar("_T")
 
 DATA_KEY_NODES = "nodes"
 DATA_KEY_LAST_NODE_ID = "last_node_id"
@@ -1107,15 +1107,24 @@
         self._subscriptions[node_id] = sub
         node.available = True
         # update attributes with current state from read request
         # NOTE: Make public method upstream for retrieving the attributeTLVCache
         # pylint: disable=protected-access
         tlv_attributes = sub._readTransaction._cache.attributeTLVCache
         node.attributes.update(parse_attributes_from_read_result(tlv_attributes))
-        node_logger.info("Subscription succeeded")
+
+        report_interval_floor, report_interval_ceiling = (
+            sub.GetReportingIntervalsSeconds()
+        )
+        node_logger.info(
+            "Subscription succeeded with report interval [%d, %d]",
+            report_interval_floor,
+            report_interval_ceiling,
+        )
+
         self._node_last_seen[node_id] = time.time()
         self.server.signal_event(EventType.NODE_UPDATED, node)
 
     def _get_next_node_id(self) -> int:
         """Return next node_id."""
         next_node_id = cast(int, self.server.storage.get(DATA_KEY_LAST_NODE_ID, 0)) + 1
         self.server.storage.set(DATA_KEY_LAST_NODE_ID, next_node_id, force=True)
```

### Comparing `python_matter_server-6.0.0b0/matter_server/server/helpers/attributes.py` & `python_matter_server-6.0.0b1/matter_server/server/helpers/attributes.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/server/helpers/custom_web_runner.py` & `python_matter_server-6.0.0b1/matter_server/server/helpers/custom_web_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Multiple host capable aiohttp Site."""
 
 from __future__ import annotations
 
 import asyncio
-from ssl import SSLContext
+from typing import TYPE_CHECKING
 
 from aiohttp import web
 from yarl import URL
 
+if TYPE_CHECKING:
+    from ssl import SSLContext
+
 
 class MultiHostTCPSite(web.BaseSite):
     """Multiple host capable aiohttp Site.
 
     Vanilla TCPSite accepts only str as host. However, the underlying asyncio's
     create_server() implementation does take a list of strings to bind to multiple
     host IP's. To support multiple server_host entries (e.g. to enable dual-stack
```

### Comparing `python_matter_server-6.0.0b0/matter_server/server/helpers/paa_certificates.py` & `python_matter_server-6.0.0b1/matter_server/server/helpers/paa_certificates.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,117 +6,144 @@
 
 All rights reserved.
 """
 
 import asyncio
 from datetime import UTC, datetime, timedelta
 import logging
-import os
 from pathlib import Path
 import re
+import warnings
 
 from aiohttp import ClientError, ClientSession
 from cryptography import x509
 from cryptography.hazmat.primitives import serialization
+from cryptography.utils import CryptographyDeprecationWarning
 
 # Git repo details
 OWNER = "project-chip"
 REPO = "connectedhomeip"
 PATH = "credentials/development/paa-root-certs"
 
 LOGGER = logging.getLogger(__name__)
 PRODUCTION_URL = "https://on.dcl.csa-iot.org"
 TEST_URL = "https://on.test-net.dcl.csa-iot.org"
 GIT_URL = f"https://raw.githubusercontent.com/{OWNER}/{REPO}/master/{PATH}"
 
 
-LAST_CERT_IDS: set[str] = set()
+# Subject Key Identifier of certificates. The Subject Key Identifier is a mandatory
+# X.509 extensions for Matter uniquely identifying the public key of PAA certificates.
+CERT_SUBJECT_KEY_IDS: set[str] = set()
 
 
 async def write_paa_root_cert(
-    paa_root_cert_dir: Path, certificate: str, subject: str
-) -> None:
+    paa_root_cert_dir: Path, base_name: str, pem_certificate: str, subject: str
+) -> bool:
     """Write certificate from string to file."""
 
-    def _write() -> None:
-        filename_base = "dcld_mirror_" + re.sub(
-            "[^a-zA-Z0-9_-]", "", re.sub("[=, ]", "_", subject)
-        )
-        filepath_base = paa_root_cert_dir.joinpath(filename_base)
+    def _write(
+        paa_root_cert_dir: Path,
+        filename_base: str,
+        pem_certificate: str,
+        der_certificate: bytes,
+    ) -> None:
         # handle PEM certificate file
-        file_path_pem = f"{filepath_base}.pem"
-        LOGGER.debug("Writing certificate %s", file_path_pem)
-        with open(file_path_pem, "w+", encoding="utf-8") as outfile:
-            outfile.write(certificate)
+        file_path_pem = paa_root_cert_dir.joinpath(f"{filename_base}.pem")
+        LOGGER.debug("Writing PEM certificate %s", file_path_pem)
+        file_path_pem.write_text(pem_certificate)
         # handle DER certificate file (converted from PEM)
-        pem_certificate = x509.load_pem_x509_certificate(certificate.encode())
-        file_path_der = f"{filepath_base}.der"
-        LOGGER.debug("Writing certificate %s", file_path_der)
-        with open(file_path_der, "wb+") as outfile:
-            der_certificate = pem_certificate.public_bytes(serialization.Encoding.DER)
-            outfile.write(der_certificate)
+        file_path_der = paa_root_cert_dir.joinpath(f"{filename_base}.der")
+        LOGGER.debug("Writing DER certificate %s", file_path_der)
+        file_path_der.write_bytes(der_certificate)
+
+    filename_base = base_name + re.sub(
+        "[^a-zA-Z0-9_-]", "", re.sub("[=, ]", "_", subject)
+    )
+
+    # Some certificates lead to a warning from the cryptography library:
+    # CryptographyDeprecationWarning: The parsed certificate contains a
+    # NULL parameter value in its signature algorithm parameters.
+    with warnings.catch_warnings():
+        if LOGGER.isEnabledFor(logging.DEBUG):
+            # Use always so warnings are printed for each offending cert.
+            warnings.simplefilter("always", CryptographyDeprecationWarning)
+        else:
+            # Ignore the warnings generally. The problem has been reported to the CSA
+            # via Slack.
+            warnings.simplefilter("ignore", CryptographyDeprecationWarning)
+
+        cert = x509.load_pem_x509_certificate(pem_certificate.encode())
+
+    ski: x509.SubjectKeyIdentifier = cert.extensions.get_extension_for_class(
+        x509.SubjectKeyIdentifier
+    ).value
+    ski_formatted = ":".join(f"{byte:02X}" for byte in ski.digest)
+    if ski_formatted in CERT_SUBJECT_KEY_IDS:
+        LOGGER.debug(
+            "Skipping '%s', certificate with the same subject key identifier already stored.",
+            subject,
+        )
+        return False
+    CERT_SUBJECT_KEY_IDS.add(ski_formatted)
+
+    der_certificate = cert.public_bytes(serialization.Encoding.DER)
+
+    await asyncio.get_running_loop().run_in_executor(
+        None,
+        _write,
+        paa_root_cert_dir,
+        f"{filename_base}_{ski.digest.hex()}",
+        pem_certificate,
+        der_certificate,
+    )
 
-    return await asyncio.get_running_loop().run_in_executor(None, _write)
+    return True
 
 
 async def fetch_dcl_certificates(
     paa_root_cert_dir: Path,
-    fetch_test_certificates: bool = True,
-    fetch_production_certificates: bool = True,
+    base_name: str,
+    base_url: str,
 ) -> int:
     """Fetch DCL PAA Certificates."""
-    LOGGER.info("Fetching the latest PAA root certificates from DCL.")
     fetch_count: int = 0
-    base_urls = set()
-    # determine which url's need to be queried.
-    # if we're going to fetch both prod and test, do test first
-    # so any duplicates will be overwritten/preferred by the production version.
 
-    # NOTE: While Matter is in BETA we fetch the test certificates by default
-    if fetch_test_certificates:
-        base_urls.add(TEST_URL)
-    if fetch_production_certificates:
-        base_urls.add(PRODUCTION_URL)
     try:
         async with ClientSession(raise_for_status=True) as http_session:
-            for url_base in base_urls:
-                # fetch the paa certificates list
-                async with http_session.get(
-                    f"{url_base}/dcl/pki/root-certificates"
-                ) as response:
+            # fetch the paa certificates list
+            async with http_session.get(
+                f"{base_url}/dcl/pki/root-certificates"
+            ) as response:
+                result = await response.json()
+            paa_list = result["approvedRootCertificates"]["certs"]
+            # grab each certificate
+            for paa in paa_list:
+                # do not fetch a certificate if we already fetched it
+                if paa["subjectKeyId"] in CERT_SUBJECT_KEY_IDS:
+                    continue
+                url = f"{base_url}/dcl/pki/certificates/{paa['subject']}/{paa['subjectKeyId']}"
+                LOGGER.debug("Downloading certificate from %s", url)
+                async with http_session.get(url) as response:
                     result = await response.json()
-                paa_list = result["approvedRootCertificates"]["certs"]
-                # grab each certificate
-                for paa in paa_list:
-                    # do not fetch a certificate if we already fetched it
-                    if paa["subjectKeyId"] in LAST_CERT_IDS:
-                        continue
-                    async with http_session.get(
-                        f"{url_base}/dcl/pki/certificates/{paa['subject']}/{paa['subjectKeyId']}"
-                    ) as response:
-                        result = await response.json()
-
-                    certificate_data: dict = result["approvedCertificates"]["certs"][0]
-                    certificate: str = certificate_data["pemCert"]
-                    subject = certificate_data["subjectAsText"]
-                    certificate = certificate.rstrip("\n")
-
-                    await write_paa_root_cert(
-                        paa_root_cert_dir,
-                        certificate,
-                        subject,
-                    )
-                    LAST_CERT_IDS.add(paa["subjectKeyId"])
+
+                certificate_data: dict = result["approvedCertificates"]["certs"][0]
+                certificate: str = certificate_data["pemCert"]
+                subject = certificate_data["subjectAsText"]
+                certificate = certificate.rstrip("\n")
+                if await write_paa_root_cert(
+                    paa_root_cert_dir,
+                    base_name,
+                    certificate,
+                    subject,
+                ):
                     fetch_count += 1
     except (ClientError, TimeoutError) as err:
         LOGGER.warning(
             "Fetching latest certificates failed: error %s", err, exc_info=err
         )
-    else:
-        LOGGER.info("Fetched %s PAA root certificates from DCL.", fetch_count)
 
     return fetch_count
 
 
 # Manufacturers release test certificates through the SDK (Git) as a part
 # of their standard product release workflow. This will ensure those certs
 # are correctly captured
@@ -132,21 +159,20 @@
             # Fetch directory contents and filter out extension
             api_url = f"https://api.github.com/repos/{OWNER}/{REPO}/contents/{PATH}"
             async with http_session.get(api_url, timeout=20) as response:
                 contents = await response.json()
                 git_certs = {item["name"].split(".")[0] for item in contents}
             # Fetch certificates
             for cert in git_certs:
-                if cert in LAST_CERT_IDS:
-                    continue
                 async with http_session.get(f"{GIT_URL}/{cert}.pem") as response:
                     certificate = await response.text()
-                await write_paa_root_cert(paa_root_cert_dir, certificate, cert)
-                LAST_CERT_IDS.add(cert)
-                fetch_count += 1
+                if await write_paa_root_cert(
+                    paa_root_cert_dir, "git_", certificate, cert
+                ):
+                    fetch_count += 1
     except (ClientError, TimeoutError) as err:
         LOGGER.warning(
             "Fetching latest certificates failed: error %s", err, exc_info=err
         )
 
     LOGGER.info("Fetched %s PAA root certificates from Git.", fetch_count)
 
@@ -156,37 +182,63 @@
 async def fetch_certificates(
     paa_root_cert_dir: Path,
     fetch_test_certificates: bool = True,
     fetch_production_certificates: bool = True,
 ) -> int:
     """Fetch PAA Certificates."""
     loop = asyncio.get_running_loop()
+    paa_root_cert_dir_version = paa_root_cert_dir / ".version"
 
-    if not paa_root_cert_dir.is_dir():
+    def _check_paa_root_dir(
+        paa_root_cert_dir: Path, paa_root_cert_dir_version: Path
+    ) -> datetime | None:
+        """Return timestamp of last fetch or None if a initial download is required."""
+        if paa_root_cert_dir.is_dir():
+            if paa_root_cert_dir_version.exists():
+                stat = paa_root_cert_dir_version.stat()
+                return datetime.fromtimestamp(stat.st_mtime, tz=UTC)
+
+            # Old certificate store version, delete all files
+            LOGGER.info("Old PAA root certificate store found, removing certificates.")
+            for path in paa_root_cert_dir.iterdir():
+                if not path.is_dir():
+                    path.unlink()
+        else:
+            paa_root_cert_dir.mkdir()
+        return None
 
-        def _make_root_cert_dir(paa_root_cert_dir: Path) -> None:
-            paa_root_cert_dir.mkdir(parents=True)
-            # Clear mtime to make sure code retries if first fetch fails.
-            os.utime(paa_root_cert_dir, (0, 0))
-
-        await loop.run_in_executor(None, _make_root_cert_dir, paa_root_cert_dir)
-    else:
-        stat = await loop.run_in_executor(None, paa_root_cert_dir.stat)
-        last_fetch = datetime.fromtimestamp(stat.st_mtime, tz=UTC)
-        if last_fetch > datetime.now(tz=UTC) - timedelta(days=1):
-            LOGGER.info(
-                "Skip fetching certificates (already fetched within the last 24h)."
-            )
-            return 0
-
-    fetch_count = await fetch_dcl_certificates(
-        paa_root_cert_dir=paa_root_cert_dir,
-        fetch_test_certificates=fetch_test_certificates,
-        fetch_production_certificates=fetch_production_certificates,
+    last_fetch = await loop.run_in_executor(
+        None, _check_paa_root_dir, paa_root_cert_dir, paa_root_cert_dir_version
     )
+    if last_fetch and last_fetch > datetime.now(tz=UTC) - timedelta(days=1):
+        LOGGER.info("Skip fetching certificates (already fetched within the last 24h).")
+        return 0
+
+    total_fetch_count = 0
+
+    LOGGER.info("Fetching the latest PAA root certificates from DCL.")
+
+    # Determine which url's need to be queried.
+    if fetch_production_certificates:
+        fetch_count = await fetch_dcl_certificates(
+            paa_root_cert_dir=paa_root_cert_dir,
+            base_name="dcld_production_",
+            base_url=PRODUCTION_URL,
+        )
+        LOGGER.info("Fetched %s PAA root certificates from DCL.", fetch_count)
+        total_fetch_count += fetch_count
+
+    if fetch_test_certificates:
+        fetch_count = await fetch_dcl_certificates(
+            paa_root_cert_dir=paa_root_cert_dir,
+            base_name="dcld_test_",
+            base_url=TEST_URL,
+        )
+        LOGGER.info("Fetched %s PAA root certificates from Test DCL.", fetch_count)
+        total_fetch_count += fetch_count
 
     if fetch_test_certificates:
-        fetch_count += await fetch_git_certificates(paa_root_cert_dir)
+        total_fetch_count += await fetch_git_certificates(paa_root_cert_dir)
 
-    await loop.run_in_executor(None, paa_root_cert_dir.touch)
+    await loop.run_in_executor(None, paa_root_cert_dir_version.write_text, "1")
 
     return fetch_count
```

### Comparing `python_matter_server-6.0.0b0/matter_server/server/helpers/utils.py` & `python_matter_server-6.0.0b1/matter_server/server/helpers/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 async def ping_ip(ip_address: str, timeout: int = 2, attempts: int = 1) -> bool:
     """Ping given (IPv4 or IPv6) IP-address."""
     is_ipv6 = ":" in ip_address
     if is_ipv6 and PLATFORM_MAC:
         # macos does not have support for -W (timeout) on ping6 ?!
         cmd = f"ping6 -c 1 {ip_address}"
     elif is_ipv6:
-        cmd = f"ping6 -c 1 -W {timeout} {ip_address}"
+        cmd = f"ping -6 -c 1 -W {timeout} {ip_address}"
     else:
         cmd = f"ping -c 1 -W {timeout} {ip_address}"
     while attempts:
         attempts -= 1
         try:
             # we add an additional timeout here as safeguard and to account for the fact
             # that macos does not seem to have timeout on ping6
```

### Comparing `python_matter_server-6.0.0b0/matter_server/server/server.py` & `python_matter_server-6.0.0b1/matter_server/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Implementation of a Websocket-based server to proxy Matter support (using CHIP SDK)."""
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Callable
 from functools import partial
 import ipaddress
 import logging
 import os
 from pathlib import Path
 import traceback
 from typing import TYPE_CHECKING, Any, cast
@@ -32,14 +31,17 @@
 from ..server.client_handler import WebsocketClientHandler
 from .const import DEFAULT_PAA_ROOT_CERTS_DIR, MIN_SCHEMA_VERSION
 from .device_controller import MatterDeviceController
 from .stack import MatterStack
 from .storage import StorageController
 from .vendor_info import VendorInfo
 
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
 DASHBOARD_DIR = Path(__file__).parent.joinpath("../dashboard/").resolve()
 DASHBOARD_DIR_EXISTS = DASHBOARD_DIR.exists()
 
 
 def _global_loop_exception_handler(_: Any, context: dict[str, Any]) -> None:
     """Handle all exception inside the core loop."""
     kwargs = {}
```

### Comparing `python_matter_server-6.0.0b0/matter_server/server/stack.py` & `python_matter_server-6.0.0b1/matter_server/server/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Implementation of a Websocket-based Matter proxy (using CHIP SDK)."""
 
 import logging
 import os
 from typing import TYPE_CHECKING
 
+import chip.CertificateAuthority
 from chip.ChipStack import ChipStack
 import chip.logging
 from chip.logging import (
     ERROR_CATEGORY_DETAIL,
     ERROR_CATEGORY_ERROR,
     ERROR_CATEGORY_NONE,
     ERROR_CATEGORY_PROGRESS,
 )
 from chip.logging.library_handle import _GetLoggingLibraryHandle
 from chip.logging.types import LogRedirectCallback_t
 import chip.native
 
 if TYPE_CHECKING:
-    from chip.CertificateAuthority import CertificateAuthorityManager
+    from chip.FabricAdmin import FabricAdmin
 
     from .server import MatterServer
 
 _LOGGER = logging.getLogger(__name__)
 
 CHIP_ERROR = logging.ERROR - 1
 CHIP_PROGRESS = logging.INFO - 1
@@ -107,18 +108,16 @@
             persistentStoragePath=storage_file,
             installDefaultLogHandler=False,
             enableServerInteractions=False,
         )
 
         # Initialize Certificate Authority Manager
         # yeah this is a bit weird just to prevent a circular import in the underlying SDK
-        self.certificate_authority_manager: CertificateAuthorityManager = (
-            chip.CertificateAuthority.CertificateAuthorityManager(
-                chipStack=self._chip_stack
-            )
+        self.certificate_authority_manager: chip.CertificateAuthority.CertificateAuthorityManager = chip.CertificateAuthority.CertificateAuthorityManager(
+            chipStack=self._chip_stack
         )
         self.certificate_authority_manager.LoadAuthoritiesFromStorage()
 
         # Get Certificate Authority (create new if we do not yet have one)
         if len(self.certificate_authority_manager.activeCaList) == 0:
             cert_auth = self.certificate_authority_manager.NewCertificateAuthority()
             cert_auth.maximizeCertChains = False
@@ -127,15 +126,15 @@
 
         # Get Fabric Admin (create new if we do not yet have one)
         for admin in cert_auth.adminList:
             if (
                 admin.vendorId == server.vendor_id
                 and admin.fabricId == server.fabric_id
             ):
-                self.fabric_admin = admin
+                self.fabric_admin: FabricAdmin = admin
                 break
         else:
             self.fabric_admin = cert_auth.NewFabricAdmin(
                 vendorId=server.vendor_id, fabricId=server.fabric_id
             )
 
         self.logger.info("CHIP Controller Stack initialized.")
```

### Comparing `python_matter_server-6.0.0b0/matter_server/server/storage.py` & `python_matter_server-6.0.0b1/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/matter_server/server/vendor_info.py` & `python_matter_server-6.0.0b1/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.0b0/pyproject.toml` & `python_matter_server-6.0.0b1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,45 +17,49 @@
     "Topic :: Home Automation",
 ]
 dependencies = [
     "aiohttp",
     "aiorun",
     "async-timeout",
     "coloredlogs",
-    "dacite",
     "orjson",
     "home-assistant-chip-clusters==2024.4.1",
 ]
 description = "Python Matter WebSocket Server"
 name = "python-matter-server"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "6.0.0b0"
+version = "6.0.0b1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 server = [
-    "home-assistant-chip-core==2024.4.1",
-    "cryptography==42.0.5",
+    "aiohttp==3.9.5",
+    "aiorun==2023.7.2",
+    "async-timeout==4.0.3",
+    "coloredlogs==15.0.1",
+    "cryptography==42.0.6",
+    "orjson==3.9.15",
     "zeroconf==0.132.2",
+    "home-assistant-chip-core==2024.4.1",
 ]
 test = [
     "codespell==2.2.6",
     "isort==5.13.2",
     "mypy==1.10.0",
     "pre-commit==3.7.0",
     "pre-commit-hooks==4.6.0",
     "pylint==3.1.0",
     "pytest==8.2.0",
     "pytest-asyncio==0.23.6",
     "pytest-aiohttp==1.0.5",
     "pytest-cov==5.0.0",
-    "ruff==0.4.2",
+    "ruff==0.4.3",
     "tomli==2.0.1",
 ]
 
 [project.scripts]
 matter-server = "matter_server.server.__main__:main"
 
 [tool.codespell]
@@ -160,24 +164,20 @@
     "D203",
     "D213",
     "D417",
     "EM102",
     "FIX002",
     "PLR2004",
     "PD011",
-    "TCH001",
-    "TCH003",
     "S101",
     "TD002",
     "TD003",
     "TD004",
     "COM812",
     "ISC001",
-    "TCH003",
-    "TCH002",
     "TID252",
     "N805",
     "EXE002",
     "T201",
     "ANN201",
     "UP032",
     "E711",
@@ -214,15 +214,14 @@
     "PYI036",
     "ANN204",
     "N818",
     "N815",
     "N801",
     "N813",
     "RUF012",
-    "TCH001",
     "ANN102",
     "B007",
     "SIM102",
     "C901",
     "PLR0911",
     "PLR0912",
     "SLF001",
```

### Comparing `python_matter_server-6.0.0b0/python_matter_server.egg-info/PKG-INFO` & `python_matter_server-6.0.0b1/python_matter_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 6.0.0b0
+Version: 6.0.0b1
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -14,33 +14,37 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: aiorun
 Requires-Dist: async-timeout
 Requires-Dist: coloredlogs
-Requires-Dist: dacite
 Requires-Dist: orjson
 Requires-Dist: home-assistant-chip-clusters==2024.4.1
 Provides-Extra: server
-Requires-Dist: home-assistant-chip-core==2024.4.1; extra == "server"
-Requires-Dist: cryptography==42.0.5; extra == "server"
+Requires-Dist: aiohttp==3.9.5; extra == "server"
+Requires-Dist: aiorun==2023.7.2; extra == "server"
+Requires-Dist: async-timeout==4.0.3; extra == "server"
+Requires-Dist: coloredlogs==15.0.1; extra == "server"
+Requires-Dist: cryptography==42.0.6; extra == "server"
+Requires-Dist: orjson==3.9.15; extra == "server"
 Requires-Dist: zeroconf==0.132.2; extra == "server"
+Requires-Dist: home-assistant-chip-core==2024.4.1; extra == "server"
 Provides-Extra: test
 Requires-Dist: codespell==2.2.6; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
 Requires-Dist: pre-commit==3.7.0; extra == "test"
 Requires-Dist: pre-commit-hooks==4.6.0; extra == "test"
 Requires-Dist: pylint==3.1.0; extra == "test"
 Requires-Dist: pytest==8.2.0; extra == "test"
 Requires-Dist: pytest-asyncio==0.23.6; extra == "test"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "test"
 Requires-Dist: pytest-cov==5.0.0; extra == "test"
-Requires-Dist: ruff==0.4.2; extra == "test"
+Requires-Dist: ruff==0.4.3; extra == "test"
 Requires-Dist: tomli==2.0.1; extra == "test"
 
 # Python Matter Server
 
 This project implements a Matter Controller Server over WebSockets using the
 [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip)
 as a base and provides both a server and client implementation.
```

### Comparing `python_matter_server-6.0.0b0/python_matter_server.egg-info/SOURCES.txt` & `python_matter_server-6.0.0b1/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

