# Comparing `tmp/supersullytools-2.5.2.tar.gz` & `tmp/supersullytools-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supersullytools-2.5.2.tar", last modified: Tue May  7 18:07:27 2024, max compression
+gzip compressed data, was "supersullytools-2.5.3.tar", last modified: Wed May  8 16:03:31 2024, max compression
```

## Comparing `supersullytools-2.5.2.tar` & `supersullytools-2.5.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.226186 supersullytools-2.5.2/
--rw-r--r--   0 msull      (501) staff       (20)     1092 2023-11-08 05:22:30.000000 supersullytools-2.5.2/LICENSE
--rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-07 18:07:27.225614 supersullytools-2.5.2/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)      297 2024-05-07 18:07:24.000000 supersullytools-2.5.2/README.md
--rw-r--r--   0 msull      (501) staff       (20)     2064 2024-05-07 18:07:24.000000 supersullytools-2.5.2/pyproject.toml
--rw-r--r--   0 msull      (501) staff       (20)       38 2024-05-07 18:07:27.226302 supersullytools-2.5.2/setup.cfg
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.211516 supersullytools-2.5.2/src/
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.212907 supersullytools-2.5.2/src/streamlit_app/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-30 16:56:26.000000 supersullytools-2.5.2/src/streamlit_app/Home.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.213594 supersullytools-2.5.2/src/streamlit_app/pages/
--rw-r--r--   0 msull      (501) staff       (20)     3497 2024-02-16 00:42:29.000000 supersullytools-2.5.2/src/streamlit_app/pages/AI Chat.py
--rw-r--r--   0 msull      (501) staff       (20)     1328 2024-02-15 00:27:25.000000 supersullytools-2.5.2/src/streamlit_app/pages/Item Paginator.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.213966 supersullytools-2.5.2/src/supersullytools/
--rw-r--r--   0 msull      (501) staff       (20)       26 2024-05-07 18:07:24.000000 supersullytools-2.5.2/src/supersullytools/__init__.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.216513 supersullytools-2.5.2/src/supersullytools/llm/
--rw-r--r--   0 msull      (501) staff       (20)        0 2024-05-06 20:11:38.000000 supersullytools-2.5.2/src/supersullytools/llm/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)    15063 2024-05-06 20:17:43.000000 supersullytools-2.5.2/src/supersullytools/llm/completions.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.217206 supersullytools-2.5.2/src/supersullytools/openai/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:46.000000 supersullytools-2.5.2/src/supersullytools/openai/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)     4329 2024-05-06 20:17:43.000000 supersullytools-2.5.2/src/supersullytools/openai/chat_session.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.218689 supersullytools-2.5.2/src/supersullytools/streamlit/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:34.000000 supersullytools-2.5.2/src/supersullytools/streamlit/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)      571 2024-03-21 19:38:09.000000 supersullytools-2.5.2/src/supersullytools/streamlit/misc.py
--rw-r--r--   0 msull      (501) staff       (20)     6115 2023-11-30 16:44:47.000000 supersullytools-2.5.2/src/supersullytools/streamlit/paginator.py
--rw-r--r--   0 msull      (501) staff       (20)    12742 2024-05-07 18:06:20.000000 supersullytools-2.5.2/src/supersullytools/streamlit/sessions.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.219771 supersullytools-2.5.2/src/supersullytools/utils/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 18:02:43.000000 supersullytools-2.5.2/src/supersullytools/utils/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)     7607 2024-05-06 23:02:18.000000 supersullytools-2.5.2/src/supersullytools/utils/fuzzy_search.py
--rw-r--r--   0 msull      (501) staff       (20)     1396 2024-02-15 22:47:53.000000 supersullytools-2.5.2/src/supersullytools/utils/misc.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.221393 supersullytools-2.5.2/src/supersullytools.egg-info/
--rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-07 18:07:27.000000 supersullytools-2.5.2/src/supersullytools.egg-info/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)      906 2024-05-07 18:07:27.000000 supersullytools-2.5.2/src/supersullytools.egg-info/SOURCES.txt
--rw-r--r--   0 msull      (501) staff       (20)        1 2024-05-07 18:07:27.000000 supersullytools-2.5.2/src/supersullytools.egg-info/dependency_links.txt
--rw-r--r--   0 msull      (501) staff       (20)      289 2024-05-07 18:07:27.000000 supersullytools-2.5.2/src/supersullytools.egg-info/requires.txt
--rw-r--r--   0 msull      (501) staff       (20)       36 2024-05-07 18:07:27.000000 supersullytools-2.5.2/src/supersullytools.egg-info/top_level.txt
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.220909 supersullytools-2.5.2/src/tests/
--rw-r--r--   0 msull      (501) staff       (20)     5073 2024-05-06 20:18:38.000000 supersullytools-2.5.2/src/tests/conftest.py
--rw-r--r--   0 msull      (501) staff       (20)     4082 2024-05-06 22:59:37.000000 supersullytools-2.5.2/src/tests/test_fuzzy_search.py
--rw-r--r--   0 msull      (501) staff       (20)      795 2024-02-16 00:44:38.000000 supersullytools-2.5.2/src/tests/test_streamlit_session.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:03:31.381492 supersullytools-2.5.3/
+-rw-r--r--   0 msull      (501) staff       (20)     1092 2023-11-08 05:22:30.000000 supersullytools-2.5.3/LICENSE
+-rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-08 16:03:31.381128 supersullytools-2.5.3/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)      297 2024-05-08 16:03:28.000000 supersullytools-2.5.3/README.md
+-rw-r--r--   0 msull      (501) staff       (20)     2064 2024-05-08 16:03:28.000000 supersullytools-2.5.3/pyproject.toml
+-rw-r--r--   0 msull      (501) staff       (20)       38 2024-05-08 16:03:31.381567 supersullytools-2.5.3/setup.cfg
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:03:31.368402 supersullytools-2.5.3/src/
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:03:31.370048 supersullytools-2.5.3/src/streamlit_app/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-30 16:56:26.000000 supersullytools-2.5.3/src/streamlit_app/Home.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:03:31.370949 supersullytools-2.5.3/src/streamlit_app/pages/
+-rw-r--r--   0 msull      (501) staff       (20)     3497 2024-02-16 00:42:29.000000 supersullytools-2.5.3/src/streamlit_app/pages/AI Chat.py
+-rw-r--r--   0 msull      (501) staff       (20)     1328 2024-02-15 00:27:25.000000 supersullytools-2.5.3/src/streamlit_app/pages/Item Paginator.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:03:31.371456 supersullytools-2.5.3/src/supersullytools/
+-rw-r--r--   0 msull      (501) staff       (20)       26 2024-05-08 16:03:28.000000 supersullytools-2.5.3/src/supersullytools/__init__.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:03:31.374255 supersullytools-2.5.3/src/supersullytools/llm/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2024-05-06 20:11:38.000000 supersullytools-2.5.3/src/supersullytools/llm/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)    16707 2024-05-08 16:03:04.000000 supersullytools-2.5.3/src/supersullytools/llm/completions.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:03:31.374856 supersullytools-2.5.3/src/supersullytools/openai/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:46.000000 supersullytools-2.5.3/src/supersullytools/openai/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)     4329 2024-05-06 20:17:43.000000 supersullytools-2.5.3/src/supersullytools/openai/chat_session.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:03:31.376043 supersullytools-2.5.3/src/supersullytools/streamlit/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:34.000000 supersullytools-2.5.3/src/supersullytools/streamlit/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)      571 2024-03-21 19:38:09.000000 supersullytools-2.5.3/src/supersullytools/streamlit/misc.py
+-rw-r--r--   0 msull      (501) staff       (20)     6115 2023-11-30 16:44:47.000000 supersullytools-2.5.3/src/supersullytools/streamlit/paginator.py
+-rw-r--r--   0 msull      (501) staff       (20)    12742 2024-05-07 18:06:20.000000 supersullytools-2.5.3/src/supersullytools/streamlit/sessions.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:03:31.376846 supersullytools-2.5.3/src/supersullytools/utils/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 18:02:43.000000 supersullytools-2.5.3/src/supersullytools/utils/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)     7607 2024-05-06 23:02:18.000000 supersullytools-2.5.3/src/supersullytools/utils/fuzzy_search.py
+-rw-r--r--   0 msull      (501) staff       (20)     1396 2024-02-15 22:47:53.000000 supersullytools-2.5.3/src/supersullytools/utils/misc.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:03:31.378035 supersullytools-2.5.3/src/supersullytools.egg-info/
+-rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-08 16:03:31.000000 supersullytools-2.5.3/src/supersullytools.egg-info/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)      906 2024-05-08 16:03:31.000000 supersullytools-2.5.3/src/supersullytools.egg-info/SOURCES.txt
+-rw-r--r--   0 msull      (501) staff       (20)        1 2024-05-08 16:03:31.000000 supersullytools-2.5.3/src/supersullytools.egg-info/dependency_links.txt
+-rw-r--r--   0 msull      (501) staff       (20)      289 2024-05-08 16:03:31.000000 supersullytools-2.5.3/src/supersullytools.egg-info/requires.txt
+-rw-r--r--   0 msull      (501) staff       (20)       36 2024-05-08 16:03:31.000000 supersullytools-2.5.3/src/supersullytools.egg-info/top_level.txt
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:03:31.377683 supersullytools-2.5.3/src/tests/
+-rw-r--r--   0 msull      (501) staff       (20)     5073 2024-05-06 20:18:38.000000 supersullytools-2.5.3/src/tests/conftest.py
+-rw-r--r--   0 msull      (501) staff       (20)     4082 2024-05-06 22:59:37.000000 supersullytools-2.5.3/src/tests/test_fuzzy_search.py
+-rw-r--r--   0 msull      (501) staff       (20)      795 2024-02-16 00:44:38.000000 supersullytools-2.5.3/src/tests/test_streamlit_session.py
```

### Comparing `supersullytools-2.5.2/LICENSE` & `supersullytools-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/PKG-INFO` & `supersullytools-2.5.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supersullytools
-Version: 2.5.2
+Version: 2.5.3
 Summary: This is a Python package that brings together a suite of utilities and helpers across several domains of software development.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -49,11 +49,11 @@
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 SuperSully Tools
 ================
 
