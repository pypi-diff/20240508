# Comparing `tmp/llama_index_llms_azure_openai-0.1.7.tar.gz` & `tmp/llama_index_llms_azure_openai-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_azure_openai-0.1.7.tar", max compression
+gzip compressed data, was "llama_index_llms_azure_openai-0.1.8.tar", max compression
```

## Comparing `llama_index_llms_azure_openai-0.1.7.tar` & `llama_index_llms_azure_openai-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       44 2024-05-05 13:46:03.974164 llama_index_llms_azure_openai-0.1.7/README.md
--rw-r--r--   0        0        0      177 2024-05-05 13:46:03.974164 llama_index_llms_azure_openai-0.1.7/llama_index/llms/azure_openai/__init__.py
--rw-r--r--   0        0        0     8395 2024-05-05 13:46:03.974164 llama_index_llms_azure_openai-0.1.7/llama_index/llms/azure_openai/base.py
--rw-r--r--   0        0        0     1245 2024-05-05 13:46:03.974164 llama_index_llms_azure_openai-0.1.7/llama_index/llms/azure_openai/utils.py
--rw-r--r--   0        0        0     1590 2024-05-05 13:46:03.974164 llama_index_llms_azure_openai-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 llama_index_llms_azure_openai-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-05-08 21:16:17.153035 llama_index_llms_azure_openai-0.1.8/README.md
+-rw-r--r--   0        0        0      177 2024-05-08 21:16:17.153035 llama_index_llms_azure_openai-0.1.8/llama_index/llms/azure_openai/__init__.py
+-rw-r--r--   0        0        0     8586 2024-05-08 21:16:17.153035 llama_index_llms_azure_openai-0.1.8/llama_index/llms/azure_openai/base.py
+-rw-r--r--   0        0        0     1245 2024-05-08 21:16:17.153035 llama_index_llms_azure_openai-0.1.8/llama_index/llms/azure_openai/utils.py
+-rw-r--r--   0        0        0     1590 2024-05-08 21:16:17.153035 llama_index_llms_azure_openai-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 llama_index_llms_azure_openai-0.1.8/PKG-INFO
```

### Comparing `llama_index_llms_azure_openai-0.1.7/llama_index/llms/azure_openai/base.py` & `llama_index_llms_azure_openai-0.1.8/llama_index/llms/azure_openai/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         callback_manager: Optional[CallbackManager] = None,
         # aliases for engine
         deployment_name: Optional[str] = None,
         deployment_id: Optional[str] = None,
         deployment: Optional[str] = None,
         # custom httpx client
         http_client: Optional[httpx.Client] = None,
+        async_http_client: Optional[httpx.AsyncClient] = None,
         # base class
         system_prompt: Optional[str] = None,
         messages_to_prompt: Optional[Callable[[Sequence[ChatMessage]], str]] = None,
         completion_to_prompt: Optional[Callable[[str], str]] = None,
         pydantic_program_mode: PydanticProgramMode = PydanticProgramMode.DEFAULT,
         output_parser: Optional[BaseOutputParser] = None,
         **kwargs: Any,
@@ -134,14 +135,15 @@
             azure_endpoint=azure_endpoint,
             azure_deployment=azure_deployment,
             azure_ad_token_provider=azure_ad_token_provider,
             use_azure_ad=use_azure_ad,
             api_version=api_version,
             callback_manager=callback_manager,
             http_client=http_client,
+            async_http_client=async_http_client,
             system_prompt=system_prompt,
             messages_to_prompt=messages_to_prompt,
             completion_to_prompt=completion_to_prompt,
             pydantic_program_mode=pydantic_program_mode,
             output_parser=output_parser,
             **kwargs,
         )
@@ -178,15 +180,17 @@
 
         if self._aclient is None:
             self._aclient = AsyncAzureOpenAI(
                 **self._get_credential_kwargs(),
             )
         return self._aclient
 
-    def _get_credential_kwargs(self, **kwargs: Any) -> Dict[str, Any]:
+    def _get_credential_kwargs(
+        self, is_async: bool = False, **kwargs: Any
+    ) -> Dict[str, Any]:
         if self.use_azure_ad:
             self._azure_ad_token = refresh_openai_azuread_token(self._azure_ad_token)
             self.api_key = self._azure_ad_token.token
         else:
             import os
 
             self.api_key = self.api_key or os.getenv("AZURE_OPENAI_API_KEY")
@@ -202,15 +206,15 @@
             "max_retries": self.max_retries,
             "timeout": self.timeout,
             "azure_endpoint": self.azure_endpoint,
             "azure_deployment": self.azure_deployment,
             "azure_ad_token_provider": self.azure_ad_token_provider,
             "api_version": self.api_version,
             "default_headers": self.default_headers,
-            "http_client": self._http_client,
+            "http_client": self._async_http_client if is_async else self._http_client,
             **kwargs,
         }
 
     def _get_model_kwargs(self, **kwargs: Any) -> Dict[str, Any]:
         model_kwargs = super()._get_model_kwargs(**kwargs)
         model_kwargs["model"] = self.engine
         return model_kwargs
```

### Comparing `llama_index_llms_azure_openai-0.1.7/llama_index/llms/azure_openai/utils.py` & `llama_index_llms_azure_openai-0.1.8/llama_index/llms/azure_openai/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_azure_openai-0.1.7/pyproject.toml` & `llama_index_llms_azure_openai-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms azure openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-azure-openai"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.11.post1"
 llama-index-llms-openai = "^0.1.1"
 azure-identity = "^1.15.0"
 httpx = "*"
```

### Comparing `llama_index_llms_azure_openai-0.1.7/PKG-INFO` & `llama_index_llms_azure_openai-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-azure-openai
-Version: 0.1.7
+Version: 0.1.8
 Summary: llama-index llms azure openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

