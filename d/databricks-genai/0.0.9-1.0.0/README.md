# Comparing `tmp/databricks-genai-0.0.9.tar.gz` & `tmp/databricks_genai-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-genai-0.0.9.tar", last modified: Thu Feb  8 04:31:54 2024, max compression
+gzip compressed data, was "databricks_genai-1.0.0.tar", last modified: Wed May  8 01:13:57 2024, max compression
```

## Comparing `databricks-genai-0.0.9.tar` & `databricks_genai-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.391224 databricks-genai-0.0.9/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1381 2024-02-08 04:31:54.390932 databricks-genai-0.0.9/PKG-INFO
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      273 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/README.md
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.381879 databricks-genai-0.0.9/databricks_genai/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      181 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/__init__.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.383660 databricks-genai-0.0.9/databricks_genai/api/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)        0 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/api/__init__.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     2695 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/config.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.386563 databricks-genai-0.0.9/databricks_genai/api/finetuning/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      325 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/__init__.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     2700 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/cancel.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     7588 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/create.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     3498 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/delete.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1048 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/get.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1646 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/get_events.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     5447 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/list.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)    12245 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/api/finetuning/utils.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      782 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/errors.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.388023 databricks-genai-0.0.9/databricks_genai/types/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      106 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/types/__init__.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     3836 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/types/common.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.389059 databricks-genai-0.0.9/databricks_genai/types/finetuning/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      143 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/databricks_genai/types/finetuning/__init__.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     5958 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/types/finetuning/finetune_config.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     8518 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/types/finetuning/finetuning_run.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      936 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/types/run_event.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     5255 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/databricks_genai/types/run_status.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)       53 2024-02-08 04:30:17.000000 databricks-genai-0.0.9/databricks_genai/version.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.390064 databricks-genai-0.0.9/databricks_genai.egg-info/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1381 2024-02-08 04:31:54.000000 databricks-genai-0.0.9/databricks_genai.egg-info/PKG-INFO
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1030 2024-02-08 04:31:54.000000 databricks-genai-0.0.9/databricks_genai.egg-info/SOURCES.txt
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)        1 2024-02-08 04:31:54.000000 databricks-genai-0.0.9/databricks_genai.egg-info/dependency_links.txt
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      291 2024-02-08 04:31:54.000000 databricks-genai-0.0.9/databricks_genai.egg-info/requires.txt
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)       17 2024-02-08 04:31:54.000000 databricks-genai-0.0.9/databricks_genai.egg-info/top_level.txt
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)    31194 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/pyproject.toml
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)       38 2024-02-08 04:31:54.391274 databricks-genai-0.0.9/setup.cfg
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1591 2024-02-08 04:30:05.000000 databricks-genai-0.0.9/setup.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-02-08 04:31:54.389483 databricks-genai-0.0.9/tests/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      332 2024-01-09 18:19:25.000000 databricks-genai-0.0.9/tests/test_package.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.580798 databricks_genai-1.0.0/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1757 2024-05-08 01:13:57.580483 databricks_genai-1.0.0/PKG-INFO
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      274 2024-04-17 00:17:05.000000 databricks_genai-1.0.0/README.md
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.570473 databricks_genai-1.0.0/databricks/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      350 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/__init__.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.571106 databricks_genai-1.0.0/databricks/model_training/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      185 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/__init__.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.572322 databricks_genai-1.0.0/databricks/model_training/api/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3170 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/config.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.573192 databricks_genai-1.0.0/databricks/model_training/api/engine/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      355 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/engine/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    32800 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/engine/engine.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6573 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/exceptions.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.575243 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      334 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2639 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/cancel.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     8601 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/create.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3611 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/delete.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1049 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/get.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3328 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/get_events.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4748 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/foundation_model/list.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    17845 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/api/utils.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.576764 databricks_genai-1.0.0/databricks/model_training/types/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      131 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/types/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5516 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/types/common.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5255 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/types/run_status.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6109 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/types/train_config.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    12046 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/databricks/model_training/types/training_run.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)       47 2024-05-08 01:12:13.000000 databricks_genai-1.0.0/databricks/model_training/version.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.579220 databricks_genai-1.0.0/databricks_genai.egg-info/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1757 2024-05-08 01:13:57.000000 databricks_genai-1.0.0/databricks_genai.egg-info/PKG-INFO
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1241 2024-05-08 01:13:57.000000 databricks_genai-1.0.0/databricks_genai.egg-info/SOURCES.txt
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        1 2024-05-08 01:13:57.000000 databricks_genai-1.0.0/databricks_genai.egg-info/dependency_links.txt
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      465 2024-05-08 01:13:57.000000 databricks_genai-1.0.0/databricks_genai.egg-info/requires.txt
+-rw-r--r--   0 nancy.hung   (502) staff       (20)       11 2024-05-08 01:13:57.000000 databricks_genai-1.0.0/databricks_genai.egg-info/top_level.txt
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    31118 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/pyproject.toml
+-rw-r--r--   0 nancy.hung   (502) staff       (20)       38 2024-05-08 01:13:57.580851 databricks_genai-1.0.0/setup.cfg
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1778 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/setup.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-05-08 01:13:57.578606 databricks_genai-1.0.0/tests/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      358 2024-05-08 01:12:06.000000 databricks_genai-1.0.0/tests/test_package.py
```

### Comparing `databricks-genai-0.0.9/PKG-INFO` & `databricks_genai-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
 Name: databricks-genai
