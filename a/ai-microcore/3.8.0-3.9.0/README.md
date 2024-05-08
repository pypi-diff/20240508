# Comparing `tmp/ai_microcore-3.8.0.tar.gz` & `tmp/ai_microcore-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_microcore-3.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ai_microcore-3.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ai_microcore-3.8.0.tar` & `ai_microcore-3.9.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.8.0/LICENSE
--rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.8.0/README.md
--rwxr-xr-x   0        0        0     3985 2024-04-27 13:13:12.779924 ai_microcore-3.8.0/microcore/__init__.py
--rwxr-xr-x   0        0        0     6975 2024-04-27 13:16:13.007972 ai_microcore-3.8.0/microcore/_env.py
--rwxr-xr-x   0        0        0     3790 2024-04-20 15:07:06.612137 ai_microcore-3.8.0/microcore/_llm_functions.py
--rwxr-xr-x   0        0        0      881 2024-04-26 20:19:54.634711 ai_microcore-3.8.0/microcore/_prepare_llm_args.py
--rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.8.0/microcore/ai_func/__init__.py
--rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.8.0/microcore/ai_func/python_ai_func.j2
--rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.8.0/microcore/ai_modules.py
--rwxr-xr-x   0        0        0    12344 2024-04-26 20:20:57.360040 ai_microcore-3.8.0/microcore/configuration.py
--rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.8.0/microcore/embedding_db/__init__.py
--rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.8.0/microcore/embedding_db/chromadb.py
--rwxr-xr-x   0        0        0     8400 2024-04-23 02:00:56.476715 ai_microcore-3.8.0/microcore/file_storage.py
--rwxr-xr-x   0        0        0     4725 2024-04-27 13:16:12.983942 ai_microcore-3.8.0/microcore/json_parsing.py
--rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.8.0/microcore/llm/__init__.py
--rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.8.0/microcore/llm/_openai_llm_v0.py
--rwxr-xr-x   0        0        0     5120 2024-04-18 17:18:22.746984 ai_microcore-3.8.0/microcore/llm/_openai_llm_v1.py
--rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.8.0/microcore/llm/anthropic.py
--rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.8.0/microcore/llm/google_genai.py
--rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.8.0/microcore/llm/google_vertex_ai.py
--rwxr-xr-x   0        0        0     3413 2024-04-23 17:22:46.408066 ai_microcore-3.8.0/microcore/llm/local_llm.py
--rwxr-xr-x   0        0        0     9811 2024-04-27 13:16:13.038509 ai_microcore-3.8.0/microcore/llm/local_transformers.py
--rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.8.0/microcore/llm/openai_llm.py
--rwxr-xr-x   0        0        0     2490 2024-04-22 18:59:09.500665 ai_microcore-3.8.0/microcore/logging.py
--rwxr-xr-x   0        0        0     1669 2024-04-26 20:21:12.539912 ai_microcore-3.8.0/microcore/message_types.py
--rwxr-xr-x   0        0        0     2224 2024-04-27 13:15:46.358788 ai_microcore-3.8.0/microcore/python.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.8.0/microcore/templating/__init__.py
--rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.8.0/microcore/templating/jinja2.py
--rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.8.0/microcore/text2speech/elevenlabs.py
--rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.8.0/microcore/types.py
--rwxr-xr-x   0        0        0     1601 2024-04-19 09:12:25.103139 ai_microcore-3.8.0/microcore/ui.py
--rwxr-xr-x   0        0        0     9089 2024-04-21 17:42:07.690371 ai_microcore-3.8.0/microcore/utils.py
--rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.8.0/microcore/wrappers/__init__.py
--rwxr-xr-x   0        0        0     1559 2024-04-18 13:05:21.831255 ai_microcore-3.8.0/microcore/wrappers/llm_response_wrapper.py
--rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.8.0/microcore/wrappers/prompt_wrapper.py
--rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.8.0/pyproject.toml
--rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.8.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1091 2023-11-04 16:00:47.197704 ai_microcore-3.9.0/LICENSE
+-rwxr-xr-x   0        0        0    11116 2024-04-04 12:54:33.488412 ai_microcore-3.9.0/README.md
+-rwxr-xr-x   0        0        0     4031 2024-05-03 14:28:24.778623 ai_microcore-3.9.0/microcore/__init__.py
+-rwxr-xr-x   0        0        0     7238 2024-05-08 15:10:19.371147 ai_microcore-3.9.0/microcore/_env.py
+-rwxr-xr-x   0        0        0     3790 2024-04-20 15:07:06.612137 ai_microcore-3.9.0/microcore/_llm_functions.py
+-rwxr-xr-x   0        0        0      881 2024-04-26 20:19:54.634711 ai_microcore-3.9.0/microcore/_prepare_llm_args.py
+-rwxr-xr-x   0        0        0     2319 2024-03-08 00:49:48.900573 ai_microcore-3.9.0/microcore/ai_func/__init__.py
+-rwxr-xr-x   0        0        0      314 2023-11-04 16:00:47.368478 ai_microcore-3.9.0/microcore/ai_func/python_ai_func.j2
+-rwxr-xr-x   0        0        0      576 2023-11-04 19:26:33.244252 ai_microcore-3.9.0/microcore/ai_modules.py
+-rwxr-xr-x   0        0        0    13670 2024-05-08 15:15:14.884497 ai_microcore-3.9.0/microcore/configuration.py
+-rwxr-xr-x   0        0        0     3133 2024-02-15 20:01:36.859722 ai_microcore-3.9.0/microcore/embedding_db/__init__.py
+-rwxr-xr-x   0        0        0     4565 2024-02-15 19:46:15.503154 ai_microcore-3.9.0/microcore/embedding_db/chromadb.py
+-rwxr-xr-x   0        0        0     8400 2024-04-23 02:00:56.476715 ai_microcore-3.9.0/microcore/file_storage.py
+-rwxr-xr-x   0        0        0     4725 2024-05-08 10:50:08.347413 ai_microcore-3.9.0/microcore/json_parsing.py
+-rwxr-xr-x   0        0        0       16 2023-11-06 23:41:28.213361 ai_microcore-3.9.0/microcore/llm/__init__.py
+-rwxr-xr-x   0        0        0     4708 2024-04-16 08:56:56.272317 ai_microcore-3.9.0/microcore/llm/_openai_llm_v0.py
+-rwxr-xr-x   0        0        0     5431 2024-05-08 10:48:21.052687 ai_microcore-3.9.0/microcore/llm/_openai_llm_v1.py
+-rwxr-xr-x   0        0        0     3655 2024-04-16 13:59:52.503374 ai_microcore-3.9.0/microcore/llm/anthropic.py
+-rwxr-xr-x   0        0        0     4479 2024-04-16 09:04:29.151454 ai_microcore-3.9.0/microcore/llm/google_genai.py
+-rwxr-xr-x   0        0        0     5801 2024-04-18 13:00:32.311278 ai_microcore-3.9.0/microcore/llm/google_vertex_ai.py
+-rwxr-xr-x   0        0        0     3540 2024-05-08 13:59:27.874473 ai_microcore-3.9.0/microcore/llm/local_llm.py
+-rwxr-xr-x   0        0        0    10203 2024-05-08 10:48:21.122263 ai_microcore-3.9.0/microcore/llm/local_transformers.py
+-rwxr-xr-x   0        0        0      272 2023-11-06 23:49:42.323932 ai_microcore-3.9.0/microcore/llm/openai_llm.py
+-rwxr-xr-x   0        0        0     2490 2024-04-22 18:59:09.500665 ai_microcore-3.9.0/microcore/logging.py
+-rwxr-xr-x   0        0        0     1669 2024-04-26 20:21:12.539912 ai_microcore-3.9.0/microcore/message_types.py
+-rwxr-xr-x   0        0        0     1520 2024-05-08 10:54:21.110757 ai_microcore-3.9.0/microcore/metrics.py
+-rwxr-xr-x   0        0        0     2309 2024-05-08 10:48:21.029687 ai_microcore-3.9.0/microcore/python.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.559200 ai_microcore-3.9.0/microcore/templating/__init__.py
+-rwxr-xr-x   0        0        0      525 2023-11-12 15:43:10.028753 ai_microcore-3.9.0/microcore/templating/jinja2.py
+-rwxr-xr-x   0        0        0     1455 2024-03-31 01:09:15.566074 ai_microcore-3.9.0/microcore/text2speech/elevenlabs.py
+-rwxr-xr-x   0        0        0     1046 2024-03-11 12:20:49.086082 ai_microcore-3.9.0/microcore/types.py
+-rwxr-xr-x   0        0        0     1601 2024-04-19 09:12:25.103139 ai_microcore-3.9.0/microcore/ui.py
+-rwxr-xr-x   0        0        0    10403 2024-05-08 14:47:04.871718 ai_microcore-3.9.0/microcore/utils.py
+-rwxr-xr-x   0        0        0        0 2023-11-04 16:00:47.618937 ai_microcore-3.9.0/microcore/wrappers/__init__.py
+-rwxr-xr-x   0        0        0     1630 2024-05-08 10:48:07.210529 ai_microcore-3.9.0/microcore/wrappers/llm_response_wrapper.py
+-rwxr-xr-x   0        0        0      480 2024-04-02 14:01:24.033112 ai_microcore-3.9.0/microcore/wrappers/prompt_wrapper.py
+-rwxr-xr-x   0        0        0     1450 2024-04-18 14:27:33.934530 ai_microcore-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11811 1970-01-01 00:00:00.000000 ai_microcore-3.9.0/PKG-INFO
```

### Comparing `ai_microcore-3.8.0/LICENSE` & `ai_microcore-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/README.md` & `ai_microcore-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/__init__.py` & `ai_microcore-3.9.0/microcore/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .message_types import UserMsg, AssistantMsg, SysMsg, Msg, PartialMsg
 from .configuration import ApiType, LLMConfigError, Config
 from .types import BadAIJsonAnswer, BadAIAnswer
 from .wrappers.prompt_wrapper import PromptWrapper
 from .wrappers.llm_response_wrapper import LLMResponse
 from ._llm_functions import llm, allm, llm_parallel
 from .utils import parse, dedent
