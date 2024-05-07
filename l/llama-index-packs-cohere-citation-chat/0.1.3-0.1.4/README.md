# Comparing `tmp/llama_index_packs_cohere_citation_chat-0.1.3.tar.gz` & `tmp/llama_index_packs_cohere_citation_chat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_cohere_citation_chat-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_packs_cohere_citation_chat-0.1.4.tar", max compression
```

## Comparing `llama_index_packs_cohere_citation_chat-0.1.3.tar` & `llama_index_packs_cohere_citation_chat-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2010 2024-03-08 02:29:54.122482 llama_index_packs_cohere_citation_chat-0.1.3/README.md
--rw-r--r--   0        0        0      129 2024-03-08 02:29:54.126482 llama_index_packs_cohere_citation_chat-0.1.3/llama_index/packs/cohere_citation_chat/__init__.py
--rw-r--r--   0        0        0     1889 2024-03-08 02:29:54.126482 llama_index_packs_cohere_citation_chat-0.1.3/llama_index/packs/cohere_citation_chat/base.py
--rw-r--r--   0        0        0    17406 2024-03-08 02:29:54.126482 llama_index_packs_cohere_citation_chat-0.1.3/llama_index/packs/cohere_citation_chat/citations_context_chat_engine.py
--rw-r--r--   0        0        0      744 2024-03-08 02:29:54.126482 llama_index_packs_cohere_citation_chat-0.1.3/llama_index/packs/cohere_citation_chat/types.py
--rw-r--r--   0        0        0     1688 2024-03-08 02:29:54.126482 llama_index_packs_cohere_citation_chat-0.1.3/llama_index/packs/cohere_citation_chat/utils.py
--rw-r--r--   0        0        0     1669 2024-03-08 02:29:54.126482 llama_index_packs_cohere_citation_chat-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 llama_index_packs_cohere_citation_chat-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2010 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/README.md
+-rw-r--r--   0        0        0      129 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/__init__.py
+-rw-r--r--   0        0        0     1889 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/base.py
+-rw-r--r--   0        0        0    17396 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/citations_context_chat_engine.py
+-rw-r--r--   0        0        0      744 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/types.py
+-rw-r--r--   0        0        0     1688 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/utils.py
+-rw-r--r--   0        0        0     1670 2024-05-07 22:47:10.990522 llama_index_packs_cohere_citation_chat-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 llama_index_packs_cohere_citation_chat-0.1.4/PKG-INFO
```

### Comparing `llama_index_packs_cohere_citation_chat-0.1.3/README.md` & `llama_index_packs_cohere_citation_chat-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_packs_cohere_citation_chat-0.1.3/llama_index/packs/cohere_citation_chat/base.py` & `llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_cohere_citation_chat-0.1.3/llama_index/packs/cohere_citation_chat/citations_context_chat_engine.py` & `llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/citations_context_chat_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 "chat_stream is None. Cannot write to history without chat_stream."
             )
         # try/except to prevent hanging on error
         try:
             final_text = ""
             for chat in self.chat_stream:
                 # LLM response queue
