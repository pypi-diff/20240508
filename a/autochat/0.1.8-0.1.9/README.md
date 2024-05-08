# Comparing `tmp/autochat-0.1.8.tar.gz` & `tmp/autochat-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autochat-0.1.8.tar", last modified: Mon Sep 11 05:35:08 2023, max compression
+gzip compressed data, was "autochat-0.1.9.tar", last modified: Thu Nov 16 16:37:38 2023, max compression
```

## Comparing `autochat-0.1.8.tar` & `autochat-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 SmileOS    (501) staff       (20)        0 2023-09-11 05:35:08.184156 autochat-0.1.8/
--rw-r--r--   0 SmileOS    (501) staff       (20)     3283 2023-09-11 05:35:08.184059 autochat-0.1.8/PKG-INFO
--rw-r--r--   0 SmileOS    (501) staff       (20)     2967 2023-09-11 05:33:54.000000 autochat-0.1.8/README.md
-drwxr-xr-x   0 SmileOS    (501) staff       (20)        0 2023-09-11 05:35:08.183416 autochat-0.1.8/autochat/
--rw-r--r--   0 SmileOS    (501) staff       (20)       23 2023-08-23 10:07:00.000000 autochat-0.1.8/autochat/__init__.py
--rw-r--r--   0 SmileOS    (501) staff       (20)    11172 2023-09-11 05:32:21.000000 autochat-0.1.8/autochat/chatgpt.py
--rw-r--r--   0 SmileOS    (501) staff       (20)     5985 2023-09-01 18:55:26.000000 autochat-0.1.8/autochat/test_utils.py
--rw-r--r--   0 SmileOS    (501) staff       (20)     3826 2023-09-05 08:50:13.000000 autochat-0.1.8/autochat/utils.py
-drwxr-xr-x   0 SmileOS    (501) staff       (20)        0 2023-09-11 05:35:08.183919 autochat-0.1.8/autochat.egg-info/
--rw-r--r--   0 SmileOS    (501) staff       (20)     3283 2023-09-11 05:35:08.000000 autochat-0.1.8/autochat.egg-info/PKG-INFO
--rw-r--r--   0 SmileOS    (501) staff       (20)      259 2023-09-11 05:35:08.000000 autochat-0.1.8/autochat.egg-info/SOURCES.txt
--rw-r--r--   0 SmileOS    (501) staff       (20)        1 2023-09-11 05:35:08.000000 autochat-0.1.8/autochat.egg-info/dependency_links.txt
--rw-r--r--   0 SmileOS    (501) staff       (20)       15 2023-09-11 05:35:08.000000 autochat-0.1.8/autochat.egg-info/requires.txt
--rw-r--r--   0 SmileOS    (501) staff       (20)        9 2023-09-11 05:35:08.000000 autochat-0.1.8/autochat.egg-info/top_level.txt
--rw-r--r--   0 SmileOS    (501) staff       (20)       38 2023-09-11 05:35:08.184190 autochat-0.1.8/setup.cfg
--rw-r--r--   0 SmileOS    (501) staff       (20)      473 2023-09-11 05:26:20.000000 autochat-0.1.8/setup.py
+drwxr-xr-x   0 SmileOS    (501) staff       (20)        0 2023-11-16 16:37:38.201025 autochat-0.1.9/
+-rw-r--r--   0 SmileOS    (501) staff       (20)     3276 2023-11-16 16:37:38.200821 autochat-0.1.9/PKG-INFO
+-rw-r--r--   0 SmileOS    (501) staff       (20)     2968 2023-11-16 16:36:50.000000 autochat-0.1.9/README.md
+drwxr-xr-x   0 SmileOS    (501) staff       (20)        0 2023-11-16 16:37:38.200008 autochat-0.1.9/autochat/
+-rw-r--r--   0 SmileOS    (501) staff       (20)       23 2023-08-23 10:07:00.000000 autochat-0.1.9/autochat/__init__.py
+-rw-r--r--   0 SmileOS    (501) staff       (20)    11216 2023-11-16 16:36:50.000000 autochat-0.1.9/autochat/chatgpt.py
+-rw-r--r--   0 SmileOS    (501) staff       (20)     5985 2023-09-01 18:55:26.000000 autochat-0.1.9/autochat/test_utils.py
+-rw-r--r--   0 SmileOS    (501) staff       (20)     3826 2023-09-05 08:50:13.000000 autochat-0.1.9/autochat/utils.py
+drwxr-xr-x   0 SmileOS    (501) staff       (20)        0 2023-11-16 16:37:38.200605 autochat-0.1.9/autochat.egg-info/
+-rw-r--r--   0 SmileOS    (501) staff       (20)     3276 2023-11-16 16:37:38.000000 autochat-0.1.9/autochat.egg-info/PKG-INFO
+-rw-r--r--   0 SmileOS    (501) staff       (20)      259 2023-11-16 16:37:38.000000 autochat-0.1.9/autochat.egg-info/SOURCES.txt
+-rw-r--r--   0 SmileOS    (501) staff       (20)        1 2023-11-16 16:37:38.000000 autochat-0.1.9/autochat.egg-info/dependency_links.txt
+-rw-r--r--   0 SmileOS    (501) staff       (20)       14 2023-11-16 16:37:38.000000 autochat-0.1.9/autochat.egg-info/requires.txt
+-rw-r--r--   0 SmileOS    (501) staff       (20)        9 2023-11-16 16:37:38.000000 autochat-0.1.9/autochat.egg-info/top_level.txt
+-rw-r--r--   0 SmileOS    (501) staff       (20)       38 2023-11-16 16:37:38.201071 autochat-0.1.9/setup.cfg
+-rw-r--r--   0 SmileOS    (501) staff       (20)      472 2023-11-16 16:36:50.000000 autochat-0.1.9/setup.py
```

### Comparing `autochat-0.1.8/PKG-INFO` & `autochat-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: autochat
-Version: 0.1.8
+Version: 0.1.9
 Summary: Small ChatGPT library to support chat templates, and function calls
 Home-page: https://github.com/benderv/autochat
 Author: Benjamin Derville
 Author-email: benderville@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: openai==1.3.0
 
