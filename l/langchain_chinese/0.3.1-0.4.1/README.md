# Comparing `tmp/langchain_chinese-0.3.1.tar.gz` & `tmp/langchain_chinese-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_chinese-0.3.1.tar", max compression
+gzip compressed data, was "langchain_chinese-0.4.1.tar", max compression
```

## Comparing `langchain_chinese-0.3.1.tar` & `langchain_chinese-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1066 2024-02-17 14:31:41.028210 langchain_chinese-0.3.1/LICENSE
--rw-r--r--   0        0        0     7068 2024-03-22 15:20:04.993433 langchain_chinese-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-02-18 04:12:40.965581 langchain_chinese-0.3.1/langchain_chinese/.pypirc
--rw-r--r--   0        0        0      743 2024-04-17 11:05:39.194120 langchain_chinese-0.3.1/langchain_chinese/__init__.py
--rw-r--r--   0        0        0       22 2024-04-16 10:55:29.186984 langchain_chinese-0.3.1/langchain_chinese/__version__.py
--rw-r--r--   0        0        0        0 2024-03-07 05:02:32.649684 langchain_chinese-0.3.1/langchain_chinese/agents/__init__.py
--rw-r--r--   0        0        0     2722 2024-03-11 11:16:28.698924 langchain_chinese-0.3.1/langchain_chinese/agents/base.py
--rw-r--r--   0        0        0     7036 2024-04-16 06:56:48.688214 langchain_chinese-0.3.1/langchain_chinese/agents/prompt.py
--rw-r--r--   0        0        0        0 2024-04-16 09:32:02.865599 langchain_chinese-0.3.1/langchain_chinese/agents/writing/__init__.py
--rw-r--r--   0        0        0     6780 2024-04-22 14:17:36.209883 langchain_chinese-0.3.1/langchain_chinese/agents/writing/base.py
--rw-r--r--   0        0        0      936 2024-04-22 08:23:19.731915 langchain_chinese-0.3.1/langchain_chinese/agents/writing/prompts/main.py
--rw-r--r--   0        0        0      385 2024-04-16 13:01:35.131996 langchain_chinese-0.3.1/langchain_chinese/agents/writing/prompts/translate.py
--rw-r--r--   0        0        0        0 2024-04-16 01:59:35.052113 langchain_chinese-0.3.1/langchain_chinese/agents/writing/reading/__init__.py
--rw-r--r--   0        0        0      112 2024-04-16 02:11:52.139352 langchain_chinese-0.3.1/langchain_chinese/agents/writing/reading/base.py
--rw-r--r--   0        0        0        0 2024-03-03 11:14:01.447370 langchain_chinese-0.3.1/langchain_chinese/document_loaders/__init__.py
--rw-r--r--   0        0        0     4252 2024-03-03 11:12:06.414308 langchain_chinese-0.3.1/langchain_chinese/document_loaders/base.py
--rw-r--r--   0        0        0       57 2024-03-17 15:26:04.636361 langchain_chinese-0.3.1/langchain_chinese/langgraph/__init__.py
--rw-r--r--   0        0        0     5269 2024-03-22 10:25:10.156397 langchain_chinese-0.3.1/langchain_chinese/langgraph/tools_calling.py
--rw-r--r--   0        0        0       77 2024-03-04 03:23:29.330261 langchain_chinese-0.3.1/langchain_chinese/memory/__init__.py
--rw-r--r--   0        0        0    10710 2024-03-04 03:27:24.792898 langchain_chinese-0.3.1/langchain_chinese/memory/base.py
--rw-r--r--   0        0        0     3612 2024-03-06 08:58:53.719955 langchain_chinese-0.3.1/langchain_chinese/memory/memory_manager.py
--rw-r--r--   0        0        0        0 2024-03-03 02:13:31.722951 langchain_chinese-0.3.1/langchain_chinese/retrievers/__init__.py
--rw-r--r--   0        0        0     3004 2024-04-16 07:36:51.110370 langchain_chinese-0.3.1/langchain_chinese/retrievers/base.py
--rw-r--r--   0        0        0      413 2024-04-18 00:26:11.920514 langchain_chinese-0.3.1/langchain_chinese/templates/agents/writing/expand/scripts.ipynb
--rw-r--r--   0        0        0      471 2024-04-18 00:25:43.311107 langchain_chinese-0.3.1/langchain_chinese/templates/agents/writing/project/README.md
--rw-r--r--   0        0        0      413 2024-04-17 09:58:36.350187 langchain_chinese-0.3.1/langchain_chinese/templates/agents/writing/project/scripts.ipynb
--rw-r--r--   0        0        0      842 2024-04-17 09:55:08.431338 langchain_chinese-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7970 1970-01-01 00:00:00.000000 langchain_chinese-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-02-17 14:31:41.028210 langchain_chinese-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1248 2024-05-08 01:33:56.028456 langchain_chinese-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-02-18 04:12:40.965581 langchain_chinese-0.4.1/langchain_chinese/.pypirc
+-rw-r--r--   0        0        0     1287 2024-05-05 08:33:33.898586 langchain_chinese-0.4.1/langchain_chinese/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-08 10:45:47.982505 langchain_chinese-0.4.1/langchain_chinese/__version__.py
+-rw-r--r--   0        0        0        0 2024-03-07 05:02:32.649684 langchain_chinese-0.4.1/langchain_chinese/agents/__init__.py
+-rw-r--r--   0        0        0     2722 2024-03-11 11:16:28.698924 langchain_chinese-0.4.1/langchain_chinese/agents/base.py
+-rw-r--r--   0        0        0     7036 2024-04-16 06:56:48.688214 langchain_chinese-0.4.1/langchain_chinese/agents/prompt.py
+-rw-r--r--   0        0        0        0 2024-03-03 11:14:01.447370 langchain_chinese-0.4.1/langchain_chinese/document_loaders/__init__.py
+-rw-r--r--   0        0        0     8955 2024-04-29 07:46:40.484137 langchain_chinese-0.4.1/langchain_chinese/document_loaders/base.py
+-rw-r--r--   0        0        0       57 2024-03-17 15:26:04.636361 langchain_chinese-0.4.1/langchain_chinese/langgraph/__init__.py
+-rw-r--r--   0        0        0     5269 2024-03-22 10:25:10.156397 langchain_chinese-0.4.1/langchain_chinese/langgraph/tools_calling.py
+-rw-r--r--   0        0        0       77 2024-03-04 03:23:29.330261 langchain_chinese-0.4.1/langchain_chinese/memory/__init__.py
+-rw-r--r--   0        0        0    10790 2024-04-28 12:26:57.200952 langchain_chinese-0.4.1/langchain_chinese/memory/base.py
+-rw-r--r--   0        0        0     3839 2024-04-28 08:39:13.373687 langchain_chinese-0.4.1/langchain_chinese/memory/history.py
+-rw-r--r--   0        0        0     3612 2024-04-28 12:18:24.523793 langchain_chinese-0.4.1/langchain_chinese/memory/memory_manager.py
+-rw-r--r--   0        0        0        0 2024-03-03 02:13:31.722951 langchain_chinese-0.4.1/langchain_chinese/retrievers/__init__.py
+-rw-r--r--   0        0        0     2999 2024-04-29 11:39:13.935381 langchain_chinese-0.4.1/langchain_chinese/retrievers/base.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:32:02.865599 langchain_chinese-0.4.1/langchain_chinese/writing/__init__.py
+-rw-r--r--   0        0        0     6780 2024-04-22 14:17:36.209883 langchain_chinese-0.4.1/langchain_chinese/writing/base.py
+-rw-r--r--   0        0        0     6073 2024-05-08 09:20:00.521804 langchain_chinese-0.4.1/langchain_chinese/writing/content.py
+-rw-r--r--   0        0        0      936 2024-04-22 08:23:19.731915 langchain_chinese-0.4.1/langchain_chinese/writing/prompts/main.py
+-rw-r--r--   0        0        0      385 2024-04-16 13:01:35.131996 langchain_chinese-0.4.1/langchain_chinese/writing/prompts/translate.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:59:35.052113 langchain_chinese-0.4.1/langchain_chinese/writing/reading/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-16 02:11:52.139352 langchain_chinese-0.4.1/langchain_chinese/writing/reading/base.py
+-rw-r--r--   0        0        0    16711 2024-05-08 10:03:51.460775 langchain_chinese-0.4.1/langchain_chinese/writing/task.py
+-rw-r--r--   0        0        0      867 2024-05-08 10:45:38.983718 langchain_chinese-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 langchain_chinese-0.4.1/PKG-INFO
```

### Comparing `langchain_chinese-0.3.1/LICENSE` & `langchain_chinese-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_chinese-0.3.1/langchain_chinese/agents/base.py` & `langchain_chinese-0.4.1/langchain_chinese/agents/base.py`

 * *Files identical despite different names*

### Comparing `langchain_chinese-0.3.1/langchain_chinese/agents/prompt.py` & `langchain_chinese-0.4.1/langchain_chinese/agents/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_chinese-0.3.1/langchain_chinese/agents/writing/base.py` & `langchain_chinese-0.4.1/langchain_chinese/writing/base.py`

 * *Files identical despite different names*

### Comparing `langchain_chinese-0.3.1/langchain_chinese/agents/writing/prompts/main.py` & `langchain_chinese-0.4.1/langchain_chinese/writing/prompts/main.py`

 * *Files identical despite different names*

### Comparing `langchain_chinese-0.3.1/langchain_chinese/langgraph/tools_calling.py` & `langchain_chinese-0.4.1/langchain_chinese/langgraph/tools_calling.py`

 * *Files identical despite different names*

### Comparing `langchain_chinese-0.3.1/langchain_chinese/memory/base.py` & `langchain_chinese-0.4.1/langchain_chinese/memory/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 from .memory_manager import MemoryManager
 
 class WithMemoryBinding(RunnableBindingBase):
     """Runnable that manages memory for another Runnable."""
 
     # 记忆管理