-**Latest Version:** 2.5.2
+**Latest Version:** 2.5.3
 
 **SupersullyTools** is a Python package that brings together a suite of utilities and helpers across several domains of
 software development. My personal toolkit of things I want in every package I'm working on, compiled in one place.
```

### Comparing `supersullytools-2.5.2/pyproject.toml` & `supersullytools-2.5.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "supersullytools"
-version = "2.5.2"
+version = "2.5.3"
 description = "This is a Python package that brings together a suite of utilities and helpers across several domains of software development."
 readme = "README.md"
 authors = [{ name = "Sully", email = "sully@sadburger.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -62,15 +62,15 @@
 line-length = 120
 
 [tool.ruff]
 line-length = 120
 target-version = "py310"
 
 [tool.bumpver]
-current_version = "2.5.2"
+current_version = "2.5.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `supersullytools-2.5.2/src/streamlit_app/pages/AI Chat.py` & `supersullytools-2.5.3/src/streamlit_app/pages/AI Chat.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/src/streamlit_app/pages/Item Paginator.py` & `supersullytools-2.5.3/src/streamlit_app/pages/Item Paginator.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/src/supersullytools/llm/completions.py` & `supersullytools-2.5.3/src/supersullytools/llm/completions.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,19 +85,43 @@
 class CompletionHandler:
     def __init__(
         self,
         logger: Logger,
         openai_client: Optional["Client"] = None,
         bedrock_runtime_client: Optional["BedrockRuntimeClient"] = None,
         available_models: Optional[list["CompletionModel"]] = None,
+        debug_output_prompt_and_response=False,
+        enable_openai=True,
+        enable_bedrock=True,
     ):
         self.logger = logger
-        self.openai_client = openai_client or openai.Client()
-        self.bedrock_runtime_client = bedrock_runtime_client or boto3.client("bedrock-runtime")
-        self.available_models = available_models or ALL_MODELS
+        self.enable_openai = enable_openai
+        self.enable_bedrock = enable_bedrock
+
+        self.openai_client = None
+        if self.enable_openai:
+            self.openai_client = openai_client or openai.Client()
+
+        self.bedrock_runtime_client = None
+        if self.enable_bedrock:
+            self.bedrock_runtime_client = bedrock_runtime_client or boto3.client("bedrock-runtime")
+
+        self.debug_output_prompt_and_response = debug_output_prompt_and_response
+        if available_models:
+            self.available_models = available_models
+        else:
+            if enable_bedrock and enable_openai:
+                self.available_models = ALL_MODELS
+            elif enable_bedrock:
+                self.available_models = [x for x in ALL_MODELS if isinstance(x, BedrockModel)]
+            elif enable_openai:
+                self.available_models = [x for x in ALL_MODELS if isinstance(x, OpenAiModel)]
+            else:
+                # what do?
+                raise ValueError("No models specified")
 
     def get_model_by_name_or_id(self, model_name_or_id: str) -> "CompletionModelType":
         try:
             return next(x for x in self.available_models if x.llm == model_name_or_id)
         except StopIteration:
             try:
                 return next(x for x in self.available_models if x.llm_id == model_name_or_id)
@@ -120,44 +144,52 @@
                 return self._get_bedrock_completion(model, prompt, max_response_tokens)
             case _:
                 raise ValueError(model)
 
     def _get_bedrock_completion(
         self, llm: BedrockModel, prompt: str | list[PromptMessage | ImagePromptMessage], max_response_tokens: int
     ) -> "CompletionResponse":
+        if not self.enable_bedrock:
+            raise RuntimeError("Bedrock completions disabled!")
         boto_input = llm.prepare_bedrock_body(prompt, max_response_tokens)
         body = json.dumps(boto_input)
+
         accept = "application/json"
         content_type = "application/json"
 
         self.logger.info(f"Generating Bedrock Completion {llm.llm_id}")
-        # self.logger.debug(boto_input)
+        if self.debug_output_prompt_and_response:
+            self.logger.debug(f"LLM input:\n{boto_input}")
 
         # Invoke Bedrock API
         started_at = datetime.now(timezone.utc)
         response = self.bedrock_runtime_client.invoke_model(
             body=body, modelId=llm.llm_id, accept=accept, contentType=content_type
         )
         finished_at = datetime.now(timezone.utc)
-        self.logger.info("Completion complete")
-        # self.logger.debug(response)
+        self.logger.info("Generation complete")
+        if self.debug_output_prompt_and_response:
+            self.logger.debug(f"LLM Response:\n{response}")
+
         parsed_response = llm.parse_bedrock_response(response)
 
         return CompletionResponse(
             content=parsed_response.content,
             input_tokens=parsed_response.input_tokens,
             output_tokens=parsed_response.output_tokens,
             llm_metadata=CompletionModel.model_validate(llm, from_attributes=True),
             generated_at=finished_at,
             completion_time_ms=int((finished_at - started_at).total_seconds() * 1000),
         )
 
     def _get_openai_completion(
         self, llm: OpenAiModel, prompt: str | list[PromptMessage | ImagePromptMessage], max_response_tokens: int
     ) -> "CompletionResponse":
+        if not self.enable_openai:
+            raise RuntimeError("OpenAI completions disabled!")
         is_image_prompt = False
         if isinstance(prompt, str):
             chat_history = [{"role": "user", "content": prompt}]
         else:
             chat_history = []
             for msg in prompt:
                 match msg:
@@ -186,31 +218,37 @@
                         raise ValueError("Base prompt type")
 
         started_at = datetime.now(timezone.utc)
         if is_image_prompt:
             if not llm.supports_images:
                 raise ValueError("Specified model does not have image prompt support")
             self.logger.info("Generating Open AI ChatCompletion with Images")
+            if self.debug_output_prompt_and_response:
+                self.logger.debug(f"LLM input:\n{chat_history}")
             # have to use requests for this one
             headers = {"Content-Type": "application/json", "Authorization": f"Bearer {self.openai_client.api_key}"}
 
             payload = {"model": llm.llm_id, "messages": chat_history, "max_tokens": max_response_tokens}
             raw_response = requests.post(
                 "https://api.openai.com/v1/chat/completions", headers=headers, json=payload, timeout=300
             )
             raw_response.raise_for_status()
             data = raw_response.json()
-            # self.logger.debug(data)
+            if self.debug_output_prompt_and_response:
+                self.logger.debug(f"LLM response:\n{data}")
             openai_response = OpenAiChatCompletion.model_validate(data)
         else:
             self.logger.info("Generating Open AI ChatCompletion")
+            if self.debug_output_prompt_and_response:
+                self.logger.debug(f"LLM input:\n{chat_history}")
             openai_response = self.openai_client.chat.completions.create(
                 model=llm.llm_id, messages=chat_history, max_tokens=max_response_tokens
             )
-            # self.logger.debug(openai_response)
+            if self.debug_output_prompt_and_response:
+                self.logger.debug(f"LLM response:\n{openai_response}")
         finished_at = datetime.now(timezone.utc)
 
         return CompletionResponse(
             content=openai_response.choices[0].message.content,
             input_tokens=openai_response.usage.prompt_tokens,
             output_tokens=openai_response.usage.completion_tokens,
             llm_metadata=CompletionModel.model_validate(llm, from_attributes=True),
```

### Comparing `supersullytools-2.5.2/src/supersullytools/openai/chat_session.py` & `supersullytools-2.5.3/src/supersullytools/openai/chat_session.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/src/supersullytools/streamlit/misc.py` & `supersullytools-2.5.3/src/supersullytools/streamlit/misc.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/src/supersullytools/streamlit/paginator.py` & `supersullytools-2.5.3/src/supersullytools/streamlit/paginator.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/src/supersullytools/streamlit/sessions.py` & `supersullytools-2.5.3/src/supersullytools/streamlit/sessions.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/src/supersullytools/utils/fuzzy_search.py` & `supersullytools-2.5.3/src/supersullytools/utils/fuzzy_search.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/src/supersullytools/utils/misc.py` & `supersullytools-2.5.3/src/supersullytools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/src/supersullytools.egg-info/PKG-INFO` & `supersullytools-2.5.3/src/supersullytools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supersullytools
-Version: 2.5.2
+Version: 2.5.3
 Summary: This is a Python package that brings together a suite of utilities and helpers across several domains of software development.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -49,11 +49,11 @@
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 SuperSully Tools
 ================
 
-**Latest Version:** 2.5.2
+**Latest Version:** 2.5.3
 
 **SupersullyTools** is a Python package that brings together a suite of utilities and helpers across several domains of
 software development. My personal toolkit of things I want in every package I'm working on, compiled in one place.
```

### Comparing `supersullytools-2.5.2/src/supersullytools.egg-info/SOURCES.txt` & `supersullytools-2.5.3/src/supersullytools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/src/tests/conftest.py` & `supersullytools-2.5.3/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/src/tests/test_fuzzy_search.py` & `supersullytools-2.5.3/src/tests/test_fuzzy_search.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.2/src/tests/test_streamlit_session.py` & `supersullytools-2.5.3/src/tests/test_streamlit_session.py`

 * *Files identical despite different names*

