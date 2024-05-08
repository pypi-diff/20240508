# Comparing `tmp/langevals_huggingface-0.1.1.tar.gz` & `tmp/langevals_huggingface-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_huggingface-0.1.1.tar", max compression
+gzip compressed data, was "langevals_huggingface-0.1.2.tar", max compression
```

## Comparing `langevals_huggingface-0.1.1.tar` & `langevals_huggingface-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1768 2024-04-28 19:56:44.504808 langevals_huggingface-0.1.1/langevals_huggingface/bert_f1.py
--rw-r--r--   0        0        0     1876 2024-04-28 19:56:44.504808 langevals_huggingface-0.1.1/langevals_huggingface/bert_precision.py
--rw-r--r--   0        0        0     2082 2024-04-28 19:56:44.504808 langevals_huggingface-0.1.1/langevals_huggingface/bert_recall.py
--rw-r--r--   0        0        0      805 2024-04-28 19:57:16.624596 langevals_huggingface-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 langevals_huggingface-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1768 2024-05-07 14:19:44.470403 langevals_huggingface-0.1.2/langevals_huggingface/bert_f1.py
+-rw-r--r--   0        0        0     1876 2024-05-07 14:19:44.470403 langevals_huggingface-0.1.2/langevals_huggingface/bert_precision.py
+-rw-r--r--   0        0        0     2082 2024-05-07 14:19:44.470403 langevals_huggingface-0.1.2/langevals_huggingface/bert_recall.py
+-rw-r--r--   0        0        0      805 2024-05-07 14:20:39.794778 langevals_huggingface-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 langevals_huggingface-0.1.2/PKG-INFO
```

### Comparing `langevals_huggingface-0.1.1/langevals_huggingface/bert_f1.py` & `langevals_huggingface-0.1.2/langevals_huggingface/bert_f1.py`

 * *Files identical despite different names*

### Comparing `langevals_huggingface-0.1.1/langevals_huggingface/bert_precision.py` & `langevals_huggingface-0.1.2/langevals_huggingface/bert_precision.py`

 * *Files identical despite different names*

### Comparing `langevals_huggingface-0.1.1/langevals_huggingface/bert_recall.py` & `langevals_huggingface-0.1.2/langevals_huggingface/bert_recall.py`

 * *Files identical despite different names*

### Comparing `langevals_huggingface-0.1.1/pyproject.toml` & `langevals_huggingface-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "langevals-huggingface"
-version = "0.1.1"
+version = "0.1.2"
 description = "LangEvals huggingface evaluators."
 authors = [ "Yevhenii Budnyk <y.budnyk789@gmail.com>",]
 license = "MIT"
 [[tool.poetry.source]]
 name = "pytorch_cpu"
 url = "https://download.pytorch.org/whl/cpu"
 priority = "explicit"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-langevals-core = "^0.1.2"
+langevals-core = "^0.1.3"
 evaluate = "^0.4.1"
 bert-score = "^0.3.13"
 [[tool.poetry.dependencies.torch]]
 version = "^2.2.2"
 source = "pytorch_cpu"
 markers = "sys_platform == 'linux'"
```

### Comparing `langevals_huggingface-0.1.1/PKG-INFO` & `langevals_huggingface-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: langevals-huggingface
-Version: 0.1.1
+Version: 0.1.2
 Summary: LangEvals huggingface evaluators.
 License: MIT
 Author: Yevhenii Budnyk
 Author-email: y.budnyk789@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bert-score (>=0.3.13,<0.4.0)
 Requires-Dist: evaluate (>=0.4.1,<0.5.0)
-Requires-Dist: langevals-core (>=0.1.2,<0.2.0)
+Requires-Dist: langevals-core (>=0.1.3,<0.2.0)
 Requires-Dist: torch (>=2.2.2,<3.0.0) ; sys_platform != "linux"
 Requires-Dist: torch (>=2.2.2,<3.0.0) ; sys_platform == "linux"
```