+from .metrics import Metrics
 
 
 def tpl(file: os.PathLike[str] | str, **kwargs) -> str | PromptWrapper:
     """Renders a prompt template using the provided parameters."""
     return PromptWrapper(env().tpl_function(file, **kwargs), kwargs)
 
 
@@ -133,11 +134,12 @@
     "file_storage",
     "message_types",
     "utils",
     "configuration",
     "Config",
     "types",
     "ui",
+    "Metrics",
     # "wrappers",
 ]
 
-__version__ = "3.8.0"
+__version__ = "3.9.0"
```

### Comparing `ai_microcore-3.8.0/microcore/_env.py` & `ai_microcore-3.9.0/microcore/_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os.path
 from dataclasses import dataclass, field, asdict, fields
 from importlib.util import find_spec
 import jinja2
 
 from .configuration import Config, ApiType, LLMConfigError
 from . import AbstractEmbeddingDB
 from .types import TplFunctionType, LLMAsyncFunctionType, LLMFunctionType
@@ -145,24 +146,28 @@
 """Applies configuration to MicroCore environment"""
 
 if True:  # pylint: disable=W0125
     # This block is inside a condition to avoid breaking IDE autocompletion
 
     _fields = list(map(lambda f: f.name, fields(Config)))
 
-    def _config_builder_wrapper(cfg: Config | dict = None, **kwargs):
+    def _config_builder_wrapper(cfg: Config | dict | str = None, **kwargs):
         """
         - Convert configuration keys to uppercase
         - Add LLM_ prefix to keys if necessary
         - Allow to configure from Config instance or dictionary
         """
         if cfg:
             assert not kwargs, "Cannot pass both cfg and kwargs"
         if isinstance(cfg, dict):
             return _config_builder_wrapper(**cfg)
