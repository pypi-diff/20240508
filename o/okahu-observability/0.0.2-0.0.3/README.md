# Comparing `tmp/okahu_observability-0.0.2.tar.gz` & `tmp/okahu_observability-0.0.3.tar.gz`

## Comparing `okahu_observability-0.0.2.tar` & `okahu_observability-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/src/okahu_apptrace/__init__.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/src/okahu_apptrace/exporter.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/src/okahu_apptrace/instrumentor.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/src/okahu_apptrace/utils.py
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/src/okahu_apptrace/wrapper.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/.gitignore
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/LICENSE
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/README.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/logprobs_sample.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/src/okahu_apptrace/__init__.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/src/okahu_apptrace/exporter.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/src/okahu_apptrace/instrumentor.py
+-rw-r--r--   0        0        0     6344 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/src/okahu_apptrace/utils.py
+-rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/src/okahu_apptrace/wrapper.py
+-rw-r--r--   0        0        0     9128 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/storage/default__vector_store.json
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/storage/docstore.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/storage/graph_store.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/storage/image__vector_store.json
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/storage/index_store.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/.gitignore
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/README.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 okahu_observability-0.0.3/PKG-INFO
```

### Comparing `okahu_observability-0.0.2/src/okahu_apptrace/exporter.py` & `okahu_observability-0.0.3/src/okahu_apptrace/exporter.py`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.2/src/okahu_apptrace/instrumentor.py` & `okahu_observability-0.0.3/src/okahu_apptrace/instrumentor.py`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.2/src/okahu_apptrace/utils.py` & `okahu_observability-0.0.3/src/okahu_apptrace/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import logging
 import os
 from opentelemetry.trace import Tracer, Span
 
 logger = logging.getLogger(__name__)
+WORKFLOW_TYPE_KEY = "workflow_type"
+
+WORKFLOW_TYPE_MAP = {
+    "llama_index": "workflow.llamaindex",
+    "langchain": "workflow.langchain"
+}
 
 def _with_tracer_wrapper(func):
     """Helper for providing tracer for wrapper functions."""
 
     def _with_tracer(tracer, to_wrap):
         def wrapper(wrapped, instance, args, kwargs):
             return func(tracer, to_wrap, wrapped, instance, args, kwargs)
@@ -28,17 +34,19 @@
     elif to_wrap.get("span_name"):
         name = to_wrap.get("span_name")
     else:
         name = f"langchain.task.{instance.__class__.__name__}"
     kind = to_wrap.get("kind")
     with tracer.start_as_current_span(name) as span:
         return_value = wrapped(*args, **kwargs)
+
         if is_root_span(span):
             workflow_name = span.resource.attributes.get("service.name")
             span.set_attribute("workflow_name",workflow_name)
+            update_workflow_type(to_wrap, span)
 
     return return_value
 
 @_with_tracer_wrapper
 async def atask_wrapper(tracer, to_wrap, wrapped, instance, args, kwargs):
     """Instruments and calls every function defined in TO_WRAP."""
 
@@ -102,17 +110,22 @@
     return return_value
 
 def update_llm_endpoint(curr_span: Span, instance):
     triton_llm_endpoint = os.environ.get("TRITON_LLM_ENDPOINT")
     if triton_llm_endpoint is not None and len(triton_llm_endpoint) > 0:
         curr_span.set_attribute("server_url", triton_llm_endpoint)
 
+    # handling for langchain
     if 'model_name' in instance.__dict__:
         model_name = instance.__dict__.get("model_name")
         curr_span.set_attribute("openai_model_name", model_name)
+    # handling for llama_index
+    if 'model' in instance.__dict__:
+        model_name = instance.__dict__.get("model")
+        curr_span.set_attribute("openai_model_name", model_name)
 
 def is_root_span(curr_span: Span) -> bool:
     return curr_span.parent == None
 
 def get_input_from_args(chain_args):
     if len(chain_args) > 0 and type(chain_args[0]) == str:
         return chain_args[0]
@@ -126,16 +139,24 @@
         if token_usage is not None:
             span.set_attribute("completion_tokens", token_usage.get("completion_tokens"))
             span.set_attribute("prompt_tokens", token_usage.get("prompt_tokens"))
             span.set_attribute("total_tokens", token_usage.get("total_tokens"))
     
     # extract token usage from llamaindex openai
     if (response is not None and hasattr(response, "raw")):
-        token_usage = response.raw.get("usage")
-        if token_usage is not None:
-            if(hasattr(token_usage, "completion_tokens")):
-                span.set_attribute("completion_tokens", token_usage.completion_tokens)
-            if(hasattr(token_usage, "prompt_tokens")):
-                span.set_attribute("prompt_tokens", token_usage.prompt_tokens)
-            if(hasattr(token_usage, "total_tokens")):
-                span.set_attribute("total_tokens", token_usage.total_tokens)
+        if response.raw is not None:
+            token_usage = response.raw.get("usage")
+            if token_usage is not None:
+                if(hasattr(token_usage, "completion_tokens")):
+                    span.set_attribute("completion_tokens", token_usage.completion_tokens)
+                if(hasattr(token_usage, "prompt_tokens")):
+                    span.set_attribute("prompt_tokens", token_usage.prompt_tokens)
+                if(hasattr(token_usage, "total_tokens")):
+                    span.set_attribute("total_tokens", token_usage.total_tokens)
+
+def update_workflow_type(to_wrap, span: Span):
+    package_name = to_wrap.get('package')
+
+    for (package, workflow_type) in WORKFLOW_TYPE_MAP.items():
+        if(package_name is not None and package in package_name):
+            span.set_attribute(WORKFLOW_TYPE_KEY, workflow_type)
```

### Comparing `okahu_observability-0.0.2/src/okahu_apptrace/wrapper.py` & `okahu_observability-0.0.3/src/okahu_apptrace/wrapper.py`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.2/.gitignore` & `okahu_observability-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.2/LICENSE` & `okahu_observability-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.2/README.md` & `okahu_observability-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This package provides okahu telemetry setup.
 
 ## Installing the package
 ```
 > python3 -m pip install pipenv
 
-> pipenv install okahu-otel
+> pipenv install okahu-observability
 ```
 
 ## References
 
 [Managing application dependencies](https://packaging.python.org/en/latest/tutorials/managing-dependencies/)
 
 ## Usage
```

### Comparing `okahu_observability-0.0.2/pyproject.toml` & `okahu_observability-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "okahu-observability"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Okahu Inc.", email="okahu-pypi@okahu.ai" },
 ]
 description = "package with okahu opentelemetry"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `okahu_observability-0.0.2/PKG-INFO` & `okahu_observability-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: okahu-observability
-Version: 0.0.2
+Version: 0.0.3
 Summary: package with okahu opentelemetry
 Project-URL: Homepage, https://github.com/okahu/demo-repository
 Project-URL: Issues, https://github.com/okahu/demo-repository/issues
 Author-email: "Okahu Inc." <okahu-pypi@okahu.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
 
 This package provides okahu telemetry setup.
 
 ## Installing the package
 ```
 > python3 -m pip install pipenv
 
-> pipenv install okahu-otel
+> pipenv install okahu-observability
 ```
 
 ## References
 
 [Managing application dependencies](https://packaging.python.org/en/latest/tutorials/managing-dependencies/)
 
 ## Usage
```