-# AutoChat: Build Conversation AI with ease.
+# AutoChat
 
-## Description
+AutoChat is a lightweight interface to the ChatGPT API, to simplify the process of creating conversational agents.
 
-AutoChat simplifies the process of creating conversational agents by providing a lightweight interface to the OpenAI ChatGPT API:
-
-- **Message Class**: A simple class, `Message`, for sending and receiving messages within the conversation
+- **ChatGPT Class**: Conversation wrapper to store instruction, context and messages histories.
+- **Message Class**: Message wrapper to handle format/parsing automatically.
 - **Function Calls**: Capability to handle function calls within the conversation, allowing complex interactions and responses.
 - **Template System**: A straightforward text-based template system for defining the behavior of the chatbot, making it easy to customize its responses and actions.
 
 ## Installation
 
 To install the package, you can use pip:
 
@@ -112,9 +110,7 @@
 ## Support
 
 If you encounter any issues or have questions, please file an issue on the GitHub project page.
 
 ## License
 
 This project is licensed under the terms of the MIT license.
-
-
```

### Comparing `autochat-0.1.8/README.md` & `autochat-0.1.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# AutoChat: Build Conversation AI with ease.
+# AutoChat
 
-## Description
+AutoChat is a lightweight interface to the ChatGPT API, to simplify the process of creating conversational agents.
 
-AutoChat simplifies the process of creating conversational agents by providing a lightweight interface to the OpenAI ChatGPT API:
-
-- **Message Class**: A simple class, `Message`, for sending and receiving messages within the conversation
+- **ChatGPT Class**: Conversation wrapper to store instruction, context and messages histories.
+- **Message Class**: Message wrapper to handle format/parsing automatically.
 - **Function Calls**: Capability to handle function calls within the conversation, allowing complex interactions and responses.
 - **Template System**: A straightforward text-based template system for defining the behavior of the chatbot, making it easy to customize its responses and actions.
 
 ## Installation
 
 To install the package, you can use pip:
```

### Comparing `autochat-0.1.8/autochat/chatgpt.py` & `autochat-0.1.9/autochat/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 import json
 import os
 import typing
 
 import openai
