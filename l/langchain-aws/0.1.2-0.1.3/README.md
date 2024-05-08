# Comparing `tmp/langchain_aws-0.1.2.tar.gz` & `tmp/langchain_aws-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_aws-0.1.2.tar", max compression
+gzip compressed data, was "langchain_aws-0.1.3.tar", max compression
```

## Comparing `langchain_aws-0.1.2.tar` & `langchain_aws-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1072 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/LICENSE
--rw-r--r--   0        0        0     1534 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/README.md
--rw-r--r--   0        0        0      611 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/__init__.py
--rw-r--r--   0        0        0      113 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/chat_models/__init__.py
--rw-r--r--   0        0        0    13294 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/chat_models/bedrock.py
--rw-r--r--   0        0        0       96 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/embeddings/__init__.py
--rw-r--r--   0        0        0     7282 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/embeddings/bedrock.py
--rw-r--r--   0        0        0      191 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/graphs/__init__.py
--rw-r--r--   0        0        0    14347 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/graphs/neptune_graph.py
--rw-r--r--   0        0        0    10331 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/graphs/neptune_rdf_graph.py
--rw-r--r--   0        0        0      297 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/llms/__init__.py
--rw-r--r--   0        0        0    31691 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/llms/bedrock.py
--rw-r--r--   0        0        0    13595 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0        0 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/py.typed
--rw-r--r--   0        0        0      251 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/retrievers/__init__.py
--rw-r--r--   0        0        0     4654 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/retrievers/bedrock.py
--rw-r--r--   0        0        0    15189 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/retrievers/kendra.py
--rw-r--r--   0        0        0     1033 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/langchain_aws/utils.py
--rw-r--r--   0        0        0     2737 2024-04-26 04:22:59.402325 langchain_aws-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2377 1970-01-01 00:00:00.000000 langchain_aws-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1537 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/README.md
+-rw-r--r--   0        0        0      611 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/chat_models/__init__.py
+-rw-r--r--   0        0        0    15869 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/chat_models/bedrock.py
+-rw-r--r--   0        0        0       96 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/embeddings/__init__.py
+-rw-r--r--   0        0        0     7282 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/embeddings/bedrock.py
+-rw-r--r--   0        0        0     3808 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/function_calling.py
+-rw-r--r--   0        0        0      191 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/graphs/__init__.py
+-rw-r--r--   0        0        0    14347 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/graphs/neptune_graph.py
+-rw-r--r--   0        0        0    10331 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/graphs/neptune_rdf_graph.py
+-rw-r--r--   0        0        0      297 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/llms/__init__.py
+-rw-r--r--   0        0        0    31761 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/llms/bedrock.py
+-rw-r--r--   0        0        0    13595 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0        0 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/py.typed
+-rw-r--r--   0        0        0      251 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/retrievers/__init__.py
+-rw-r--r--   0        0        0     4745 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/retrievers/bedrock.py
+-rw-r--r--   0        0        0    15189 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/retrievers/kendra.py
+-rw-r--r--   0        0        0     1033 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/utils.py
+-rw-r--r--   0        0        0     2737 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 langchain_aws-0.1.3/PKG-INFO
```

### Comparing `langchain_aws-0.1.2/LICENSE` & `langchain_aws-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.2/README.md` & `langchain_aws-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,19 +50,19 @@
 retriever = AmazonKendraRetriever(
     index_id="561be2b6d-9804c7e7-f6a0fbb8-5ccd350"
 )
 
 retriever.get_relevant_documents(query="What is the meaning of life?")
 ```
 
-`AmazonKnowlegeBasesRetriever` class provides a retriever to connect with Amazon Knowlege Bases.
+`AmazonKnowledgeBasesRetriever` class provides a retriever to connect with Amazon Knowledge Bases.
 
 ```python
 from langchain_aws import AmazonKnowledgeBasesRetriever
 
 retriever = AmazonKnowledgeBasesRetriever(
     knowledge_base_id="IAPJ4QPUEU",
     retrieval_config={"vectorSearchConfiguration": {"numberOfResults": 4}},
 )
 
 retriever.get_relevant_documents(query="What is the meaning of life?")
-```
+```
```

### Comparing `langchain_aws-0.1.2/langchain_aws/__init__.py` & `langchain_aws-0.1.3/langchain_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.2/langchain_aws/chat_models/bedrock.py` & `langchain_aws-0.1.3/langchain_aws/chat_models/bedrock.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 import re
 from collections import defaultdict
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Union, cast
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 from langchain_core._api.deprecation import deprecated
 from langchain_core.callbacks import (
     CallbackManagerForLLMRun,
 )
