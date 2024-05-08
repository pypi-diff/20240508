# Comparing `tmp/syntrac_sdk-0.0.5.tar.gz` & `tmp/syntrac_sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_sdk-0.0.5.tar", max compression
+gzip compressed data, was "syntrac_sdk-0.0.6.tar", max compression
```

## Comparing `syntrac_sdk-0.0.5.tar` & `syntrac_sdk-0.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      395 2024-04-18 00:59:56.678927 syntrac_sdk-0.0.5/README.md
--rw-r--r--   0        0        0     2072 2024-04-18 00:59:56.701004 syntrac_sdk-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     7767 2024-04-18 00:59:56.681758 syntrac_sdk-0.0.5/syntrac/sdk/__init__.py
--rw-r--r--   0        0        0      358 2024-04-18 00:59:56.683801 syntrac_sdk-0.0.5/syntrac/sdk/config/__init__.py
--rw-r--r--   0        0        0     1117 2024-04-18 00:59:56.684152 syntrac_sdk-0.0.5/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11612 2024-04-18 00:59:56.684642 syntrac_sdk-0.0.5/syntrac/sdk/decorators/__init__.py
--rw-r--r--   0        0        0    16396 2024-04-18 00:59:56.685162 syntrac_sdk-0.0.5/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4393 2024-04-18 00:59:56.685342 syntrac_sdk-0.0.5/syntrac/sdk/fetcher.py
--rw-r--r--   0        0        0      465 2024-04-18 00:59:56.685474 syntrac_sdk-0.0.5/syntrac/sdk/instruments.py
--rw-r--r--   0        0        0        0 2024-04-18 00:59:56.685658 syntrac_sdk-0.0.5/syntrac/sdk/metrics/__init__.py
--rw-r--r--   0        0        0      202 2024-04-18 00:59:56.685889 syntrac_sdk-0.0.5/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3362 2024-04-18 00:59:56.686135 syntrac_sdk-0.0.5/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
--rw-r--r--   0        0        0     2109 2024-04-18 00:59:56.686387 syntrac_sdk-0.0.5/syntrac/sdk/metrics/metrics.py
--rw-r--r--   0        0        0     2721 2024-04-18 00:59:56.686749 syntrac_sdk-0.0.5/syntrac/sdk/otlp/json/__init__.py
--rw-r--r--   0        0        0     2638 2024-04-18 00:59:56.687218 syntrac_sdk-0.0.5/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      225 2024-04-18 00:59:56.687500 syntrac_sdk-0.0.5/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     7151 2024-04-18 00:59:56.687890 syntrac_sdk-0.0.5/syntrac/sdk/otlp/json/trace_exporter/__init__.py
--rw-r--r--   0        0        0     9686 2024-04-18 00:59:56.688266 syntrac_sdk-0.0.5/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      607 2024-04-18 00:59:56.688509 syntrac_sdk-0.0.5/syntrac/sdk/otlp/json/version.py
--rw-r--r--   0        0        0      152 2024-04-18 00:59:56.688766 syntrac_sdk-0.0.5/syntrac/sdk/prompts/__init__.py
--rw-r--r--   0        0        0      514 2024-04-18 00:59:56.689012 syntrac_sdk-0.0.5/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9274 2024-04-18 00:59:56.689160 syntrac_sdk-0.0.5/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     4571 2024-04-18 00:59:56.689350 syntrac_sdk-0.0.5/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     1345 2024-04-18 00:59:56.689488 syntrac_sdk-0.0.5/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc
--rw-r--r--   0        0        0     5583 2024-04-18 00:59:56.689636 syntrac_sdk-0.0.5/syntrac/sdk/prompts/client.py
--rw-r--r--   0        0        0     1558 2024-04-18 00:59:56.689778 syntrac_sdk-0.0.5/syntrac/sdk/prompts/model.py
--rw-r--r--   0        0        0      408 2024-04-18 00:59:56.689933 syntrac_sdk-0.0.5/syntrac/sdk/prompts/registry.py
--rw-r--r--   0        0        0     2424 2024-04-18 00:59:56.690265 syntrac_sdk-0.0.5/syntrac/sdk/telemetry.py
--rw-r--r--   0        0        0     6148 2024-04-18 00:59:56.690613 syntrac_sdk-0.0.5/syntrac/sdk/tracing/.DS_Store
--rw-r--r--   0        0        0      248 2024-04-18 00:59:56.690867 syntrac_sdk-0.0.5/syntrac/sdk/tracing/__init__.py
--rw-r--r--   0        0        0      559 2024-04-18 00:59:56.691239 syntrac_sdk-0.0.5/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1969 2024-04-18 00:59:56.691383 syntrac_sdk-0.0.5/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
--rw-r--r--   0        0        0      877 2024-04-18 00:59:56.691603 syntrac_sdk-0.0.5/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
--rw-r--r--   0        0        0      818 2024-04-18 00:59:56.691840 syntrac_sdk-0.0.5/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc
--rw-r--r--   0        0        0    29511 2024-04-18 00:59:56.692223 syntrac_sdk-0.0.5/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
--rw-r--r--   0        0        0      846 2024-04-18 00:59:56.692393 syntrac_sdk-0.0.5/syntrac/sdk/tracing/content_allow_list.py
--rw-r--r--   0        0        0      297 2024-04-18 00:59:56.692616 syntrac_sdk-0.0.5/syntrac/sdk/tracing/context_manager.py
--rw-r--r--   0        0        0      322 2024-04-18 00:59:56.692847 syntrac_sdk-0.0.5/syntrac/sdk/tracing/context_passing.py
--rw-r--r--   0        0        0    23992 2024-04-18 00:59:56.693177 syntrac_sdk-0.0.5/syntrac/sdk/tracing/tracing.py
--rw-r--r--   0        0        0      604 2024-04-18 00:59:56.693844 syntrac_sdk-0.0.5/syntrac/sdk/utils/__init__.py
--rw-r--r--   0        0        0     1487 2024-04-18 00:59:56.694337 syntrac_sdk-0.0.5/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2112 2024-04-18 00:59:56.694590 syntrac_sdk-0.0.5/syntrac/sdk/utils/in_memory_span_exporter.py
--rw-r--r--   0        0        0       22 2024-04-18 00:59:56.694739 syntrac_sdk-0.0.5/syntrac/sdk/version.py
--rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      395 2024-05-08 11:06:52.376394 syntrac_sdk-0.0.6/README.md
+-rw-r--r--   0        0        0     2072 2024-05-08 11:06:52.396781 syntrac_sdk-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     7767 2024-05-08 11:06:52.378540 syntrac_sdk-0.0.6/syntrac/sdk/__init__.py
+-rw-r--r--   0        0        0      358 2024-05-08 11:06:52.380801 syntrac_sdk-0.0.6/syntrac/sdk/config/__init__.py
+-rw-r--r--   0        0        0     1117 2024-05-08 11:06:52.381123 syntrac_sdk-0.0.6/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11612 2024-05-08 11:06:52.381461 syntrac_sdk-0.0.6/syntrac/sdk/decorators/__init__.py
+-rw-r--r--   0        0        0    16396 2024-05-08 11:06:52.382016 syntrac_sdk-0.0.6/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4393 2024-05-08 11:06:52.382247 syntrac_sdk-0.0.6/syntrac/sdk/fetcher.py
+-rw-r--r--   0        0        0      465 2024-05-08 11:06:52.382367 syntrac_sdk-0.0.6/syntrac/sdk/instruments.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:06:52.382541 syntrac_sdk-0.0.6/syntrac/sdk/metrics/__init__.py
+-rw-r--r--   0        0        0      202 2024-05-08 11:06:52.382761 syntrac_sdk-0.0.6/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3362 2024-05-08 11:06:52.383012 syntrac_sdk-0.0.6/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
+-rw-r--r--   0        0        0     2109 2024-05-08 11:06:52.383285 syntrac_sdk-0.0.6/syntrac/sdk/metrics/metrics.py
+-rw-r--r--   0        0        0     2721 2024-05-08 11:06:52.383564 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/__init__.py
+-rw-r--r--   0        0        0     2638 2024-05-08 11:06:52.383907 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      225 2024-05-08 11:06:52.384152 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0     7151 2024-05-08 11:06:52.384368 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/trace_exporter/__init__.py
+-rw-r--r--   0        0        0     9686 2024-05-08 11:06:52.384690 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      607 2024-05-08 11:06:52.385135 syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/version.py
+-rw-r--r--   0        0        0      152 2024-05-08 11:06:52.385435 syntrac_sdk-0.0.6/syntrac/sdk/prompts/__init__.py
+-rw-r--r--   0        0        0      514 2024-05-08 11:06:52.385695 syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9274 2024-05-08 11:06:52.385838 syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     4571 2024-05-08 11:06:52.386119 syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0        0        0     1345 2024-05-08 11:06:52.386260 syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc
+-rw-r--r--   0        0        0     5583 2024-05-08 11:06:52.386400 syntrac_sdk-0.0.6/syntrac/sdk/prompts/client.py
+-rw-r--r--   0        0        0     1558 2024-05-08 11:06:52.386523 syntrac_sdk-0.0.6/syntrac/sdk/prompts/model.py
+-rw-r--r--   0        0        0      408 2024-05-08 11:06:52.386661 syntrac_sdk-0.0.6/syntrac/sdk/prompts/registry.py
+-rw-r--r--   0        0        0     2424 2024-05-08 11:06:52.386791 syntrac_sdk-0.0.6/syntrac/sdk/telemetry.py
+-rw-r--r--   0        0        0     6148 2024-05-08 11:06:52.387182 syntrac_sdk-0.0.6/syntrac/sdk/tracing/.DS_Store
+-rw-r--r--   0        0        0      248 2024-05-08 11:06:52.387397 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-08 11:06:52.387697 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1969 2024-05-08 11:06:52.387835 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
+-rw-r--r--   0        0        0      877 2024-05-08 11:06:52.388017 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
+-rw-r--r--   0        0        0      818 2024-05-08 11:06:52.388350 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc
+-rw-r--r--   0        0        0    29511 2024-05-08 11:06:52.388737 syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
+-rw-r--r--   0        0        0      846 2024-05-08 11:06:52.388857 syntrac_sdk-0.0.6/syntrac/sdk/tracing/content_allow_list.py
+-rw-r--r--   0        0        0      297 2024-05-08 11:06:52.389080 syntrac_sdk-0.0.6/syntrac/sdk/tracing/context_manager.py
+-rw-r--r--   0        0        0      322 2024-05-08 11:06:52.389300 syntrac_sdk-0.0.6/syntrac/sdk/tracing/context_passing.py
+-rw-r--r--   0        0        0    23992 2024-05-08 11:06:52.389629 syntrac_sdk-0.0.6/syntrac/sdk/tracing/tracing.py
+-rw-r--r--   0        0        0      604 2024-05-08 11:06:52.389828 syntrac_sdk-0.0.6/syntrac/sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1487 2024-05-08 11:06:52.390133 syntrac_sdk-0.0.6/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2112 2024-05-08 11:06:52.390363 syntrac_sdk-0.0.6/syntrac/sdk/utils/in_memory_span_exporter.py
+-rw-r--r--   0        0        0       22 2024-05-08 11:06:52.390578 syntrac_sdk-0.0.6/syntrac/sdk/version.py
+-rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.6/PKG-INFO
```

### Comparing `syntrac_sdk-0.0.5/pyproject.toml` & `syntrac_sdk-0.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "syntrac-sdk"
-version = "0.0.5"
+version = "0.0.6"
 description = "Syntrac Software Development Kit (SDK) for Python"
 authors = [ "Vuong Ngo <vuongngo.pd@gmail.com>" ]
 repository = "https://github.com/syntracAI/syntrac"
 documentation = "https://syntrac.com/docs/openllmetry"
 license = "Apache-2.0"
 readme = "README.md"
 
