# Comparing `tmp/langevals-0.1.3.tar.gz` & `tmp/langevals-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals-0.1.3.tar", max compression
+gzip compressed data, was "langevals-0.1.4.tar", max compression
```

## Comparing `langevals-0.1.3.tar` & `langevals-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      112 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/__init__.py
--rw-r--r--   0        0        0     3447 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/evaluation.py
--rw-r--r--   0        0        0     4358 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/expect.py
--rw-r--r--   0        0        0        0 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/pytest_plugins/__init__.py
--rw-r--r--   0        0        0     4074 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/pytest_plugins/pass_rate_plugin.py
--rw-r--r--   0        0        0     3481 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/server.py
--rw-r--r--   0        0        0     2955 2024-04-28 19:56:44.504808 langevals-0.1.3/langevals/utils.py
--rw-r--r--   0        0        0     2114 2024-04-28 19:57:35.936431 langevals-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2036 1970-01-01 00:00:00.000000 langevals-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-07 14:19:44.466403 langevals-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0      112 2024-05-07 14:19:44.474403 langevals-0.1.4/langevals/__init__.py
+-rw-r--r--   0        0        0     3654 2024-05-07 14:19:44.474403 langevals-0.1.4/langevals/evaluation.py
+-rw-r--r--   0        0        0     4358 2024-05-07 14:19:44.474403 langevals-0.1.4/langevals/expect.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:19:44.474403 langevals-0.1.4/langevals/pytest_plugins/__init__.py
+-rw-r--r--   0        0        0     4074 2024-05-07 14:19:44.474403 langevals-0.1.4/langevals/pytest_plugins/pass_rate_plugin.py
+-rw-r--r--   0        0        0     3481 2024-05-07 14:19:44.474403 langevals-0.1.4/langevals/server.py
+-rw-r--r--   0        0        0     2955 2024-05-07 14:19:44.474403 langevals-0.1.4/langevals/utils.py
+-rw-r--r--   0        0        0     2114 2024-05-07 14:20:56.414884 langevals-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2036 1970-01-01 00:00:00.000000 langevals-0.1.4/PKG-INFO
```

### Comparing `langevals-0.1.3/langevals/evaluation.py` & `langevals-0.1.4/langevals/evaluation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import Optional
 from langevals_core.base_evaluator import (
     BaseEvaluator,
     BatchEvaluationResult,
     EvaluationResult,
     EvaluatorEntry,
 )
@@ -76,19 +77,25 @@
 
 
 # TODO: docs, and auto-generated docs from evaluators
 def evaluate(
     entries: pd.DataFrame, evaluators: list[BaseEvaluator]
 ) -> EvaluationResultSet:
     entries_ = _pandas_to_generic_entries(entries)
-    result_set: list[BatchEvaluationResult] = []
-    # TODO: process this in parallel (maybe copy python-sdk batch eval?)
-    # TODO: add tqdm, be sure to handle it on the evaluate_batch_below
-    for evaluator in evaluators:
-        result_set.append(evaluator.evaluate_batch(entries_))
+    result_set: list[BatchEvaluationResult] = [[]] * len(evaluators)
+
+    with ThreadPoolExecutor(max_workers=5) as executor:
+        future_to_index = {
+            executor.submit(evaluator.evaluate_batch, entries_): idx
+            for idx, evaluator in enumerate(evaluators)
+        }
+
+        for future in as_completed(future_to_index):
+            idx = future_to_index[future]
+            result_set[idx] = future.result()
 
     return EvaluationResultSet(
         entries=entries_, evaluators=evaluators, results=result_set
     )
 
 
 def _pandas_to_generic_entries(entries: pd.DataFrame) -> list[EvaluatorEntry]:
```

### Comparing `langevals-0.1.3/langevals/expect.py` & `langevals-0.1.4/langevals/expect.py`

 * *Files identical despite different names*

### Comparing `langevals-0.1.3/langevals/pytest_plugins/pass_rate_plugin.py` & `langevals-0.1.4/langevals/pytest_plugins/pass_rate_plugin.py`

 * *Files identical despite different names*

### Comparing `langevals-0.1.3/langevals/server.py` & `langevals-0.1.4/langevals/server.py`

 * *Files identical despite different names*

### Comparing `langevals-0.1.3/langevals/utils.py` & `langevals-0.1.4/langevals/utils.py`

 * *Files identical despite different names*

### Comparing `langevals-0.1.3/pyproject.toml` & `langevals-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "langevals"
-version = "0.1.3"
+version = "0.1.4"
 description = "A platform to evaluate LLM outputs using various evaluators."
 authors = [ "Rogerio Chaves <rogerio@langwatch.ai>",]
 license = "MIT"
 [[tool.poetry.source]]
 name = "pytorch_cpu"
 url = "https://download.pytorch.org/whl/cpu"
 priority = "explicit"
