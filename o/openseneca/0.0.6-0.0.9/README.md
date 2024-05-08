# Comparing `tmp/openseneca-0.0.6.tar.gz` & `tmp/openseneca-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openseneca-0.0.6.tar", last modified: Tue Apr 30 15:15:07 2024, max compression
+gzip compressed data, was "openseneca-0.0.9.tar", last modified: Wed May  8 14:48:42 2024, max compression
```

## Comparing `openseneca-0.0.6.tar` & `openseneca-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,57 @@
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.494617 openseneca-0.0.6/
--rw-r--r--   0 otto       (501) staff       (20)      828 2024-04-30 15:15:07.494346 openseneca-0.0.6/PKG-INFO
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.490557 openseneca-0.0.6/openseneca/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/__init__.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.491613 openseneca-0.0.6/openseneca/classify/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:02.000000 openseneca-0.0.6/openseneca/classify/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     1967 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/classify/categories.py
--rw-r--r--   0 otto       (501) staff       (20)     2950 2024-04-30 14:01:40.000000 openseneca-0.0.6/openseneca/classify/llm.py
--rw-r--r--   0 otto       (501) staff       (20)      386 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/classify/static.py
--rw-r--r--   0 otto       (501) staff       (20)     1306 2024-04-28 17:17:13.000000 openseneca-0.0.6/openseneca/config.yml
--rw-r--r--   0 otto       (501) staff       (20)     1478 2024-04-30 14:58:39.000000 openseneca-0.0.6/openseneca/costs.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.492202 openseneca-0.0.6/openseneca/interfaces/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:56.000000 openseneca-0.0.6/openseneca/interfaces/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     3398 2024-04-30 14:58:10.000000 openseneca-0.0.6/openseneca/interfaces/models.py
--rw-r--r--   0 otto       (501) staff       (20)      844 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/interfaces/providers.py
--rw-r--r--   0 otto       (501) staff       (20)     1021 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/interfaces/response.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.493228 openseneca-0.0.6/openseneca/models/
--rw-r--r--   0 otto       (501) staff       (20)      612 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     1900 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/cohere.py
--rw-r--r--   0 otto       (501) staff       (20)      983 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/gpt3.py
--rw-r--r--   0 otto       (501) staff       (20)      974 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/gpt4.py
--rw-r--r--   0 otto       (501) staff       (20)     3134 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/llama2.py
--rw-r--r--   0 otto       (501) staff       (20)     2160 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/llama3.py
--rw-r--r--   0 otto       (501) staff       (20)     1034 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/mistral.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.493442 openseneca-0.0.6/openseneca/providers/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:49.000000 openseneca-0.0.6/openseneca/providers/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     5297 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/providers/azure.py
--rw-r--r--   0 otto       (501) staff       (20)   222818 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/router.pk
--rw-r--r--   0 otto       (501) staff       (20)     5111 2024-04-30 14:56:41.000000 openseneca-0.0.6/openseneca/router.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.493864 openseneca-0.0.6/openseneca/utils/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:18.000000 openseneca-0.0.6/openseneca/utils/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     1799 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/utils/inspection.py
--rw-r--r--   0 otto       (501) staff       (20)     2715 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/utils/logger.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.494036 openseneca-0.0.6/openseneca.egg-info/
--rw-r--r--   0 otto       (501) staff       (20)      828 2024-04-30 15:15:07.000000 openseneca-0.0.6/openseneca.egg-info/PKG-INFO
--rw-r--r--   0 otto       (501) staff       (20)      887 2024-04-30 15:15:07.000000 openseneca-0.0.6/openseneca.egg-info/SOURCES.txt
--rw-r--r--   0 otto       (501) staff       (20)        1 2024-04-30 15:15:07.000000 openseneca-0.0.6/openseneca.egg-info/dependency_links.txt
--rw-r--r--   0 otto       (501) staff       (20)      322 2024-04-30 15:15:07.000000 openseneca-0.0.6/openseneca.egg-info/requires.txt
--rw-r--r--   0 otto       (501) staff       (20)       11 2024-04-30 15:15:07.000000 openseneca-0.0.6/openseneca.egg-info/top_level.txt
--rw-r--r--   0 otto       (501) staff       (20)       38 2024-04-30 15:15:07.494660 openseneca-0.0.6/setup.cfg
--rw-r--r--   0 otto       (501) staff       (20)      852 2024-04-30 15:15:05.000000 openseneca-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:48:42.431146 openseneca-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-08 14:46:01.000000 openseneca-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-08 14:48:42.431146 openseneca-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-08 14:46:01.000000 openseneca-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:48:42.423146 openseneca-0.0.9/openseneca/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:48:42.427147 openseneca-0.0.9/openseneca/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/classify/categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/classify/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/classify/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/costs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:48:42.427147 openseneca-0.0.9/openseneca/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/interfaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/interfaces/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/interfaces/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:48:42.427147 openseneca-0.0.9/openseneca/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/models/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/models/gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/models/gpt4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/models/llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/models/llama3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/models/mistral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:48:42.427147 openseneca-0.0.9/openseneca/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/providers/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:48:42.431146 openseneca-0.0.9/openseneca/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/utils/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-08 14:46:01.000000 openseneca-0.0.9/openseneca/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)   384383 2024-05-08 14:48:39.000000 openseneca-0.0.9/openseneca/weights.pk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:48:42.431146 openseneca-0.0.9/openseneca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-08 14:48:42.000000 openseneca-0.0.9/openseneca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-08 14:48:42.000000 openseneca-0.0.9/openseneca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:48:42.000000 openseneca-0.0.9/openseneca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 14:48:42.000000 openseneca-0.0.9/openseneca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 14:48:42.000000 openseneca-0.0.9/openseneca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:48:42.431146 openseneca-0.0.9/ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:46:01.000000 openseneca-0.0.9/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17576 2024-05-08 14:46:01.000000 openseneca-0.0.9/ranking/battle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 14:46:01.000000 openseneca-0.0.9/ranking/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-08 14:46:01.000000 openseneca-0.0.9/ranking/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-08 14:46:01.000000 openseneca-0.0.9/ranking/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:48:42.431146 openseneca-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-08 14:46:01.000000 openseneca-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:48:42.431146 openseneca-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:46:01.000000 openseneca-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-08 14:46:01.000000 openseneca-0.0.9/tests/_dummies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-08 14:46:01.000000 openseneca-0.0.9/tests/test_gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-08 14:46:01.000000 openseneca-0.0.9/tests/test_gpt4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-08 14:46:01.000000 openseneca-0.0.9/tests/test_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-08 14:46:01.000000 openseneca-0.0.9/tests/test_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-08 14:46:01.000000 openseneca-0.0.9/tests/test_mistral.py
```

### Comparing `openseneca-0.0.6/openseneca/classify/categories.py` & `openseneca-0.0.9/openseneca/classify/categories.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/classify/llm.py` & `openseneca-0.0.9/openseneca/classify/llm.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/config.yml` & `openseneca-0.0.9/openseneca/config.yml`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/costs.py` & `openseneca-0.0.9/openseneca/costs.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/interfaces/models.py` & `openseneca-0.0.9/openseneca/interfaces/models.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/interfaces/response.py` & `openseneca-0.0.9/openseneca/interfaces/response.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/models/__init__.py` & `openseneca-0.0.9/openseneca/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/models/cohere.py` & `openseneca-0.0.9/openseneca/models/cohere.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/models/gpt3.py` & `openseneca-0.0.9/openseneca/models/gpt3.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/models/gpt4.py` & `openseneca-0.0.9/openseneca/models/gpt4.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/models/llama2.py` & `openseneca-0.0.9/openseneca/models/llama2.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/models/llama3.py` & `openseneca-0.0.9/openseneca/models/llama3.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/models/mistral.py` & `openseneca-0.0.9/openseneca/models/mistral.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/providers/azure.py` & `openseneca-0.0.9/openseneca/providers/azure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from math import cos
 from openseneca.interfaces.providers import BaseProvider
 from openseneca.interfaces.response import ProviderResponse
 from openseneca.utils.logger import Logger
 from openseneca.costs import CostCalculator
 from typing import Generator
-import http.client
-import logging
 import requests
 import time
 import json
 
 # ----------------------------
 # TODO, make this configurable.
 # Enable debug output in the http.client module
@@ -22,22 +20,14 @@
 # requests_log.propagate = True
 # ----------------------------
 
 
 logger = Logger()
 
 class AzureProvider(BaseProvider):
-  def __init__(self, stream: bool = False):
-    """
-    Initializes an instance of the Azure class.
-
-    Args:
-      stream (bool, optional): Whether to enable streaming. Defaults to False.
-    """
-    self.stream = stream
 
   def request(self,
          endpoint: str,
          authentication_header: dict = None,
          body: dict = None,
          content_type: str = 'application/json',
          ) -> Generator[ProviderResponse, None, None]:
@@ -72,29 +62,32 @@
     logger.info(f"Is streaming: {stream}")
 
     if stream:
       body.update({
         "stream": stream
       })
 
+    # Retry the request up to 3 times.
     retry_attempts = 3
-    retry_delay = 5
+    # Wait 10 seconds before retrying, just to try to avoid rate limiting.
+    retry_delay = 10
+
     costs_calulator = CostCalculator(self.llm_name)
 
     for attempt in range(retry_attempts):
       logger.debug(f"Sending request to {endpoint}")
       logger.debug(f"Body: {body}")
       logger.debug(f"Attempt {attempt + 1} of {retry_attempts}")
       try:
 
         response = requests.post(
           endpoint,
           json=body,
           headers=headers,
-          timeout=120,  # TODO: Make this configurable
+          timeout=self.timeout,
           stream=stream
         )
 
         if stream:
           json_object = {}
           # Process the response in chunks
           for chunk in response.iter_lines():
@@ -122,15 +115,14 @@
                   yield ProviderResponse(200, {}, json.dumps(json_object))
                 except json.JSONDecodeError:
                   pass  # silence, it's an empty response.
             logger.debug(f"Chunk: {chunk}")
           time.sleep(0.1)
 
         else:  # not streaming, just return the entire response
-          logger.info('not streaming')
           json_object = json.loads(response.text)
           if json_object and 'usage' in json_object:
             _usage = json_object['usage']
             logger.info(f"Usage: {_usage}")
 
             costs = costs_calulator.calculate(
               _usage['prompt_tokens'],
@@ -141,27 +133,30 @@
               response.status_code,
               response.headers,
               response.text,
               cost=costs
             )
 
           else:
-            # mh?
             final_response = ProviderResponse(
               response.status_code,
               response.headers,
               response.text,
             )
 
           logger.debug(f"Response: {final_response}")
           if 'error' in json.loads(final_response.content):
             logger.error(f"Error in response: {final_response.content}")
             yield ProviderResponse(0, {}, "{}")
 
           yield final_response
       except requests.exceptions.Timeout:
-        if attempt < retry_attempts - 1:
+        if attempt < (retry_attempts - 1):
+          logger.error(f"Request timed out. Retrying in {retry_delay}s...")
           time.sleep(retry_delay)
+          continue # retry
         else:
+          logger.error("Request timed out. No more retries. " \
+            "Emitting empty response.")
           yield ProviderResponse(0, {}, "{}")
 
-      return
+    return
```

### Comparing `openseneca-0.0.6/openseneca/router.py` & `openseneca-0.0.9/openseneca/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,17 +115,17 @@
   #     top_p = filtered_df.iloc[0]['top_p']
   #   except (ValueError, IndexError):
   #     return self.default_model, 0.5, 0.92
 
   #   return best_model, temperature, top_p
 
 
-router_path = os.path.dirname(os.path.abspath(__file__)) + '/router.pk'
+router_path = os.path.dirname(os.path.abspath(__file__)) + '/weights.pk'
 if not os.path.exists(router_path):
-  router_pk_path = pkg_resources.resource_filename('openseneca', 'router.pk')
+  router_pk_path = pkg_resources.resource_filename('openseneca', 'weights.pk')
 router = Router(router_path)
 
 class Prompt:
   messages: List[Dict[Any, Any]]
   user_prompt: str
   language: str
   label: str
```

### Comparing `openseneca-0.0.6/openseneca/utils/inspection.py` & `openseneca-0.0.9/openseneca/utils/inspection.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.6/openseneca/utils/logger.py` & `openseneca-0.0.9/openseneca/utils/logger.py`

 * *Files identical despite different names*

