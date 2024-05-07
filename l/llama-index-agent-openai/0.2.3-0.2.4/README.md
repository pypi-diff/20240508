# Comparing `tmp/llama_index_agent_openai-0.2.3.tar.gz` & `tmp/llama_index_agent_openai-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_agent_openai-0.2.3.tar", max compression
+gzip compressed data, was "llama_index_agent_openai-0.2.4.tar", max compression
```

## Comparing `llama_index_agent_openai-0.2.3.tar` & `llama_index_agent_openai-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       39 2024-04-22 18:00:39.394410 llama_index_agent_openai-0.2.3/README.md
--rw-r--r--   0        0        0      342 2024-04-22 18:00:39.394410 llama_index_agent_openai-0.2.3/llama_index/agent/openai/__init__.py
--rw-r--r--   0        0        0     4745 2024-04-22 18:00:39.394410 llama_index_agent_openai-0.2.3/llama_index/agent/openai/base.py
--rw-r--r--   0        0        0    18794 2024-04-22 18:00:39.394410 llama_index_agent_openai-0.2.3/llama_index/agent/openai/openai_assistant_agent.py
--rw-r--r--   0        0        0    28600 2024-04-22 18:00:39.394410 llama_index_agent_openai-0.2.3/llama_index/agent/openai/step.py
--rw-r--r--   0        0        0      772 2024-04-22 18:00:39.394410 llama_index_agent_openai-0.2.3/llama_index/agent/openai/utils.py
--rw-r--r--   0        0        0     1522 2024-04-22 18:00:39.394410 llama_index_agent_openai-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 llama_index_agent_openai-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/README.md
+-rw-r--r--   0        0        0      342 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/llama_index/agent/openai/__init__.py
+-rw-r--r--   0        0        0     4745 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/llama_index/agent/openai/base.py
+-rw-r--r--   0        0        0    18794 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/llama_index/agent/openai/openai_assistant_agent.py
+-rw-r--r--   0        0        0    28597 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/llama_index/agent/openai/step.py
+-rw-r--r--   0        0        0      772 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/llama_index/agent/openai/utils.py
+-rw-r--r--   0        0        0     1522 2024-05-07 22:47:10.634523 llama_index_agent_openai-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 llama_index_agent_openai-0.2.4/PKG-INFO
```

### Comparing `llama_index_agent_openai-0.2.3/llama_index/agent/openai/base.py` & `llama_index_agent_openai-0.2.4/llama_index/agent/openai/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.3/llama_index/agent/openai/openai_assistant_agent.py` & `llama_index_agent_openai-0.2.4/llama_index/agent/openai/openai_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.3/llama_index/agent/openai/step.py` & `llama_index_agent_openai-0.2.4/llama_index/agent/openai/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,17 +385,17 @@
         thread = Thread(
             target=chat_stream_response.write_response_to_history,
             args=(task.extra_state["new_memory"],),
             kwargs={"on_stream_end_fn": partial(self.finalize_task, task)},
         )
         thread.start()
         # Wait for the event to be set
-        chat_stream_response._is_function_not_none_thread_event.wait()
+        chat_stream_response.is_function_not_none_thread_event.wait()
         # If it is executing an openAI function, wait for the thread to finish
-        if chat_stream_response._is_function:
+        if chat_stream_response.is_function:
             thread.join()
 
         # if it's false, return the answer (to stream)
         return chat_stream_response
 
     async def _get_async_stream_ai_response(
         self, task: Task, **llm_chat_kwargs: Any
@@ -410,15 +410,15 @@
                 task.extra_state["new_memory"],
                 on_stream_end_fn=partial(self.finalize_task, task),
             )
         )
         chat_stream_response._ensure_async_setup()
 
         # wait until openAI functions stop executing
-        await chat_stream_response._is_function_false_event.wait()
+        await chat_stream_response.is_function_false_event.wait()
 
         # return response stream
         return chat_stream_response
 
     def _get_agent_response(
         self, task: Task, mode: ChatResponseMode, **llm_chat_kwargs: Any
     ) -> AGENT_CHAT_RESPONSE_TYPE:
```

### Comparing `llama_index_agent_openai-0.2.3/llama_index/agent/openai/utils.py` & `llama_index_agent_openai-0.2.4/llama_index/agent/openai/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.3/pyproject.toml` & `llama_index_agent_openai-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index agent openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-agent-openai"
 readme = "README.md"
-version = "0.2.3"
+version = "0.2.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.30"
+llama-index-core = "^0.10.35"
 llama-index-llms-openai = "^0.1.5"
 openai = ">=1.14.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
```

### Comparing `llama_index_agent_openai-0.2.3/PKG-INFO` & `llama_index_agent_openai-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-agent-openai
-Version: 0.2.3
+Version: 0.2.4
 Summary: llama-index agent openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.30,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
 Requires-Dist: llama-index-llms-openai (>=0.1.5,<0.2.0)
 Requires-Dist: openai (>=1.14.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Agent Integration: Openai
```