+        if isinstance(cfg, str):
+            if not os.path.isfile(cfg):
+                raise LLMConfigError(f"Configuration file not found: {cfg}")
+            return _config_builder_wrapper(Config(USE_DOT_ENV=True, DOT_ENV_FILE=cfg))
         kwargs = {str(k).upper(): v for k, v in kwargs.items()}
         for k in list(kwargs.keys()):
             if not hasattr(Config, k) and (
                 hasattr(Config, key := f"LLM_{k}") or key in _fields
             ):
                 kwargs[key] = kwargs.pop(k)
         return _Configure(**(cfg and asdict(cfg) or kwargs))
```

### Comparing `ai_microcore-3.8.0/microcore/_llm_functions.py` & `ai_microcore-3.9.0/microcore/_llm_functions.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/_prepare_llm_args.py` & `ai_microcore-3.9.0/microcore/_prepare_llm_args.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/ai_func/__init__.py` & `ai_microcore-3.9.0/microcore/ai_func/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/ai_modules.py` & `ai_microcore-3.9.0/microcore/ai_modules.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/configuration.py` & `ai_microcore-3.9.0/microcore/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,65 @@
+import json
 import logging
 import os
 from dataclasses import dataclass, field, fields
 from pathlib import Path
-from typing import Any
-from typing import Union, Callable
+from typing import Any, Union, Callable
 
 import dotenv
 from colorama import Fore
 
 _MISSING = object()
 
 TRUE_VALUES = ["1", "TRUE", "YES", "ON", "ENABLED", "Y", "+"]
 """@private"""
 
 
-def from_env(default=None):
+def from_env(default=None, dtype=None):
     """
     Provides default value for the configuration dataclass
     from the environment variable with the name equal to field name in upper case"""
-    return field(default=_MISSING, metadata=dict(_from_env=True, _default=default))
+    return field(
+        default=_MISSING, metadata=dict(_from_env=True, _default=default, _dtype=dtype)
+    )
 
 
-def get_bool_from_env(env_var: str, default: bool = False) -> bool:
+def get_bool_from_env(env_var: str, default: bool | None = False) -> bool | None:
     """Convert value of environment variable to boolean"""
