# Comparing `tmp/langfun-0.0.2.dev20240507.tar.gz` & `tmp/langfun-0.0.2.dev20240508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240507.tar", last modified: Tue May  7 08:03:49 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240508.tar", last modified: Wed May  8 08:03:49 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240507.tar` & `langfun-0.0.2.dev20240508.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.427838 langfun-0.0.2.dev20240507/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-07 08:03:49.427838 langfun-0.0.2.dev20240507/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.407838 langfun-0.0.2.dev20240507/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.411838 langfun-0.0.2.dev20240507/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.411838 langfun-0.0.2.dev20240507/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.415838 langfun-0.0.2.dev20240507/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.415838 langfun-0.0.2.dev20240507/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/eval/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/eval/patching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20202 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.419838 langfun-0.0.2.dev20240507/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.419838 langfun-0.0.2.dev20240507/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/llms/openai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.419838 langfun-0.0.2.dev20240507/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.419838 langfun-0.0.2.dev20240507/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.423838 langfun-0.0.2.dev20240507/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.427838 langfun-0.0.2.dev20240507/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:03:49.427838 langfun-0.0.2.dev20240507/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-07 08:03:49.000000 langfun-0.0.2.dev20240507/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-07 08:03:49.000000 langfun-0.0.2.dev20240507/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:03:49.000000 langfun-0.0.2.dev20240507/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 08:03:49.000000 langfun-0.0.2.dev20240507/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 08:03:49.000000 langfun-0.0.2.dev20240507/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:03:49.427838 langfun-0.0.2.dev20240507/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-07 08:03:27.000000 langfun-0.0.2.dev20240507/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.365272 langfun-0.0.2.dev20240508/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.373272 langfun-0.0.2.dev20240508/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.373272 langfun-0.0.2.dev20240508/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.373272 langfun-0.0.2.dev20240508/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.377272 langfun-0.0.2.dev20240508/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/patching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20202 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.377272 langfun-0.0.2.dev20240508/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.377272 langfun-0.0.2.dev20240508/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/llms/openai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.381272 langfun-0.0.2.dev20240508/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.381272 langfun-0.0.2.dev20240508/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-08 08:03:49.000000 langfun-0.0.2.dev20240508/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-08 08:03:49.000000 langfun-0.0.2.dev20240508/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:03:49.000000 langfun-0.0.2.dev20240508/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 08:03:49.000000 langfun-0.0.2.dev20240508/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 08:03:49.000000 langfun-0.0.2.dev20240508/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:03:49.385272 langfun-0.0.2.dev20240508/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-08 08:03:28.000000 langfun-0.0.2.dev20240508/setup.py
```

### Comparing `langfun-0.0.2.dev20240507/LICENSE` & `langfun-0.0.2.dev20240508/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/PKG-INFO` & `langfun-0.0.2.dev20240508/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240507
+Version: 0.0.2.dev20240508
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240507/README.md` & `langfun-0.0.2.dev20240508/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/__init__.py` & `langfun-0.0.2.dev20240508/langfun/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,19 @@
 parse = structured.parse
 query = structured.query
 describe = structured.describe
 complete = structured.complete
 score = structured.score
 generate_class = structured.generate_class
 
+# Helper functions for input/output transformations based on
+# `lf.query` (e.g. jax-on-beam could use these for batch processing)
+query_prompt = structured.query_prompt
+query_output = structured.query_output
+
 source_form = structured.source_form
 function_gen = structured.function_gen
 
 from langfun.core import eval  # pylint: disable=redefined-builtin
 from langfun.core import templates
 from langfun.core import coding
```

### Comparing `langfun-0.0.2.dev20240507/langfun/core/__init__.py` & `langfun-0.0.2.dev20240508/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240508/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/component.py` & `langfun-0.0.2.dev20240508/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/component_test.py` & `langfun-0.0.2.dev20240508/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240508/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240508/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/console.py` & `langfun-0.0.2.dev20240508/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/console_test.py` & `langfun-0.0.2.dev20240508/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240508/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240508/langfun/core/eval/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1175,15 +1175,15 @@
 
   def call_postprocess(self, lm_response: str) -> str:
     """Post-process for `lf.call`. Subclass can override."""
     return lm_response
 
   def process(self, example: Any, **kwargs) -> lf.Message:
     """Process an example and returns its output."""