@@ -18,25 +18,25 @@
 python = "^3.11"
 fastapi = "^0.110.0"
 hypercorn = "^0.16.0"
 pydantic = "^2.6.4"
 python-dotenv = "1.0.1"
 mangum = "^0.17.0"
 pandas = "^2.2.2"
-langevals-core = "^0.1.2"
-langevals-azure = "^0.1.2"
-langevals-openai = "^0.1.2"
-langevals-example = "^0.1.2"
-langevals-ragas = "^0.1.2"
-langevals-google_cloud = "^0.1.2"
-langevals-custom = "^0.1.1"
-langevals-lingua = "^0.1.1"
-langevals-aws = "^0.1.1"
-langevals-huggingface = "^0.1.1"
-langevals-langevals = "^0.1.1"
+langevals-core = "^0.1.3"
+langevals-azure = "^0.1.3"
+langevals-openai = "^0.1.3"
+langevals-example = "^0.1.3"
+langevals-ragas = "^0.1.3"
+langevals-google_cloud = "^0.1.3"
+langevals-custom = "^0.1.2"
+langevals-lingua = "^0.1.2"
+langevals-aws = "^0.1.2"
+langevals-huggingface = "^0.1.2"
+langevals-langevals = "^0.1.2"
 [[tool.poetry.dependencies.torch]]
 version = "^2.2.2"
 optional = true
 source = "pytorch_cpu"
 markers = "sys_platform == 'linux'"
 
 [[tool.poetry.dependencies.torch]]
```

### Comparing `langevals-0.1.3/PKG-INFO` & `langevals-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langevals
-Version: 0.1.3
+Version: 0.1.4
 Summary: A platform to evaluate LLM outputs using various evaluators.
 License: MIT
 Author: Rogerio Chaves
 Author-email: rogerio@langwatch.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,25 +19,25 @@
 Provides-Extra: huggingface
 Provides-Extra: langevals
 Provides-Extra: lingua
 Provides-Extra: openai
 Provides-Extra: ragas
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: hypercorn (>=0.16.0,<0.17.0)
-Requires-Dist: langevals-aws (>=0.1.1,<0.2.0) ; extra == "aws" or extra == "all"
-Requires-Dist: langevals-azure (>=0.1.2,<0.2.0) ; extra == "azure" or extra == "all"
-Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
-Requires-Dist: langevals-custom (>=0.1.1,<0.2.0) ; extra == "custom" or extra == "all"
-Requires-Dist: langevals-example (>=0.1.2,<0.2.0) ; extra == "example" or extra == "all"
-Requires-Dist: langevals-google_cloud (>=0.1.2,<0.2.0) ; extra == "google-cloud" or extra == "all"
-Requires-Dist: langevals-huggingface (>=0.1.1,<0.2.0) ; extra == "huggingface" or extra == "all"
-Requires-Dist: langevals-langevals (>=0.1.1,<0.2.0) ; extra == "langevals" or extra == "all"
-Requires-Dist: langevals-lingua (>=0.1.1,<0.2.0) ; extra == "lingua" or extra == "all"
-Requires-Dist: langevals-openai (>=0.1.2,<0.2.0) ; extra == "openai" or extra == "all"
-Requires-Dist: langevals-ragas (>=0.1.2,<0.2.0) ; extra == "ragas" or extra == "all"
+Requires-Dist: langevals-aws (>=0.1.2,<0.2.0) ; extra == "aws" or extra == "all"
+Requires-Dist: langevals-azure (>=0.1.3,<0.2.0) ; extra == "azure" or extra == "all"
+Requires-Dist: langevals-core (>=0.1.3,<0.2.0)
+Requires-Dist: langevals-custom (>=0.1.2,<0.2.0) ; extra == "custom" or extra == "all"
+Requires-Dist: langevals-example (>=0.1.3,<0.2.0) ; extra == "example" or extra == "all"
+Requires-Dist: langevals-google_cloud (>=0.1.3,<0.2.0) ; extra == "google-cloud" or extra == "all"
+Requires-Dist: langevals-huggingface (>=0.1.2,<0.2.0) ; extra == "huggingface" or extra == "all"
+Requires-Dist: langevals-langevals (>=0.1.2,<0.2.0) ; extra == "langevals" or extra == "all"
+Requires-Dist: langevals-lingua (>=0.1.2,<0.2.0) ; extra == "lingua" or extra == "all"
+Requires-Dist: langevals-openai (>=0.1.3,<0.2.0) ; extra == "openai" or extra == "all"
+Requires-Dist: langevals-ragas (>=0.1.3,<0.2.0) ; extra == "ragas" or extra == "all"
 Requires-Dist: mangum (>=0.17.0,<0.18.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pytest (>=8.1.2,<9.0.0)
 Requires-Dist: python-dotenv (==1.0.1)
 Requires-Dist: torch (>=2.2.2,<3.0.0) ; sys_platform != "linux"
 Requires-Dist: torch (>=2.2.2,<3.0.0) ; sys_platform == "linux"
```

