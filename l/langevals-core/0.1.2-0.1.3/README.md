# Comparing `tmp/langevals_core-0.1.2.tar.gz` & `tmp/langevals_core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_core-0.1.2.tar", max compression
+gzip compressed data, was "langevals_core-0.1.3.tar", max compression
```

## Comparing `langevals_core-0.1.2.tar` & `langevals_core-0.1.3.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     6566 2024-04-28 13:24:54.120394 langevals_core-0.1.2/langevals_core/base_evaluator.py
--rw-r--r--   0        0        0      455 2024-04-28 13:24:54.120394 langevals_core-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 langevals_core-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7175 2024-05-07 14:19:44.474403 langevals_core-0.1.3/langevals_core/base_evaluator.py
+-rw-r--r--   0        0        0      472 2024-05-07 14:19:44.474403 langevals_core-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 langevals_core-0.1.3/PKG-INFO
```

### Comparing `langevals_core-0.1.2/langevals_core/base_evaluator.py` & `langevals_core-0.1.3/langevals_core/base_evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     TypeVar,
     get_args,
     get_type_hints,
 )
 
 from pydantic import BaseModel, ConfigDict, Field
 import pandas as pd
+from tqdm import tqdm
+from concurrent.futures import ThreadPoolExecutor, as_completed
 
 EvalCategories = Literal[
     "quality", "rag", "safety", "policy", "other", "custom", "similarity"
 ]
 
 TSettings = TypeVar("TSettings", bound=BaseModel)
 
@@ -174,26 +176,37 @@
 
         except KeyError:
             raise EnvMissingException(f"Variable {var} not defined in environment.")
 
     def evaluate(self, entry: TEntry) -> SingleEvaluationResult:
         raise NotImplementedError("This method should be implemented by subclasses.")
 
-    def evaluate_batch(self, data: List[TEntry]) -> BatchEvaluationResult:
-        results = []
-        for entry in data:
-            try:
-                results.append(self.evaluate(entry))
-            except BaseException as exception:
-                results.append(
-                    EvaluationResultError(
-                        error_type=type(exception).__name__,
-                        message=str(exception),
-                        traceback=list(
-                            traceback.TracebackException.from_exception(
-                                exception
-                            ).format()
-                        ),
-                    )
-                )
+    def _evaluate_entry(self, entry):
+        try:
+            return self.evaluate(entry)
+        except Exception as exception:
+            return EvaluationResultError(
+                error_type=type(exception).__name__,
+                message=str(exception),
+                traceback=list(
+                    traceback.TracebackException.from_exception(exception).format()
+                ),
+            )
+
+    def evaluate_batch(self, data: List[TEntry], index=0) -> BatchEvaluationResult:
+        results: list[SingleEvaluationResult] = [
+            EvaluationResultSkipped(details="not processed")
+        ] * len(data)
+        # Use max_workers=None to use as many workers as there are CPUs
+        with ThreadPoolExecutor(max_workers=50) as executor:
+            future_to_index = {
+                executor.submit(self._evaluate_entry, entry): idx
+                for idx, entry in enumerate(data)
+            }
+
+            with tqdm(total=len(future_to_index), position=index) as progress:
+                for future in as_completed(future_to_index):
+                    idx = future_to_index[future]
+                    results[idx] = future.result()
+                    progress.update(1)
 
         return results
```

### Comparing `langevals_core-0.1.2/PKG-INFO` & `langevals_core-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: langevals-core
-Version: 0.1.2
+Version: 0.1.3
 Summary: Core package for LLM evaluation platform, providing base classes and utilities.
 License: MIT
 Author: Rogerio Chaves
 Author-email: rogerio@langwatch.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
```