-    prompt = self.prompt.render(example=example).text
+    prompt = lf.Template.from_value(self.prompt, example=example)
     if self.method == 'call':
       return lf_structured.call(
           prompt,
           self.schema,
           lm=self.lm,
           parsing_lm=self.parsing_lm,
           parsing_examples=self.fewshot_examples,
@@ -1203,15 +1203,17 @@
           autofix_lm=self.autofix_lm,
           returns_message=True,
           **kwargs,
       )
     else:
       assert self.method == 'complete', self.method
       assert isinstance(self.schema.spec, pg.typing.Object), self.schema
-      input_value = self.schema.spec.cls.partial(prompt)
+      # TODO(daiyip): Currently multi-modal inputs within the prompt for
+      # completion is not supported.
+      input_value = self.schema.spec.cls.partial(prompt.render().text)
       return lf_structured.complete(
           input_value,
           lm=self.lm,
           examples=self.fewshot_examples,
           autofix=self.autofix,
           autofix_lm=self.autofix_lm,
           returns_message=True,
```

### Comparing `langfun-0.0.2.dev20240507/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240508/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240508/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240508/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/eval/patching.py` & `langfun-0.0.2.dev20240508/langfun/core/eval/patching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/eval/patching_test.py` & `langfun-0.0.2.dev20240508/langfun/core/eval/patching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240508/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240508/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240508/langfun/core/langfunc.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """LangFunc: Language-based functions."""
 
 import dataclasses
-from typing import Annotated, Type, Union
+from typing import Annotated, Type
 
 from langfun.core import component
 from langfun.core import language_model
 from langfun.core import message as message_lib
 from langfun.core import subscription
 from langfun.core import template as template_lib
 import pyglove as pg
@@ -324,30 +324,14 @@
     return lm_input
 
   def transform_output(
       self, lm_output: message_lib.Message) -> message_lib.Message:
     """Transforms the output message before returning from __call__."""
     return lm_output
 
-  @classmethod
-  def from_value(
-      cls, value: Union[str, template_lib.Template], **kwargs
-  ) -> 'LangFunc':
-    """Create a LangFunc object from a string or template."""
-    if isinstance(value, LangFunc):
-      return value
-    if isinstance(value, template_lib.Template):
-      lfun = LangFunc(value.template_str, **kwargs)
-      # So lfun could acccess all attributes from value.
-      lfun.sym_setparent(value)
-      return lfun
-    if isinstance(value, str):
-      return LangFunc(template_str=value, **kwargs)
-    return LangFunc('{{input}}', input=value, **kwargs)
-
 
 # Register converter from str to LangFunc, therefore we can always
 # pass strs to attributes that accept LangFunc.
 pg.typing.register_converter(str, LangFunc, LangFunc)
 
 
 #
```

### Comparing `langfun-0.0.2.dev20240507/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240508/langfun/core/langfunc_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,18 @@
   def test_from_value(self):
     l1 = LangFunc.from_value('Hello')
     self.assertEqual(l1.template_str, 'Hello')
 
     l2 = LangFunc.from_value(l1)
     self.assertIs(l2, l1)
 
+    l3 = LangFunc.from_value(l1, x=1)
+    self.assertIsNot(l3, l1)
+    self.assertTrue(pg.eq(l3, LangFunc('Hello', x=1)))
+
     c = template_lib.Template(
         '{{x}} + {{l}}',
         x=1,
         l=template_lib.Template('{{x}} + {{y}}', y=2))
     l3 = LangFunc.from_value(c.l)
     self.assertEqual(l3.render(), '1 + 2')
```

### Comparing `langfun-0.0.2.dev20240507/langfun/core/language_model.py` & `langfun-0.0.2.dev20240508/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240508/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/fake.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,45 +53,45 @@
 
 
 @lf.use_init_args(['response'])
 class StaticResponse(Fake):
   """Language model that always gives the same canned response."""
 
   response: Annotated[
-      str,
+      str | lf.Message,
       'A canned response that will be returned regardless of the prompt.'
   ]
 
   def _response_from(self, prompt: lf.Message) -> lf.Message:
-    return lf.AIMessage(self.response)
+    return lf.AIMessage.from_value(self.response)
 
 
 @lf.use_init_args(['mapping'])
 class StaticMapping(Fake):
   """A static mapping from prompt to response."""
 
   mapping: Annotated[
-      dict[str, str],
+      dict[str, str | lf.Message],
       'A mapping from prompt to response.'
   ]
 
   def _response_from(self, prompt: lf.Message) -> lf.Message:
-    return lf.AIMessage(self.mapping[prompt])
+    return lf.AIMessage.from_value(self.mapping[prompt])
 
 
 @lf.use_init_args(['sequence'])
 class StaticSequence(Fake):
   """A static sequence of responses to use."""
 
   sequence: Annotated[
-      list[str],
+      list[str | lf.Message],
       'A sequence of strings as the response.'
   ]
 
   def _on_bound(self):
     super()._on_bound()
     self._pos = 0
 
   def _response_from(self, prompt: lf.Message) -> lf.Message:
-    r = lf.AIMessage(self.sequence[self._pos])
+    r = lf.AIMessage.from_value(self.sequence[self._pos])
     self._pos += 1
     return r
```

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240508/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240508/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240508/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240508/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/memory.py` & `langfun-0.0.2.dev20240508/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/message.py` & `langfun-0.0.2.dev20240508/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/message_test.py` & `langfun-0.0.2.dev20240508/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240508/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240508/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240508/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240508/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240508/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240508/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240508/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/modality.py` & `langfun-0.0.2.dev20240508/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240508/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240508/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240508/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/sampling.py` & `langfun-0.0.2.dev20240508/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240508/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 from langfun.core.structured.parsing import parse
 from langfun.core.structured.parsing import call
 
 from langfun.core.structured.prompting import QueryStructure
 from langfun.core.structured.prompting import QueryStructureJson
 from langfun.core.structured.prompting import QueryStructurePython
 from langfun.core.structured.prompting import query
+from langfun.core.structured.prompting import query_prompt
+from langfun.core.structured.prompting import query_output
 
 from langfun.core.structured.description import DescribeStructure
 from langfun.core.structured.description import describe
 
 from langfun.core.structured.completion import CompleteStructure
 from langfun.core.structured.completion import complete
```

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/prompting.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Symbolic query."""
 
 from typing import Any, Callable, Type, Union
 
 import langfun.core as lf
+from langfun.core.llms import fake
 from langfun.core.structured import mapping
 from langfun.core.structured import schema as schema_lib
 import pyglove as pg
 
 
 @lf.use_init_args(['schema', 'default', 'examples'])
 class QueryStructure(mapping.Mapping):
@@ -210,21 +211,16 @@
   prompt_kwargs = kwargs.copy()
 
   # NOTE(daiyip): when `template_str` is passed in, it's intended to modify the
   # QueryStructure template string. Therefore, we pop out the argument for
   # prompt rendering.
   prompt_kwargs.pop('template_str', None)
 
-  if isinstance(prompt, str):
-    prompt = lf.Template(prompt, **prompt_kwargs)
-  elif isinstance(prompt, lf.Template):
-    prompt = prompt.rebind(**prompt_kwargs, raise_on_no_change=False)
-
-  if isinstance(prompt, lf.Template):
-    prompt = prompt.render(lm=lm)
+  if isinstance(prompt, (str, lf.Message, lf.Template)):
+    prompt = lf.Template.from_value(prompt, **prompt_kwargs).render(lm=lm)
   else:
     prompt = schema_lib.mark_missing(prompt)
 
   output = _query_structure_cls(protocol)(
       input=prompt,
       schema=schema,
       default=default,
@@ -236,7 +232,35 @@
   )(
       lm=lm,
       autofix_lm=autofix_lm or lm,
       cache_seed=cache_seed,
       skip_lm=skip_lm,
   )
   return output if returns_message else output.result
+
+
+def query_prompt(
+    prompt: Union[str, pg.Symbolic],
+    schema: Union[
+        schema_lib.Schema, Type[Any], list[Type[Any]], dict[str, Any], None
+    ] = None,
+    **kwargs,
+) -> lf.Message:
+  """Returns the final prompt sent to LLM for `lf.query`."""
+  kwargs.pop('returns_message', None)
+  kwargs.pop('skip_lm', None)
+  return query(prompt, schema, skip_lm=True, returns_message=True, **kwargs)
+
+
+def query_output(
+    response: Union[str, lf.Message],
+    schema: Union[
+        schema_lib.Schema, Type[Any], list[Type[Any]], dict[str, Any], None
+    ],
+    **kwargs,
+) -> Any:
+  """Returns the final output of `lf.query` from a provided LLM response."""
+  kwargs.pop('prompt', None)
+  kwargs.pop('lm', None)
+  return query(
+      'Unused prompt', schema, lm=fake.StaticResponse(response), **kwargs
+  )
```

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/prompting_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,14 +281,57 @@
         expected_modalities=2,
     )
 
   def test_bad_protocol(self):
     with self.assertRaisesRegex(ValueError, 'Unknown protocol'):
       prompting.query('what is 1 + 1', int, protocol='text')
 
+  def test_query_prompt(self):
+    self.assertEqual(
+        prompting.query_prompt('what is this?', int),
+        inspect.cleandoc("""
+            Please respond to the last INPUT_OBJECT with OUTPUT_OBJECT according to OUTPUT_TYPE.
+
+            INPUT_OBJECT:
+              1 + 1 =
+
+            OUTPUT_TYPE:
+              Answer
+
+              ```python
+              class Answer:
+                final_answer: int
+              ```
+
+            OUTPUT_OBJECT:
+              ```python
+              Answer(
+                final_answer=2
+              )
+              ```
+
+            INPUT_OBJECT:
+              what is this?
+
+            OUTPUT_TYPE:
+              int
+
+            OUTPUT_OBJECT:
+            """),
+    )
+
+  def test_query_output(self):
+    self.assertEqual(
+        prompting.query_output(
+            lf.AIMessage('1'),
+            int,
+        ),
+        1,
+    )
+
 
 class QueryStructurePythonTest(unittest.TestCase):
 
   def test_render_no_examples(self):
     l = prompting.QueryStructurePython(
         input=lf.AIMessage('Compute 12 / 6 + 2.'), schema=int
     )
```

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240508/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/subscription.py` & `langfun-0.0.2.dev20240508/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240508/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/template.py` & `langfun-0.0.2.dev20240508/langfun/core/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """langfun text template with compositionality."""
 
 import contextlib
 import dataclasses
 import functools
 import inspect
-from typing import Annotated, Any, Callable, Iterator, Set, Tuple, Type
+from typing import Annotated, Any, Callable, Iterator, Set, Tuple, Type, Union
 
 import jinja2
 from jinja2 import meta as jinja2_meta
 from langfun.core import component
 from langfun.core import message as message_lib
 from langfun.core import modality
 from langfun.core import natural_language
@@ -491,14 +491,35 @@
         )
     t = Template(base_template)
     # NOTE(daiyip): Set the parent of the newly created template to self so
     # it could access all the contextual variables.
     t.sym_setparent(self)
     return t
 
+  @classmethod
+  def from_value(
+      cls,
+      value: Union[str, message_lib.Message, 'Template'],
+      **kwargs
+  ) -> 'Template':
+    """Create a template object from a string or template."""
+    if isinstance(value, cls):
+      return value.clone(override=kwargs) if kwargs else value  # pylint: disable=no-value-for-parameter
+    if isinstance(value, str):
+      return cls(template_str=value, **kwargs)
+    if isinstance(value, message_lib.Message):
+      kwargs.update(value.metadata)
+      return cls(template_str=value.text, **kwargs)
+    if isinstance(value, Template):
+      lfun = cls(template_str=value.template_str, **kwargs)
+      # So lfun could acccess all attributes from value.
+      lfun.sym_setparent(value)
+      return lfun
+    return cls(template_str='{{input}}', input=value, **kwargs)
+
 
 # Register converter from str to LangFunc, therefore we can always
 # pass strs to attributes that accept LangFunc.
 pg.typing.register_converter(str, Template, Template)
 
 
 @dataclasses.dataclass
```

### Comparing `langfun-0.0.2.dev20240507/langfun/core/template_test.py` & `langfun-0.0.2.dev20240508/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240508/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240508/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240508/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240508/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240508/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240508/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240508/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240508/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240508/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240508/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240508/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240508/langfun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240507
+Version: 0.0.2.dev20240508
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240507/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240508/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240507/setup.py` & `langfun-0.0.2.dev20240508/setup.py`

 * *Files identical despite different names*