-    memory_manager:MemoryManager
+    memory_manager: MemoryManager
     input_messages_key: Optional[str] = None
     output_messages_key: Optional[str] = None
     history_messages_key: Optional[str] = None
     history_factory_config: Sequence[ConfigurableFieldSpec]
 
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
@@ -57,33 +57,33 @@
         self,
         runnable: Runnable[
             MessagesOrDictWithMessages,
             Union[str, BaseMessage, MessagesOrDictWithMessages],
         ],
         memory_manager: MemoryManager,
         *,
-        input_messages_key: Optional[str] = None,
+        input_messages_key: Optional[str] = "input",
         output_messages_key: Optional[str] = None,
-        history_messages_key: Optional[str] = None,
+        history_messages_key: Optional[str] = "history",
         history_factory_config: Optional[Sequence[ConfigurableFieldSpec]] = None,
         **kwargs: Any,
     ) -> None:
-        # 提取记忆 _enter_history / _aenter_history
+        # 提取记忆 _enter_memory / _aenter_memory
         history_chain: Runnable = RunnableLambda(
-            self._enter_history, self._aenter_history
+            self._enter_memory, self._aenter_memory
         ).with_config(run_name="load_history")
         messages_key = history_messages_key or input_messages_key
         if messages_key:
             history_chain = RunnablePassthrough.assign(
                 **{messages_key: history_chain}
             ).with_config(run_name="insert_history")
 