+    if env_var not in os.environ:
+        return default
     return os.getenv(env_var, str(default)).upper() in TRUE_VALUES
 
 
+def get_object_from_env(env_var: str, dtype: type, default: Any = None):
+    val_from_env = os.getenv(
+        env_var, _MISSING
+    )  # pylint: disable=invalid-envvar-default
+    if isinstance(val_from_env, str):
+        val_from_env = val_from_env.strip()
+        if val_from_env:
+            try:
+                val_from_env = json.loads(val_from_env.strip())
+                assert isinstance(
+                    val_from_env, dtype
+                ), f"Expected {dtype.__name__}, got {type(val_from_env).__name__}"
+            except (json.JSONDecodeError, AssertionError) as e:
+                raise LLMConfigError(
+                    f"Invalid value in environment variable '{env_var}'. "
+                    f"Expected: JSON {dtype.__name__}, received: '{val_from_env}'"
+                ) from e
+        else:
+            val_from_env = _MISSING
+    if val_from_env is _MISSING:
+        if default is None:  # instead of default factory
+            default = dtype()
+        val_from_env = default
+    return val_from_env
+
+
 class ApiType:
     """LLM API types"""
 
     OPEN_AI = "open_ai"
     AZURE = "azure"
     """See https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/models"""
     ANYSCALE = "anyscale"
@@ -75,15 +105,25 @@
                 dotenv.load_dotenv(override=True, dotenv_path=self.DOT_ENV_FILE)
             if not self.DOT_ENV_FILE:
                 _default_dotenv_loaded = True
 
     def _update_from_env(self):
         for f in fields(self):
             if f.metadata.get("_from_env") and getattr(self, f.name) is _MISSING:
-                setattr(self, f.name, os.getenv(f.name.upper(), f.metadata["_default"]))
+                env_name = f.name.upper()
+                default = f.metadata["_default"]
+                dtype = f.metadata.get("_dtype")
+                if dtype is bool:
+                    val_from_env = get_bool_from_env(env_name, default)
+                elif dtype in [dict, list]:
+                    val_from_env = get_object_from_env(env_name, dtype, default)
+                else:
+                    val_from_env = os.getenv(env_name, default)
+
+                setattr(self, f.name, val_from_env)
 
     def __iter__(self):
         for f in fields(self):
             value = getattr(self, f.name)
             yield f.name, value
 
 
@@ -104,18 +144,18 @@
 
 
 @dataclass
 class _GoogleVertexAiEnvVars:
     GOOGLE_VERTEX_ACCESS_TOKEN: str = from_env()
     GOOGLE_VERTEX_PROJECT_ID: str = from_env()
     GOOGLE_VERTEX_LOCATION: str = from_env()
-    GOOGLE_VERTEX_GCLOUD_AUTH: bool = None
+    GOOGLE_VERTEX_GCLOUD_AUTH: bool = from_env(dtype=bool)
 
-    GOOGLE_VERTEX_RESPONSE_VALIDATION: bool = None
-    GOOGLE_GEMINI_SAFETY_SETTINGS: dict = None
+    GOOGLE_VERTEX_RESPONSE_VALIDATION: bool = from_env(dtype=bool, default=False)
+    GOOGLE_GEMINI_SAFETY_SETTINGS: dict = from_env(dtype=dict)
 
 
 @dataclass
 class LLMConfig(BaseConfig, _OpenAIEnvVars, _AnthropicEnvVars, _GoogleVertexAiEnvVars):
     """LLM configuration"""
 
     LLM_API_TYPE: str = from_env()
@@ -131,27 +171,27 @@
     LLM_API_VERSION: str = from_env()
     LLM_DEPLOYMENT_ID: str = from_env()
     """Required by `ApiType.AZURE`"""
 
     MODEL: str = from_env()
     """Language model name"""
 
-    LLM_DEFAULT_ARGS: dict = field(default_factory=dict)
+    LLM_DEFAULT_ARGS: dict = from_env(dtype=dict)
     """
     You may specify here default arguments for the LLM API calls,
      i. e. temperature, max_tokens, etc.
      """
 
     AZURE_DEPLOYMENT_ID: str = from_env()
 
-    INFERENCE_FUNC: Union[Callable, str] = None
+    INFERENCE_FUNC: Union[Callable, str] = from_env()
     """Inference function for local models"""
-    CHAT_MODE: bool = None
+    CHAT_MODE: bool = from_env(dtype=bool)
     """Is it a chat or completion model"""
-    INIT_PARAMS: dict = field(default_factory=dict)
+    INIT_PARAMS: dict = from_env(dtype=dict)
     """Custom initialization parameters for the model"""
 
     def __post_init__(self):
         super().__post_init__()
         self._init_llm_options()
         self.validate()
 
