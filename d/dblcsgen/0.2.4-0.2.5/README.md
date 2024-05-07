# Comparing `tmp/dblcsgen-0.2.4.tar.gz` & `tmp/dblcsgen-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblcsgen-0.2.4.tar", last modified: Thu Apr 25 16:22:05 2024, max compression
+gzip compressed data, was "dblcsgen-0.2.5.tar", last modified: Tue May  7 22:44:33 2024, max compression
```

## Comparing `dblcsgen-0.2.4.tar` & `dblcsgen-0.2.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.767481 dblcsgen-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 16:22:03.000000 dblcsgen-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-25 16:22:05.767481 dblcsgen-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-25 16:22:03.000000 dblcsgen-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.763481 dblcsgen-0.2.4/dblcsgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-25 16:22:05.000000 dblcsgen-0.2.4/dblcsgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-25 16:22:05.000000 dblcsgen-0.2.4/dblcsgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:22:05.000000 dblcsgen-0.2.4/dblcsgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-25 16:22:05.000000 dblcsgen-0.2.4/dblcsgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 16:22:05.000000 dblcsgen-0.2.4/dblcsgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:22:05.767481 dblcsgen-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.751481 dblcsgen-0.2.4/sglang/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.751481 dblcsgen-0.2.4/sglang/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/backend/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/backend/runtime_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/global_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.755481 dblcsgen-0.2.4/sglang/lang/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/chat_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    27168 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/launch_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.755481 dblcsgen-0.2.4/sglang/srt/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.755481 dblcsgen-0.2.4/sglang/srt/constrained/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/constrained/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/constrained/fsm_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/constrained/jump_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/hf_transformers_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.759481 dblcsgen-0.2.4/sglang/srt/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/layers/context_flashattention_nopad.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/layers/extend_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/layers/logits_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/layers/radix_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/layers/token_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.759481 dblcsgen-0.2.4/sglang/srt/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/detokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/io_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/openai_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.759481 dblcsgen-0.2.4/sglang/srt/managers/router/
--rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/infer_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    28072 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/model_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/model_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/radix_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/tokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/memory_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/mm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.763481 dblcsgen-0.2.4/sglang/srt/models/
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/dbrx.py
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/dbrx_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/gemma.py
--rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/mixtral.py
--rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/qwen.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/qwen2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/stablelm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/yivl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/sampling_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/server_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.763481 dblcsgen-0.2.4/sglang/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/test/test_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/test/test_openai_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/test/test_programs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.842866 dblcsgen-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 22:44:31.000000 dblcsgen-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-05-07 22:44:33.842866 dblcsgen-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-05-07 22:44:31.000000 dblcsgen-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.838866 dblcsgen-0.2.5/dblcsgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-05-07 22:44:33.000000 dblcsgen-0.2.5/dblcsgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-07 22:44:33.000000 dblcsgen-0.2.5/dblcsgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:44:33.000000 dblcsgen-0.2.5/dblcsgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 22:44:33.000000 dblcsgen-0.2.5/dblcsgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 22:44:33.000000 dblcsgen-0.2.5/dblcsgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:44:33.842866 dblcsgen-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.830866 dblcsgen-0.2.5/sglang/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.830866 dblcsgen-0.2.5/sglang/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/backend/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/backend/runtime_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/global_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.830866 dblcsgen-0.2.5/sglang/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/lang/chat_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/lang/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27168 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/lang/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/lang/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/lang/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/launch_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.834866 dblcsgen-0.2.5/sglang/srt/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.834866 dblcsgen-0.2.5/sglang/srt/constrained/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/constrained/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/constrained/fsm_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/constrained/jump_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/hf_transformers_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.834866 dblcsgen-0.2.5/sglang/srt/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/layers/context_flashattention_nopad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/layers/extend_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/layers/logits_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/layers/radix_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/layers/token_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.834866 dblcsgen-0.2.5/sglang/srt/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/managers/detokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/managers/io_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/managers/openai_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.834866 dblcsgen-0.2.5/sglang/srt/managers/router/
+-rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/managers/router/infer_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/managers/router/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28072 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/managers/router/model_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/managers/router/model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/managers/router/radix_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/managers/router/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/managers/tokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/memory_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/mm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.838866 dblcsgen-0.2.5/sglang/srt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/models/dbrx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/models/dbrx_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/models/gemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/models/llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/models/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/models/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/models/mixtral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/models/qwen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/models/qwen2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/models/stablelm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/models/yivl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/sampling_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/server_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/srt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:44:33.838866 dblcsgen-0.2.5/sglang/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/test/test_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/test/test_openai_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/test/test_programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-07 22:44:28.000000 dblcsgen-0.2.5/sglang/utils.py
```

### Comparing `dblcsgen-0.2.4/LICENSE` & `dblcsgen-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/PKG-INFO` & `dblcsgen-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.4
+Version: 0.2.5
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -218,15 +218,15 @@
 Requires-Dist: fastapi; extra == "srt"
 Requires-Dist: psutil; extra == "srt"
 Requires-Dist: rpyc; extra == "srt"
 Requires-Dist: torch; extra == "srt"
 Requires-Dist: uvloop; extra == "srt"
 Requires-Dist: uvicorn; extra == "srt"
 Requires-Dist: zmq; extra == "srt"