-Version: 0.0.9
+Version: 1.0.0
 Summary: Interact with the Databricks Generative AI APIs in python
 Home-page: https://docs.mosaicml.com/projects/mcli/en/latest/finetuning/finetuning.html
 Author: Databricks
 Author-email: genai-eng-team@databricks.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: databricks-sdk>=0.14.0
-Requires-Dist: typing_extensions>=4.7.1
+Requires-Dist: backoff>=2.2.1
+Requires-Dist: databricks-sdk==0.18.0
+Requires-Dist: datasets<=2.17.0,>=2.16.1
+Requires-Dist: gql[websockets]>=3.4.0
+Requires-Dist: mlflow<=2.10.2,>=2.9.2
 Requires-Dist: mosaicml-cli==0.6.5
-Requires-Dist: datasets>=2.16.1
-Requires-Dist: mlflow>=2.9.2
+Requires-Dist: requests<3,>=2.26.0
+Requires-Dist: typing_extensions>=4.7.1
+Requires-Dist: IPython<9,>=8
 Provides-Extra: dev
 Requires-Dist: isort>=5.9.3; extra == "dev"
 Requires-Dist: packaging<23,>=21; extra == "dev"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
 Requires-Dist: pylint>=3.0.0; extra == "dev"
 Requires-Dist: pyright==1.1.256; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: yapf>=0.40.0; extra == "dev"
+Provides-Extra: notebook
+Requires-Dist: ipywidgets<9,>=8; extra == "notebook"
 Provides-Extra: all
-Requires-Dist: pyright==1.1.256; extra == "all"
 Requires-Dist: isort>=5.9.3; extra == "all"
-Requires-Dist: yapf>=0.40.0; extra == "all"
-Requires-Dist: pytest>=7.4.0; extra == "all"
 Requires-Dist: packaging<23,>=21; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: ipywidgets<9,>=8; extra == "all"
 Requires-Dist: pylint>=3.0.0; extra == "all"
+Requires-Dist: pyright==1.1.256; extra == "all"
+Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: yapf>=0.40.0; extra == "all"
```

### Comparing `databricks-genai-0.0.9/databricks_genai/api/config.py` & `databricks_genai-1.0.0/databricks/model_training/api/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,67 @@
 """Wrapper around MAPI engine in MCLI."""
 
 import logging
 import os
 from typing import Any, Callable, Tuple, TypeVar
 
 from databricks.sdk import WorkspaceClient
-from mcli import MAPIException, config
-from mcli.api.exceptions import MultiMAPIException
+from mcli import config
 
-from databricks_genai import errors
+# pylint: disable=ungrouped-imports
+from databricks.model_training.api.exceptions import (DatabricksModelTrainingRequestError, MAPIException,
+                                                      MultiMAPIException)
 
 _TCallable = TypeVar('_TCallable', bound=Callable[..., Any])  # pylint: disable=invalid-name
 
 logger = logging.getLogger(__name__)
 
 GENAI_LOCAL_ENV = 'GENAI_LOCAL'
 
+GENAI_TOKEN_OVERRIDE_ENV = 'GENAI_PERSONAL_ACCESS_TOKEN'
+GENAI_MAPI_OVERRIDE_ENV = 'GENAI_MAPI_ENDPOINT'
+
+GENAI_MAPI_ENDPOINT_SUFFIX = '/api/2.0/genai-mapi/graphql'
+
 
 def get_me() -> str:
     """
     Get who is currently logged in.
 
     Returns:
         str: The name of the current user.
     """
 
     if os.environ.get(GENAI_LOCAL_ENV, '').lower() == 'true':
         return 'me'
 
     w = WorkspaceClient()
-    me = w.current_user.me().user_name
+    me = w.current_user.me().user_name or ''
     logger.debug(f'You are {me}')
     return me
 
 
 def get_config_from_env() -> Tuple[str, str]:
     """
     Get api key and endpoint from the current MAPI environment.
 
     Returns:
         Tuple[str, str]: The API key and endpoint.
     """
     if os.environ.get(GENAI_LOCAL_ENV, '').lower() == 'true':
         return 'local', 'local'
 
+    if GENAI_TOKEN_OVERRIDE_ENV in os.environ and GENAI_MAPI_OVERRIDE_ENV in os.environ:
+        return os.environ[GENAI_TOKEN_OVERRIDE_ENV], os.environ[GENAI_MAPI_OVERRIDE_ENV]
+
     w = WorkspaceClient()
     ctx = w.dbutils.entry_point.getDbutils().notebook().getContext()
     api_url = ctx.apiUrl().get()
     api_token = ctx.apiToken().get()