@@ -163,18 +203,14 @@
             if not self.LLM_API_TYPE:
                 self.LLM_API_TYPE = ApiType.FUNCTION
         if self.uses_local_model():
             return
 
         # Use defaults from ENV variables expected by OpenAI API
         self.LLM_API_TYPE = self.LLM_API_TYPE or self.OPENAI_API_TYPE
-        if self.GOOGLE_VERTEX_RESPONSE_VALIDATION is None:
-            self.GOOGLE_VERTEX_RESPONSE_VALIDATION = get_bool_from_env(
-                "GOOGLE_VERTEX_RESPONSE_VALIDATION", False
-            )
 
         if self.LLM_API_TYPE == ApiType.AZURE:
             self.LLM_API_VERSION = self.LLM_API_VERSION or self.OPENAI_API_VERSION
             self.LLM_DEPLOYMENT_ID = self.LLM_DEPLOYMENT_ID or self.AZURE_DEPLOYMENT_ID
         elif self.LLM_API_TYPE == ApiType.GOOGLE_AI_STUDIO:
             self.MODEL = self.MODEL or "gemini-pro"
         elif self.LLM_API_TYPE == ApiType.GOOGLE_VERTEX_AI:
@@ -211,21 +247,14 @@
             )
         if self.LLM_API_TYPE == ApiType.FUNCTION:
             if not self.INFERENCE_FUNC:
                 raise LLMConfigError(
                     "LLM configuration error: "
                     "INFERENCE_FUNC should be provided for local models"
                 )
-            if (
-                isinstance(self.INFERENCE_FUNC, str)
-                and self.INFERENCE_FUNC not in globals()
-            ):
-                raise LLMConfigError(
-                    f"LLM configuration error: inference function '{self.INFERENCE_FUNC}' not found"
-                )
         elif self.LLM_API_TYPE == ApiType.TRANSFORMERS:
             if not self.MODEL:
                 raise LLMConfigError(
                     "LLM configuration error: "
                     "MODEL should be provided for local transformers models"
                 )
 
@@ -275,23 +304,28 @@
                         "LLM_API_VERSION is required for using Azure models"
                     )
 
     def describe(self, return_dict=False):
         """
         Informal description of the configuration
         """
+        prev_env = os.environ.copy()
+        os.environ.clear()
         default = Config(LLM_API_TYPE=ApiType.NONE, USE_DOT_ENV=False)
+        os.environ.update(prev_env)
         data = {
             k.lower().replace("llm_", ""): v
             for k, v in dict(self).items()
             if v is not None and v != getattr(default, k) and k != "USE_DOT_ENV"
         }
         for k, v in data.items():
             if "_key" in k and isinstance(v, str):
-                data[k] = v[:1] + "****" + v[-2:]
+                if len(v) <= 3:
+                    continue
+                data[k] = v[: 1 if len(v) <= 12 else 3] + "****" + v[-2:]
         if return_dict:
             return data
 
         print("Config:")
         for k, v in data.items():
             print(f"  {k}: {Fore.GREEN}{v}{Fore.RESET}")
         return None
@@ -301,43 +335,41 @@
     """LLM configuration error"""
 
 
 @dataclass
 class Config(LLMConfig):
     """MicroCore configuration"""
 
-    USE_LOGGING: bool = False
+    USE_LOGGING: bool = from_env(default=False)
     """Whether to use logging or not, see `microcore.use_logging`"""
 
     PROMPT_TEMPLATES_PATH: str | Path = from_env("tpl")
     """Path to the folder with prompt templates, ./tpl by default"""
 
     STORAGE_PATH: str | Path = from_env("storage")
     """Path to the folder with file storage, ./storage by default"""
 
-    STORAGE_DEFAULT_FILE_EXT: str = field(default="")
+    STORAGE_DEFAULT_FILE_EXT: str = from_env(default="")
 
-    EMBEDDING_DB_FOLDER: str = "embedding_db"
+    EMBEDDING_DB_FOLDER: str = from_env(default="embedding_db")
     """Folder within microcore.config.Config.STORAGE_PATH for storing embeddings"""
 
     EMBEDDING_DB_FUNCTION: Any = from_env()
 
-    EMBEDDING_DB_ALLOW_DUPLICATES: bool = False
+    EMBEDDING_DB_ALLOW_DUPLICATES: bool = from_env(dtype=bool, default=False)
 
     DEFAULT_ENCODING: str = from_env("utf-8")
     """Used in file system operations, utf-8 by default"""
 
-    JINJA2_AUTO_ESCAPE: bool = None
+    JINJA2_AUTO_ESCAPE: bool = from_env(dtype=bool, default=False)
 
     ELEVENLABS_API_KEY: str = from_env()
 
     TEXT_TO_SPEECH_PATH: str | Path = from_env()
     """Path to the folder with generated voice files"""
 