-from tenacity import retry, stop_after_attempt, wait_random_exponential
+from openai import OpenAI
+from tenacity import (
+    retry,
+    retry_if_not_exception_type,
+    stop_after_attempt,
+    wait_random_exponential,
+)
 
 from autochat.utils import csv_dumps, parse_function
 
 # https://platform.openai.com/docs/models/gpt-4
 DEFAULT_MODEL = "gpt-4"
 OPENAI_MODEL = os.getenv("OPENAI_MODEL", DEFAULT_MODEL)
 
 
+client = OpenAI()
+
+
 class FunctionCallParsingError(Exception):
     def __init__(self, obj):
         self.obj = obj
 
     def __str__(self):
         return f"Invalid function_call: {self.obj.function_call}"
 
@@ -300,16 +309,18 @@
             )
             yield message
 
     @retry(
         stop=stop_after_attempt(4),
         wait=wait_random_exponential(multiplier=2, max=10),
         # If we get a context_length_exceeded error, we stop the conversation
-        retry=lambda x: isinstance(x, ContextLengthExceededError) is False
-        and isinstance(x, InvalidRequestError) is False,
+        retry=(
+            retry_if_not_exception_type(ContextLengthExceededError)
+            & retry_if_not_exception_type(InvalidRequestError)
+        ),
         # After 5 attempts, we throw the error
         reraise=True,
     )
     def fetch_openai(self):
         first_message = self.history[0].to_openai_dict()
         if self.context:
             first_message["content"] = self.context + "\n" + first_message["content"]
@@ -317,33 +328,31 @@
             [x.to_openai_dict() for x in self.pre_history]
             + [first_message]
             + [x.to_openai_dict() for x in self.history[1:]]
         )
 
         try:
             if self.functions_schema:
-                res = openai.ChatCompletion.create(
+                res = client.chat.completions.create(
                     model=OPENAI_MODEL,
                     messages=messages,
                     functions=self.functions_schema,
                 )
             else:
-                res = openai.ChatCompletion.create(
-                    model=OPENAI_MODEL,
-                    messages=messages,
+                res = client.chat.completions.create(
+                    model=OPENAI_MODEL, messages=messages
                 )
-        except openai.error.InvalidRequestError as e:
+        except openai.BadRequestError as e:
             if e.code == "context_length_exceeded":
                 raise ContextLengthExceededError(e)
             if e.code == "invalid_request_error":
                 raise InvalidRequestError(e)
-        except openai.error.APIError as e:
+        except openai.APIError as e:
             raise e
 
         message = res.choices[0].message
-        function_call = message.get("function_call")
         return Message.from_openai_dict(
             role=message.role,
             content=message.content,
-            function_call=function_call,
+            function_call=message.function_call,
             id=res.id,  # We use the response id as the message id
         )
```

### Comparing `autochat-0.1.8/autochat/test_utils.py` & `autochat-0.1.9/autochat/test_utils.py`

 * *Files identical despite different names*

### Comparing `autochat-0.1.8/autochat/utils.py` & `autochat-0.1.9/autochat/utils.py`

 * *Files identical despite different names*

### Comparing `autochat-0.1.8/autochat.egg-info/PKG-INFO` & `autochat-0.1.9/autochat.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: autochat
-Version: 0.1.8
+Version: 0.1.9
 Summary: Small ChatGPT library to support chat templates, and function calls
 Home-page: https://github.com/benderv/autochat
 Author: Benjamin Derville
 Author-email: benderville@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: openai==1.3.0
 
-# AutoChat: Build Conversation AI with ease.
+# AutoChat
 
-## Description
+AutoChat is a lightweight interface to the ChatGPT API, to simplify the process of creating conversational agents.
 
-AutoChat simplifies the process of creating conversational agents by providing a lightweight interface to the OpenAI ChatGPT API:
-
-- **Message Class**: A simple class, `Message`, for sending and receiving messages within the conversation
+- **ChatGPT Class**: Conversation wrapper to store instruction, context and messages histories.
+- **Message Class**: Message wrapper to handle format/parsing automatically.
 - **Function Calls**: Capability to handle function calls within the conversation, allowing complex interactions and responses.
 - **Template System**: A straightforward text-based template system for defining the behavior of the chatbot, making it easy to customize its responses and actions.
 
 ## Installation
 
 To install the package, you can use pip:
 
@@ -112,9 +110,7 @@
 ## Support
 
 If you encounter any issues or have questions, please file an issue on the GitHub project page.
 
 ## License
 
 This project is licensed under the terms of the MIT license.
-
-
```