-    return api_token, f'{api_url}/api/2.0/genai-mapi/graphql'
+    return api_token, f'{api_url}{GENAI_MAPI_ENDPOINT_SUFFIX}'
 
 
 def configure_request(func: _TCallable) -> _TCallable:
     """
     Decorator that configures a default retry policy for all MAPI requests
 
     Args:
@@ -61,28 +70,28 @@
 
     def setup(*args, **kwargs):
         api_token, endpoint = get_config_from_env()
 
         previous_api_key = os.getenv(config.MOSAICML_API_KEY_ENV)
         previous_endpoint = os.getenv(config.MOSAICML_API_ENDPOINT_ENV)
 
-        logger.debug(f"Setting up MAPI connection with api_token {api_token} and endpoint {endpoint}")
+        logger.debug(f'Setting up MAPI connection with api_token {api_token} and endpoint {endpoint}')
 
         if os.environ.get('GENAI_LOCAL', '').lower() != 'true':
             os.environ[config.MOSAICML_API_KEY_ENV] = f'Bearer {api_token}'
             os.environ[config.MOSAICML_API_ENDPOINT_ENV] = endpoint
 
         try:
             res = func(*args, **kwargs)
         except TimeoutError as e:
-            raise errors.DatabricksGenAIRequestError(f'Timeout connecting to {endpoint}') from e
+            raise DatabricksModelTrainingRequestError(f'Timeout connecting to {endpoint}') from e
         except MAPIException as e:
             if isinstance(e, MultiMAPIException):
                 e = e.errors[0]
-            raise errors.DatabricksGenAIRequestError(e.message)
+            raise DatabricksModelTrainingRequestError(e.message) from e
 
         if previous_api_key:
             os.environ[config.MOSAICML_API_KEY_ENV] = previous_api_key
         if previous_endpoint:
             os.environ[config.MOSAICML_API_ENDPOINT_ENV] = previous_endpoint
 
         return res
```

### Comparing `databricks-genai-0.0.9/databricks_genai/api/finetuning/cancel.py` & `databricks_genai-1.0.0/databricks/model_training/api/foundation_model/cancel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Cancel a finetuning run"""
+"""Cancel a model training run"""
 
 from typing import Any, Dict, List, Union
 
-from mcli.api.engine.engine import get_return_response, run_plural_mapi_request
 from mcli.config import MCLIConfig
 
-from databricks_genai.api.config import configure_request
-from databricks_genai.errors import DatabricksGenAIRequestError
-from databricks_genai.types.finetuning import FinetuningRun
+from databricks.model_training.api.config import configure_request
+from databricks.model_training.api.engine import get_return_response, run_plural_mapi_request
+from databricks.model_training.api.exceptions import DatabricksModelTrainingRequestError
+from databricks.model_training.types.training_run import TrainingRun
 
 QUERY_FUNCTION = 'stopFinetunes'
 VARIABLE_DATA_NAME = 'getFinetunesData'
 OPTIONAL_DATA_NAME = 'stopFinetunesData'
 QUERY = f"""
 mutation StopFinetunes(${VARIABLE_DATA_NAME}: GetFinetunesInput!, ${OPTIONAL_DATA_NAME}: StopFinetunesInput) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}, {OPTIONAL_DATA_NAME}: ${OPTIONAL_DATA_NAME}) {{
@@ -27,55 +27,48 @@
     reason
     isDeleted
   }}
 }}"""
 
 
 @configure_request
-def cancel(finetuning_runs: Union[str, FinetuningRun, List[str], List[FinetuningRun]]) -> int:
-    """Cancel a finetuning run or list of finetuning runs without deleting them
-    
+def cancel(runs: Union[str, TrainingRun, List[str], List[TrainingRun]]) -> int:
+    """Cancel a training run or list of training runs without deleting them.
+    If the run does not exist or if the run has already terminated, an error will be raised.
+
     Args:
-        finetuning_runs (Union[str, FinetuningRun, List[str], List[FinetuningRun]]): The
-            finetuning run(s) to cancel. Can be a single run or a list of runs.
-    
+        runs (Union[str, TrainingRun, List[str], List[TrainingRun]]): The
+            training run(s) to cancel. Can be a single run or a list of runs.
+
     Returns:
-        int: The number of finetuning runs cancelled
+        int: The number of training runs cancelled
     """
 
-    if not finetuning_runs:
-        raise DatabricksGenAIRequestError('Must provide finetuning run(s) to cancel')
+    if not runs:
+        raise DatabricksModelTrainingRequestError('Must provide training run(s) to cancel')
 
-    finetuning_runs_list: List[Union[str, FinetuningRun]] = [finetuning_runs] if isinstance(
-        finetuning_runs, (str, FinetuningRun)) else finetuning_runs  # pyright: ignore
+    runs_list: List[Union[str, TrainingRun]] = [runs] if isinstance(runs,
+                                                                    (str, TrainingRun)) else runs  # pyright: ignore
 
     # Extract run names
-    finetuning_run_names = [r if isinstance(r, str) else r.name for r in finetuning_runs_list]
+    training_run_names = [r if isinstance(r, str) else r.name for r in runs_list]
 
     filters = {}
-    if finetuning_run_names:
-        filters['name'] = {'in': finetuning_run_names}
+    if training_run_names:
+        filters['name'] = {'in': training_run_names}
 
     variables: Dict[str, Dict[str, Any]] = {VARIABLE_DATA_NAME: {'filters': filters}}
 
     cfg = MCLIConfig.load_config()
     cfg.update_entity(variables[VARIABLE_DATA_NAME])
 
-    response = run_plural_mapi_request(
-        query=QUERY,
-        query_function=QUERY_FUNCTION,
-        return_model_type=FinetuningRun,
-        variables=variables,
-    )
-
     try:
         response = run_plural_mapi_request(
             query=QUERY,
             query_function=QUERY_FUNCTION,
-            return_model_type=FinetuningRun,
+            return_model_type=TrainingRun,
             variables=variables,
         )
         return len(get_return_response(response))
     except Exception as e:
-        raise DatabricksGenAIRequestError(
-            f'Failed to cancel finetuning run(s) {finetuning_runs}. Please make sure the run '
-            'has not completed or failed and try again.') from e
+        raise DatabricksModelTrainingRequestError(f'Failed to cancel training run(s) {runs}. Please make sure the run '
+                                                  'has not completed or failed and try again.') from e
```

### Comparing `databricks-genai-0.0.9/databricks_genai/api/finetuning/create.py` & `databricks_genai-1.0.0/databricks/model_training/api/foundation_model/create.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-"""Create a finetuning run"""
+"""Create a model training run"""
 
 from typing import Dict, List, Optional, Union
 
-from mcli.api.engine.engine import get_return_response, run_singular_mapi_request
-
-from databricks_genai.api.config import configure_request, get_me
-from databricks_genai.api.finetuning.utils import (SAVE_FOLDER_PATH, format_path, is_cluster_sql,
-                                                   validate_create_finetuning_run_inputs)
-from databricks_genai.types.finetuning import FinetuningRun
-from databricks_genai.types.finetuning.finetune_config import FinetuneConfig
+from databricks.model_training.api.config import configure_request, get_me
+from databricks.model_training.api.engine import get_return_response, run_singular_mapi_request
+from databricks.model_training.api.utils import (SAVE_FOLDER_PATH, format_path, is_cluster_sql,
+                                                 validate_create_training_run_inputs)
+from databricks.model_training.types import TrainingRun
+from databricks.model_training.types.train_config import TrainConfig, TrainTaskType
 
 QUERY_FUNCTION = 'createFinetune'
 VARIABLE_DATA_NAME = 'createFinetuneData'
 # This returns the same data that the create_run function returns
 # for consistency when rendering the describe output
 QUERY = f"""
 mutation CreateFinetune(${VARIABLE_DATA_NAME}: CreateFinetuneInput!) {{
@@ -48,127 +47,151 @@
 
 @configure_request
 def create(
     model: str,
     train_data_path: str,
     register_to: str,
     *,
-    experiment_path: Optional[str] = "{}",
-    task_type: Optional[str] = "INSTRUCTION_FINETUNE",
+    experiment_path: Optional[str] = '',
+    task_type: Optional[str] = 'INSTRUCTION_FINETUNE',
     eval_data_path: Optional[str] = None,
     eval_prompts: Optional[List[str]] = None,
     custom_weights_path: Optional[str] = None,
     training_duration: Optional[str] = None,
     learning_rate: Optional[float] = None,
     context_length: Optional[int] = None,
     validate_inputs: Optional[bool] = True,
     data_prep_cluster_id: Optional[str] = None,
-) -> FinetuningRun:
-    """Create a finetuning run
+) -> TrainingRun:
+    """Create a model training run
 
     Args:
         model (str): The name of the Hugging Face model to use.
         train_data_path (str): The full remote location of your training data.
             The format of this data depends on the task type:
-            - ``INSTRUCTION_FINETUNE``:  JSONL format, where each line is a 
+            - ``INSTRUCTION_FINETUNE``:  JSONL format, where each line is a
                 prompt and response JSON object, for example:
                 {"prompt": "What is the capital of France?", "response": "Paris"}
             - ``CONTINUED_PRETRAIN``: A text file containing raw text data.
+            - ``CHAT_COMPLETION``: JSONL format, where each line is a list of messages,
+                for example: [
+                    {
+                        'role': 'system',
+                        'content': 'You are a helpful assistant.'
+                    },
+                    {
+                        'role': 'user',
+                        'content': 'Hello, I need some help with my task.'
+                    },
+                    {
+                        'role': 'assistant',
+                        'content': 'Yes, I can help you with that. What do you need?'
+                    }]
         register_to (str): A Unity Catalog location where the model will
             be registered after training for easy deployment. Specify a location
             as either ``<catalog_name>.<schema_name>`` or
             ``<catalog_name>.<schema_name>.<model_name>``. The former will create
-            a model with the same name as the finetuning run.
+            a model with the same name as the training run.
         experiment_path (str, optional): The path to the MLflow experiment where
-            the final model checkpoint will be saved. Defaults to the run name
+            the final model checkpoint will be saved. Defaults to the user's personal
+            workspace with the run name as the experiment name.
         task_type (str, optional): The type of task to train for. Options:
             - ``INSTRUCTION_FINETUNE`` (default): Finetune a model with instructions
                 relative to a specific task.
             - ``CONTINUED_PRETRAIN``: Continue pretraining a model using additional
                 raw text data.
+            - ``CHAT_COMPLETION``: Finetune a model with chat message data.
         eval_data_path (str, optional): The remote location of your evaluation data
             (if any). Defaults to no evaluation. Must follow the same format as
             ``train_data_path``.
-        eval_prompts (List[str], optional): A list of prompt strings to generate 
+        eval_prompts (List[str], optional): A list of prompt strings to generate
             during evaluation. Results will be logged to the experiment every tim
             the model is checkpointed. Default is ``None`` (do not generate prompts).
-        custom_weights_path (str, None) The remote location of a custom model checkpoint 
-            to use for finetuning. If provided, these weights will be used instead of 
-            the original pretrained weights of the model. This must be a Composer 
+        custom_weights_path (str, None) The remote location of a custom model checkpoint
+            to use for training run. If provided, these weights will be used instead of
+            the original pretrained weights of the model. This must be a Composer
             checkpoint. Default is ``None``.
-        training_duration: The total duration of your finetuning run. 
+        training_duration: The total duration of your training run.
             This can be specified:
             - In batches (e.g. ``100ba``)
             - In epochs (e.g. ``10ep``)
             - In tokens (e.g. ``1_000_000tok``)
             Default is ``1ep``.
-        learning_rate: The peak learning rate to use for finetuning. Default is ``5e-7``. 
+        learning_rate: The peak learning rate to use for your training run. Default is ``5e-7``.
         context_length: The maximum sequence length to use. This will be used to truncate
-            any data that is too long. The default is the default for the provided Hugging 
+            any data that is too long. The default is the default for the provided Hugging
             Face model. We do not support extending the context length beyond each model's
             default.
-        validate_inputs: Whether to validate the access to input paths before submitting 
-            the finetuning job. Default is ``True``.
+        validate_inputs: Whether to validate the access to input paths before submitting
+            the training run. Default is ``True``.
         data_prep_cluster_id: Cluster id for Spark data processing.
-            This is required to support Delta table as an input for the finetuning API
-            because we need to concatenate underlying Delta data files into a single location 
+            This is required to support Delta table as an input for the model training API
+            because we need to concatenate underlying Delta data files into a single location
             and then convert to JSONL for IFT, and MDS for CPT.
 
     Returns:
-        FinetuningRun: The finetuning run object that was created
+        TrainingRun: The training run object that was created
     """
-    databricks_username = get_me()
+    full_experiment_path = experiment_path
+    default_experiment_name = '{}'
+    if not experiment_path:
+        databricks_username = get_me()
+        full_experiment_path = f'/Users/{databricks_username}/{default_experiment_name}'
     experiment_tracker = {
         'mlflow': {
-            'experiment_path': f'/Users/{databricks_username}/{experiment_path}',
+            'experiment_path': full_experiment_path,
             'model_registry_path': register_to,
+            'createExperimentAndRun': True,
         }
     }
 
     train_data_path = format_path(train_data_path)
     if eval_data_path is not None:
         eval_data_path = format_path(eval_data_path)
     if custom_weights_path is not None:
         custom_weights_path = format_path(custom_weights_path)
     save_folder = SAVE_FOLDER_PATH
+    if task_type is None:
+        task_type = 'INSTRUCTION_FINETUNE'
+
     if validate_inputs:
         # don't validate experiment path if it's the default
-        # TODO: create FinetuneConfig object for this SDK, so we can pass in object
+        # TODO: create TrainConfig object for this SDK, so we can pass in object
         # instead of a list of params in the next line
-        experiment_path_to_validate = experiment_tracker['mlflow'][
-            'experiment_path'] if experiment_path != "{}" else None
-        validate_create_finetuning_run_inputs(train_data_path, register_to, experiment_path_to_validate, eval_data_path,
-                                              data_prep_cluster_id, custom_weights_path)
+        experiment_path_to_validate = full_experiment_path if experiment_path else None
+        validate_create_training_run_inputs(train_data_path, register_to, experiment_path_to_validate, eval_data_path,
+                                            data_prep_cluster_id, custom_weights_path, TrainTaskType(task_type))
+
     data_prep_config: Optional[Dict[str, Union[str, bool]]] = None
     # TODO: add translations for snake to camel case
     if data_prep_cluster_id is not None:
         data_prep_config = {'clusterId': data_prep_cluster_id}
         if is_cluster_sql(data_prep_cluster_id):
             data_prep_config['useSql'] = True
 
-    config = FinetuneConfig.from_dict({
+    config = TrainConfig.from_dict({
         'model': model,
         'task_type': task_type,
         'train_data_path': train_data_path,
         'save_folder': save_folder,
         'eval_data_path': eval_data_path,
         'eval_prompts': eval_prompts,
         'training_duration': training_duration,
         'experiment_tracker': experiment_tracker,
         'learning_rate': learning_rate,
         'context_length': context_length,
         'custom_weights_path': custom_weights_path,
         'data_prep_config': data_prep_config,
         'disable_credentials_check': not validate_inputs,
     })
-    finetune_config = config.to_create_finetune_api_input()
+    finetune_config = config.to_create_api_input()
     variables = {
         VARIABLE_DATA_NAME: finetune_config,
     }
 
     response = run_singular_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
-        return_model_type=FinetuningRun,
+        return_model_type=TrainingRun,
         variables=variables,
     )
     return get_return_response(response)
```

### Comparing `databricks-genai-0.0.9/databricks_genai/api/finetuning/list.py` & `databricks_genai-1.0.0/databricks/model_training/api/foundation_model/list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-"""List multiple finetuning runs"""
+"""List multiple model training runs"""
 
 from datetime import datetime
 from typing import List, Optional, Union
 
-from mcli.api.engine.engine import get_return_response, run_paginated_mapi_request
 from mcli.config import MCLIConfig
 
-from databricks_genai.api.config import configure_request
-from databricks_genai.types.common import ObjectList
-from databricks_genai.types.finetuning import FinetuningRun
-from databricks_genai.types.run_status import RunStatus
+from databricks.model_training.api.config import configure_request
+from databricks.model_training.api.engine import get_return_response, run_paginated_mapi_request
+from databricks.model_training.types import TrainingRun
+from databricks.model_training.types.common import ObjectList
+from databricks.model_training.types.run_status import RunStatus
+
+DEFAULT_LIMIT = 100
 
 QUERY_FUNCTION = 'getFinetunesPaginated'
 VARIABLE_DATA_NAME = 'getFinetunesPaginatedData'
 
 QUERY = f"""
 query GetFinetunesPaginated(${VARIABLE_DATA_NAME}: GetFinetunesPaginatedInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
@@ -66,70 +68,51 @@
             contextLength
             experimentTracker
             customWeightsPath
             dataPrepConfig
             formattedFinetuningEvents {{
                 eventType
                 eventTime
-                eventMessage    
+                eventMessage
             }}
         }}
     }}
   }}
 }}"""
 
 
 @configure_request
 def list(  # pylint: disable=redefined-builtin
-    finetuning_runs: Optional[Union[List[str], List[FinetuningRun], ObjectList[FinetuningRun]]] = None,
+    training_runs: Optional[Union[List[str], List[TrainingRun], ObjectList[TrainingRun]]] = None,
     *,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     user_emails: Optional[List[str]] = None,
     before: Optional[Union[str, datetime]] = None,
     after: Optional[Union[str, datetime]] = None,
-    limit: Optional[int] = None,
-):
-    """ 
-    Internal db get finetuning runs to include dataPrepConfig in details.
-    """
-    return get_finetuning_runs_paginated(finetuning_runs=finetuning_runs,
-                                         statuses=statuses,
-                                         user_emails=user_emails,
-                                         before=before,
-                                         after=after,
-                                         limit=limit)
-
+    include_details: bool = True,
+    limit: Optional[int] = DEFAULT_LIMIT,
+) -> ObjectList[TrainingRun]:
+    """List training runs
 
