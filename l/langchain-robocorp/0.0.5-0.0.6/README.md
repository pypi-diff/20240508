# Comparing `tmp/langchain_robocorp-0.0.5.tar.gz` & `tmp/langchain_robocorp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_robocorp-0.0.5.tar", max compression
+gzip compressed data, was "langchain_robocorp-0.0.6.tar", max compression
```

## Comparing `langchain_robocorp-0.0.5.tar` & `langchain_robocorp-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-04-01 18:34:48.983729 langchain_robocorp-0.0.5/LICENSE
--rw-r--r--   0        0        0      420 2024-04-01 18:34:48.983729 langchain_robocorp-0.0.5/README.md
--rw-r--r--   0        0        0      102 2024-04-01 18:34:48.983729 langchain_robocorp-0.0.5/langchain_robocorp/__init__.py
--rw-r--r--   0        0        0     4568 2024-04-01 18:34:48.987729 langchain_robocorp-0.0.5/langchain_robocorp/_common.py
--rw-r--r--   0        0        0      525 2024-04-01 18:34:48.987729 langchain_robocorp-0.0.5/langchain_robocorp/_prompts.py
--rw-r--r--   0        0        0        0 2024-04-01 18:34:48.987729 langchain_robocorp-0.0.5/langchain_robocorp/py.typed
--rw-r--r--   0        0        0     7573 2024-04-01 18:34:48.987729 langchain_robocorp-0.0.5/langchain_robocorp/toolkits.py
--rw-r--r--   0        0        0     2552 2024-04-01 18:34:48.987729 langchain_robocorp-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 langchain_robocorp-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/LICENSE
+-rw-r--r--   0        0        0      420 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/README.md
+-rw-r--r--   0        0        0      102 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/langchain_robocorp/__init__.py
+-rw-r--r--   0        0        0     4568 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/langchain_robocorp/_common.py
+-rw-r--r--   0        0        0      525 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/langchain_robocorp/_prompts.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/langchain_robocorp/py.typed
+-rw-r--r--   0        0        0     7500 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/langchain_robocorp/toolkits.py
+-rw-r--r--   0        0        0     2552 2024-05-08 20:17:39.401467 langchain_robocorp-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 langchain_robocorp-0.0.6/PKG-INFO
```

### Comparing `langchain_robocorp-0.0.5/LICENSE` & `langchain_robocorp-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.5/langchain_robocorp/_common.py` & `langchain_robocorp-0.0.6/langchain_robocorp/_common.py`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.5/langchain_robocorp/_prompts.py` & `langchain_robocorp-0.0.6/langchain_robocorp/_prompts.py`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.5/langchain_robocorp/toolkits.py` & `langchain_robocorp-0.0.6/langchain_robocorp/toolkits.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     model_to_dict,
     reduce_openapi_spec,
 )
 from langchain_robocorp._prompts import (
     API_CONTROLLER_PROMPT,
 )
 
-MAX_RESPONSE_LENGTH = 5000
 LLM_TRACE_HEADER = "X-action-trace"
 
 
 class RunDetailsCallbackHandler(BaseCallbackHandler):
     """Callback handler to add run details to the run."""
 
     def __init__(self, run_details: dict) -> None:
@@ -237,10 +236,9 @@
                     headers[LLM_TRACE_HEADER] = run.url
         except Exception:
             pass
 
         url = urljoin(self.url, endpoint)
 
         response = requests.post(url, headers=headers, data=json.dumps(data))
-        output = response.text[:MAX_RESPONSE_LENGTH]
 
-        return output
+        return response.text
```

### Comparing `langchain_robocorp-0.0.5/pyproject.toml` & `langchain_robocorp-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-robocorp"
-version = "0.0.5"
+version = "0.0.6"
 description = "An integration package connecting Robocorp Action Server and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_robocorp-0.0.5/PKG-INFO` & `langchain_robocorp-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-robocorp
-Version: 0.0.5
+Version: 0.0.6
 Summary: An integration package connecting Robocorp Action Server and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