@@ -29,15 +29,15 @@
   opentelemetry-instrumentation-urllib3 = "0.44b0"
   syntrac-opentelemetry-semantic-conventions-ai = "0.0.1"
   syntrac-opentelemetry-instrumentation-openai = "0.0.2"
   syntrac-opentelemetry-instrumentation-anthropic = "0.0.2"
   syntrac-opentelemetry-instrumentation-cohere = "0.0.2"
   syntrac-opentelemetry-instrumentation-pinecone = "0.0.2"
   syntrac-opentelemetry-instrumentation-qdrant = "0.0.2"
-  syntrac-opentelemetry-instrumentation-langchain = "0.0.2"
+  syntrac-opentelemetry-instrumentation-langchain = "0.0.3"
   syntrac-opentelemetry-instrumentation-chromadb = "0.0.2"
   syntrac-opentelemetry-instrumentation-transformers = "0.0.2"
   syntrac-opentelemetry-instrumentation-llamaindex = "0.0.2"
   syntrac-opentelemetry-instrumentation-haystack = "0.0.2"
   syntrac-opentelemetry-instrumentation-bedrock = "0.0.2"
   syntrac-opentelemetry-instrumentation-replicate = "0.0.2"
   syntrac-opentelemetry-instrumentation-vertexai = "0.0.2"