-def get_finetuning_runs_paginated(
-    finetuning_runs: Optional[Union[List[str], List[FinetuningRun], ObjectList[FinetuningRun]]] = None,
-    *,
-    statuses: Optional[Union[List[str], List[RunStatus]]] = None,
-    user_emails: Optional[List[str]] = None,
-    before: Optional[Union[str, datetime]] = None,
-    after: Optional[Union[str, datetime]] = None,
-    include_details: bool = False,
-    limit: Optional[int] = None,
-) -> List[FinetuningRun]:
-    """List finetuning runs
-    
     Args:
-        finetuning_runs (Optional[Union[List[str], List[FinetuningRun], ObjectList[FinetuningRun]]], optional): 
-        The finetuning runs to list. Defaults to None.
+        training_runs (Optional[Union[List[str], List[TrainingRun], ObjectList[TrainingRun]]], optional):
+        The training runs to list. Defaults to None.
         statuses (Optional[Union[List[str], List[RunStatus]], optional): The statuses to filter by. Defaults to None.
         user_emails (Optional[List[str]], optional): The user emails to filter by. Defaults to None.
+        include_details (bool, optional): Whether to include details in the response. Defaults to True.
         before (Optional[Union[str, datetime]], optional): The date to filter before. Defaults to None.
         after (Optional[Union[str, datetime]], optional): The date to filter after. Defaults to None.
-        limit (Optional[int], optional): The maximum number of runs to return. Defaults to None.
-    
+        limit (Optional[int], optional): The maximum number of runs to return. Defaults to the 100 most recent.
+
     Returns:
-        ObjectList[FinetuningRun]: A list of finetuning runs
+        ObjectList[TrainingRun]: A list of training runs
     """
     filters = {}
