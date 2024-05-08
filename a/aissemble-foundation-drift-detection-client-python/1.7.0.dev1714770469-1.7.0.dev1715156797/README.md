# Comparing `tmp/aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469.tar.gz` & `tmp/aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469.tar", max compression
+gzip compressed data, was "aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797.tar", max compression
```

## Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469.tar` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     9580 2024-05-03 21:07:33.875107 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/LICENSE
--rw-r--r--   0        0        0        0 2024-05-03 20:59:00.608690 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/README.md
--rw-r--r--   0        0        0      661 2024-05-03 21:07:49.834684 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/pyproject.toml
--rw-r--r--   0        0        0      194 2024-05-03 20:59:00.608690 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/src/config/__init__.py
--rw-r--r--   0        0        0      672 2024-05-03 20:59:00.608690 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/src/config/rest_config.py
--rw-r--r--   0        0        0      194 2024-05-03 20:59:00.608690 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/src/drift/__init__.py
--rw-r--r--   0        0        0      194 2024-05-03 20:59:00.608690 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/src/drift/detection/__init__.py
--rw-r--r--   0        0        0      194 2024-05-03 20:59:00.608690 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/src/drift/detection/rest/__init__.py
--rw-r--r--   0        0        0      194 2024-05-03 20:59:00.608690 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/src/drift/detection/rest/client/__init__.py
--rw-r--r--   0        0        0     1755 2024-05-03 20:59:00.608690 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/src/drift/detection/rest/client/drift_rest_client.py
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-08 08:26:24.240709 aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-08 08:12:08.913494 aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/README.md
+-rw-r--r--   0        0        0      661 2024-05-08 08:26:37.480355 aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/pyproject.toml
+-rw-r--r--   0        0        0      194 2024-05-08 08:12:08.913494 aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/src/config/__init__.py
+-rw-r--r--   0        0        0      672 2024-05-08 08:12:08.913494 aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/src/config/rest_config.py
+-rw-r--r--   0        0        0      194 2024-05-08 08:12:08.913494 aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/src/drift/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-08 08:12:08.913494 aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/src/drift/detection/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-08 08:12:08.913494 aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/src/drift/detection/rest/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-08 08:12:08.913494 aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/src/drift/detection/rest/client/__init__.py
+-rw-r--r--   0        0        0     1755 2024-05-08 08:12:08.913494 aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/src/drift/detection/rest/client/drift_rest_client.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/PKG-INFO
```

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/LICENSE` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/pyproject.toml` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-drift-detection-client-python"
-version = "1.7.0.dev1714770469"
+version = "1.7.0.dev1715156797"
 description = ""
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "config", from = "src"},
     {include = "drift", from = "src"}
 ]
```

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/src/config/rest_config.py` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/src/config/rest_config.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/src/drift/detection/rest/client/drift_rest_client.py` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/src/drift/detection/rest/client/drift_rest_client.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_drift_detection_client_python-1.7.0.dev1714770469/PKG-INFO` & `aissemble_foundation_drift_detection_client_python-1.7.0.dev1715156797/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-drift-detection-client-python
-Version: 1.7.0.dev1714770469
+Version: 1.7.0.dev1715156797
 Summary: 
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cryptography (>=42.0.4)
```