-    MAX_CONCURRENT_TASKS: int = from_env(None)
+    MAX_CONCURRENT_TASKS: int = from_env(default=None)
 
     def __post_init__(self):
-        if self.JINJA2_AUTO_ESCAPE is None:
-            self.JINJA2_AUTO_ESCAPE = get_bool_from_env("JINJA2_AUTO_ESCAPE", False)
         super().__post_init__()
         if self.TEXT_TO_SPEECH_PATH is None:
             self.TEXT_TO_SPEECH_PATH = Path(self.STORAGE_PATH) / "voicing"
```

### Comparing `ai_microcore-3.8.0/microcore/embedding_db/__init__.py` & `ai_microcore-3.9.0/microcore/embedding_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/embedding_db/chromadb.py` & `ai_microcore-3.9.0/microcore/embedding_db/chromadb.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/file_storage.py` & `ai_microcore-3.9.0/microcore/file_storage.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/json_parsing.py` & `ai_microcore-3.9.0/microcore/json_parsing.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/llm/_openai_llm_v0.py` & `ai_microcore-3.9.0/microcore/llm/_openai_llm_v0.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/llm/_openai_llm_v1.py` & `ai_microcore-3.9.0/microcore/llm/_openai_llm_v1.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import openai
 
 from ..configuration import Config, ApiType
 from .._prepare_llm_args import prepare_chat_messages, prepare_prompt
-from ..types import LLMAsyncFunctionType, LLMFunctionType
+from ..types import LLMAsyncFunctionType, LLMFunctionType, BadAIAnswer
 from ..wrappers.llm_response_wrapper import LLMResponse
 from ..utils import is_chat_model
 
 OPENAI_V1_API = True
 
 
 def _get_chunk_text(chunk, mode_chat_model: bool):
@@ -63,14 +63,19 @@
         cb = args.pop("callback")
         if cb:
             callbacks.append(cb)
     args["stream"] = bool(callbacks)
     return args, {"callbacks": callbacks}
 
 