-    if finetuning_runs:
-        filters['name'] = {'in': [r.name if isinstance(r, FinetuningRun) else r for r in finetuning_runs]}
+    if training_runs:
+        filters['name'] = {'in': [r.name if isinstance(r, TrainingRun) else r for r in training_runs]}
     if statuses:
         filters['status'] = {'in': [s.value if isinstance(s, RunStatus) else s for s in statuses]}
     if before or after:
         date_filters = {}
         if before:
             date_filters['lt'] = before.astimezone().isoformat() if isinstance(before, datetime) else before
         if after:
@@ -151,11 +134,11 @@
             variables[VARIABLE_DATA_NAME]['entity']['emails'] = user_emails
         else:
             variables[VARIABLE_DATA_NAME]['entity'] = {'emails': user_emails}
 
     response = run_paginated_mapi_request(
         query=QUERY_WITH_DETAILS_DB if include_details else QUERY,
         query_function=QUERY_FUNCTION,
-        return_model_type=FinetuningRun,
+        return_model_type=TrainingRun,
         variables=variables,
     )
     return get_return_response(response)
```

### Comparing `databricks-genai-0.0.9/databricks_genai/types/finetuning/finetune_config.py` & `databricks_genai-1.0.0/databricks/model_training/types/train_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 """ Finetune config """
 import logging
 from dataclasses import asdict, dataclass
+from enum import Enum
 from typing import Any, Dict, List, Optional
 
 import yaml
-from mcli.api.exceptions import MCLIConfigError
-from mcli.models.finetune_task_type import FinetuneTaskType
 from mcli.utils.utils_config import (BaseSubmissionConfig, ExperimentTrackerConfig, ExperimentTrackerTranslation,
                                      strip_nones)
 from mcli.utils.utils_string_functions import camel_case_to_snake_case, snake_case_to_camel_case
 
+from databricks.model_training.api.exceptions import DatabricksGenAIConfigError
+
 logger = logging.getLogger(__name__)
 
 
+class TrainTaskType(Enum):
+    """ The Type of Finetune Task to run """
+    INSTRUCTION_FINETUNE = 'INSTRUCTION_FINETUNE'
+    CONTINUED_PRETRAIN = 'CONTINUED_PRETRAIN'
+    CHAT_COMPLETION = 'CHAT_COMPLETION'
+
+
 @dataclass
-class FinetuneConfig(BaseSubmissionConfig):
-    """Input for finetuning run
+class TrainConfig(BaseSubmissionConfig):
+    """Input for training run
 
     Args:
         model (str): Model to finetune (e.g. 'mosaicml/mpt-30b')
-        task_type (FinetuneTaskType): Task type to finetune on (options are 'INSTRUCTION_FINETUNE' or
-            'CONTINUED_PRETRAIN')
+        task_type (str): Task type to finetune on
         train_data_path (str): HF dataset or remote path to training data
         save_folder (str): Folder to save checkpoints and HF checkpoints, currently must be an s3 or GCP path
         eval_data_path (Optional[str]): HF dataset or remote path to eval data
         eval_prompts (Optional[List[str]]): A list of prompt strings to generate from periodically during training
