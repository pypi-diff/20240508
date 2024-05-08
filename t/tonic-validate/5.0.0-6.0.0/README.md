# Comparing `tmp/tonic_validate-5.0.0.tar.gz` & `tmp/tonic_validate-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_validate-5.0.0.tar", max compression
+gzip compressed data, was "tonic_validate-6.0.0.tar", max compression
```

## Comparing `tonic_validate-5.0.0.tar` & `tonic_validate-6.0.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0     1063 2024-04-30 02:42:36.442480 tonic_validate-5.0.0/LICENSE
--rw-r--r--   0        0        0    26128 2024-04-30 02:42:36.446480 tonic_validate-5.0.0/README.md
--rw-r--r--   0        0        0      854 2024-04-30 02:42:36.506479 tonic_validate-5.0.0/pyproject.toml
--rw-r--r--   0        0        0      459 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/__init__.py
--rw-r--r--   0        0        0      387 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/__init__.py
--rw-r--r--   0        0        0     2106 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/benchmark.py
--rw-r--r--   0        0        0      247 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/exceptions.py
--rw-r--r--   0        0        0     1023 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/llm_response.py
--rw-r--r--   0        0        0     2630 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/run.py
--rw-r--r--   0        0        0      314 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/classes/user_info.py
--rw-r--r--   0        0        0      805 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/config.py
--rw-r--r--   0        0        0     1483 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/__init__.py
--rw-r--r--   0        0        0     1693 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/answer_consistency_binary_metric.py
--rw-r--r--   0        0        0     2077 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/answer_consistency_metric.py
--rw-r--r--   0        0        0     2878 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/answer_contains_pii_metric.py
--rw-r--r--   0        0        0     1369 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/answer_match_metric.py
--rw-r--r--   0        0        0     1837 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/answer_similarity_metric.py
--rw-r--r--   0        0        0     1952 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/augmentation_accuracy_metric.py
--rw-r--r--   0        0        0     2442 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/augmentation_precision_metric.py
--rw-r--r--   0        0        0     1556 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/binary_metric.py
--rw-r--r--   0        0        0     1834 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/contains_text_metric.py
--rw-r--r--   0        0        0     2902 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/context_contains_pii_metric.py
--rw-r--r--   0        0        0     1880 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/context_length_metric.py
--rw-r--r--   0        0        0     1264 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/duplication_metric.py
--rw-r--r--   0        0        0     1185 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/hate_speech_content_metric.py
--rw-r--r--   0        0        0     1285 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/latency_metric.py
--rw-r--r--   0        0        0      819 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/metric.py
--rw-r--r--   0        0        0     1351 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/regex_metric.py
--rw-r--r--   0        0        0     1542 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/response_length_metric.py
--rw-r--r--   0        0        0     1903 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/metrics/retrieval_precision_metric.py
--rw-r--r--   0        0        0     5882 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/services/litellm_service.py
--rw-r--r--   0        0        0     4737 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/services/openai_service.py
--rw-r--r--   0        0        0    18492 2024-04-30 02:42:36.510480 tonic_validate-5.0.0/tonic_validate/tests/test_scorer.py
--rw-r--r--   0        0        0        0 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/__init__.py
--rw-r--r--   0        0        0     2880 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/http_client.py
--rw-r--r--   0        0        0      527 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/llm_cache.py
--rw-r--r--   0        0        0    19347 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/llm_calls.py
--rw-r--r--   0        0        0     2198 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/metrics_util.py
--rw-r--r--   0        0        0     4961 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/utils/telemetry.py
--rw-r--r--   0        0        0     4431 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/validate_api.py
--rw-r--r--   0        0        0    13685 2024-04-30 02:42:36.514479 tonic_validate-5.0.0/tonic_validate/validate_scorer.py
--rw-r--r--   0        0        0    27006 1970-01-01 00:00:00.000000 tonic_validate-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-08 13:45:12.264462 tonic_validate-6.0.0/LICENSE
+-rw-r--r--   0        0        0    26140 2024-05-08 13:45:12.264462 tonic_validate-6.0.0/README.md
+-rw-r--r--   0        0        0      854 2024-05-08 13:45:12.328462 tonic_validate-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0      535 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/__init__.py
+-rw-r--r--   0        0        0      387 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/classes/__init__.py
+-rw-r--r--   0        0        0     2106 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/classes/benchmark.py
+-rw-r--r--   0        0        0      247 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/classes/exceptions.py
+-rw-r--r--   0        0        0     1023 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/classes/llm_response.py
+-rw-r--r--   0        0        0     2630 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/classes/run.py
+-rw-r--r--   0        0        0      314 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/classes/user_info.py
+-rw-r--r--   0        0        0      805 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/config.py
+-rw-r--r--   0        0        0     1525 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/__init__.py
+-rw-r--r--   0        0        0     2055 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/answer_consistency_binary_metric.py
+-rw-r--r--   0        0        0     2371 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/answer_consistency_metric.py
+-rw-r--r--   0        0        0     3366 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/answer_contains_pii_metric.py
+-rw-r--r--   0        0        0     1934 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/answer_match_metric.py
+-rw-r--r--   0        0        0     2207 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/answer_similarity_metric.py
+-rw-r--r--   0        0        0     2279 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/augmentation_accuracy_metric.py
+-rw-r--r--   0        0        0     2758 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/augmentation_precision_metric.py
+-rw-r--r--   0        0        0     1881 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/binary_metric.py
+-rw-r--r--   0        0        0     2392 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/contains_text_metric.py
+-rw-r--r--   0        0        0     3392 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/context_contains_pii_metric.py
+-rw-r--r--   0        0        0     2448 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/context_length_metric.py
+-rw-r--r--   0        0        0     1553 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/duplication_metric.py
+-rw-r--r--   0        0        0     1510 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/hate_speech_content_metric.py
+-rw-r--r--   0        0        0     1653 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/latency_metric.py
+-rw-r--r--   0        0        0     1408 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/metric.py
+-rw-r--r--   0        0        0     1902 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/regex_metric.py
+-rw-r--r--   0        0        0     2110 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/response_length_metric.py
+-rw-r--r--   0        0        0     2226 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/metrics/retrieval_precision_metric.py
+-rw-r--r--   0        0        0     5882 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/services/litellm_service.py
+-rw-r--r--   0        0        0     4737 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/services/openai_service.py
+-rw-r--r--   0        0        0    18492 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/tests/test_scorer.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/utils/__init__.py
+-rw-r--r--   0        0        0     2880 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/utils/http_client.py
+-rw-r--r--   0        0        0      527 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/utils/llm_cache.py
+-rw-r--r--   0        0        0    19347 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/utils/llm_calls.py
+-rw-r--r--   0        0        0     2198 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/utils/metrics_util.py
+-rw-r--r--   0        0        0     4961 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/utils/telemetry.py
+-rw-r--r--   0        0        0     4431 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/validate_api.py
+-rw-r--r--   0        0        0     3287 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/validate_monitorer.py
+-rw-r--r--   0        0        0    14239 2024-05-08 13:45:12.332462 tonic_validate-6.0.0/tonic_validate/validate_scorer.py
+-rw-r--r--   0        0        0    27018 1970-01-01 00:00:00.000000 tonic_validate-6.0.0/PKG-INFO
```

### Comparing `tonic_validate-5.0.0/LICENSE` & `tonic_validate-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/README.md` & `tonic_validate-6.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -293,18 +293,18 @@
 ```python
 import os
 os.environ["OPENAI_API_KEY"] = "put-your-openai-api-key-here"
 ```
 If you already have the `OPENAI_API_KEY` set in your system's environment variables then you can skip this step. Otherwise, please set the environment variable before proceeding.
 
 ##### Using Azure
