# Comparing `tmp/langevals_ragas-0.1.2.tar.gz` & `tmp/langevals_ragas-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_ragas-0.1.2.tar", max compression
+gzip compressed data, was "langevals_ragas-0.1.3.tar", max compression
```

## Comparing `langevals_ragas-0.1.2.tar` & `langevals_ragas-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/answer_relevancy.py
--rw-r--r--   0        0        0     1189 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/context_precision.py
--rw-r--r--   0        0        0     1131 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/context_recall.py
--rw-r--r--   0        0        0     1159 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/context_relevancy.py
--rw-r--r--   0        0        0     1173 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/context_utilization.py
--rw-r--r--   0        0        0     1090 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/faithfulness.py
--rw-r--r--   0        0        0     5441 2024-04-28 19:56:44.504808 langevals_ragas-0.1.2/langevals_ragas/lib/common.py
--rw-r--r--   0        0        0      589 2024-04-28 19:57:32.208456 langevals_ragas-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 langevals_ragas-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-07 14:19:44.474403 langevals_ragas-0.1.3/langevals_ragas/answer_relevancy.py
+-rw-r--r--   0        0        0     1189 2024-05-07 14:19:44.474403 langevals_ragas-0.1.3/langevals_ragas/context_precision.py
+-rw-r--r--   0        0        0     1131 2024-05-07 14:19:44.474403 langevals_ragas-0.1.3/langevals_ragas/context_recall.py
+-rw-r--r--   0        0        0     1159 2024-05-07 14:19:44.474403 langevals_ragas-0.1.3/langevals_ragas/context_relevancy.py
+-rw-r--r--   0        0        0     1173 2024-05-07 14:19:44.474403 langevals_ragas-0.1.3/langevals_ragas/context_utilization.py
+-rw-r--r--   0        0        0     1090 2024-05-07 14:19:44.474403 langevals_ragas-0.1.3/langevals_ragas/faithfulness.py
+-rw-r--r--   0        0        0     5441 2024-05-07 14:19:44.474403 langevals_ragas-0.1.3/langevals_ragas/lib/common.py
+-rw-r--r--   0        0        0      589 2024-05-07 14:20:52.894862 langevals_ragas-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 langevals_ragas-0.1.3/PKG-INFO
```

### Comparing `langevals_ragas-0.1.2/langevals_ragas/answer_relevancy.py` & `langevals_ragas-0.1.3/langevals_ragas/answer_relevancy.py`

 * *Files identical despite different names*

### Comparing `langevals_ragas-0.1.2/langevals_ragas/context_precision.py` & `langevals_ragas-0.1.3/langevals_ragas/context_precision.py`

 * *Files identical despite different names*

### Comparing `langevals_ragas-0.1.2/langevals_ragas/context_recall.py` & `langevals_ragas-0.1.3/langevals_ragas/context_recall.py`

 * *Files identical despite different names*

### Comparing `langevals_ragas-0.1.2/langevals_ragas/context_relevancy.py` & `langevals_ragas-0.1.3/langevals_ragas/context_relevancy.py`

 * *Files identical despite different names*

### Comparing `langevals_ragas-0.1.2/langevals_ragas/context_utilization.py` & `langevals_ragas-0.1.3/langevals_ragas/context_utilization.py`

 * *Files identical despite different names*

### Comparing `langevals_ragas-0.1.2/langevals_ragas/faithfulness.py` & `langevals_ragas-0.1.3/langevals_ragas/faithfulness.py`

 * *Files identical despite different names*

### Comparing `langevals_ragas-0.1.2/langevals_ragas/lib/common.py` & `langevals_ragas-0.1.3/langevals_ragas/lib/common.py`

 * *Files identical despite different names*

### Comparing `langevals_ragas-0.1.2/pyproject.toml` & `langevals_ragas-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "langevals-ragas"
-version = "0.1.2"
+version = "0.1.3"
 description = "LangEvals Ragas evaluator"
 authors = [ "Your Name <your.email@example.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-langevals-core = "^0.1.2"
+langevals-core = "^0.1.3"
 ragas = "0.1.0"
 langchain-openai = "^0.0.8"
 langchain_community = "^0.0.27"
 datasets = "^2.18.0"
 litellm = "^1.31.3"
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langevals_ragas-0.1.2/PKG-INFO` & `langevals_ragas-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: langevals-ragas
-Version: 0.1.2
+Version: 0.1.3
 Summary: LangEvals Ragas evaluator
 License: MIT
 Author: Your Name
 Author-email: your.email@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: datasets (>=2.18.0,<3.0.0)
 Requires-Dist: langchain-openai (>=0.0.8,<0.0.9)
 Requires-Dist: langchain_community (>=0.0.27,<0.0.28)
-Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
+Requires-Dist: langevals-core (>=0.1.3,<0.2.0)
 Requires-Dist: litellm (>=1.31.3,<2.0.0)
 Requires-Dist: ragas (==0.1.0)
```

