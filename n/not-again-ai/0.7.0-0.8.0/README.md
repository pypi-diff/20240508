# Comparing `tmp/not_again_ai-0.7.0.tar.gz` & `tmp/not_again_ai-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not_again_ai-0.7.0.tar", max compression
+gzip compressed data, was "not_again_ai-0.8.0.tar", max compression
```

## Comparing `not_again_ai-0.7.0.tar` & `not_again_ai-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1071 2024-01-28 17:31:42.037063 not_again_ai-0.7.0/LICENSE
--rw-r--r--   0        0        0    12588 2024-05-05 20:32:34.349097 not_again_ai-0.7.0/README.md
--rw-r--r--   0        0        0     4258 2024-05-05 20:20:05.431962 not_again_ai-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.7.0/src/not_again_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 01:25:46.292824 not_again_ai-0.7.0/src/not_again_ai/base/__init__.py
--rw-r--r--   0        0        0      949 2024-05-05 19:23:23.729901 not_again_ai-0.7.0/src/not_again_ai/base/file_system.py
--rw-r--r--   0        0        0     3448 2023-10-22 01:25:46.292824 not_again_ai-0.7.0/src/not_again_ai/base/parallel.py
--rw-r--r--   0        0        0      451 2024-04-20 17:53:46.881490 not_again_ai-0.7.0/src/not_again_ai/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 23:24:18.378976 not_again_ai-0.7.0/src/not_again_ai/llm/ollama/__init__.py
--rw-r--r--   0        0        0     3682 2024-05-05 15:31:46.904124 not_again_ai-0.7.0/src/not_again_ai/llm/ollama/chat_completion.py
--rw-r--r--   0        0        0      765 2024-05-05 17:54:10.555899 not_again_ai-0.7.0/src/not_again_ai/llm/ollama/ollama_client.py
--rw-r--r--   0        0        0     2900 2024-05-05 15:41:24.299807 not_again_ai-0.7.0/src/not_again_ai/llm/ollama/service.py
--rw-r--r--   0        0        0        0 2024-05-05 15:59:08.566121 not_again_ai-0.7.0/src/not_again_ai/llm/openai/__init__.py
--rw-r--r--   0        0        0     8623 2024-05-05 16:51:37.036182 not_again_ai-0.7.0/src/not_again_ai/llm/openai/chat_completion.py
--rw-r--r--   0        0        0     3431 2024-05-05 16:01:20.819891 not_again_ai-0.7.0/src/not_again_ai/llm/openai/context_management.py
--rw-r--r--   0        0        0     2500 2024-01-29 00:33:04.305624 not_again_ai-0.7.0/src/not_again_ai/llm/openai/embeddings.py
--rw-r--r--   0        0        0     2470 2024-01-28 00:29:53.278594 not_again_ai-0.7.0/src/not_again_ai/llm/openai/openai_client.py
--rw-r--r--   0        0        0     7094 2024-04-20 19:17:25.528556 not_again_ai-0.7.0/src/not_again_ai/llm/openai/prompts.py
--rw-r--r--   0        0        0     4301 2024-04-20 19:20:27.986968 not_again_ai-0.7.0/src/not_again_ai/llm/openai/tokens.py
--rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.7.0/src/not_again_ai/py.typed
--rw-r--r--   0        0        0      466 2024-04-20 17:53:46.881490 not_again_ai-0.7.0/src/not_again_ai/statistics/__init__.py
--rw-r--r--   0        0        0     4429 2024-01-28 00:06:13.617140 not_again_ai-0.7.0/src/not_again_ai/statistics/dependence.py
--rw-r--r--   0        0        0      447 2024-04-20 17:53:46.881490 not_again_ai-0.7.0/src/not_again_ai/viz/__init__.py
--rw-r--r--   0        0        0     3382 2023-11-19 21:07:35.038071 not_again_ai-0.7.0/src/not_again_ai/viz/barplots.py
--rw-r--r--   0        0        0     4354 2023-10-22 01:25:46.292824 not_again_ai-0.7.0/src/not_again_ai/viz/distributions.py
--rw-r--r--   0        0        0     2290 2023-10-22 01:25:46.292824 not_again_ai-0.7.0/src/not_again_ai/viz/scatterplot.py
--rw-r--r--   0        0        0     5212 2024-01-27 23:36:54.323725 not_again_ai-0.7.0/src/not_again_ai/viz/time_series.py
--rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.7.0/src/not_again_ai/viz/utils.py
--rw-r--r--   0        0        0    14203 1970-01-01 00:00:00.000000 not_again_ai-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-28 17:31:42.037063 not_again_ai-0.8.0/LICENSE
+-rw-r--r--   0        0        0    12588 2024-05-06 13:18:28.310413 not_again_ai-0.8.0/README.md
+-rw-r--r--   0        0        0     4258 2024-05-08 00:01:11.052089 not_again_ai-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.8.0/src/not_again_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 01:25:46.292824 not_again_ai-0.8.0/src/not_again_ai/base/__init__.py
+-rw-r--r--   0        0        0      949 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/base/file_system.py
+-rw-r--r--   0        0        0     3448 2023-10-22 01:25:46.292824 not_again_ai-0.8.0/src/not_again_ai/base/parallel.py
+-rw-r--r--   0        0        0      451 2024-04-20 17:53:46.881490 not_again_ai-0.8.0/src/not_again_ai/llm/__init__.py
+-rw-r--r--   0        0        0     3070 2024-05-07 13:02:01.955836 not_again_ai-0.8.0/src/not_again_ai/llm/chat_completion.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/ollama/__init__.py
+-rw-r--r--   0        0        0     3682 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/ollama/chat_completion.py
+-rw-r--r--   0        0        0      765 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/ollama/ollama_client.py
+-rw-r--r--   0        0        0     2900 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/ollama/service.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/__init__.py
+-rw-r--r--   0        0        0     8623 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/chat_completion.py
+-rw-r--r--   0        0        0     3435 2024-05-06 13:37:12.093962 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/context_management.py
+-rw-r--r--   0        0        0     2500 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/embeddings.py
+-rw-r--r--   0        0        0     2470 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/openai_client.py
+-rw-r--r--   0        0        0     7094 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/prompts.py
+-rw-r--r--   0        0        0     4301 2024-05-06 13:18:28.322414 not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/tokens.py
+-rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.8.0/src/not_again_ai/py.typed
+-rw-r--r--   0        0        0      466 2024-04-20 17:53:46.881490 not_again_ai-0.8.0/src/not_again_ai/statistics/__init__.py
+-rw-r--r--   0        0        0     4429 2024-01-28 00:06:13.617140 not_again_ai-0.8.0/src/not_again_ai/statistics/dependence.py
+-rw-r--r--   0        0        0      447 2024-04-20 17:53:46.881490 not_again_ai-0.8.0/src/not_again_ai/viz/__init__.py
+-rw-r--r--   0        0        0     3382 2023-11-19 21:07:35.038071 not_again_ai-0.8.0/src/not_again_ai/viz/barplots.py
+-rw-r--r--   0        0        0     4354 2023-10-22 01:25:46.292824 not_again_ai-0.8.0/src/not_again_ai/viz/distributions.py
+-rw-r--r--   0        0        0     2290 2023-10-22 01:25:46.292824 not_again_ai-0.8.0/src/not_again_ai/viz/scatterplot.py
+-rw-r--r--   0        0        0     5212 2024-01-27 23:36:54.323725 not_again_ai-0.8.0/src/not_again_ai/viz/time_series.py
+-rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.8.0/src/not_again_ai/viz/utils.py
+-rw-r--r--   0        0        0    14203 1970-01-01 00:00:00.000000 not_again_ai-0.8.0/PKG-INFO
```

### Comparing `not_again_ai-0.7.0/LICENSE` & `not_again_ai-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/README.md` & `not_again_ai-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/pyproject.toml` & `not_again_ai-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "not-again-ai"
-version = "0.7.0"
+version = "0.8.0"
 description = "Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place."
 authors = ["DaveCoDev <dave.co.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/DaveCoDev/not-again-ai"
 documentation = "https://github.com/DaveCoDev/not-again-ai"
 classifiers = [
```

### Comparing `not_again_ai-0.7.0/src/not_again_ai/base/file_system.py` & `not_again_ai-0.8.0/src/not_again_ai/base/file_system.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/base/parallel.py` & `not_again_ai-0.8.0/src/not_again_ai/base/parallel.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/llm/ollama/chat_completion.py` & `not_again_ai-0.8.0/src/not_again_ai/llm/ollama/chat_completion.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/llm/ollama/ollama_client.py` & `not_again_ai-0.8.0/src/not_again_ai/llm/ollama/ollama_client.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/llm/ollama/service.py` & `not_again_ai-0.8.0/src/not_again_ai/llm/ollama/service.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/llm/openai/chat_completion.py` & `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/chat_completion.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/llm/openai/context_management.py` & `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/context_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 
-from not_again_ai.llm.openai.tokens import num_tokens_from_messages, truncate_str
+from not_again_ai.llm.openai_api.tokens import num_tokens_from_messages, truncate_str
 
 
 def _inject_variable(
     messages_unformatted: list[dict[str, str]], variable_name: str, variable_text: str
 ) -> list[dict[str, str]]:
     """Injects variables into the messages using Python string formatting."""
     messages_formatted = copy.deepcopy(messages_unformatted)
```

### Comparing `not_again_ai-0.7.0/src/not_again_ai/llm/openai/embeddings.py` & `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/embeddings.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/llm/openai/openai_client.py` & `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/openai_client.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/llm/openai/prompts.py` & `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/prompts.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/llm/openai/tokens.py` & `not_again_ai-0.8.0/src/not_again_ai/llm/openai_api/tokens.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/statistics/dependence.py` & `not_again_ai-0.8.0/src/not_again_ai/statistics/dependence.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/viz/barplots.py` & `not_again_ai-0.8.0/src/not_again_ai/viz/barplots.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/viz/distributions.py` & `not_again_ai-0.8.0/src/not_again_ai/viz/distributions.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/viz/scatterplot.py` & `not_again_ai-0.8.0/src/not_again_ai/viz/scatterplot.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/src/not_again_ai/viz/time_series.py` & `not_again_ai-0.8.0/src/not_again_ai/viz/time_series.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.7.0/PKG-INFO` & `not_again_ai-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not-again-ai
-Version: 0.7.0
+Version: 0.8.0
 Summary: Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place.
 Home-page: https://github.com/DaveCoDev/not-again-ai
 License: MIT
 Author: DaveCoDev
 Author-email: dave.co.dev@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Development Status :: 3 - Alpha
```