```

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/__init__.py` & `syntrac_sdk-0.0.6/syntrac/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/decorators/__init__.py` & `syntrac_sdk-0.0.6/syntrac/sdk/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/fetcher.py` & `syntrac_sdk-0.0.6/syntrac/sdk/fetcher.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/metrics/metrics.py` & `syntrac_sdk-0.0.6/syntrac/sdk/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/otlp/json/__init__.py` & `syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/otlp/json/trace_exporter/__init__.py` & `syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/trace_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/otlp/json/version.py` & `syntrac_sdk-0.0.6/syntrac/sdk/otlp/json/version.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/prompts/client.py` & `syntrac_sdk-0.0.6/syntrac/sdk/prompts/client.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/prompts/model.py` & `syntrac_sdk-0.0.6/syntrac/sdk/prompts/model.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/telemetry.py` & `syntrac_sdk-0.0.6/syntrac/sdk/telemetry.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/tracing/.DS_Store` & `syntrac_sdk-0.0.6/syntrac/sdk/tracing/.DS_Store`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/tracing/content_allow_list.py` & `syntrac_sdk-0.0.6/syntrac/sdk/tracing/content_allow_list.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/tracing/tracing.py` & `syntrac_sdk-0.0.6/syntrac/sdk/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/utils/__init__.py` & `syntrac_sdk-0.0.6/syntrac/sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.6/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/syntrac/sdk/utils/in_memory_span_exporter.py` & `syntrac_sdk-0.0.6/syntrac/sdk/utils/in_memory_span_exporter.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.5/PKG-INFO` & `syntrac_sdk-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntrac-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: Syntrac Software Development Kit (SDK) for Python
 Home-page: https://github.com/syntracAI/syntrac
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,15 +25,15 @@
 Requires-Dist: posthog (>=3.0.2,<4.0.0)
 Requires-Dist: pydantic (>=1)
 Requires-Dist: syntrac-opentelemetry-instrumentation-anthropic (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-bedrock (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-chromadb (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-cohere (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-haystack (==0.0.2)
-Requires-Dist: syntrac-opentelemetry-instrumentation-langchain (==0.0.2)
+Requires-Dist: syntrac-opentelemetry-instrumentation-langchain (==0.0.3)
 Requires-Dist: syntrac-opentelemetry-instrumentation-llamaindex (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-openai (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-pinecone (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-qdrant (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-replicate (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-transformers (==0.0.2)
 Requires-Dist: syntrac-opentelemetry-instrumentation-vertexai (==0.0.2)
```

