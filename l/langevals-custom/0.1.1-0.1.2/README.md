# Comparing `tmp/langevals_custom-0.1.1.tar.gz` & `tmp/langevals_custom-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_custom-0.1.1.tar", max compression
+gzip compressed data, was "langevals_custom-0.1.2.tar", max compression
```

## Comparing `langevals_custom-0.1.1.tar` & `langevals_custom-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2638 2024-04-28 13:24:54.116394 langevals_custom-0.1.1/langevals_custom/basic.py
--rw-r--r--   0        0        0     5602 2024-04-28 13:24:54.116394 langevals_custom-0.1.1/langevals_custom/llm_boolean.py
--rw-r--r--   0        0        0     5445 2024-04-28 13:24:54.116394 langevals_custom-0.1.1/langevals_custom/llm_score.py
--rw-r--r--   0        0        0     4320 2024-04-28 13:24:54.116394 langevals_custom-0.1.1/langevals_custom/similarity.py
--rw-r--r--   0        0        0      549 2024-04-28 13:25:28.768500 langevals_custom-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 langevals_custom-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2638 2024-05-07 14:19:44.470403 langevals_custom-0.1.2/langevals_custom/basic.py
+-rw-r--r--   0        0        0     5602 2024-05-07 14:19:44.470403 langevals_custom-0.1.2/langevals_custom/llm_boolean.py
+-rw-r--r--   0        0        0     5445 2024-05-07 14:19:44.470403 langevals_custom-0.1.2/langevals_custom/llm_score.py
+-rw-r--r--   0        0        0     4320 2024-05-07 14:19:44.470403 langevals_custom-0.1.2/langevals_custom/similarity.py
+-rw-r--r--   0        0        0      549 2024-05-07 14:20:28.374717 langevals_custom-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 langevals_custom-0.1.2/PKG-INFO
```

### Comparing `langevals_custom-0.1.1/langevals_custom/basic.py` & `langevals_custom-0.1.2/langevals_custom/basic.py`

 * *Files identical despite different names*

### Comparing `langevals_custom-0.1.1/langevals_custom/llm_boolean.py` & `langevals_custom-0.1.2/langevals_custom/llm_boolean.py`

 * *Files identical despite different names*

### Comparing `langevals_custom-0.1.1/langevals_custom/llm_score.py` & `langevals_custom-0.1.2/langevals_custom/llm_score.py`

 * *Files identical despite different names*

### Comparing `langevals_custom-0.1.1/langevals_custom/similarity.py` & `langevals_custom-0.1.2/langevals_custom/similarity.py`

 * *Files identical despite different names*

### Comparing `langevals_custom-0.1.1/pyproject.toml` & `langevals_custom-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "langevals-custom"
-version = "0.1.1"
+version = "0.1.2"
 description = "Custom evaluators you can build using other LLMs to do the eval, semantic matching or simple regexes or string matching."
 authors = [ "Rogerio Chaves <rogerio@langwatch.ai>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-langevals-core = "^0.1.2"
+langevals-core = "^0.1.3"
 litellm = "^1.31.3"
 numpy = "^1.26.4"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.2"
 python-dotenv = "1.0.1"
```

### Comparing `langevals_custom-0.1.1/PKG-INFO` & `langevals_custom-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: langevals-custom
-Version: 0.1.1
+Version: 0.1.2
 Summary: Custom evaluators you can build using other LLMs to do the eval, semantic matching or simple regexes or string matching.
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
 Requires-Dist: litellm (>=1.31.3,<2.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
```