-                self._is_function = is_function(chat.message)
+                self.is_function = is_function(chat.message)
                 self.put_in_queue(chat.delta)
                 final_text += chat.delta or ""
                 if chat.raw is not None:
                     # Citations stream event
                     if (
                         chat.raw.get("event_type", "")
                         == self.citations_settings.citations_stream_event_type
@@ -88,31 +88,31 @@
                     if (
                         chat.raw.get("event_type", "")
                         == self.citations_settings.documents_stream_event_type
                     ):
                         self.documents += convert_chat_response_to_documents(
                             chat, self.citations_settings
                         )
-            if self._is_function is not None:  # if loop has gone through iteration
+            if self.is_function is not None:  # if loop has gone through iteration
                 # NOTE: this is to handle the special case where we consume some of the
                 # chat stream, but not all of it (e.g. in react agent)
                 chat.message.content = final_text.strip()  # final message
                 memory.put(chat.message)
         except Exception as e:
             if not raise_error:
                 logger.warning(
                     f"Encountered exception writing response to history: {e}"
                 )
             else:
                 raise
 
-        self._is_done = True
+        self.is_done = True
 
         # This act as is_done events for any consumers waiting
-        self._is_function_not_none_thread_event.set()
+        self.is_function_not_none_thread_event.set()
 
     async def awrite_response_to_history(
         self,
         memory: BaseMemory,
     ) -> None:
         if self.achat_stream is None:
             raise ValueError(
@@ -120,19 +120,19 @@
                 "history without achat_stream."
             )
         # try/except to prevent hanging on error
         try:
             final_text = ""
             async for chat in self.achat_stream:
                 # Chat response queue
-                self._is_function = is_function(chat.message)
+                self.is_function = is_function(chat.message)
                 self.aput_in_queue(chat.delta)
                 final_text += chat.delta or ""
-                if self._is_function is False:
-                    self._is_function_false_event.set()
+                if self.is_function is False:
+                    self.is_function_false_event.set()
                 if chat.raw is not None:
                     # Citations stream event
                     if (
                         chat.raw.get("event_type", "")
                         == self.citations_settings.citations_stream_event_type
                     ):
                         self.citations += convert_chat_response_to_citations(
@@ -142,23 +142,23 @@
                     if (
                         chat.raw.get("event_type", "")
                         == self.citations_settings.documents_stream_event_type
                     ):
                         self.documents += convert_chat_response_to_documents(
                             chat, self.citations_settings
                         )
-                self._new_item_event.set()
-            if self._is_function is not None:  # if loop has gone through iteration
+                self.new_item_event.set()
+            if self.is_function is not None:  # if loop has gone through iteration
                 # NOTE: this is to handle the special case where we consume some of the
                 # chat stream, but not all of it (e.g. in react agent)
                 chat.message.content = final_text.strip()  # final message
                 memory.put(chat.message)
         except Exception as e:
             logger.warning(f"Encountered exception writing response to history: {e}")
-        self._is_done = True
+        self.is_done = True
 
 
 class ChatModeCitations(str, Enum):
     """Chat Engine Modes."""
 
     SIMPLE = "simple"
     """Corresponds to `SimpleChatEngine`.
```

### Comparing `llama_index_packs_cohere_citation_chat-0.1.3/llama_index/packs/cohere_citation_chat/types.py` & `llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_cohere_citation_chat-0.1.3/llama_index/packs/cohere_citation_chat/utils.py` & `llama_index_packs_cohere_citation_chat-0.1.4/llama_index/packs/cohere_citation_chat/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_cohere_citation_chat-0.1.3/pyproject.toml` & `llama_index_packs_cohere_citation_chat-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 description = "llama-index packs cohere_citation_chat integration"
 exclude = ["**/BUILD"]
 keywords = ["chat", "citation", "cite", "cohere", "engine", "index"]
 license = "MIT"
 maintainers = ["EugeneLightsOn"]
 name = "llama-index-packs-cohere-citation-chat"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.35"
 llama-index-llms-cohere = "^0.1.2"
 llama-index-embeddings-cohere = "^0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
```

### Comparing `llama_index_packs_cohere_citation_chat-0.1.3/PKG-INFO` & `llama_index_packs_cohere_citation_chat-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-cohere-citation-chat
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index packs cohere_citation_chat integration
 License: MIT
 Keywords: chat,citation,cite,cohere,engine,index
 Author: Your Name
 Author-email: you@example.com
 Maintainer: EugeneLightsOn
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
 Requires-Dist: llama-index-embeddings-cohere (>=0.1.2,<0.2.0)
 Requires-Dist: llama-index-llms-cohere (>=0.1.2,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Cohere Citations Chat Engine Pack
 
 Creates and runs a custom `VectorStoreIndexWithCitationsChat` -- which provides the chat engine with documents/citation mode.
```