-        # 写入记忆 _exit_history
+        # 写入记忆 _exit_memory
         bound = (
-            history_chain | runnable.with_listeners(on_end=self._exit_history)
+            history_chain | runnable.with_listeners(on_end=self._exit_memory)
         ).with_config(run_name="RunnableWithMessageHistory")
 
         # 构造 configurable 中的参数
         if history_factory_config:
             _config_specs = history_factory_config
         else:
             # 如果没有专门指定，就使用默认的 session_id
@@ -161,45 +161,46 @@
             )
 
     def _get_output_messages(
         self, output_val: Union[str, BaseMessage, Sequence[BaseMessage], dict]
     ) -> List[BaseMessage]:
         from langchain_core.messages import BaseMessage
 
+        # 如果output_val是字典就取其中的output键或指定名字的键
         if isinstance(output_val, dict):
             output_val = output_val[self.output_messages_key or "output"]
 
         if isinstance(output_val, str):
             from langchain_core.messages import AIMessage
 
             return [AIMessage(content=output_val)]
         elif isinstance(output_val, BaseMessage):
             return [output_val]
         elif isinstance(output_val, (list, tuple)):
             return list(output_val)
         else:
             raise ValueError()
 
-    def _enter_history(self, input: Any, config: RunnableConfig) -> List[BaseMessage]:
+    def _enter_memory(self, input: Any, config: RunnableConfig) -> List[BaseMessage]:
         memory = config["configurable"]["memory"]
         # 提取记忆中应当插入到提示语中的部份
         if self.history_messages_key:
             return memory.buffer_as_messages
         else:
             input_val = (
                 input if not self.input_messages_key else input[self.input_messages_key]
             )
             return memory.buffer_as_messages + self._get_input_messages(input_val)
 
