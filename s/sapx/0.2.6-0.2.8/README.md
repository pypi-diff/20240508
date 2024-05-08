# Comparing `tmp/sapx-0.2.6.tar.gz` & `tmp/sapx-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapx-0.2.6.tar", last modified: Sun Feb 25 17:36:12 2024, max compression
+gzip compressed data, was "sapx-0.2.8.tar", last modified: Wed May  8 09:22:52 2024, max compression
```

## Comparing `sapx-0.2.6.tar` & `sapx-0.2.8.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.867457 sapx-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-25 17:36:12.867457 sapx-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 17:36:04.000000 sapx-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-25 17:36:04.000000 sapx-0.2.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.863457 sapx-0.2.6/sap/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.863457 sapx-0.2.6/sap/beanie/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/beanie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/beanie/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/beanie/document.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/beanie/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/beanie/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/beanie/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/beanie/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/beanie/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.863457 sapx-0.2.6/sap/chart/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/chart/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.863457 sapx-0.2.6/sap/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/fastapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/fastapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/fastapi/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/fastapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/fastapi/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/fastapi/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/fastapi/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/fastapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.863457 sapx-0.2.6/sap/pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/pydantic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.863457 sapx-0.2.6/sap/rest/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/rest/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/rest/rest_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.867457 sapx-0.2.6/sap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/tests/crons.py
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/tests/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.867457 sapx-0.2.6/sap/typing/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/typing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.867457 sapx-0.2.6/sap/worker/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/worker/amqp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/worker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/worker/crons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/worker/crons_airtable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/worker/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/worker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/worker/lambdas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/worker/packet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-25 17:36:04.000000 sapx-0.2.6/sap/worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.867457 sapx-0.2.6/sapx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-25 17:36:12.000000 sapx-0.2.6/sapx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-25 17:36:12.000000 sapx-0.2.6/sapx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 17:36:12.000000 sapx-0.2.6/sapx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-25 17:36:12.000000 sapx-0.2.6/sapx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-25 17:36:12.000000 sapx-0.2.6/sapx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 17:36:12.867457 sapx-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-02-25 17:36:04.000000 sapx-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 17:36:12.867457 sapx-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-25 17:36:04.000000 sapx-0.2.6/tests/test_fastapi_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-25 17:36:04.000000 sapx-0.2.6/tests/test_rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.033253 sapx-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-08 09:22:52.033253 sapx-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 09:22:45.000000 sapx-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-08 09:22:45.000000 sapx-0.2.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.025253 sapx-0.2.8/sap/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.025253 sapx-0.2.8/sap/beanie/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.025253 sapx-0.2.8/sap/chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/chart/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/pydantic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/rest/rest_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/tests/crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/tests/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/typing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/crons_airtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/lambdas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.033253 sapx-0.2.8/sapx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-08 09:22:52.000000 sapx-0.2.8/sapx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 09:22:52.000000 sapx-0.2.8/sapx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:22:52.000000 sapx-0.2.8/sapx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 09:22:52.000000 sapx-0.2.8/sapx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 09:22:52.000000 sapx-0.2.8/sapx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:22:52.033253 sapx-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-08 09:22:45.000000 sapx-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.033253 sapx-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-08 09:22:45.000000 sapx-0.2.8/tests/test_rest_client.py
```

### Comparing `sapx-0.2.6/PKG-INFO` & `sapx-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapx
-Version: 0.2.6
+Version: 0.2.8
 Summary: Library of re-usable utilities for python web apps.
 Home-page: https://github.com/trellixio/sap
 Author: Trellix Dev
 Author-email: contact@trellix.io
 License: COPYRIGHT @ Trellix
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

### Comparing `sapx-0.2.6/pyproject.toml` & `sapx-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/beanie/client.py` & `sapx-0.2.8/sap/beanie/client.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/beanie/document.py` & `sapx-0.2.8/sap/beanie/document.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/beanie/link.py` & `sapx-0.2.8/sap/beanie/link.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/beanie/mixins.py` & `sapx-0.2.8/sap/beanie/mixins.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/beanie/patch.py` & `sapx-0.2.8/sap/beanie/patch.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/beanie/query.py` & `sapx-0.2.8/sap/beanie/query.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/chart/serializers.py` & `sapx-0.2.8/sap/chart/serializers.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/fastapi/__init__.py` & `sapx-0.2.8/sap/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/fastapi/auth.py` & `sapx-0.2.8/sap/fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/fastapi/exceptions.py` & `sapx-0.2.8/sap/fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/fastapi/forms.py` & `sapx-0.2.8/sap/fastapi/forms.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/fastapi/middleware.py` & `sapx-0.2.8/sap/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/fastapi/pagination.py` & `sapx-0.2.8/sap/fastapi/pagination.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utils for pagination."""
+
 from typing import Any, Generic, Optional, TypedDict, TypeVar
 
 from fastapi import Request
 from pydantic import BaseModel
 
 from . import utils
 
@@ -20,14 +21,15 @@
 class CursorInfo:
     """
     Contains information on how the list should paginated.
 
     This is a fake cursor paginator.
     """
 
+    count: int = -1
     offset: int = 0
     limit: int = 10
     limit_max: int = 250
     sort: str = "-doc_meta.created"
 
     def __init__(self, request: Request) -> None:
         """Initialize the cursor info."""
@@ -46,23 +48,33 @@
         """Return params to apply to the database query when using beanie."""
         return {
             "limit": self.limit,
             "skip": self.offset,
             "sort": self.sort,
         }
 
