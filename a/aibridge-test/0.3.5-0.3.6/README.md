# Comparing `tmp/aibridge_test-0.3.5.tar.gz` & `tmp/aibridge_test-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.3.5.tar", last modified: Wed May  8 11:30:07 2024, max compression
+gzip compressed data, was "aibridge_test-0.3.6.tar", last modified: Wed May  8 12:11:11 2024, max compression
```

## Comparing `aibridge_test-0.3.5.tar` & `aibridge_test-0.3.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 11:30:07.461558 aibridge_test-0.3.5/
-drwxrwxrwx   0        0        0        0 2024-05-08 11:30:06.940559 aibridge_test-0.3.5/AIBridge/
--rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.3.5/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 11:30:07.107596 aibridge_test-0.3.5/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     9364 2024-04-19 04:13:29.000000 aibridge_test-0.3.5/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0    13743 2024-05-08 11:06:06.000000 aibridge_test-0.3.5/AIBridge/ai_services/anthropic_ai.py
--rw-rw-rw-   0        0        0    12317 2024-04-19 04:14:01.000000 aibridge_test-0.3.5/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    14692 2024-05-08 11:27:54.000000 aibridge_test-0.3.5/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.3.5/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    11902 2024-04-19 04:13:01.000000 aibridge_test-0.3.5/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.3.5/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     9249 2024-04-19 04:14:42.000000 aibridge_test-0.3.5/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.3.5/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-05-08 11:30:07.128561 aibridge_test-0.3.5/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     7755 2024-04-16 09:20:57.000000 aibridge_test-0.3.5/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.3.5/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-05-08 11:30:07.166557 aibridge_test-0.3.5/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-08 11:30:07.210559 aibridge_test-0.3.5/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.3.5/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-08 11:30:07.231556 aibridge_test-0.3.5/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.3.5/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.3.5/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-05-08 11:30:07.252593 aibridge_test-0.3.5/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-05-08 11:30:07.298567 aibridge_test-0.3.5/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.3.5/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-04-16 09:21:15.000000 aibridge_test-0.3.5/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/LICENSE
--rw-rw-rw-   0        0        0    21534 2024-05-08 11:30:07.451558 aibridge_test-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 11:30:07.445573 aibridge_test-0.3.5/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21534 2024-05-08 11:30:06.000000 aibridge_test-0.3.5/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2024-05-08 11:30:06.000000 aibridge_test-0.3.5/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 11:30:06.000000 aibridge_test-0.3.5/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2024-05-08 11:30:06.000000 aibridge_test-0.3.5/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 11:30:06.000000 aibridge_test-0.3.5/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 11:30:07.461558 aibridge_test-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     2863 2024-05-08 11:28:48.000000 aibridge_test-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:11:11.092936 aibridge_test-0.3.6/
+drwxrwxrwx   0        0        0        0 2024-05-08 12:11:10.448939 aibridge_test-0.3.6/AIBridge/
+-rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.3.6/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:11:10.580950 aibridge_test-0.3.6/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     9364 2024-04-19 04:13:29.000000 aibridge_test-0.3.6/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0    13992 2024-05-08 12:10:07.000000 aibridge_test-0.3.6/AIBridge/ai_services/anthropic_ai.py
+-rw-rw-rw-   0        0        0    12317 2024-04-19 04:14:01.000000 aibridge_test-0.3.6/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    14692 2024-05-08 11:27:54.000000 aibridge_test-0.3.6/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.3.6/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11902 2024-04-19 04:13:01.000000 aibridge_test-0.3.6/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.3.6/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9249 2024-04-19 04:14:42.000000 aibridge_test-0.3.6/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.3.6/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:11:10.596942 aibridge_test-0.3.6/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     7755 2024-04-16 09:20:57.000000 aibridge_test-0.3.6/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.3.6/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:11:10.629936 aibridge_test-0.3.6/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:11:10.652944 aibridge_test-0.3.6/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.3.6/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:11:10.699937 aibridge_test-0.3.6/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.3.6/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.3.6/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:11:10.764936 aibridge_test-0.3.6/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:11:10.832936 aibridge_test-0.3.6/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.3.6/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-04-16 09:21:15.000000 aibridge_test-0.3.6/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0    21534 2024-05-08 12:11:11.090938 aibridge_test-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 12:11:11.080940 aibridge_test-0.3.6/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21534 2024-05-08 12:11:10.000000 aibridge_test-0.3.6/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-05-08 12:11:10.000000 aibridge_test-0.3.6/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 12:11:10.000000 aibridge_test-0.3.6/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2024-05-08 12:11:10.000000 aibridge_test-0.3.6/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 12:11:10.000000 aibridge_test-0.3.6/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 12:11:11.093938 aibridge_test-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     2863 2024-05-08 12:10:15.000000 aibridge_test-0.3.6/setup.py
```

### Comparing `aibridge_test-0.3.5/AIBridge/__init__.py` & `aibridge_test-0.3.6/AIBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.3.6/AIBridge/ai_services/ai21labs_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.3.6/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/anthropic_ai.py` & `aibridge_test-0.3.6/AIBridge/ai_services/anthropic_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,19 @@
 
                     context_list.append({"role": key, "content": _context["context"]})
                 prev_role = key
             if context_list:
                 data_test = context_list[-1]
                 if data_test["role"] == "user":
                     context_list.append({"role": "assistant", "content": "understood"})
+                data = context_list[0]
+                if data["role"] == "assistant":
+                    context_list = [
+                        {"role": "user", "parts": ["you are friendly assistance"]}
+                    ] + context_list
         return context_list
 
     @classmethod
     def get_response(
         self,
         prompts,
         model="claude-3-opus-20240229",
```

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.3.6/AIBridge/ai_services/cohere_llm.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.3.6/AIBridge/ai_services/geminin_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.3.6/AIBridge/ai_services/image_optimisaton.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.3.6/AIBridge/ai_services/openai_images.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.3.6/AIBridge/ai_services/openai_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.3.6/AIBridge/ai_services/palm_chat.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.3.6/AIBridge/ai_services/palm_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/process_mq.py` & `aibridge_test-0.3.6/AIBridge/ai_services/process_mq.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.3.6/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/constant/common.py` & `aibridge_test-0.3.6/AIBridge/constant/common.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/constant/constant.py` & `aibridge_test-0.3.6/AIBridge/constant/constant.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/database/db_layer.py` & `aibridge_test-0.3.6/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/database/no_sql_service.py` & `aibridge_test-0.3.6/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/database/session.py` & `aibridge_test-0.3.6/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/database/sql_service.py` & `aibridge_test-0.3.6/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/exceptions.py` & `aibridge_test-0.3.6/AIBridge/exceptions.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/output_validation/convertors.py` & `aibridge_test-0.3.6/AIBridge/output_validation/convertors.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/output_validation/validations.py` & `aibridge_test-0.3.6/AIBridge/output_validation/validations.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.3.6/AIBridge/prompts/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.3.6/AIBridge/prompts/prompts_save.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.3.6/AIBridge/prompts/prompts_varibales.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.3.6/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.3.6/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.3.6/AIBridge/queue_integration/response_class.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/AIBridge/setconfig.py` & `aibridge_test-0.3.6/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/LICENSE` & `aibridge_test-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/PKG-INFO` & `aibridge_test-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.3.5
+Version: 0.3.6
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.3.5/README.md` & `aibridge_test-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.3.6/aibridge_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.3.5
+Version: 0.3.6
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.3.5/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.3.6/aibridge_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.5/setup.py` & `aibridge_test-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.3.5"
+VERSION = "0.3.6"
 REQUIRED = [
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
```