+from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import BaseChatModel
 from langchain_core.messages import (
     AIMessage,
     AIMessageChunk,
     BaseMessage,
     ChatMessage,
     HumanMessage,
     SystemMessage,
 )
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
-from langchain_core.pydantic_v1 import Extra
+from langchain_core.pydantic_v1 import BaseModel, Extra
+from langchain_core.runnables import Runnable
+from langchain_core.tools import BaseTool
 
+from langchain_aws.function_calling import convert_to_anthropic_tool, get_system_message
 from langchain_aws.llms.bedrock import BedrockBase
 from langchain_aws.utils import (
     get_num_tokens_anthropic,
     get_token_ids_anthropic,
 )
 
 
@@ -260,14 +277,16 @@
 
 _message_type_lookups = {"human": "user", "ai": "assistant"}
 
 
 class ChatBedrock(BaseChatModel, BedrockBase):
     """A chat model that uses the Bedrock API."""
 
+    system_prompt_with_tools: str = ""
+
     @property
     def _llm_type(self) -> str:
         """Return type of chat model."""
         return "amazon_bedrock_chat"
 
     @classmethod
     def is_lc_serializable(cls) -> bool:
@@ -303,14 +322,19 @@
         provider = self._get_provider()
         prompt, system, formatted_messages = None, None, None
 
         if provider == "anthropic":
             system, formatted_messages = ChatPromptAdapter.format_messages(
                 provider, messages
             )
+            if self.system_prompt_with_tools:
+                if system:
+                    system = self.system_prompt_with_tools + f"\n{system}"
+                else:
+                    system = self.system_prompt_with_tools
         else:
             prompt = ChatPromptAdapter.convert_messages_to_prompt(
                 provider=provider, messages=messages
             )
 
         for chunk in self._prepare_input_and_invoke_stream(
             prompt=prompt,
@@ -341,14 +365,19 @@
             prompt, system, formatted_messages = None, None, None
             params: Dict[str, Any] = {**kwargs}
 
             if provider == "anthropic":
                 system, formatted_messages = ChatPromptAdapter.format_messages(
                     provider, messages
                 )
+                if self.system_prompt_with_tools:
+                    if system:
+                        system = self.system_prompt_with_tools + f"\n{system}"
+                    else:
+                        system = self.system_prompt_with_tools
             else:
                 prompt = ChatPromptAdapter.convert_messages_to_prompt(
                     provider=provider, messages=messages
                 )
 
             if stop:
                 params["stop_sequences"] = stop
@@ -395,11 +424,47 @@
 
     def get_token_ids(self, text: str) -> List[int]:
         if self._model_is_anthropic:
             return get_token_ids_anthropic(text)
         else:
             return super().get_token_ids(text)
 
+    def set_system_prompt_with_tools(self, xml_tools_system_prompt: str) -> None:
+        """Workaround to bind. Sets the system prompt with tools"""
+        self.system_prompt_with_tools = xml_tools_system_prompt
+
+    def bind_tools(
+        self,
+        tools: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable, BaseTool]],
+        *,
+        tool_choice: Optional[Union[dict, str, Literal["auto", "none"], bool]] = None,
+        **kwargs: Any,
+    ) -> Runnable[LanguageModelInput, BaseMessage]:
+        """Bind tool-like objects to this chat model.
+
+        Assumes model has a tool calling API.
+
+        Args:
+            tools: A list of tool definitions to bind to this chat model.
+                Can be  a dictionary, pydantic model, callable, or BaseTool. Pydantic
+                models, callables, and BaseTools will be automatically converted to
+                their schema dictionary representation.
+            tool_choice: Which tool to require the model to call.
+                Must be the name of the single provided function or
+                "auto" to automatically determine which function to call
+                (if any), or a dict of the form:
+                {"type": "function", "function": {"name": <<tool_name>>}}.
+            **kwargs: Any additional parameters to pass to the
+                :class:`~langchain.runnable.Runnable` constructor.
+        """
+        provider = self._get_provider()
+
+        if provider == "anthropic":
+            formatted_tools = [convert_to_anthropic_tool(tool) for tool in tools]
+            system_formatted_tools = get_system_message(formatted_tools)
+            self.set_system_prompt_with_tools(system_formatted_tools)
+        return self
+
 
 @deprecated(since="0.1.0", removal="0.2.0", alternative="ChatBedrock")
 class BedrockChat(ChatBedrock):
     pass