-Requires-Dist: vllm>=0.3.3; extra == "srt"
+Requires-Dist: vllm>=0.4.0; extra == "srt"
 Requires-Dist: interegular; extra == "srt"
 Requires-Dist: pydantic; extra == "srt"
 Requires-Dist: pillow; extra == "srt"
 Requires-Dist: outlines==0.0.34; extra == "srt"
 Provides-Extra: all
 Requires-Dist: sglang[srt]; extra == "all"
```

### Comparing `dblcsgen-0.2.4/README.md` & `dblcsgen-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/dblcsgen.egg-info/PKG-INFO` & `dblcsgen-0.2.5/dblcsgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.4
+Version: 0.2.5
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -218,15 +218,15 @@
 Requires-Dist: fastapi; extra == "srt"
 Requires-Dist: psutil; extra == "srt"
 Requires-Dist: rpyc; extra == "srt"
 Requires-Dist: torch; extra == "srt"
 Requires-Dist: uvloop; extra == "srt"
 Requires-Dist: uvicorn; extra == "srt"
 Requires-Dist: zmq; extra == "srt"
-Requires-Dist: vllm>=0.3.3; extra == "srt"
+Requires-Dist: vllm>=0.4.0; extra == "srt"
 Requires-Dist: interegular; extra == "srt"
 Requires-Dist: pydantic; extra == "srt"
 Requires-Dist: pillow; extra == "srt"
 Requires-Dist: outlines==0.0.34; extra == "srt"
 Provides-Extra: all
 Requires-Dist: sglang[srt]; extra == "all"
```

### Comparing `dblcsgen-0.2.4/dblcsgen.egg-info/SOURCES.txt` & `dblcsgen-0.2.5/dblcsgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/pyproject.toml` & `dblcsgen-0.2.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dblcsgen"
-version = "0.2.4"
+version = "0.2.5"
 description = "DBLC Fast Structured Generation"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
@@ -16,15 +16,15 @@
 dependencies = [
     "requests",
     "tqdm",
 ]
 
 [project.optional-dependencies]
 srt = ["aiohttp", "fastapi", "psutil", "rpyc", "torch", "uvloop", "uvicorn",
-    "zmq", "vllm>=0.3.3", "interegular", "pydantic", "pillow",
+    "zmq", "vllm>=0.4.0", "interegular", "pydantic", "pillow",
     "outlines==0.0.34" # There is a breaking change to regexes on 0.0.35, not handled by SGLang atm
 ]
 all = ["sglang[srt]"]
 
 [project.urls]
 "Homepage" = "https://github.com/sgl-project/sglang"
 "Bug Tracker" = "https://github.com/sgl-project/sglang/issues"