-        custom_weights_path (Optional[str]): Remote location of custom weights to use for finetuning
+        custom_weights_path (Optional[str]): Remote location of custom weights to use for model training
         training_duration (str): Composer variable for the total number of epochs or tokens to train on
             (e.g. 2ep or 10000tok)
         experiment_tracker (Optional[ExperimentTrackerConfig]): Experiment tracker config
         learning_rate (Optional[float]): Learning rate to use
         context_length (Optional[int]): Context length of the model. Override only works for MPT model families
         disable_credentials_check (Optional[bool]): Flag to disable checking credentials (S3, Databricks, etc.)
             on finetune submission
     """
 
     model: str
     train_data_path: str
     save_folder: str = 'dbfs:/databricks/mlflow-tracking/{mlflow_experiment_id}/{mlflow_run_id}/artifacts'
-    task_type: Optional[str] = "INSTRUCTION_FINETUNE"
+    task_type: Optional[str] = 'INSTRUCTION_FINETUNE'
     eval_data_path: Optional[str] = None
     eval_prompts: Optional[List[str]] = None
     custom_weights_path: Optional[str] = None
     training_duration: Optional[str] = None
     experiment_tracker: Optional[ExperimentTrackerConfig] = None
     learning_rate: Optional[float] = None
     context_length: Optional[int] = None
@@ -68,17 +75,18 @@
         """
         config_dict = strip_nones(dict_to_use)
         unused_keys = set(config_dict) - cls._finetune_properties
         for key in unused_keys:
             del config_dict[key]
         missing = cls._required_properties - set(dict_to_use)
         if missing:
-            raise MCLIConfigError(f'Missing required fields: {", ".join(missing)}',)
+            raise DatabricksGenAIConfigError(f'Missing required fields: {", ".join(missing)}',)
         if len(unused_keys) > 0 and show_unused_warning:
-            raise MCLIConfigError(f'Encountered unknown fields in finetuning config: {", ".join(unused_keys)}.')
+            raise DatabricksGenAIConfigError(
+                f'Encountered unknown fields in training config: {", ".join(unused_keys)}.')
         return config_dict
 
     @classmethod
     def from_dict(cls, dict_to_use: Dict[str, Any], show_unused_warning: bool = True):
         """Load the config from the provided dictionary.
         """
         config_dict = cls.validate_dict(dict_to_use, show_unused_warning)
@@ -86,38 +94,38 @@
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]):
         """Load the config from mapi response.
         """
         experiment_tracker_result = {}
         for key, value in response.items():
-            if key == "experimentTracker":
-                experiment_tracker_result["experiment_tracker"] = ExperimentTrackerTranslation.from_mapi(value)
+            if key == 'experimentTracker':
+                experiment_tracker_result['experiment_tracker'] = ExperimentTrackerTranslation.from_mapi(value)
             else:
                 experiment_tracker_result[camel_case_to_snake_case(key)] = value
         return cls.from_dict(experiment_tracker_result)
 
-    def to_create_finetune_api_input(self) -> Dict[str, Dict[str, Any]]:
-        """Converts the FinetuneConfig object to Compute and Finetune that can be used to create a finetune run
+    def to_create_api_input(self) -> Dict[str, Dict[str, Any]]:
+        """Converts the TrainConfig object to Compute and Finetune that can be used to create a finetune run
         """
         finetune = {}
         config_dict = strip_nones(self.__dict__)
         for key, val in config_dict.items():
             if key == 'experiment_tracker':
                 finetune['experimentTracker'] = ExperimentTrackerTranslation.to_mapi(val)
                 continue
             translated_key = snake_case_to_camel_case(key)
             if key in self._finetune_properties:
                 finetune[translated_key] = val
 
         return {'config': finetune}
 
     def to_yaml(self) -> str:
-        """Converts the FinetuneConfig object to a yaml string with only used keys
+        """Converts the TrainConfig object to a yaml string with only used keys
         """
         filtered_config = {k: v for k, v in self.__dict__.items() if v}
         return yaml.safe_dump(filtered_config)
 
     def __post_init__(self):
-        if not FinetuneTaskType.validate_task_type(self.task_type):
-            raise MCLIConfigError(f'Invalid task_type: {self.task_type}, currently '
-                                  f'supported options are: {", ".join([x.value for x in FinetuneTaskType])}')
+        if self.task_type not in TrainTaskType.__members__:
+            raise DatabricksGenAIConfigError(f'Invalid task_type: {self.task_type}, currently '
+                                             f'supported options are: {", ".join([x.value for x in TrainTaskType])}')
```

### Comparing `databricks-genai-0.0.9/databricks_genai/types/run_status.py` & `databricks_genai-1.0.0/databricks/model_training/types/run_status.py`

 * *Files identical despite different names*

### Comparing `databricks-genai-0.0.9/databricks_genai.egg-info/PKG-INFO` & `databricks_genai-1.0.0/databricks_genai.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
 Name: databricks-genai
-Version: 0.0.9
+Version: 1.0.0
 Summary: Interact with the Databricks Generative AI APIs in python
 Home-page: https://docs.mosaicml.com/projects/mcli/en/latest/finetuning/finetuning.html
 Author: Databricks
 Author-email: genai-eng-team@databricks.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: databricks-sdk>=0.14.0
