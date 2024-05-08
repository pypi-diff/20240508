# Comparing `tmp/syntrac_opentelemetry_instrumentation_langchain-0.0.2.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_langchain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_langchain-0.0.2.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_langchain-0.0.3.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.2.tar` & `syntrac_opentelemetry_instrumentation_langchain-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1164 2024-04-16 14:32:15.460571 syntrac_opentelemetry_instrumentation_langchain-0.0.2/README.md
--rw-r--r--   0        0        0     1183 2024-04-16 14:32:15.469969 syntrac_opentelemetry_instrumentation_langchain-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5853 2024-04-16 14:32:15.463342 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     2165 2024-04-16 14:32:15.464779 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py
--rw-r--r--   0        0        0     2958 2024-04-16 14:32:15.464899 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/task_wrapper.py
--rw-r--r--   0        0        0      809 2024-04-16 14:32:15.465021 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/utils.py
--rw-r--r--   0        0        0       22 2024-04-16 14:32:15.465128 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/version.py
--rw-r--r--   0        0        0     2318 2024-04-16 14:32:15.465237 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py
--rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_langchain-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1164 2024-05-08 11:05:49.789487 syntrac_opentelemetry_instrumentation_langchain-0.0.3/README.md
+-rw-r--r--   0        0        0     1183 2024-05-08 11:05:49.799750 syntrac_opentelemetry_instrumentation_langchain-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5978 2024-05-08 11:05:49.792343 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-08 11:05:49.794483 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/config.py
+-rw-r--r--   0        0        0     3895 2024-05-08 11:05:49.794623 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/custom_chat_wrapper.py
+-rw-r--r--   0        0        0     2165 2024-05-08 11:05:49.794860 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py
+-rw-r--r--   0        0        0     2958 2024-05-08 11:05:49.794998 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/task_wrapper.py
+-rw-r--r--   0        0        0     2627 2024-05-08 11:05:49.795137 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/utils.py
+-rw-r--r--   0        0        0       22 2024-05-08 11:05:49.795287 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/version.py
+-rw-r--r--   0        0        0     2318 2024-05-08 11:05:49.795420 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_langchain-0.0.3/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.2/README.md` & `syntrac_opentelemetry_instrumentation_langchain-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.2/pyproject.toml` & `syntrac_opentelemetry_instrumentation_langchain-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "syntrac-opentelemetry-instrumentation-langchain"
-version = "0.0.2"
+version = "0.0.3"
 description = "OpenTelemetry Langchain instrumentation"
 authors = [ "Vuong Ngo <vuongngo.pd@gmail.com>" ]
 repository = "https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-instrumentation-langchain"
 license = "Apache-2.0"
 readme = "README.md"
 
   [[tool.poetry.packages]]
```

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/__init__.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     workflow_wrapper,
     aworkflow_wrapper,
 )
 from syntrac_opentelemetry.instrumentation.langchain.custom_llm_wrapper import (
     llm_wrapper,
     allm_wrapper,
 )
+from syntrac_opentelemetry.instrumentation.langchain.custom_chat_wrapper import (
+    chat_wrapper,
+    achat_wrapper,
+)
 from syntrac_opentelemetry.instrumentation.langchain.version import __version__
 
 from syntrac_opentelemetry.semconv.ai import SyntracSpanKindValues
 
 logger = logging.getLogger(__name__)
 
 _instruments = ("langchain >= 0.0.346", "langchain-core > 0.1.0")
@@ -97,22 +101,22 @@
         "object": "BasePromptTemplate",
         "method": "ainvoke",
         "wrapper": atask_wrapper,
     },
     {
         "package": "langchain.chat_models.base",
         "object": "BaseChatModel",
-        "method": "invoke",
-        "wrapper": task_wrapper,
+        "method": "generate",
+        "wrapper": chat_wrapper,
     },
     {
         "package": "langchain.chat_models.base",
         "object": "BaseChatModel",
-        "method": "ainvoke",
-        "wrapper": atask_wrapper,
+        "method": "agenerate",
+        "wrapper": achat_wrapper,
     },
     {
         "package": "langchain.schema",
         "object": "BaseOutputParser",
         "method": "invoke",
         "wrapper": task_wrapper,
     },
```

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/task_wrapper.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/task_wrapper.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.2/PKG-INFO` & `syntrac_opentelemetry_instrumentation_langchain-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntrac-opentelemetry-instrumentation-langchain
-Version: 0.0.2
+Version: 0.0.3
 Summary: OpenTelemetry Langchain instrumentation
 Home-page: https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-instrumentation-langchain
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: syntrac-opentelemetry-instrumentation-langchain
-Version: 0.0.2 Summary: OpenTelemetry Langchain instrumentation Home-page:
+Version: 0.0.3 Summary: OpenTelemetry Langchain instrumentation Home-page:
 https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-
 instrumentation-langchain License: Apache-2.0 Author: Vuong Ngo Author-email:
 vuongngo.pd@gmail.com Requires-Python: >=3.9,<4 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
```