-    async def _aenter_history(
+    async def _aenter_memory(
         self, input: Dict[str, Any], config: RunnableConfig
     ) -> List[BaseMessage]:
-        return await run_in_executor(config, self._enter_history, input, config)
+        return await run_in_executor(config, self._enter_memory, input, config)
 
-    def _exit_history(self, run: Run, config: RunnableConfig) -> None:
+    def _exit_memory(self, run: Run, config: RunnableConfig) -> None:
         memory = config["configurable"]["memory"]
         hist = memory.chat_memory
 
         # Get the input messages
         inputs = load(run.inputs)
         input_val = inputs[self.input_messages_key or "input"]
         input_messages = self._get_input_messages(input_val)
```

### Comparing `langchain_chinese-0.3.1/langchain_chinese/memory/memory_manager.py` & `langchain_chinese-0.4.1/langchain_chinese/memory/memory_manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
     # 短期记忆管理，用于记忆模板
     _shorterm_memory: BaseChatMemory
     
     # 为每一个session_id单独建立记忆管理器
     _shorterm_memory_store: dict[str, BaseChatMemory] = {}
 
+    # 基于内存的记忆存储
+    _history_in_memory: dict[str, ChatMessageHistory] = {}
+
     # 记忆存储的回调函数，要求使用 session_id 位置参数
     get_longterm_memory_factory: Callable[[str], BaseChatMessageHistory]
 
     def __init__(
         self,
         longterm_memory_factory: Optional[Callable[[str], BaseChatMessageHistory]] = None,
         shorterm_memory: Optional[BaseChatMemory] = None
@@ -68,15 +71,12 @@
             if session_id not in self._shorterm_memory_store:
                 self._shorterm_memory_store[session_id] = copy.copy(self._shorterm_memory)
                 self._shorterm_memory_store[session_id].chat_memory = history
             return self._shorterm_memory_store[session_id]
         else:
             raise ValueError("Session ID is required")        
 
-    # 基于内存的记忆存储
-    _history_in_memory: dict[str, ChatMessageHistory] = {}
-
     def _get_history_in_memory(self, session_id: str) -> BaseChatMessageHistory:
         """默认的基于内存的记忆"""
         if session_id not in self._history_in_memory:
             self._history_in_memory[session_id] = ChatMessageHistory()
         return self._history_in_memory[session_id]
```

### Comparing `langchain_chinese-0.3.1/langchain_chinese/retrievers/base.py` & `langchain_chinese-0.4.1/langchain_chinese/retrievers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Callable, Any, Optional, Type, Union
 from langchain_core.prompts import ChatPromptTemplate
-from langchain_core.runnables import RunnablePassthrough, Runnable, RunnableAssign
+from langchain_core.runnables import RunnablePassthrough, Runnable, RunnableAssign, chain
 from langchain_core.output_parsers import StrOutputParser
 from langchain.agents import tool
 from langchain.tools import BaseTool
 from langchain.pydantic_v1 import BaseModel, Field
 from langchain.callbacks.manager import CallbackManagerForToolRun
 from langchain_core.messages import BaseMessage
 from functools import wraps
@@ -28,29 +28,29 @@
     if isinstance(message, BaseMessage):
         return message.content
     else:
         return message
 
 def create_qa_chain(llm: Runnable, retriever: Callable, prompt: str = DEFAULT_QA_CHAIN_PROMPT) -> Callable:
     """
-    使用 create_qa_chain 构建的LCEL链时，参数应当是一个消息列表。
+    使用 create_qa_chain 构建的LCEL链时，参数应当是一个消息。
     
     例如：    
     chain = creat_qa_chain(llm, rectriever)
-    chain.invoke(["langchain_chinese是啥？"])
+    chain.invoke("langchain_chinese是啥？")
     """
 
-    prompt = ChatPromptTemplate.from_template(prompt)
+    _prompt = ChatPromptTemplate.from_template(prompt)
 
     return (
         {
-            "context": (lambda x: convert_message_to_str(x[0])) | retriever | format_docs,
-            "question": lambda x: convert_message_to_str(x[0]) ,
+            "context": (lambda x: convert_message_to_str(x)) | retriever | format_docs,
+            "question": lambda x: convert_message_to_str(x) ,
         }
-        | prompt
+        | _prompt
         | llm
     )
 
 def make_safe_tool(func: Callable) -> Callable:
     """Create a new function that wraps the given function with error handling"""
     @wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> str:
```

### Comparing `langchain_chinese-0.3.1/pyproject.toml` & `langchain_chinese-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "langchain_chinese"
-version = "0.3.1"
+version = "0.4.1"
 description = "Prepare some firendly tool for Chinese LLMs and langchain"
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/langchain_chinese"
 repository = "https://github.com/arcstep/langchain_chinese.git"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.12"
 asyncio = "^3.4.3"
 pydantic = ">=1,<3"
 langchain = "^0.1.10"
 langchain-community = "^0.0.25"
 python-dotenv = "^1.0.1"
 
 [tool.poetry.group.dev.dependencies]
@@ -21,14 +21,15 @@
 poetry2setup = "^1.1.0"
 python-dotenv = "^1.0.1"
 ipykernel = "^6.29.2"
 pytest = "^8.0.1"
 pydantic = "1.10.13"
 docx2txt = "^0.8"
 pypdf = "^4.1.0"
+markdown = "^3.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
 include = "langchain_chinese/**/*"
```