-Requires-Dist: typing_extensions>=4.7.1
+Requires-Dist: backoff>=2.2.1
+Requires-Dist: databricks-sdk==0.18.0
+Requires-Dist: datasets<=2.17.0,>=2.16.1
+Requires-Dist: gql[websockets]>=3.4.0
+Requires-Dist: mlflow<=2.10.2,>=2.9.2
 Requires-Dist: mosaicml-cli==0.6.5
-Requires-Dist: datasets>=2.16.1
-Requires-Dist: mlflow>=2.9.2
+Requires-Dist: requests<3,>=2.26.0
+Requires-Dist: typing_extensions>=4.7.1
+Requires-Dist: IPython<9,>=8
 Provides-Extra: dev
 Requires-Dist: isort>=5.9.3; extra == "dev"
 Requires-Dist: packaging<23,>=21; extra == "dev"
+Requires-Dist: pre-commit>=2.17.0; extra == "dev"
 Requires-Dist: pylint>=3.0.0; extra == "dev"
 Requires-Dist: pyright==1.1.256; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: yapf>=0.40.0; extra == "dev"
+Provides-Extra: notebook
+Requires-Dist: ipywidgets<9,>=8; extra == "notebook"
 Provides-Extra: all
-Requires-Dist: pyright==1.1.256; extra == "all"
 Requires-Dist: isort>=5.9.3; extra == "all"
-Requires-Dist: yapf>=0.40.0; extra == "all"
-Requires-Dist: pytest>=7.4.0; extra == "all"
 Requires-Dist: packaging<23,>=21; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: ipywidgets<9,>=8; extra == "all"
 Requires-Dist: pylint>=3.0.0; extra == "all"
+Requires-Dist: pyright==1.1.256; extra == "all"
+Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: yapf>=0.40.0; extra == "all"
```

### Comparing `databricks-genai-0.0.9/pyproject.toml` & `databricks_genai-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 # iSort
 [tool.isort]
 multi_line_output = 0
 line_length = 120
-skip = [ "env", "wandb", "venv", "databricks_genai/proto", "notebooks" ]
+skip = [ "env", "wandb", "venv", "databricks/proto", "notebooks" ]
 
 # Pyright
 [tool.pyright]
 include = [
-    "databricks_genai/**",
+    "databricks/**",
     "tests/**"
 ]
 
 exclude = [
-    "databricks_genai/proto/**",
+    "databricks/proto/**",
     "notebooks",
 ]
 
 reportUnknownMemberType = "none"
 reportImportCycles = "none"
 reportUnnecessaryIsInstance = "none"
 reportMissingTypeStubs = "none"
@@ -33,15 +33,15 @@
 # Pytest - register custom markers
 [tool.pytest]
 addopts = "--strict-markers"
 
 # Yapf
 [tool.yapfignore]
 ignore_patterns = [
-    "databricks_genai/proto/**",
+    "databricks/proto/**",
     "notebooks",
 ]
 
 [tool.yapf]
 # Align closing bracket with visual indentation.
 align_closing_bracket_with_visual_indent = false
 
@@ -462,15 +462,14 @@
 fail-under=10.0
 
 # Files or directories to be skipped. They should be base names, not paths.
 ignore="CVS"
 
 # Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against paths and can be in Posix or Windows format.
-ignore-paths=["databricks_genai/proto/mint_pb2.py"]
 
 # Files or directories matching the regex patterns are skipped. The regex
 # matches against base names, not paths.
 ignore-patterns=""
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
```

### Comparing `databricks-genai-0.0.9/setup.py` & `databricks_genai-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,53 @@
-import setuptools
-from setuptools import setup
+from setuptools import find_packages, setup
 
 # pylint: disable-next=exec-used,consider-using-with
-exec(open('databricks_genai/version.py', 'r', encoding='utf-8').read())
+exec(open('databricks/model_training/version.py', 'r', encoding='utf-8').read())
 
 install_requires = [
-    'databricks-sdk>=0.14.0',
-    'typing_extensions>=4.7.1',
+    'backoff>=2.2.1',
+    'databricks-sdk==0.18.0',
+    'datasets>=2.16.1,<=2.17.0',
+    'gql[websockets]>=3.4.0',
+    'mlflow>=2.9.2,<=2.10.2',
     'mosaicml-cli==0.6.5',
-    'datasets>=2.16.1',
-    'mlflow>=2.9.2'
+    'requests>=2.26.0,<3',
+    'typing_extensions>=4.7.1',
+    'IPython>=8,<9'
 ]
 
 extra_deps = {}
 
 extra_deps['dev'] = [
     # 'build>=0.10.0',
     'isort>=5.9.3',
     'packaging>=21,<23',
+    'pre-commit>=2.17.0',
     'pylint>=3.0.0',
     'pyright==1.1.256',
     'pytest>=7.4.0',
     'yapf>=0.40.0',
     # 'twine>=4.0.2',
 ]
 
+
+extra_deps['notebook'] = ["ipywidgets>=8,<9"]
+
 extra_deps['all'] = set(dep for deps in extra_deps.values() for dep in deps)
 
 setup(
     name='databricks-genai',
     version=__version__,  # type: ignore pylint: disable=undefined-variable
     author='Databricks',
     author_email='genai-eng-team@databricks.com',
     description='Interact with the Databricks Generative AI APIs in python',
     url='https://docs.mosaicml.com/projects/mcli/en/latest/finetuning/finetuning.html',  # TODO: update with DBX docs
     include_package_data=True,
     package_data={},
-    packages=setuptools.find_packages(exclude=['tests']),
+    packages=find_packages(exclude=['tests']),
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
```

