# Comparing `tmp/aissemble_foundation_pdp_client_python-1.7.0.dev1715156498.tar.gz` & `tmp/aissemble_foundation_pdp_client_python-1.7.0.dev1715156502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_pdp_client_python-1.7.0.dev1715156498.tar", max compression
+gzip compressed data, was "aissemble_foundation_pdp_client_python-1.7.0.dev1715156502.tar", max compression
```

## Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1715156498.tar` & `aissemble_foundation_pdp_client_python-1.7.0.dev1715156502.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     9580 2024-05-08 08:21:28.918586 aissemble_foundation_pdp_client_python-1.7.0.dev1715156498/LICENSE
--rw-r--r--   0        0        0      680 2024-05-08 08:12:08.973492 aissemble_foundation_pdp_client_python-1.7.0.dev1715156498/README.md
--rw-r--r--   0        0        0      628 2024-05-08 08:21:38.748323 aissemble_foundation_pdp_client_python-1.7.0.dev1715156498/pyproject.toml
--rw-r--r--   0        0        0      228 2024-05-08 08:12:08.973492 aissemble_foundation_pdp_client_python-1.7.0.dev1715156498/src/aiops_security/__init__.py
--rw-r--r--   0        0        0      951 2024-05-08 08:12:08.973492 aissemble_foundation_pdp_client_python-1.7.0.dev1715156498/src/aiops_security/pdp_client.py
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 aissemble_foundation_pdp_client_python-1.7.0.dev1715156498/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-08 08:21:30.935025 aissemble_foundation_pdp_client_python-1.7.0.dev1715156502/LICENSE
+-rw-r--r--   0        0        0      680 2024-05-08 08:12:13.030269 aissemble_foundation_pdp_client_python-1.7.0.dev1715156502/README.md
+-rw-r--r--   0        0        0      628 2024-05-08 08:21:42.662019 aissemble_foundation_pdp_client_python-1.7.0.dev1715156502/pyproject.toml
+-rw-r--r--   0        0        0      228 2024-05-08 08:12:13.030269 aissemble_foundation_pdp_client_python-1.7.0.dev1715156502/src/aiops_security/__init__.py
+-rw-r--r--   0        0        0      951 2024-05-08 08:12:13.030269 aissemble_foundation_pdp_client_python-1.7.0.dev1715156502/src/aiops_security/pdp_client.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 aissemble_foundation_pdp_client_python-1.7.0.dev1715156502/PKG-INFO
```

### Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1715156498/LICENSE` & `aissemble_foundation_pdp_client_python-1.7.0.dev1715156502/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1715156498/README.md` & `aissemble_foundation_pdp_client_python-1.7.0.dev1715156502/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1715156498/pyproject.toml` & `aissemble_foundation_pdp_client_python-1.7.0.dev1715156502/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-pdp-client-python"
-version = "1.7.0.dev1715156498"
+version = "1.7.0.dev1715156502"
 description = "REST Policy Decision Point (PDP) client for Python-based components"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "aiops_security", from = "src"}
 ]
```

### Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1715156498/src/aiops_security/pdp_client.py` & `aissemble_foundation_pdp_client_python-1.7.0.dev1715156502/src/aiops_security/pdp_client.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1715156498/PKG-INFO` & `aissemble_foundation_pdp_client_python-1.7.0.dev1715156502/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-pdp-client-python
-Version: 1.7.0.dev1715156498
+Version: 1.7.0.dev1715156502
 Summary: REST Policy Decision Point (PDP) client for Python-based components
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.26.0)
```