-If you are using Azure, instead of setting the `OPENAI_API_KEY` environment variable, you instead need to set `AZURE_OPENAI_KEY` and `AZURE_OPENAI_ENDPOINT`. `AZURE_OPENAI_ENDPOINT` is the endpoint url for your Azure OpenAI deployment and `AZURE_OPENAI_KEY` is your API key.
+If you are using Azure, instead of setting the `OPENAI_API_KEY` environment variable, you instead need to set `AZURE_OPENAI_API_KEY` and `AZURE_OPENAI_ENDPOINT`. `AZURE_OPENAI_ENDPOINT` is the endpoint url for your Azure OpenAI deployment and `AZURE_OPENAI_API_KEY` is your API key.
 ```python
 import os
-os.environ["AZURE_OPENAI_KEY"] = "put-your-azure-openai-api-key-here"
+os.environ["AZURE_OPENAI_API_KEY"] = "put-your-azure-openai-api-key-here"
 os.environ["AZURE_OPENAI_ENDPOINT"] = "put-your-azure-endpoint-here"
 ```
 
 #### Using Gemini
 If you already have the `GEMINI_API_KEY` set in your system's environment variables then you can skip this step. Otherwise, please set the environment variable before proceeding.
 ```python
 import os
```

### Comparing `tonic_validate-5.0.0/pyproject.toml` & `tonic_validate-6.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tonic-validate"
-version = "5.0.0"
+version = "6.0.0"
 description = "RAG evaluation metrics."
 authors = ["Joe Ferrara <joeferrara@tonic.ai>", "Ethan Philpott <ephilpott@tonic.ai>", "Adam Kamor <adam@tonic.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 openai = ">=1.0.0"
@@ -16,15 +16,15 @@
 typing-extensions = "^4.10.0"
 litellm = "^1.35.8"
 google-generativeai = { version = "^0.5.2", python = ">=3.9" }
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^7.0.0"
 sphinx-rtd-theme = ">=1.2,<3.0"
-ruff = ">=0.1.15,<0.4.0"
+ruff = ">=0.1.15,<0.5.0"
 tonic-textual = "^1.0.5"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `tonic_validate-5.0.0/tonic_validate/classes/benchmark.py` & `tonic_validate-6.0.0/tonic_validate/classes/benchmark.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/classes/llm_response.py` & `tonic_validate-6.0.0/tonic_validate/classes/llm_response.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/classes/run.py` & `tonic_validate-6.0.0/tonic_validate/classes/run.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/config.py` & `tonic_validate-6.0.0/tonic_validate/config.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/__init__.py` & `tonic_validate-6.0.0/tonic_validate/metrics/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .duplication_metric import DuplicationMetric
 from .regex_metric import RegexMetric
 from .response_length_metric import ResponseLengthMetric
 from .hate_speech_content_metric import HateSpeechContentMetric
 from .latency_metric import LatencyMetric
 from .context_contains_pii_metric import ContextContainsPiiMetric
 from .answer_contains_pii_metric import AnswerContainsPiiMetric
+from .metric import Metric
 
 __all__ = [
     "AnswerConsistencyBinaryMetric",
     "AnswerConsistencyMetric",
     "AnswerSimilarityMetric",
     "AugmentationAccuracyMetric",
     "AugmentationPrecisionMetric",
@@ -29,9 +30,10 @@
     "ContextLengthMetric",
     "DuplicationMetric",
     "RegexMetric",
     "ResponseLengthMetric",
     "HateSpeechContentMetric",
     "LatencyMetric",
     "ContextContainsPiiMetric",
-    "AnswerContainsPiiMetric"
+    "AnswerContainsPiiMetric",
+    "Metric",
 ]
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/answer_consistency_binary_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/answer_consistency_binary_metric.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 import logging
-from typing import Union
+from typing import Any, Dict, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
+from tonic_validate.metrics.metric import Metric, MetricRequirement
 from tonic_validate.utils.metrics_util import parse_boolean_response
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
-from tonic_validate.utils.llm_calls import answer_consistent_with_context_call, context_consistency_prompt
+from tonic_validate.utils.llm_calls import (
+    answer_consistent_with_context_call,
+    context_consistency_prompt,
+)
 
 logger = logging.getLogger()
 
 
 class AnswerConsistencyBinaryMetric(BinaryMetric):
     name: str = "answer_consistency_binary"
     prompt: str = context_consistency_prompt()
+    requirements = {MetricRequirement.LLM_ANSWER, MetricRequirement.LLM_CONTEXT}
 
     def __init__(self):
         """
         Binary metric that checks whether there is information in the LLM answer that does not come from the context.
         Returns either 1 (consistent) or 0 (inconsistent).
         """
         super().__init__(self.name, self.metric_callback)
 
+    def serialize_config(self):
+        return {}
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return AnswerConsistencyBinaryMetric()
+
     async def metric_callback(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> bool:
         """Check if answer is consistent with context.
 
         Parameters
         ----------
         llm_response: LLMResponse
             The response from the LLM system.
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/answer_consistency_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/augmentation_accuracy_metric.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 import logging
-from typing import Union
+from typing import Any, Dict, List, Tuple, Union
 from tonic_validate.classes.llm_response import LLMResponse
-from tonic_validate.metrics.metric import Metric
-from tonic_validate.utils.metrics_util import (
-    parse_boolean_response,
-    parse_bullet_list_response,
-)
+from tonic_validate.metrics.metric import Metric, MetricRequirement
+from tonic_validate.utils.metrics_util import parse_boolean_response
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
 from tonic_validate.utils.llm_calls import (
-    main_points_call,
-    statement_derived_from_context_call,
-    statement_derived_from_context_prompt,
-    main_points_prompt,
+    answer_contains_context_call,
+    answer_contains_context_prompt,
 )
 
 logger = logging.getLogger()
 
 
-class AnswerConsistencyMetric(Metric):
-    name: str = "answer_consistency"
-    prompt: str = (
-        "-------------------\n"
-        f"{main_points_prompt()}\n"
-        "-------------------\n"
-        f"{statement_derived_from_context_prompt(statement='EXAMPLE STATEMENT', context_list=[])}\n"
-        "-------------------\n"
-    )
+class AugmentationAccuracyMetric(Metric):
+    name: str = "augmentation_accuracy"
+    prompt: str = answer_contains_context_prompt()
+    requirements = {MetricRequirement.LLM_ANSWER, MetricRequirement.LLM_CONTEXT}
 
     def __init__(self):
         """
-        Metric that checks whether the LLM answer contains information that does not come from the context.
-        Returns a float between 0 and 1, where 1 is completely consistent and 0 is completely inconsistent.
+        Metric that checks whether the LLM answer includes all of the context.
+        Returns a float between 0 and 1. 1 indicates that the answer contains all of the context. 0 indicates that it contains none of the context.
         """
         pass
 
+    def serialize_config(self):
+        return {}
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return AugmentationAccuracyMetric()
+
     async def score(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> float:
-        main_points_response = await main_points_call(
-            llm_response.llm_answer, llm_service
-        )
-        main_point_list = parse_bullet_list_response(main_points_response)
-        main_point_derived_from_context_list = []
-        for main_point in main_point_list:
-            statement_derived_from_context_response = (
-                await statement_derived_from_context_call(
-                    main_point, llm_response.llm_context_list, llm_service
-                )
+        return (await self.calculate_metric(llm_response, llm_service))[0]
+
+    async def calculate_metric(
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
+    ) -> Tuple[float, List[bool]]:
+        contains_context_list: List[bool] = []
+        if len(llm_response.llm_context_list) == 0:
+            raise ValueError(
+                "No context provided, cannot calculate augmentation accuracy"
+            )
+        for context in llm_response.llm_context_list:
+            contains_context_response = await answer_contains_context_call(
+                llm_response.llm_answer, context, llm_service
             )
-            main_point_derived_from_context_list.append(
-                parse_boolean_response(statement_derived_from_context_response)
+            contains_context_list.append(
+                parse_boolean_response(contains_context_response)
             )
-        return sum(main_point_derived_from_context_list) / len(main_point_list)
+
+        score = sum(contains_context_list) / len(contains_context_list)
+        return (score, contains_context_list)
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/answer_contains_pii_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/context_contains_pii_metric.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,74 @@
 import os
 import requests
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
+from tonic_validate.metrics.metric import Metric, MetricRequirement
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
 
 
-class AnswerContainsPiiMetric(BinaryMetric):
+class ContextContainsPiiMetric(BinaryMetric):
+    requirements = {MetricRequirement.LLM_CONTEXT}
+
     def __init__(self, pii_types: List[str], textual_api_key: Optional[str] = None):
         """
-        Checks to see if PII is contained in the RAG provided answer.  The types of PII looked for are found in the pii_types list.
+        Checks to see if PII is contained in the RAG provided context.  The types of PII looked for are found in the pii_types list.
 
         Parameters
         ----------
         pii_types: List[str]
-        The list of PII types which are looked for in the RAG answer.  The list of possible options are those available in via tonic-textual. Using this Metric requries a Tonic Textual API key.
+        The list of PII types which are looked for in the RAG context.  The list of possible options are those available in via tonic-textual. Using this Metric requries a Tonic Textual API key.
         You can create an API key for free at at https://textual.tonic.ai.  You can pass your API key into this constructor OR set TONIC_TEXTUAL_API_KEY in your ENVIRONMENT.
 
         textual_api_key: Optional[str]
         Your Textual API key.  This value is optional. It is preferred that you set TONIC_TEXTUAL_API_KEY via your ENVIRONMENT.
 
         """
         try:
             from tonic_textual.api import TonicTextual  # type: ignore
         except ImportError:
             raise ImportError(
-                "You must install tonic-textual to use the AnswerContainsPiiMetric. You can install it via pip: pip install tonic-textual"
+                "You must install tonic-textual to use the ContextContainsPiiMetric. You can install it via pip: pip install tonic-textual"
             )
         self.pii_types = [p.lower() for p in pii_types]
         if textual_api_key is None:
             if os.getenv("TONIC_TEXTUAL_API_KEY") is None:
                 raise ValueError(
                     "You must set TONIC_TEXTUAL_API_KEY in your ENV or pass your Textual API key into the constructor."
                 )
             self.textual = TonicTextual("https://textual.tonic.ai")
         else:
             self.textual = TonicTextual("https://textual.tonic.ai", textual_api_key)
 
-        super().__init__("answer_contains_pii", self.metric_callback)
+        super().__init__("context_contains_pii", self.metric_callback)
+
+    def serialize_config(self):
+        return {"pii_types": self.pii_types, "textual_api_key": self.textual.api_key}
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return ContextContainsPiiMetric(
+            pii_types=config["pii_types"],
+            textual_api_key=config["textual_api_key"],
+        )
 
     def metric_callback(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> bool:
         try:
-            response = self.textual.redact(llm_response.llm_answer)
+            response = self.textual.redact("\n".join(llm_response.llm_context_list))
             for d in response.de_identify_results:
                 if d.label.lower() in self.pii_types:
                     return True
             return False
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == 401:
                 raise ValueError(
-                    "Cannot compute AnswerContainsPiiMetric. Your Textual API Key is INVALID."
+                    "Cannot compute ContextContainsPiiMetric. Your Textual API Key is INVALID."
                 )
         raise ValueError(
-            "Cannot compute AnswerContainsPiiMetric. Error occured communicating with Textual.  Please try again later or reach out via GitHub issues."
+            "Cannot compute ContextContainsPiiMetric. Error occured communicating with Textual.  Please try again later or reach out via GitHub issues."
         )
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/answer_match_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/answer_match_metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import logging
 
-from typing import Union
+from typing import Any, Dict, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
+from tonic_validate.metrics.metric import Metric, MetricRequirement
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class AnswerMatchMetric(BinaryMetric):
+    requirements = {MetricRequirement.LLM_ANSWER}
+
     def __init__(self, name: str, answer: str, case_sensitive: bool = False):
         """
         Create a metric that checks if the answer matches a given string.
         Returns 1 (True) if the LLM response matches the given string. Returns 0 (False) if the response does not match.
 
         Parameters
         ----------
@@ -24,13 +27,30 @@
         case_sensitive: bool
             If True, the comparison will be case sensitive
         """
         super().__init__(name, self.metric_callback)
         self.answer = answer
         self.case_sensitive = case_sensitive
 
+    def serialize_config(self):
+        return {
+            "name": self.name,
+            "answer": self.answer,
+            "case_sensitive": self.case_sensitive,
+        }
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return AnswerMatchMetric(
+            name=config["name"],
+            answer=config["answer"],
+            case_sensitive=config["case_sensitive"],
+        )
+
     def metric_callback(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> bool:
         if self.case_sensitive:
             return self.answer == llm_response.llm_answer
         return self.answer.lower() == llm_response.llm_answer.lower()
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/answer_similarity_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/answer_similarity_metric.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,48 @@
 import logging
-from typing import Union
+from typing import Any, Dict, Union
 from tonic_validate.classes.llm_response import LLMResponse
-from tonic_validate.metrics.metric import Metric
+from tonic_validate.metrics.metric import Metric, MetricRequirement
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
-from tonic_validate.utils.llm_calls import similarity_score_call, similarity_score_prompt
+from tonic_validate.utils.llm_calls import (
+    similarity_score_call,
+    similarity_score_prompt,
+)
 
 logger = logging.getLogger()
 
 
 class AnswerSimilarityMetric(Metric):
     name: str = "answer_similarity"
     prompt: str = similarity_score_prompt()
+    requirements = {
+        MetricRequirement.QUESTION,
+        MetricRequirement.REFERENCE_ANSWER,
+        MetricRequirement.LLM_ANSWER,
+    }
 
     def __init__(self) -> None:
         """
         Metric that checks how well the reference answer matches the LLM answer.
         Returns a float between 0 and 5, where 5 is the most similar and 0 is the least similar.
         """
         pass
 
+    def serialize_config(self):
+        return {}
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return AnswerSimilarityMetric()
+
     async def score(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> float:
         # Check that the benchmark item has an answer
         if llm_response.benchmark_item.answer is None:
             raise ValueError("The benchmark item does not have an answer")
 
         similarity_score_response = await similarity_score_call(
             llm_response.benchmark_item.question,
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/augmentation_precision_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/augmentation_precision_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 import logging
-from typing import List, Union
+from typing import Any, Dict, List, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.augmentation_accuracy_metric import (
     AugmentationAccuracyMetric,
 )
 from tonic_validate.metrics.metric import Metric
 from tonic_validate.metrics.retrieval_precision_metric import RetrievalPrecisionMetric
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class AugmentationPrecisionMetric(Metric):
     name: str = "augmentation_precision"
+    requirements = AugmentationAccuracyMetric.requirements.union(
+        RetrievalPrecisionMetric.requirements
+    )
 
     def __init__(self) -> None:
         """
         Metric that checks whether the LLM answer contains the relevant context.
         Returns a float between 0 and 1. 1 indicates that the answer contains all of the relevant context. 0 indicates that it contains none of the relevant context.
         """
         self.augmentation_accuracy = AugmentationAccuracyMetric()
         self.retrieval_precision = RetrievalPrecisionMetric()
 
+    def serialize_config(self):
+        return {}
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return AugmentationPrecisionMetric()
+
     async def score(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> float:
         retrieval_precision_score = await self.retrieval_precision.calculate_metric(
             llm_response, llm_service
         )
         context_relevant_list = retrieval_precision_score[1]
         augmentation_accuracy_score = await self.augmentation_accuracy.calculate_metric(
             llm_response, llm_service
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/binary_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/response_length_metric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,63 @@
 import logging
-from typing import Awaitable, Callable, Union
+from typing import Any, Dict, Optional, Union
 
 from tonic_validate.classes.llm_response import LLMResponse
-from tonic_validate.metrics.metric import Metric
+from tonic_validate.metrics.binary_metric import BinaryMetric
+from tonic_validate.metrics.metric import Metric, MetricRequirement
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
-import inspect
 
 logger = logging.getLogger()
 
 
-class BinaryMetric(Metric):
-    @property
-    def name(self) -> str:
-        return self._name
+class ResponseLengthMetric(BinaryMetric):
+    requirements = {MetricRequirement.LLM_ANSWER}
 
     def __init__(
         self,
         name: str,
-        callback: Callable[[LLMResponse, Union[LiteLLMService, OpenAIService]], Union[Awaitable[bool], bool]],
+        min_length: Optional[int] = None,
+        max_length: Optional[int] = None,
     ):
         """
-        Create a binary metric with a name and a callback. A binary metric returns either True (1) or False (0).
+        Creates a binary metric that checks whether the LLM response length falls within a given range.
+        Returns 1 (True) if the length is within the range. Returns 0 (False) if the length falls outside of the range.
 
         Parameters
         ----------
         name: str
             The name of the metric that displays in the UI
-        callback: Callable[[LLMResponse, OpenAIService], Union[Awaitable[bool], bool]]
-            The callback that takes an LLMResponse and an OpenAIService and returns a boolean.
-            The callback can be either an async function or a regular function.
+        min_length: Optional[int]
+            The minimum length of the LLM response
+        max_length: Optional[int]
+            The maximum length of the LLM response
         """
+        super().__init__(name, self.metric_callback)
+        self.min_length = min_length
+        self.max_length = max_length
+
+    def serialize_config(self):
+        return {
+            "name": self.name,
+            "min_length": self.min_length,
+            "max_length": self.max_length,
+        }
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return ResponseLengthMetric(
+            name=config["name"],
+            min_length=config["min_length"],
+            max_length=config["max_length"],
+        )
 
-        self._name = name
-        self.callback = callback
-
-    async def score(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
-    ) -> float:
-        if inspect.iscoroutinefunction(self.callback):
-            result = await self.callback(llm_response, llm_service)
-        else:
-            result = self.callback(llm_response, llm_service)
-        return 1.0 if result else 0.0
+    def metric_callback(
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
+    ) -> bool:
+        if self.min_length and len(llm_response.llm_answer) < self.min_length:
+            return False
+        if self.max_length and len(llm_response.llm_answer) > self.max_length:
+            return False
+        return True
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/contains_text_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/contains_text_metric.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import logging
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
+from tonic_validate.metrics.metric import Metric, MetricRequirement
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class ContainsTextMetric(BinaryMetric):
     """Checks whether or not response contains the given text."""
 
+    requirements = {MetricRequirement.LLM_ANSWER}
+
     def __init__(
         self,
         name: str,
         text: Union[str, List[str]],
         case_sensitive: Optional[bool] = False,
     ):
         """
@@ -31,16 +34,33 @@
         case_sensitive: Optional[bool]
             If True, the comparison will be case sensitive
         """
         super().__init__(name, self.metric_callback)
         self.text = text
         self.case_sensitive = case_sensitive
 
+    def serialize_config(self):
+        return {
+            "name": self.name,
+            "text": self.text,
+            "case_sensitive": self.case_sensitive,
+        }
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return ContainsTextMetric(
+            name=config["name"],
+            text=config["text"],
+            case_sensitive=config["case_sensitive"],
+        )
+
     def metric_callback(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> bool:
         if isinstance(self.text, list):
             return all(self.contains_text(llm_response, text) for text in self.text)
         return self.contains_text(llm_response, self.text)
 
     def contains_text(self, llm_response: LLMResponse, text_to_find: str) -> bool:
         if self.case_sensitive:
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/context_contains_pii_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/answer_contains_pii_metric.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,74 @@
 import os
 import requests
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
+from tonic_validate.metrics.metric import Metric, MetricRequirement
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
 
 
-class ContextContainsPiiMetric(BinaryMetric):
+class AnswerContainsPiiMetric(BinaryMetric):
+    requirements = {MetricRequirement.LLM_ANSWER}
+
     def __init__(self, pii_types: List[str], textual_api_key: Optional[str] = None):
         """
-        Checks to see if PII is contained in the RAG provided context.  The types of PII looked for are found in the pii_types list.
+        Checks to see if PII is contained in the RAG provided answer.  The types of PII looked for are found in the pii_types list.
 
         Parameters
         ----------
         pii_types: List[str]
-        The list of PII types which are looked for in the RAG context.  The list of possible options are those available in via tonic-textual. Using this Metric requries a Tonic Textual API key.
+        The list of PII types which are looked for in the RAG answer.  The list of possible options are those available in via tonic-textual. Using this Metric requries a Tonic Textual API key.
         You can create an API key for free at at https://textual.tonic.ai.  You can pass your API key into this constructor OR set TONIC_TEXTUAL_API_KEY in your ENVIRONMENT.
 
         textual_api_key: Optional[str]
         Your Textual API key.  This value is optional. It is preferred that you set TONIC_TEXTUAL_API_KEY via your ENVIRONMENT.
 
         """
         try:
             from tonic_textual.api import TonicTextual  # type: ignore
         except ImportError:
             raise ImportError(
-                "You must install tonic-textual to use the ContextContainsPiiMetric. You can install it via pip: pip install tonic-textual"
+                "You must install tonic-textual to use the AnswerContainsPiiMetric. You can install it via pip: pip install tonic-textual"
             )
         self.pii_types = [p.lower() for p in pii_types]
         if textual_api_key is None:
             if os.getenv("TONIC_TEXTUAL_API_KEY") is None:
                 raise ValueError(
                     "You must set TONIC_TEXTUAL_API_KEY in your ENV or pass your Textual API key into the constructor."
                 )
             self.textual = TonicTextual("https://textual.tonic.ai")
         else:
             self.textual = TonicTextual("https://textual.tonic.ai", textual_api_key)
 
-        super().__init__("context_contains_pii", self.metric_callback)
+        super().__init__("answer_contains_pii", self.metric_callback)
+
+    def serialize_config(self):
+        return {"pii_types": self.pii_types, "textual_api_key": self.textual.api_key}
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return AnswerContainsPiiMetric(
+            pii_types=config["pii_types"],
+            textual_api_key=config["textual_api_key"],
+        )
 
     def metric_callback(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> bool:
         try:
-            response = self.textual.redact("\n".join(llm_response.llm_context_list))
+            response = self.textual.redact(llm_response.llm_answer)
             for d in response.de_identify_results:
                 if d.label.lower() in self.pii_types:
                     return True
             return False
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == 401:
                 raise ValueError(
-                    "Cannot compute ContextContainsPiiMetric. Your Textual API Key is INVALID."
+                    "Cannot compute AnswerContainsPiiMetric. Your Textual API Key is INVALID."
                 )
         raise ValueError(
-            "Cannot compute ContextContainsPiiMetric. Error occured communicating with Textual.  Please try again later or reach out via GitHub issues."
+            "Cannot compute AnswerContainsPiiMetric. Error occured communicating with Textual.  Please try again later or reach out via GitHub issues."
         )
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/context_length_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/context_length_metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import logging
-from typing import Optional, Union
+from typing import Any, Dict, Optional, Union
 
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
+from tonic_validate.metrics.metric import Metric, MetricRequirement
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class ContextLengthMetric(BinaryMetric):
     """Checks that context length is within a certain range."""
 
+    requirements = {MetricRequirement.LLM_CONTEXT}
+
     def __init__(
         self,
         name: str,
         min_length: Optional[int] = None,
         max_length: Optional[int] = None,
     ):
         """
@@ -31,16 +34,33 @@
         max_length: Optional[int]
             The maximum length of the context
         """
         super().__init__(name, self.metric_callback)
         self.min_length = min_length
         self.max_length = max_length
 
+    def serialize_config(self):
+        return {
+            "name": self.name,
+            "min_length": self.min_length,
+            "max_length": self.max_length,
+        }
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return ContextLengthMetric(
+            name=config["name"],
+            min_length=config["min_length"],
+            max_length=config["max_length"],
+        )
+
     def metric_callback(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> bool:
         # For all items in the context list, check if the length is within the min and max length
         return all(
             self.check_context_length(context)
             for context in llm_response.llm_context_list
         )
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/duplication_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/duplication_metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 import logging
 
-from typing import Union
+from typing import Any, Dict, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
+from tonic_validate.metrics.metric import Metric, MetricRequirement
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
-from tonic_validate.utils.llm_calls import contains_duplicate_information, contains_duplicate_info_prompt
+from tonic_validate.utils.llm_calls import (
+    contains_duplicate_information,
+    contains_duplicate_info_prompt,
+)
 from tonic_validate.utils.metrics_util import parse_boolean_response
 
 logger = logging.getLogger()
 
 
 class DuplicationMetric(BinaryMetric):
     name: str = "duplication_metric"
     prompt: str = contains_duplicate_info_prompt()
+    requirements = {MetricRequirement.LLM_ANSWER}
 
     def __init__(self):
         """
         Binary metric that checks whether the response contains duplicate information.
         Returns 1 (True) if the response contains duplicate information. Returns 0 (False) if it does not contain duplicate information.
         """
         super().__init__(self.name, self.metric_callback)
 
+    def serialize_config(self):
+        return {}
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return DuplicationMetric()
+
     async def metric_callback(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> bool:
         return parse_boolean_response(
-            await contains_duplicate_information(
-                llm_response.llm_answer, llm_service
-            )
+            await contains_duplicate_information(llm_response.llm_answer, llm_service)
         )
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/hate_speech_content_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/hate_speech_content_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 import logging
 
-from typing import Union
+from typing import Any, Dict, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
+from tonic_validate.metrics.metric import Metric, MetricRequirement
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
-from tonic_validate.utils.llm_calls import contains_hate_speech, contains_hate_speech_prompt
+from tonic_validate.utils.llm_calls import (
+    contains_hate_speech,
+    contains_hate_speech_prompt,
+)
 from tonic_validate.utils.metrics_util import parse_boolean_response
 
 logger = logging.getLogger()
 
 
 class HateSpeechContentMetric(BinaryMetric):
     name: str = "hate_speech_content"
     prompt: str = contains_hate_speech_prompt()
+    requirements = {MetricRequirement.LLM_ANSWER}
 
     def __init__(self):
         """
         Binary metric that checks whether the response contains hate speech.
         Returns 1 (True) if the response contains hate speech. Returns 0 (False) if it does not contain hate speech.
         """
         super().__init__(self.name, self.metric_callback)
 
+    def serialize_config(self):
+        return {}
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return HateSpeechContentMetric()
+
     async def metric_callback(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> bool:
         return parse_boolean_response(
             await contains_hate_speech(llm_response.llm_answer, llm_service)
         )
```

### Comparing `tonic_validate-5.0.0/tonic_validate/metrics/latency_metric.py` & `tonic_validate-6.0.0/tonic_validate/metrics/latency_metric.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 import logging
-from typing import Union
+from typing import Any, Dict, Union
 from tonic_validate.classes.llm_response import LLMResponse
 from tonic_validate.metrics.binary_metric import BinaryMetric
+from tonic_validate.metrics.metric import Metric, MetricRequirement
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
 
 logger = logging.getLogger()
 
 
 class LatencyMetric(BinaryMetric):
     name: str = "latency_metric"
+    requirements = {MetricRequirement.LLM_RUN_TIME}
 
     def __init__(self, target_time: float = 5.0) -> None:
         """
         Measures how long it takes for the LLM to complete a request.
         Returns 0.0 if the LLM takes longer than the target time, and 1.0 otherwise.
 
         Parameters
         ----------
         target_time: float
             The target time for the model to complete the request in seconds.
         """
         self.target_time = target_time
 
+    def serialize_config(self):
+        return {"target_time": self.target_time}
+
+    @staticmethod
+    def from_config(config: Dict[str, Any]) -> Metric:
+        return LatencyMetric(target_time=config["target_time"])
+
     # We do async here for consistency even though this method doesn't use async
     async def score(
-        self, llm_response: LLMResponse, llm_service: Union[LiteLLMService, OpenAIService]
+        self,
+        llm_response: LLMResponse,
+        llm_service: Union[LiteLLMService, OpenAIService],
     ) -> float:
         # Check that llm_response.run_time is not None
         if llm_response.run_time is None:
             raise ValueError("No run time provided in LLMResponse")
         if llm_response.run_time > self.target_time:
             return 0.0
         return 1.0
```

### Comparing `tonic_validate-5.0.0/tonic_validate/services/litellm_service.py` & `tonic_validate-6.0.0/tonic_validate/services/litellm_service.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/services/openai_service.py` & `tonic_validate-6.0.0/tonic_validate/services/openai_service.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/tests/test_scorer.py` & `tonic_validate-6.0.0/tonic_validate/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/utils/http_client.py` & `tonic_validate-6.0.0/tonic_validate/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/utils/llm_cache.py` & `tonic_validate-6.0.0/tonic_validate/utils/llm_cache.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/utils/llm_calls.py` & `tonic_validate-6.0.0/tonic_validate/utils/llm_calls.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/utils/metrics_util.py` & `tonic_validate-6.0.0/tonic_validate/utils/metrics_util.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/utils/telemetry.py` & `tonic_validate-6.0.0/tonic_validate/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/validate_api.py` & `tonic_validate-6.0.0/tonic_validate/validate_api.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-5.0.0/tonic_validate/validate_scorer.py` & `tonic_validate-6.0.0/tonic_validate/validate_scorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 from asyncio import Semaphore
 import asyncio
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
-from typing import Awaitable, Callable, DefaultDict, List, Dict, Union
+from typing import Any, Awaitable, Callable, DefaultDict, List, Dict, Type, Union
 
 from pydantic import ConfigDict, TypeAdapter, validate_call
 from tonic_validate.classes.benchmark import Benchmark, BenchmarkItem
 import logging
 from tonic_validate.classes.exceptions import LLMException
 
 from tonic_validate.classes.llm_response import CallbackLLMResponse, LLMResponse
 from tonic_validate.classes.run import Run, RunData
-from tonic_validate.metrics.answer_consistency_metric import AnswerConsistencyMetric
-from tonic_validate.metrics.answer_similarity_metric import AnswerSimilarityMetric
-from tonic_validate.metrics.augmentation_precision_metric import (
-    AugmentationPrecisionMetric,
-)
-
-from tonic_validate.metrics.metric import Metric
+import tonic_validate.metrics as tonic_metrics
 from tonic_validate.services.openai_service import OpenAIService
 from tonic_validate.services.litellm_service import LiteLLMService
 import tiktoken
 from tonic_validate.utils.telemetry import Telemetry
 from tqdm.asyncio import tqdm as async_tqdm
 from tqdm import tqdm
 import time
 
 logger = logging.getLogger()
 CallbackValidator = TypeAdapter(CallbackLLMResponse)
 
+# Gets a list of all the metric names
+metric_dict: Dict[str, Type[tonic_metrics.Metric]] = {}
+for metric in tonic_metrics.__all__:
+    cls = getattr(tonic_metrics, metric)
+    if not issubclass(cls, tonic_metrics.Metric):
+        continue
+    try:
+        metric_dict[cls.__name__] = cls
+    except AttributeError:
+        print(f"The Metric {metric} does not have a '__name__' attribute.")
+
 
 class ValidateScorer:
     DEFAULT_PARALLELISM_CALLBACK = 1
     DEFAULT_PARALLELISM_SCORING = 50
 
     @validate_call(config=ConfigDict(arbitrary_types_allowed=True))
     def __init__(
         self,
-        metrics: List[Metric] = [
-            AnswerSimilarityMetric(),
-            AugmentationPrecisionMetric(),
-            AnswerConsistencyMetric(),
+        metrics: List[tonic_metrics.Metric] = [
+            tonic_metrics.AnswerSimilarityMetric(),
+            tonic_metrics.AugmentationPrecisionMetric(),
+            tonic_metrics.AnswerConsistencyMetric(),
         ],
         model_evaluator: str = "gpt-4-turbo-preview",
         max_parsing_retries: int = 3,
         max_llm_retries: int = 10,
         fail_on_error: bool = False,
         quiet: bool = False,
     ):
@@ -362,7 +367,16 @@
                     total=len(benchmark.items),
                     desc="Retrieving responses",
                     disable=self.quiet,
                 )
             )
 
         return self.score_responses(responses, scoring_parallelism)
