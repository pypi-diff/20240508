# Comparing `tmp/langevals_lingua-0.1.1.tar.gz` & `tmp/langevals_lingua-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_lingua-0.1.1.tar", max compression
+gzip compressed data, was "langevals_lingua-0.1.2.tar", max compression
```

## Comparing `langevals_lingua-0.1.1.tar` & `langevals_lingua-0.1.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     6619 2024-04-28 19:56:44.504808 langevals_lingua-0.1.1/langevals_lingua/language_detection.py
--rw-r--r--   0        0        0      477 2024-04-28 19:57:24.748537 langevals_lingua-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 langevals_lingua-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6619 2024-05-07 14:19:44.474403 langevals_lingua-0.1.2/langevals_lingua/language_detection.py
+-rw-r--r--   0        0        0      477 2024-05-07 14:20:46.310813 langevals_lingua-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 langevals_lingua-0.1.2/PKG-INFO
```

### Comparing `langevals_lingua-0.1.1/langevals_lingua/language_detection.py` & `langevals_lingua-0.1.2/langevals_lingua/language_detection.py`

 * *Files identical despite different names*

### Comparing `langevals_lingua-0.1.1/PKG-INFO` & `langevals_lingua-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: langevals-lingua
-Version: 0.1.1
+Version: 0.1.2
 Summary: LangEvals lingua evaluator for language detection.
 License: MIT
 Author: Rogerio Chaves
 Author-email: rogerio@langwatch.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
+Requires-Dist: langevals-core (>=0.1.3,<0.2.0)
 Requires-Dist: lingua-language-detector (>=2.0.2,<3.0.0)
```