```

### Comparing `dblcsgen-0.2.4/sglang/api.py` & `dblcsgen-0.2.5/sglang/api.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/backend/base_backend.py` & `dblcsgen-0.2.5/sglang/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/backend/runtime_endpoint.py` & `dblcsgen-0.2.5/sglang/backend/runtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/global_config.py` & `dblcsgen-0.2.5/sglang/global_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/lang/chat_template.py` & `dblcsgen-0.2.5/sglang/lang/chat_template.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/lang/compiler.py` & `dblcsgen-0.2.5/sglang/lang/compiler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/lang/interpreter.py` & `dblcsgen-0.2.5/sglang/lang/interpreter.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/lang/ir.py` & `dblcsgen-0.2.5/sglang/lang/ir.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/lang/tracer.py` & `dblcsgen-0.2.5/sglang/lang/tracer.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/constrained/__init__.py` & `dblcsgen-0.2.5/sglang/srt/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/constrained/base_cache.py` & `dblcsgen-0.2.5/sglang/srt/constrained/base_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/constrained/fsm_cache.py` & `dblcsgen-0.2.5/sglang/srt/constrained/fsm_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/constrained/jump_forward.py` & `dblcsgen-0.2.5/sglang/srt/constrained/jump_forward.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/conversation.py` & `dblcsgen-0.2.5/sglang/srt/conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/hf_transformers_utils.py` & `dblcsgen-0.2.5/sglang/srt/hf_transformers_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/layers/context_flashattention_nopad.py` & `dblcsgen-0.2.5/sglang/srt/layers/context_flashattention_nopad.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/layers/extend_attention.py` & `dblcsgen-0.2.5/sglang/srt/layers/extend_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/layers/logits_processor.py` & `dblcsgen-0.2.5/sglang/srt/layers/logits_processor.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/layers/radix_attention.py` & `dblcsgen-0.2.5/sglang/srt/layers/radix_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/layers/token_attention.py` & `dblcsgen-0.2.5/sglang/srt/layers/token_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/managers/detokenizer_manager.py` & `dblcsgen-0.2.5/sglang/srt/managers/detokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/managers/io_struct.py` & `dblcsgen-0.2.5/sglang/srt/managers/io_struct.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/managers/openai_protocol.py` & `dblcsgen-0.2.5/sglang/srt/managers/openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/managers/router/infer_batch.py` & `dblcsgen-0.2.5/sglang/srt/managers/router/infer_batch.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/managers/router/manager.py` & `dblcsgen-0.2.5/sglang/srt/managers/router/manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/managers/router/model_rpc.py` & `dblcsgen-0.2.5/sglang/srt/managers/router/model_rpc.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/managers/router/model_runner.py` & `dblcsgen-0.2.5/sglang/srt/managers/router/model_runner.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/managers/router/radix_cache.py` & `dblcsgen-0.2.5/sglang/srt/managers/router/radix_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/managers/router/scheduler.py` & `dblcsgen-0.2.5/sglang/srt/managers/router/scheduler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/managers/tokenizer_manager.py` & `dblcsgen-0.2.5/sglang/srt/managers/tokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/memory_pool.py` & `dblcsgen-0.2.5/sglang/srt/memory_pool.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/mm_utils.py` & `dblcsgen-0.2.5/sglang/srt/mm_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/model_config.py` & `dblcsgen-0.2.5/sglang/srt/model_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/models/dbrx.py` & `dblcsgen-0.2.5/sglang/srt/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/models/dbrx_config.py` & `dblcsgen-0.2.5/sglang/srt/models/dbrx_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/models/gemma.py` & `dblcsgen-0.2.5/sglang/srt/models/gemma.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/models/llama2.py` & `dblcsgen-0.2.5/sglang/srt/models/llama2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/models/llava.py` & `dblcsgen-0.2.5/sglang/srt/models/llava.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/models/mixtral.py` & `dblcsgen-0.2.5/sglang/srt/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/models/qwen.py` & `dblcsgen-0.2.5/sglang/srt/models/qwen.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/models/qwen2.py` & `dblcsgen-0.2.5/sglang/srt/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/models/stablelm.py` & `dblcsgen-0.2.5/sglang/srt/models/stablelm.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/models/yivl.py` & `dblcsgen-0.2.5/sglang/srt/models/yivl.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/sampling_params.py` & `dblcsgen-0.2.5/sglang/srt/sampling_params.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/server.py` & `dblcsgen-0.2.5/sglang/srt/server.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/server_args.py` & `dblcsgen-0.2.5/sglang/srt/server_args.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/srt/utils.py` & `dblcsgen-0.2.5/sglang/srt/utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/test/test_conversation.py` & `dblcsgen-0.2.5/sglang/test/test_conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/test/test_openai_protocol.py` & `dblcsgen-0.2.5/sglang/test/test_openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/test/test_programs.py` & `dblcsgen-0.2.5/sglang/test/test_programs.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/test/test_utils.py` & `dblcsgen-0.2.5/sglang/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.4/sglang/utils.py` & `dblcsgen-0.2.5/sglang/utils.py`

 * *Files identical despite different names*