+
+    @staticmethod
+    def metric_config_to_list(config: Dict[str, Dict[str, Any]]):
+        metrics: List[tonic_metrics.Metric] = []
+        for metric in config:
+            if metric not in metric_dict:
+                raise Exception(f"Metric {metric} not found.")
+            metrics.append(metric_dict[metric].from_config(config[metric]))
+        return metrics
```

### Comparing `tonic_validate-5.0.0/PKG-INFO` & `tonic_validate-6.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic-validate
-Version: 5.0.0
+Version: 6.0.0
 Summary: RAG evaluation metrics.
 Author: Joe Ferrara
 Author-email: joeferrara@tonic.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -316,18 +316,18 @@
 ```python
 import os
 os.environ["OPENAI_API_KEY"] = "put-your-openai-api-key-here"
 ```
 If you already have the `OPENAI_API_KEY` set in your system's environment variables then you can skip this step. Otherwise, please set the environment variable before proceeding.
 
 ##### Using Azure
-If you are using Azure, instead of setting the `OPENAI_API_KEY` environment variable, you instead need to set `AZURE_OPENAI_KEY` and `AZURE_OPENAI_ENDPOINT`. `AZURE_OPENAI_ENDPOINT` is the endpoint url for your Azure OpenAI deployment and `AZURE_OPENAI_KEY` is your API key.
+If you are using Azure, instead of setting the `OPENAI_API_KEY` environment variable, you instead need to set `AZURE_OPENAI_API_KEY` and `AZURE_OPENAI_ENDPOINT`. `AZURE_OPENAI_ENDPOINT` is the endpoint url for your Azure OpenAI deployment and `AZURE_OPENAI_API_KEY` is your API key.
 ```python
 import os
-os.environ["AZURE_OPENAI_KEY"] = "put-your-azure-openai-api-key-here"
+os.environ["AZURE_OPENAI_API_KEY"] = "put-your-azure-openai-api-key-here"
 os.environ["AZURE_OPENAI_ENDPOINT"] = "put-your-azure-endpoint-here"
 ```
 
 #### Using Gemini
 If you already have the `GEMINI_API_KEY` set in your system's environment variables then you can skip this step. Otherwise, please set the environment variable before proceeding.
 ```python
 import os
```