+def check_for_errors(response):
+    if hasattr(response, "object") and response.object == "error":
+        raise BadAIAnswer(response.message)
+
+
 def make_llm_functions(config: Config) -> tuple[LLMFunctionType, LLMAsyncFunctionType]:
     if config.LLM_API_TYPE == ApiType.AZURE:
         connection_type = openai.AzureOpenAI
         async_connection_type = openai.AsyncAzureOpenAI
         params = {
             "api_key": config.LLM_API_KEY,
             "azure_endpoint": config.LLM_API_BASE,
@@ -91,51 +96,53 @@
 
     async def allm(prompt, **kwargs):
         args, options = _prepare_llm_arguments(config, kwargs)
         if is_chat_model(args["model"], config):
             response = await _async_connection.chat.completions.create(
                 messages=prepare_chat_messages(prompt), **args
             )
+            check_for_errors(response)
             if args["stream"]:
                 return await _a_process_streamed_response(
                     response, options["callbacks"], chat_model_used=True
                 )
 
             for cb in options["callbacks"]:
                 cb(response.choices[0].message.content)
             return LLMResponse(response.choices[0].message.content, response.__dict__)
 
         response = await _async_connection.completions.create(
             prompt=prepare_prompt(prompt), **args
         )
+        check_for_errors(response)
         if args["stream"]:
             return await _a_process_streamed_response(
                 response, options["callbacks"], chat_model_used=False
             )
-
         return LLMResponse(response.choices[0].text, response.__dict__)
 
     def llm(prompt, **kwargs):
         args, options = _prepare_llm_arguments(config, kwargs)
         if is_chat_model(args["model"], config):
             response = _connection.chat.completions.create(
                 messages=prepare_chat_messages(prompt), **args
             )
+            check_for_errors(response)
             if args["stream"]:
                 return _process_streamed_response(
                     response, options["callbacks"], chat_model_used=True
                 )
 
             for cb in options["callbacks"]:
                 cb(response.choices[0].message.content)
             return LLMResponse(response.choices[0].message.content, response.__dict__)
 
         # Else (if it is text completion model)
         response = _connection.completions.create(prompt=prepare_prompt(prompt), **args)
+        check_for_errors(response)
         if args["stream"]:
             return _process_streamed_response(
                 response, options["callbacks"], chat_model_used=False
             )
-
         return LLMResponse(response.choices[0].text, response.__dict__)
 
     return llm, allm
```

### Comparing `ai_microcore-3.8.0/microcore/llm/anthropic.py` & `ai_microcore-3.9.0/microcore/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/llm/google_genai.py` & `ai_microcore-3.9.0/microcore/llm/google_genai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/llm/google_vertex_ai.py` & `ai_microcore-3.9.0/microcore/llm/google_vertex_ai.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/llm/local_llm.py` & `ai_microcore-3.9.0/microcore/llm/local_llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import asyncio
 import inspect
 import threading
 from typing import Awaitable, Optional, Any, TypeVar
 
-from ..configuration import Config
+from ..configuration import Config, LLMConfigError
 from .._prepare_llm_args import prepare_chat_messages, prepare_prompt
 from ..types import LLMAsyncFunctionType, LLMFunctionType
+from ..utils import resolve_callable
 from ..wrappers.llm_response_wrapper import LLMResponse
 
 T = TypeVar("T")
 
 
 class _sync_await:
     def __init__(self):
@@ -41,17 +42,21 @@
             callbacks.append(cb)
     return args, {"callbacks": callbacks}
 
 
 def make_llm_functions(
     config: Config, overriden_inference_func: callable = None
 ) -> tuple[LLMFunctionType, LLMAsyncFunctionType]:
-    inference_fn = overriden_inference_func or config.INFERENCE_FUNC
-    if isinstance(inference_fn, str):
-        inference_fn = globals()[inference_fn]
+    try:
+        inference_fn = resolve_callable(
+            overriden_inference_func or config.INFERENCE_FUNC
+        )
+    except ValueError as e:
+        raise LLMConfigError(f"Invalid inference function, {e}") from e
+
     if inspect.iscoroutinefunction(inference_fn):
 
         async def allm(prompt, **kwargs):
             args, options = _prepare_llm_arguments(config, kwargs)
             prompt = (
                 prepare_chat_messages(prompt)
                 if config.CHAT_MODE
```

### Comparing `ai_microcore-3.8.0/microcore/llm/local_transformers.py` & `ai_microcore-3.9.0/microcore/llm/local_transformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,14 +199,23 @@
     stops_from_chat_template: list[callable] = []
     if params.get("stops_from_chat_template", True) and ending:
         stops_from_chat_template: list[callable] = make_stopping_criteria(
             ending.strip()
         )
 
     def wrapped_inference(prompt: list[dict] | str, **kwargs):
+        if (n := kwargs.pop("n", None)) is not None:  # open_ai style
+            kwargs["num_return_sequences"] = n
+
+        if (seed := kwargs.pop("seed", None)) is not None:  # open_ai style
+            transformers.set_seed(seed)
+
+        if (stop := kwargs.pop("stop", None)) is not None:  # open_ai style
+            kwargs["stopping_criteria"] = make_stopping_criteria(stop)
+
         partial_msg_used = False
         if config.CHAT_MODE:
             sc = kwargs.get("stopping_criteria", [])
             if stops_from_chat_template:
                 sc += stops_from_chat_template
             if isinstance(prompt, list) and len(prompt) > 0:
                 last = prompt[-1]
```

### Comparing `ai_microcore-3.8.0/microcore/logging.py` & `ai_microcore-3.9.0/microcore/logging.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/message_types.py` & `ai_microcore-3.9.0/microcore/message_types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/python.py` & `ai_microcore-3.9.0/microcore/python.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,17 @@
                 stdout, stderr = proc.communicate(timeout=timeout)
                 if proc.returncode != 0:
                     log_errors and logging.error(
                         f"Error executing the program, STDERR:\n<\n{stderr}\n>\n",
                     )
             except subprocess.TimeoutExpired:
                 proc.kill()
-                error = "The command timed out"
+                error = (
+                    f"The command timed out (max execution time is {timeout} seconds)"
+                )
                 stderr = f"{stderr}\n{error}"
                 log_errors and logging.error(stderr)
     finally:
         if cleanup:
             try:
                 storage.delete(fn)
             except Exception as e:  # pylint: disable=broad-except
```

### Comparing `ai_microcore-3.8.0/microcore/templating/jinja2.py` & `ai_microcore-3.9.0/microcore/templating/jinja2.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/text2speech/elevenlabs.py` & `ai_microcore-3.9.0/microcore/text2speech/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/types.py` & `ai_microcore-3.9.0/microcore/types.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/ui.py` & `ai_microcore-3.9.0/microcore/ui.py`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/microcore/utils.py` & `ai_microcore-3.9.0/microcore/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import sys
 import re
 import subprocess
 from dataclasses import dataclass
 from fnmatch import fnmatch
 from pathlib import Path
-from typing import Any
+from typing import Any, Union, Callable
 
 from colorama import Fore
 
 from .configuration import Config
 from .types import BadAIAnswer
 from .message_types import UserMsg, SysMsg, AssistantMsg
 
@@ -212,14 +212,15 @@
         )
     except subprocess.CalledProcessError:
         msg = "No GPU found or nvidia-smi is not installed"
         return f"{Fore.RED}{msg}{Fore.RESET}" if as_string else None
 
 
 def show_vram_usage():
+    """Prints GPU VRAM usage."""
     print(get_vram_usage(as_string=True))
 
 
 def return_default(default, *args):
     if isinstance(default, type) and issubclass(default, BaseException):
         raise default()
     if isinstance(default, BaseException):
@@ -238,14 +239,17 @@
 def extract_number(
     text: str,
     default=None,
     position="last",
     dtype: type | str = float,
     rounding: bool = False,
 ) -> int | float | Any:
+    """
+    Extract a number from a string.
+    """
     assert position in ["last", "first"], f"Invalid position: {position}"
     idx = {"last": -1, "first": 0}[position]
 
     dtype = {"int": int, "float": float}.get(dtype, dtype)
     assert dtype in [int, float], f"Invalid dtype: {dtype}"
     if rounding:
         dtype = float
@@ -257,15 +261,19 @@
             value = dtype(numbers[idx].strip())
             return round(value) if rounding else value
         except (ValueError, OverflowError):
             ...
     return return_default(default, text)
 
 
-def dedent(text: str):
+def dedent(text: str) -> str:
+    """
+    Removes minimal shared leading whitespace from each line
+    and strips leading and trailing empty lines.
+    """
     lines = text.splitlines()
     while lines and lines[0].strip() == "":
         lines.pop(0)
     while lines and lines[-1].strip() == "":
         lines.pop()
     non_empty_lines = [line for line in lines if line.strip()]
     if non_empty_lines:
@@ -276,14 +284,46 @@
         ]
     else:
         dedented_lines = lines
     return "\n".join(dedented_lines)
 
 
 async def run_parallel(tasks: list, max_concurrent_tasks: int):
+    """
+    Run tasks in parallel with a limit on the number of concurrent tasks.
+    """
     semaphore = asyncio.Semaphore(max_concurrent_tasks)
 
     async def worker(task):
         async with semaphore:
             return await task
 
     return await asyncio.gather(*[worker(task) for task in tasks])
+
+
+def resolve_callable(
+    fn: Union[Callable, str, None], allow_empty=False
+) -> Union[Callable, None]:
+    """
+    Resolves a callable function from a string (module.function)
+    """
+    if callable(fn):
+        return fn
+    if not fn:
+        if allow_empty:
+            return None
+        raise ValueError("Function is not specified")
+    try:
+        if "." not in fn:
+            fn = globals()[fn]
+        else:
+            parts = fn.split(".")
+            module_name = ".".join(parts[:-1])
+            func_name = parts[-1]
+            if not module_name:
+                raise ValueError(f"Invalid module name: {module_name}")
+            module = __import__(module_name, fromlist=[func_name])
+            fn = getattr(module, func_name)
+        assert callable(fn)
+    except (ImportError, AttributeError, AssertionError, ValueError) as e:
+        raise ValueError(f"Can't resolve callable by name '{fn}', {e}") from e
+    return fn
```

### Comparing `ai_microcore-3.8.0/microcore/wrappers/llm_response_wrapper.py` & `ai_microcore-3.9.0/microcore/wrappers/llm_response_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 
     - https://platform.openai.com/docs/api-reference/completions/object
     - https://platform.openai.com/docs/api-reference/chat/object
     """
 
     def __new__(cls, string: str, attrs: dict = None):
         attrs = {
+            **(attrs or {}),
             "role": Role.ASSISTANT,
             "content": str(string),
+            # generation duration in seconds (float), used in metrics
             "gen_duration": None,
-            **(attrs or {}),
         }
         obj = ExtendedString.__new__(cls, string, attrs)
         return obj
 
     def parse_json(
         self, raise_errors: bool = True, required_fields: list[str] = None
     ) -> list | dict | float | int | str:
```

### Comparing `ai_microcore-3.8.0/pyproject.toml` & `ai_microcore-3.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai_microcore-3.8.0/PKG-INFO` & `ai_microcore-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-microcore
-Version: 3.8.0
+Version: 3.9.0
 Summary: # Minimalistic Foundation for AI Applications
 Keywords: llm,large language models,ai,similarity search,ai search,gpt,openai
 Author-email: Vitalii Stepanenko <mail@vitalii.in>
 Maintainer-email: Vitalii Stepanenko <mail@vitalii.in>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai-microcore Version: 3.8.0 Summary: # Minimalistic
+Metadata-Version: 2.1 Name: ai-microcore Version: 3.9.0 Summary: # Minimalistic
 Foundation for AI Applications Keywords: llm,large language
 models,ai,similarity search,ai search,gpt,openai Author-email: Vitalii
 Stepanenko
 vitalii.in> Maintainer-email: Vitalii Stepanenko
 vitalii.in> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