+    def set_count(self, value: int) -> int:
+        """Set the total count of the query."""
+        self.count = value
+
+    def get_count(self) -> int:
+        """Return the total count of the query."""
+        return self.count
+
     def get_next(self) -> Optional[str]:
         """Get the cursor to paginate forward."""
         offset = self.offset + self.limit
+        if offset >= self.get_count() >= 0:
+            return None
         return utils.base64_url_encode(f"{self.limit},{offset}")
 
     def get_previous(self) -> Optional[str]:
         """Get the cursor to paginate backward."""
         offset = self.offset - self.limit
-        if offset <= 0:
+        if offset < 0:
             return None
         return utils.base64_url_encode(f"{self.limit},{offset}")
 
 
 class PaginatedData(BaseModel, Generic[PageDataT]):
     """Represent the structure of an API paginated list response."""
```

### Comparing `sapx-0.2.6/sap/fastapi/serializers.py` & `sapx-0.2.8/sap/fastapi/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 # Serializers.
 
 Handle data validation.
 """
+
 from __future__ import annotations
 
 import datetime
 import inspect
 from typing import TYPE_CHECKING, Any, ClassVar, Generic, List, Optional, TypeVar, Union, get_args, get_origin
 
 from typing_extensions import Literal
@@ -107,21 +108,18 @@
     def read_page(
         cls,
         instance_list: list[ModelT],
         cursor_info: CursorInfo,
         request: Request,
     ) -> PaginatedData["SerializerT"]:
         """Serialize a list of objects."""
-
-        # TODO: implemented proper cursor pagination, for now fake it till you make it.
-
         page_next = cursor_info.get_next()
         page_previous = cursor_info.get_previous()
         return PaginatedData(
-            count=0,
+            count=cursor_info.get_count(),
             next=str(request.url.include_query_params(cursor=page_next)) if page_next else None,
             previous=str(request.url.include_query_params(cursor=page_previous)) if page_previous else None,
             data=cls.read_list(instance_list),
         )
 
 
 SerializerT = TypeVar("SerializerT", bound=ObjectSerializer[Any])
```

### Comparing `sapx-0.2.6/sap/fastapi/user.py` & `sapx-0.2.8/sap/fastapi/user.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/fastapi/utils.py` & `sapx-0.2.8/sap/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/rest/client.py` & `sapx-0.2.8/sap/rest/client.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/rest/rest_exceptions.py` & `sapx-0.2.8/sap/rest/rest_exceptions.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/settings.py` & `sapx-0.2.8/sap/settings.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/tests/crons.py` & `sapx-0.2.8/sap/tests/crons.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/tests/rest.py` & `sapx-0.2.8/sap/tests/rest.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/tests/utils.py` & `sapx-0.2.8/sap/tests/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -113,10 +113,13 @@
     response = await self.send(request, auth=auth, follow_redirects=follow_redirects)
 
     response_data = {
         "status_code": response.status_code,
         # "headers": response.headers,
     }
     if response.content:
-        response_data["json"] = response.json()
-    print(response_data)
+        if response.headers.get("content-type") == "application/json":
+            response_data["json"] = response.json()
+        else:
+            response_data["content"] = response.content
+        print(response_data)
     return response
```

### Comparing `sapx-0.2.6/sap/worker/__init__.py` & `sapx-0.2.8/sap/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/worker/amqp.py` & `sapx-0.2.8/sap/worker/amqp.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/worker/config.py` & `sapx-0.2.8/sap/worker/config.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/worker/crons.py` & `sapx-0.2.8/sap/worker/crons.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/worker/crons_airtable.py` & `sapx-0.2.8/sap/worker/crons_airtable.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/worker/debug.py` & `sapx-0.2.8/sap/worker/debug.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/worker/lambdas.py` & `sapx-0.2.8/sap/worker/lambdas.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/worker/packet.py` & `sapx-0.2.8/sap/worker/packet.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sap/worker/utils.py` & `sapx-0.2.8/sap/worker/utils.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.6/sapx.egg-info/PKG-INFO` & `sapx-0.2.8/sapx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapx
-Version: 0.2.6
+Version: 0.2.8
 Summary: Library of re-usable utilities for python web apps.
 Home-page: https://github.com/trellixio/sap
 Author: Trellix Dev
 Author-email: contact@trellix.io
 License: COPYRIGHT @ Trellix
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

### Comparing `sapx-0.2.6/sapx.egg-info/SOURCES.txt` & `sapx-0.2.8/sapx.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -44,9 +44,8 @@
 sap/worker/packet.py
 sap/worker/utils.py
 sapx.egg-info/PKG-INFO
 sapx.egg-info/SOURCES.txt
 sapx.egg-info/dependency_links.txt
 sapx.egg-info/requires.txt
 sapx.egg-info/top_level.txt
-tests/test_fastapi_utils.py
 tests/test_rest_client.py
```

### Comparing `sapx-0.2.6/setup.py` & `sapx-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
-VERSION = "0.2.6"
+VERSION = "0.2.8"
 
 setup(
     name="sapx",
     version=VERSION,
     packages=find_packages(include=("sap.*", "sap")),
     package_data={"sap": ["py.typed"]},
     include_package_data=True,
```

### Comparing `sapx-0.2.6/tests/test_rest_client.py` & `sapx-0.2.8/tests/test_rest_client.py`

 * *Files identical despite different names*

