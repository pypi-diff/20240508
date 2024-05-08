# Comparing `tmp/langevals_azure-0.1.2.tar.gz` & `tmp/langevals_azure-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_azure-0.1.2.tar", max compression
+gzip compressed data, was "langevals_azure-0.1.3.tar", max compression
```

## Comparing `langevals_azure-0.1.2.tar` & `langevals_azure-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3847 2024-04-28 13:24:54.112394 langevals_azure-0.1.2/langevals_azure/content_safety.py
--rw-r--r--   0        0        0     2275 2024-04-28 13:24:54.112394 langevals_azure-0.1.2/langevals_azure/jailbreak.py
--rw-r--r--   0        0        0      499 2024-04-28 13:25:25.604491 langevals_azure-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 langevals_azure-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3847 2024-05-07 14:19:44.466403 langevals_azure-0.1.3/langevals_azure/content_safety.py
+-rw-r--r--   0        0        0     2275 2024-05-07 14:19:44.466403 langevals_azure-0.1.3/langevals_azure/jailbreak.py
+-rw-r--r--   0        0        0      499 2024-05-07 14:20:23.414689 langevals_azure-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 langevals_azure-0.1.3/PKG-INFO
```

### Comparing `langevals_azure-0.1.2/langevals_azure/content_safety.py` & `langevals_azure-0.1.3/langevals_azure/content_safety.py`

 * *Files identical despite different names*

### Comparing `langevals_azure-0.1.2/langevals_azure/jailbreak.py` & `langevals_azure-0.1.3/langevals_azure/jailbreak.py`

 * *Files identical despite different names*

### Comparing `langevals_azure-0.1.2/PKG-INFO` & `langevals_azure-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: langevals-azure
-Version: 0.1.2
+Version: 0.1.3
 Summary: LangEvals Azure Content Safety evaluator for LLM outputs.
 License: MIT
 Author: Rogerio Chaves
 Author-email: rogerio@langwatch.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: azure-ai-contentsafety (>=1.0.0,<2.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
+Requires-Dist: langevals-core (>=0.1.3,<0.2.0)
```