```

### Comparing `langchain_aws-0.1.2/langchain_aws/embeddings/bedrock.py` & `langchain_aws-0.1.3/langchain_aws/embeddings/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.2/langchain_aws/graphs/neptune_graph.py` & `langchain_aws-0.1.3/langchain_aws/graphs/neptune_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.2/langchain_aws/graphs/neptune_rdf_graph.py` & `langchain_aws-0.1.3/langchain_aws/graphs/neptune_rdf_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.2/langchain_aws/llms/bedrock.py` & `langchain_aws-0.1.3/langchain_aws/llms/bedrock.py`

 * *Files 4% similar despite different names*

```diff
@@ -339,17 +339,17 @@
         "amazon": "stopSequences",
         "ai21": "stop_sequences",
         "cohere": "stop_sequences",
         "mistral": "stop_sequences",
     }
 
     guardrails: Optional[Mapping[str, Any]] = {
-        "id": None,
-        "version": None,
-        "trace": False,
+        "trace": None,
+        "guardrailIdentifier": None,
+        "guardrailVersion": None,
     }
     """
     An optional dictionary to configure guardrails for Bedrock.
 
     This field 'guardrails' consists of two keys: 'id' and 'version',
     which should be strings, but are initialized to None. It's used to
     determine if specific guardrails are enabled and properly set.
@@ -442,15 +442,17 @@
     @property
     def _identifying_params(self) -> Dict[str, Any]:
         _model_kwargs = self.model_kwargs or {}
         return {
             "model_id": self.model_id,
             "provider": self._get_provider(),
             "stream": self.streaming,
-            "guardrails": self.guardrails,
+            "trace": self.guardrails.get("trace"),  # type: ignore[union-attr]
+            "guardrailIdentifier": self.guardrails.get("guardrailIdentifier", None),  # type: ignore[union-attr]
+            "guardrailVersion": self.guardrails.get("guardrailVersion", None),  # type: ignore[union-attr]
             **_model_kwargs,
         }
 
     def _get_provider(self) -> str:
         if self.provider:
             return self.provider
         if self.model_id.startswith("arn"):
@@ -476,55 +478,38 @@
             bool: True if guardrails are correctly configured, False otherwise.
         Raises:
             TypeError: If 'guardrails' lacks 'id' or 'version' keys.
         """
         try:
             return (
                 isinstance(self.guardrails, dict)
-                and bool(self.guardrails["id"])
-                and bool(self.guardrails["version"])
+                and bool(self.guardrails["guardrailIdentifier"])
+                and bool(self.guardrails["guardrailVersion"])
             )
 
         except KeyError as e:
             raise TypeError(
-                "Guardrails must be a dictionary with 'id' and 'version' keys."
+                "Guardrails must be a dictionary with 'guardrailIdentifier'  \
+                and 'guardrailVersion' keys."
             ) from e
 
-    def _get_guardrails_canonical(self) -> Dict[str, Any]:
-        """
-        The canonical way to pass in guardrails to the bedrock service
-        adheres to the following format:
-
-        "amazon-bedrock-guardrailDetails": {
-            "guardrailId": "string",
-            "guardrailVersion": "string"
-        }
-        """
-        return {
-            "amazon-bedrock-guardrailDetails": {
-                "guardrailId": self.guardrails.get("id"),  # type: ignore[union-attr]
-                "guardrailVersion": self.guardrails.get("version"),  # type: ignore[union-attr]
-            }
-        }
-
     def _prepare_input_and_invoke(
         self,
         prompt: Optional[str] = None,
         system: Optional[str] = None,
         messages: Optional[List[Dict]] = None,
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> Tuple[str, Dict[str, Any]]:
         _model_kwargs = self.model_kwargs or {}
 
         provider = self._get_provider()
         params = {**_model_kwargs, **kwargs}
-        if self._guardrails_enabled:
-            params.update(self._get_guardrails_canonical())
+
         input_body = LLMInputOutputAdapter.prepare_input(
             provider=provider,
             model_kwargs=params,
             prompt=prompt,
             system=system,
             messages=messages,
         )
@@ -536,15 +521,20 @@
             "body": body,
             "modelId": self.model_id,
             "accept": accept,
             "contentType": contentType,
         }
 
         if self._guardrails_enabled:
-            request_options["guardrail"] = "ENABLED"
+            request_options["guardrailIdentifier"] = self.guardrails.get(  # type: ignore[union-attr]
+                "guardrailIdentifier", ""
+            )
+            request_options["guardrailVersion"] = self.guardrails.get(  # type: ignore[union-attr]
+                "guardrailVersion", ""
+            )
             if self.guardrails.get("trace"):  # type: ignore[union-attr]
                 request_options["trace"] = "ENABLED"
 
         try:
             response = self.client.invoke_model(**request_options)
 
             text, body, usage_info = LLMInputOutputAdapter.prepare_output(
@@ -624,17 +614,14 @@
                 _model_kwargs[k] = stop
 
         if provider == "cohere":
             _model_kwargs["stream"] = True
 
         params = {**_model_kwargs, **kwargs}
 
-        if self._guardrails_enabled:
-            params.update(self._get_guardrails_canonical())
-
         input_body = LLMInputOutputAdapter.prepare_input(
             provider=provider,
             prompt=prompt,
             system=system,
             messages=messages,
             model_kwargs=params,
         )
@@ -644,15 +631,20 @@
             "body": body,
             "modelId": self.model_id,
             "accept": "application/json",
             "contentType": "application/json",
         }
 
         if self._guardrails_enabled:
-            request_options["guardrail"] = "ENABLED"
+            request_options["guardrailIdentifier"] = self.guardrails.get(  # type: ignore[union-attr]
+                "guardrailIdentifier", ""
+            )
+            request_options["guardrailVersion"] = self.guardrails.get(  # type: ignore[union-attr]
+                "guardrailVersion", ""
+            )
             if self.guardrails.get("trace"):  # type: ignore[union-attr]
                 request_options["trace"] = "ENABLED"
 
         try:
             response = self.client.invoke_model_with_response_stream(**request_options)
 
         except Exception as e:
```

### Comparing `langchain_aws-0.1.2/langchain_aws/llms/sagemaker_endpoint.py` & `langchain_aws-0.1.3/langchain_aws/llms/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.2/langchain_aws/retrievers/bedrock.py` & `langchain_aws-0.1.3/langchain_aws/retrievers/bedrock.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,18 +110,21 @@
             retrievalQuery={"text": query.strip()},
             knowledgeBaseId=self.knowledge_base_id,
             retrievalConfiguration=self.retrieval_config.dict(),
         )
         results = response["retrievalResults"]
         documents = []
         for result in results:
+            content = result["content"]["text"]
+            result.pop("content")
+            if "score" not in result:
+                result["score"] = 0
+            if "metadata" in result:
+                result["source_metadata"] = result.pop("metadata")
             documents.append(
                 Document(
-                    page_content=result["content"]["text"],
-                    metadata={
-                        "location": result["location"],
-                        "score": result["score"] if "score" in result else 0,
-                    },
+                    page_content=content,
+                    metadata=result,
                 )
             )
 
         return documents
```

### Comparing `langchain_aws-0.1.2/langchain_aws/retrievers/kendra.py` & `langchain_aws-0.1.3/langchain_aws/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.2/langchain_aws/utils.py` & `langchain_aws-0.1.3/langchain_aws/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.2/pyproject.toml` & `langchain_aws-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-aws"
-version = "0.1.2"
+version = "0.1.3"
 description = "An integration package connecting AWS and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-aws"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_aws-0.1.2/PKG-INFO` & `langchain_aws-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-aws
-Version: 0.1.2
+Version: 0.1.3
 Summary: An integration package connecting AWS and LangChain
 Home-page: https://github.com/langchain-ai/langchain-aws
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -70,19 +70,20 @@
 retriever = AmazonKendraRetriever(
     index_id="561be2b6d-9804c7e7-f6a0fbb8-5ccd350"
 )
 
 retriever.get_relevant_documents(query="What is the meaning of life?")
 ```
 
-`AmazonKnowlegeBasesRetriever` class provides a retriever to connect with Amazon Knowlege Bases.
+`AmazonKnowledgeBasesRetriever` class provides a retriever to connect with Amazon Knowledge Bases.
 
 ```python
 from langchain_aws import AmazonKnowledgeBasesRetriever
 
 retriever = AmazonKnowledgeBasesRetriever(
     knowledge_base_id="IAPJ4QPUEU",
     retrieval_config={"vectorSearchConfiguration": {"numberOfResults": 4}},
 )
 
 retriever.get_relevant_documents(query="What is the meaning of life?")
 ```
+
```

