# Comparing `tmp/llama_index_agent_openai_legacy-0.1.3.tar.gz` & `tmp/llama_index_agent_openai_legacy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_agent_openai_legacy-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_agent_openai_legacy-0.1.4.tar", max compression
```

## Comparing `llama_index_agent_openai_legacy-0.1.3.tar` & `llama_index_agent_openai_legacy-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       46 2024-03-23 00:06:28.923403 llama_index_agent_openai_legacy-0.1.3/README.md
--rw-r--r--   0        0        0      412 2024-03-23 00:06:28.923403 llama_index_agent_openai_legacy-0.1.3/llama_index/agent/openai_legacy/__init__.py
--rw-r--r--   0        0        0     7463 2024-03-23 00:06:28.923403 llama_index_agent_openai_legacy-0.1.3/llama_index/agent/openai_legacy/context_retriever_agent.py
--rw-r--r--   0        0        0    22757 2024-03-23 00:06:28.923403 llama_index_agent_openai_legacy-0.1.3/llama_index/agent/openai_legacy/openai_agent.py
--rw-r--r--   0        0        0      857 2024-03-23 00:06:28.923403 llama_index_agent_openai_legacy-0.1.3/llama_index/agent/openai_legacy/retriever_openai_agent.py
--rw-r--r--   0        0        0      772 2024-03-23 00:06:28.923403 llama_index_agent_openai_legacy-0.1.3/llama_index/agent/openai_legacy/utils.py
--rw-r--r--   0        0        0     1540 2024-03-23 00:06:28.923403 llama_index_agent_openai_legacy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 llama_index_agent_openai_legacy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/README.md
+-rw-r--r--   0        0        0      412 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/__init__.py
+-rw-r--r--   0        0        0     7463 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/context_retriever_agent.py
+-rw-r--r--   0        0        0    22754 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/openai_agent.py
+-rw-r--r--   0        0        0      857 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/retriever_openai_agent.py
+-rw-r--r--   0        0        0      772 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/utils.py
+-rw-r--r--   0        0        0     1541 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 llama_index_agent_openai_legacy-0.1.4/PKG-INFO
```

### Comparing `llama_index_agent_openai_legacy-0.1.3/llama_index/agent/openai_legacy/context_retriever_agent.py` & `llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/context_retriever_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai_legacy-0.1.3/llama_index/agent/openai_legacy/openai_agent.py` & `llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/openai_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,17 +224,17 @@
         # Get the response in a separate thread so we can yield the response
         thread = Thread(
             target=chat_stream_response.write_response_to_history,
             args=(self.memory,),
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
         self, **llm_chat_kwargs: Any
@@ -245,15 +245,15 @@
         )
         # create task to write chat response to history
         asyncio.create_task(
             chat_stream_response.awrite_response_to_history(self.memory)
         )
         # wait until openAI functions stop executing
         chat_stream_response._ensure_async_setup()
-        await chat_stream_response._is_function_false_event.wait()
+        await chat_stream_response.is_function_false_event.wait()
 
         # return response stream
         return chat_stream_response
 
     def _call_function(self, tools: List[BaseTool], tool_call: OpenAIToolCall) -> None:
         function_call = tool_call.function
         # validations to get passed mypy
```

### Comparing `llama_index_agent_openai_legacy-0.1.3/llama_index/agent/openai_legacy/retriever_openai_agent.py` & `llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/retriever_openai_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai_legacy-0.1.3/llama_index/agent/openai_legacy/utils.py` & `llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai_legacy-0.1.3/pyproject.toml` & `llama_index_agent_openai_legacy-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index agent openai-legacy integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-agent-openai-legacy"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.35"
 llama-index-llms-openai = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
```

### Comparing `llama_index_agent_openai_legacy-0.1.3/PKG-INFO` & `llama_index_agent_openai_legacy-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-agent-openai-legacy
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index agent openai-legacy integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
 Requires-Dist: llama-index-llms-openai (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Agent Integration: Openai-Legacy
```

