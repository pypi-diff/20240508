# Comparing `tmp/llm-foundry-0.7.0.tar.gz` & `tmp/llm-foundry-0.9.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-foundry-0.7.0.tar", last modified: Wed Mar 27 05:19:11 2024, max compression
+gzip compressed data, was "llm-foundry-0.9.0.dev0.tar", last modified: Wed May  8 01:43:25 2024, max compression
```

## Comparing `llm-foundry-0.7.0.tar` & `llm-foundry-0.9.0.dev0.tar`

### file list

```diff
@@ -1,109 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.752860 llm-foundry-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-03-27 05:19:11.752860 llm-foundry-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.740860 llm-foundry-0.7.0/llm_foundry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-03-27 05:19:11.000000 llm-foundry-0.7.0/llm_foundry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-27 05:19:11.000000 llm-foundry-0.7.0/llm_foundry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 05:19:11.000000 llm-foundry-0.7.0/llm_foundry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-27 05:19:11.000000 llm-foundry-0.7.0/llm_foundry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-03-27 05:19:11.000000 llm-foundry-0.7.0/llm_foundry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-27 05:19:11.000000 llm-foundry-0.7.0/llm_foundry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.740860 llm-foundry-0.7.0/llmfoundry/
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.740860 llm-foundry-0.7.0/llmfoundry/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.740860 llm-foundry-0.7.0/llmfoundry/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22746 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/callbacks/async_eval_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/callbacks/curriculum_learning_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     9357 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/callbacks/eval_gauntlet_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/callbacks/fdiff_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    19041 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/callbacks/hf_checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/callbacks/monolithic_ckpt_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/callbacks/resumption_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/callbacks/scheduled_gc_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.744860 llm-foundry-0.7.0/llmfoundry/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/cli/registry_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.744860 llm-foundry-0.7.0/llmfoundry/data/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/data/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/data/dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.744860 llm-foundry-0.7.0/llmfoundry/data/finetuning/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/data/finetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19697 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/data/finetuning/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)    28886 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/data/finetuning/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    39462 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/data/finetuning/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    18057 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/data/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18460 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/data/text_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.744860 llm-foundry-0.7.0/llmfoundry/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/interfaces/callback_with_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.744860 llm-foundry-0.7.0/llmfoundry/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/loggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.744860 llm-foundry-0.7.0/llmfoundry/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/metrics/token_acc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.744860 llm-foundry-0.7.0/llmfoundry/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.744860 llm-foundry-0.7.0/llmfoundry/models/hf/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/hf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13644 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/hf/hf_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/hf/hf_fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/hf/hf_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/hf/model_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.748860 llm-foundry-0.7.0/llmfoundry/models/inference_api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/inference_api_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/inference_api_wrapper/fmapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/inference_api_wrapper/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/inference_api_wrapper/openai_causal_lm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.748860 llm-foundry-0.7.0/llmfoundry/models/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27661 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/layers/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/layers/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/layers/custom_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/layers/fc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/layers/ffn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/layers/norm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.748860 llm-foundry-0.7.0/llmfoundry/models/mpt/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/mpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17388 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/mpt/configuration_mpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    45260 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/mpt/modeling_mpt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.748860 llm-foundry-0.7.0/llmfoundry/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/utils/act_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/utils/meta_init_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    15082 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/models/utils/param_init_fns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.748860 llm-foundry-0.7.0/llmfoundry/optim/
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18249 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/optim/adaptive_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/optim/outlier_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/optim/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.752860 llm-foundry-0.7.0/llmfoundry/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15297 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/tokenizers/tiktoken.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.752860 llm-foundry-0.7.0/llmfoundry/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23151 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    15947 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/checkpoint_conversion_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/data_prep_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/huggingface_hub_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/model_download_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/mosaicml_logger_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/prompt_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/llmfoundry/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15125 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 05:19:11.752860 llm-foundry-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:19:11.752860 llm-foundry-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/tests/test_smoketest.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-27 05:19:01.000000 llm-foundry-0.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.547032 llm-foundry-0.9.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19633 2024-05-08 01:43:25.547032 llm-foundry-0.9.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19181 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.531032 llm-foundry-0.9.0.dev0/llm_foundry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19633 2024-05-08 01:43:25.000000 llm-foundry-0.9.0.dev0/llm_foundry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-08 01:43:25.000000 llm-foundry-0.9.0.dev0/llm_foundry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:43:25.000000 llm-foundry-0.9.0.dev0/llm_foundry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 01:43:25.000000 llm-foundry-0.9.0.dev0/llm_foundry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 01:43:25.000000 llm-foundry-0.9.0.dev0/llm_foundry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 01:43:25.000000 llm-foundry-0.9.0.dev0/llm_foundry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.531032 llm-foundry-0.9.0.dev0/llmfoundry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.531032 llm-foundry-0.9.0.dev0/llmfoundry/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.535032 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22934 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/async_eval_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/curriculum_learning_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/eval_gauntlet_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/eval_output_logging_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/fdiff_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25723 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/hf_checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/log_mbmoe_tok_per_expert_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/monolithic_ckpt_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/resumption_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/callbacks/scheduled_gc_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.535032 llm-foundry-0.9.0.dev0/llmfoundry/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/cli/registry_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.535032 llm-foundry-0.9.0.dev0/llmfoundry/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/data/dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.535032 llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19557 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30847 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40793 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/data/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17293 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/data/text_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.535032 llm-foundry-0.9.0.dev0/llmfoundry/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/eval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.539032 llm-foundry-0.9.0.dev0/llmfoundry/eval/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/eval/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70690 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/eval/datasets/in_context_learning_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/eval/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.539032 llm-foundry-0.9.0.dev0/llmfoundry/eval/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/eval/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22148 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/eval/metrics/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.539032 llm-foundry-0.9.0.dev0/llmfoundry/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/interfaces/callback_with_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/layers_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.539032 llm-foundry-0.9.0.dev0/llmfoundry/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/loggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.539032 llm-foundry-0.9.0.dev0/llmfoundry/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/metrics/token_acc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.539032 llm-foundry-0.9.0.dev0/llmfoundry/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.539032 llm-foundry-0.9.0.dev0/llmfoundry/models/hf/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/hf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15971 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/hf/hf_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/hf/hf_fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/hf/hf_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/hf/model_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.539032 llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/fmapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/openai_causal_lm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.543032 llm-foundry-0.9.0.dev0/llmfoundry/models/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27930 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/layers/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/layers/custom_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/layers/dmoe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/layers/fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/layers/ffn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/layers/layer_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/layers/norm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.543032 llm-foundry-0.9.0.dev0/llmfoundry/models/mpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/mpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17835 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/mpt/configuration_mpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47730 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/mpt/modeling_mpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.543032 llm-foundry-0.9.0.dev0/llmfoundry/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/utils/act_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/utils/config_moe_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/utils/meta_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/utils/mpt_param_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31016 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/models/utils/param_init_fns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.543032 llm-foundry-0.9.0.dev0/llmfoundry/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18558 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/optim/adaptive_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/optim/outlier_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/optim/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.543032 llm-foundry-0.9.0.dev0/llmfoundry/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/tokenizers/tiktoken.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.547032 llm-foundry-0.9.0.dev0/llmfoundry/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22754 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16245 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/checkpoint_conversion_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13944 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/data_prep_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/huggingface_hub_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/model_download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/mosaicml_logger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/prompt_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/llmfoundry/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15403 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:43:25.547032 llm-foundry-0.9.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-08 01:43:14.000000 llm-foundry-0.9.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:43:25.547032 llm-foundry-0.9.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-05-08 01:43:15.000000 llm-foundry-0.9.0.dev0/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-08 01:43:15.000000 llm-foundry-0.9.0.dev0/tests/test_smoketest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 01:43:15.000000 llm-foundry-0.9.0.dev0/tests/test_utils.py
```

### Comparing `llm-foundry-0.7.0/LICENSE` & `llm-foundry-0.9.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.7.0/PKG-INFO` & `llm-foundry-0.9.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-foundry
-Version: 0.7.0
+Version: 0.9.0.dev0
 Summary: LLM Foundry
 Home-page: https://github.com/mosaicml/llm-foundry/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,16 +13,16 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: databricks
 Provides-Extra: tensorboard
 Provides-Extra: gpu-flash2
 Provides-Extra: gpu
 Provides-Extra: peft
-Provides-Extra: olmo
 Provides-Extra: openai
+Provides-Extra: megablocks
 Provides-Extra: all-cpu
 Provides-Extra: all
 Provides-Extra: all-flash2
 License-File: LICENSE
 
 
 
@@ -54,14 +54,28 @@
     * `train/benchmarking` - profile training throughput and MFU
   * `inference/` - convert models to HuggingFace or ONNX format, and generate responses
     * `inference/benchmarking` - profile inference latency and throughput
   * `eval/` - evaluate LLMs on academic (or custom) in-context-learning tasks
 * `mcli/` - launch any of these workloads using [MCLI](https://docs.mosaicml.com/projects/mcli/en/latest/) and the [MosaicML platform](https://www.mosaicml.com/platform)
 * `TUTORIAL.md` - a deeper dive into the repo, example workflows, and FAQs
 
+# DBRX
+
+DBRX is a state-of-the-art open source LLM trained by Databricks Mosaic team. It uses the Mixture-of-Experts (MoE) architecture and was trained with optimized versions of [Composer](https://github.com/mosaicml/composer), LLM Foundry, and [MegaBlocks](https://github.com/databricks/megablocks). The model has 132B total parameters and 36B active parameters. We have released two DBRX models:
+
+
+| Model              | Context Length | Download                                           |
+| ------------------ | -------------- | -------------------------------------------------- |
+| DBRX Base          | 32768          | https://huggingface.co/databricks/dbrx-base        |
+| DBRX Instruct      | 32768          | https://huggingface.co/databricks/dbrx-instruct    |
+
+Our model weights and code are licensed for both researchers and commercial entities. The Databricks Open Source License can be found at [LICENSE](https://github.com/databricks/dbrx/LICENSE), and our Acceptable Use Policy can be found [here](https://www.databricks.com/legal/acceptable-use-policy-open-model).
+
+For more information about the DBRX models, see https://github.com/databricks/dbrx.
+
 # MPT
 
 Mosaic Pretrained Transformers (MPT) are GPT-style models with some special features -- Flash Attention for efficiency, ALiBi for context length extrapolation, and stability improvements to mitigate loss spikes. As part of MosaicML's Foundation series, we have open-sourced several MPT models:
 
 
 | Model              | Context Length | Download                                           | Commercial use? |
 | ------------------ | -------------- | -------------------------------------------------- | --------------- |
@@ -91,14 +105,15 @@
 * [MPT-7B StoryWriter Intro](https://www.youtube.com/watch?v=O9Y_ZdsuKWQ) by [AItrepreneur](https://www.youtube.com/@Aitrepreneur)
 * [Fine-tuning MPT-7B on a single GPU](https://www.youtube.com/watch?v=KSlWkrByc0o&t=9s) by [@AIology2022](https://www.youtube.com/@AIology2022)
 * [How to Fine-tune MPT-7B-Instruct on Google Colab](https://youtu.be/3de0Utr9XnI) by [@VRSEN](https://www.youtube.com/@vrsen)
 
 Something missing? Contribute with a PR!
 
 # Latest News
+* [Blog: Introducing DBRX: A New State-of-the-Art Open LLM](https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm)
 * [Blog: LLM Training and Inference with Intel Gaudi2 AI Accelerators](https://www.databricks.com/blog/llm-training-and-inference-intel-gaudi2-ai-accelerators)
 * [Blog: Training LLMs at Scale with AMD MI250 GPUs](https://www.databricks.com/blog/training-llms-scale-amd-mi250-gpus)
 * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://www.mosaicml.com/blog/amd-mi250)
 * [Blog: Announcing MPT-7B-8K: 8K Context Length for Document Understanding](https://www.mosaicml.com/blog/long-context-mpt-7b-8k)
 * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://www.mosaicml.com/blog/amd-mi250)
 * [Blog: MPT-30B: Raising the bar for open-source foundation models](https://www.mosaicml.com/blog/mpt-30b)
 * [Blog: Introducing MPT-7B](https://www.mosaicml.com/blog/mpt-7b)
@@ -112,32 +127,32 @@
 # Hardware and Software Requirements
 This codebase has been tested with PyTorch 2.2 with NVIDIA A100s and H100s.
 This codebase may also work on systems with other devices, such as consumer NVIDIA cards and AMD cards, but we are not actively testing these systems.
 If you have success/failure using LLM Foundry on other systems, please let us know in a Github issue and we will update the support matrix!
 
 | Device         | Torch Version | Cuda Version | Status                       |
 | -------------- | ------------- | ------------ | ---------------------------- |
-| A100-40GB/80GB | 2.2.1         | 12.1         | :white_check_mark: Supported |
-| H100-80GB      | 2.2.1         | 12.1         | :white_check_mark: Supported |
+| A100-40GB/80GB | 2.3.0         | 12.1         | :white_check_mark: Supported |
+| H100-80GB      | 2.3.0         | 12.1         | :white_check_mark: Supported |
 
 ## MosaicML Docker Images
 We highly recommend using our prebuilt Docker images. You can find them here: https://hub.docker.com/orgs/mosaicml/repositories.
 
 The `mosaicml/pytorch` images are pinned to specific PyTorch and CUDA versions, and are stable and rarely updated.
 
 The `mosaicml/llm-foundry` images are built with new tags upon every commit to the `main` branch.
-You can select a specific commit hash such as `mosaicml/llm-foundry:2.2.1_cu121_flash2-36ab1ba` or take the latest one using `mosaicml/llm-foundry:2.2.1_cu121_flash2-latest`.
+You can select a specific commit hash such as `mosaicml/llm-foundry:2.3.0_cu121_flash2-36ab1ba` or take the latest one using `mosaicml/llm-foundry:2.3.0_cu121_flash2-latest`.
 
 **Please Note:** The `mosaicml/llm-foundry` images do not come with the `llm-foundry` package preinstalled, just the dependencies. You will still need to `pip install llm-foundry` either from PyPi or from source.
 
 | Docker Image                                           | Torch Version | Cuda Version      | LLM Foundry dependencies installed? |
 | ------------------------------------------------------ | ------------- | ----------------- | ----------------------------------- |
-| `mosaicml/pytorch:2.2.1_cu121-python3.11-ubuntu20.04`  | 2.2.1         | 12.1 (Infiniband) | No                                  |
-| `mosaicml/llm-foundry:2.2.1_cu121_flash2-latest`       | 2.2.1         | 12.1 (Infiniband) | Yes                                 |
-| `mosaicml/llm-foundry:2.2.1_cu121_flash2_aws-latest`   | 2.2.1         | 12.1 (EFA)        | Yes                                 |
+| `mosaicml/pytorch:2.3.0_cu121-python3.11-ubuntu20.04`  | 2.3.0         | 12.1 (Infiniband) | No                                  |
+| `mosaicml/llm-foundry:2.3.0_cu121_flash2-latest`       | 2.3.0         | 12.1 (Infiniband) | Yes                                 |
+| `mosaicml/llm-foundry:2.3.0_cu121_flash2_aws-latest`   | 2.3.0         | 12.1 (EFA)        | Yes                                 |
 
 
 # Installation
 
 This assumes you already have PyTorch, CMake, and packaging installed. If not, you can install them with `pip install cmake packaging torch`.
 
 To get started, clone the repo and set up your environment. Instructions to do so differ slightly depending on whether you're using Docker.
@@ -305,15 +320,15 @@
 name = "foundry_registry"
 version = "0.1.0"
 dependencies = [
     "mosaicml",
     "llm-foundry",
 ]
 
-[project.entry-points."llm_foundry.loggers"]
+[project.entry-points."llmfoundry_loggers"]
 my_logger = "foundry_registry.loggers:MyLogger"
 ```
 
 ### Direct call to register
 
 You can also register a component directly in your code:
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: llm-foundry Version: 0.7.0 Summary: LLM Foundry
-Home-page: https://github.com/mosaicml/llm-foundry/ Author: MosaicML Author-
-email: team@mosaicml.com Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1 Name: llm-foundry Version: 0.9.0.dev0 Summary: LLM
+Foundry Home-page: https://github.com/mosaicml/llm-foundry/ Author: MosaicML
+Author-email: team@mosaicml.com Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
 dev Provides-Extra: databricks Provides-Extra: tensorboard Provides-Extra: gpu-
-flash2 Provides-Extra: gpu Provides-Extra: peft Provides-Extra: olmo Provides-
-Extra: openai Provides-Extra: all-cpu Provides-Extra: all Provides-Extra: all-
-flash2 License-File: LICENSE
+flash2 Provides-Extra: gpu Provides-Extra: peft Provides-Extra: openai
+Provides-Extra: megablocks Provides-Extra: all-cpu Provides-Extra: all
+Provides-Extra: all-flash2 License-File: LICENSE
           _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _P_a_c_k_a_g_e_ _V_e_r_s_i_o_n_]_[_C_h_a_t_ _@_ _S_l_a_c_k_]_[_L_i_c_e_n_s_e_]
 
 # LLM Foundry This repository contains code for training, finetuning,
 evaluating, and deploying LLMs for inference with [Composer](https://
 github.com/mosaicml/composer) and the [MosaicML platform](https://
 forms.mosaicml.com/
 demo?utm_source=github.com&utm_medium=referral&utm_campaign=llm-foundry).
@@ -23,38 +23,52 @@
 HuggingFace and MPT models from 125M - 70B parameters * `train/benchmarking` -
 profile training throughput and MFU * `inference/` - convert models to
 HuggingFace or ONNX format, and generate responses * `inference/benchmarking` -
 profile inference latency and throughput * `eval/` - evaluate LLMs on academic
 (or custom) in-context-learning tasks * `mcli/` - launch any of these workloads
 using [MCLI](https://docs.mosaicml.com/projects/mcli/en/latest/) and the
 [MosaicML platform](https://www.mosaicml.com/platform) * `TUTORIAL.md` - a
-deeper dive into the repo, example workflows, and FAQs # MPT Mosaic Pretrained
-Transformers (MPT) are GPT-style models with some special features -- Flash
-Attention for efficiency, ALiBi for context length extrapolation, and stability
-improvements to mitigate loss spikes. As part of MosaicML's Foundation series,
-we have open-sourced several MPT models: | Model | Context Length | Download |
-Commercial use? | | ------------------ | -------------- | ---------------------
------------------------------ | --------------- | | MPT-30B | 8192 | https://
-huggingface.co/mosaicml/mpt-30b | Yes | | MPT-30B-Instruct | 8192 | https://
-huggingface.co/mosaicml/mpt-30b-instruct | Yes | | MPT-30B-Chat | 8192 | https:
-//huggingface.co/mosaicml/mpt-30b-chat | No | | MPT-7b-8k | 8192 | https://
-huggingface.co/mosaicml/mpt-7b-8k | Yes | | MPT-7b-8k-Chat | 8192 | https://
-huggingface.co/mosaicml/mpt-7b-8k-chat | No | | MPT-7B | 2048 | https://
-huggingface.co/mosaicml/mpt-7b | Yes | | MPT-7B-Instruct | 2048 | https://
-huggingface.co/mosaicml/mpt-7b-instruct | Yes | | MPT-7B-Chat | 2048 | https://
-huggingface.co/mosaicml/mpt-7b-chat | No | | MPT-7B-StoryWriter | 65536 |
-https://huggingface.co/mosaicml/mpt-7b-storywriter | Yes | To try out these
-models locally, [follow the instructions](https://github.com/mosaicml/llm-
-foundry/tree/main/scripts/inference#interactive-generation-with-modelgenerate)
-in `scripts/inference/README.md` to prompt HF models using our [hf_generate.py]
-(https://github.com/mosaicml/llm-foundry/blob/main/scripts/inference/
-hf_generate.py) or [hf_chat.py](https://github.com/mosaicml/llm-foundry/blob/
-main/scripts/inference/hf_chat.py) scripts. # MPT Community We've been
-overwhelmed by all the amazing work the community has put into MPT! Here we
-provide a few links to some of them: * [ReplitLM](https://github.com/replit/
+deeper dive into the repo, example workflows, and FAQs # DBRX DBRX is a state-
+of-the-art open source LLM trained by Databricks Mosaic team. It uses the
+Mixture-of-Experts (MoE) architecture and was trained with optimized versions
+of [Composer](https://github.com/mosaicml/composer), LLM Foundry, and
+[MegaBlocks](https://github.com/databricks/megablocks). The model has 132B
+total parameters and 36B active parameters. We have released two DBRX models: |
+Model | Context Length | Download | | ------------------ | -------------- | ---
+----------------------------------------------- | | DBRX Base | 32768 | https:/
+/huggingface.co/databricks/dbrx-base | | DBRX Instruct | 32768 | https://
+huggingface.co/databricks/dbrx-instruct | Our model weights and code are
+licensed for both researchers and commercial entities. The Databricks Open
+Source License can be found at [LICENSE](https://github.com/databricks/dbrx/
+LICENSE), and our Acceptable Use Policy can be found [here](https://
+www.databricks.com/legal/acceptable-use-policy-open-model). For more
+information about the DBRX models, see https://github.com/databricks/dbrx. #
+MPT Mosaic Pretrained Transformers (MPT) are GPT-style models with some special
+features -- Flash Attention for efficiency, ALiBi for context length
+extrapolation, and stability improvements to mitigate loss spikes. As part of
+MosaicML's Foundation series, we have open-sourced several MPT models: | Model
+| Context Length | Download | Commercial use? | | ------------------ | --------
+------ | -------------------------------------------------- | --------------- |
+| MPT-30B | 8192 | https://huggingface.co/mosaicml/mpt-30b | Yes | | MPT-30B-
+Instruct | 8192 | https://huggingface.co/mosaicml/mpt-30b-instruct | Yes | |
+MPT-30B-Chat | 8192 | https://huggingface.co/mosaicml/mpt-30b-chat | No | |
+MPT-7b-8k | 8192 | https://huggingface.co/mosaicml/mpt-7b-8k | Yes | | MPT-7b-
+8k-Chat | 8192 | https://huggingface.co/mosaicml/mpt-7b-8k-chat | No | | MPT-7B
+| 2048 | https://huggingface.co/mosaicml/mpt-7b | Yes | | MPT-7B-Instruct |
+2048 | https://huggingface.co/mosaicml/mpt-7b-instruct | Yes | | MPT-7B-Chat |
+2048 | https://huggingface.co/mosaicml/mpt-7b-chat | No | | MPT-7B-StoryWriter
+| 65536 | https://huggingface.co/mosaicml/mpt-7b-storywriter | Yes | To try out
+these models locally, [follow the instructions](https://github.com/mosaicml/
+llm-foundry/tree/main/scripts/inference#interactive-generation-with-
+modelgenerate) in `scripts/inference/README.md` to prompt HF models using our
+[hf_generate.py](https://github.com/mosaicml/llm-foundry/blob/main/scripts/
+inference/hf_generate.py) or [hf_chat.py](https://github.com/mosaicml/llm-
+foundry/blob/main/scripts/inference/hf_chat.py) scripts. # MPT Community We've
+been overwhelmed by all the amazing work the community has put into MPT! Here
+we provide a few links to some of them: * [ReplitLM](https://github.com/replit/
 replitLM): `replit-code-v1-3b` is a 2.7B Causal Language Model focused on Code
 Completion. The model has been trained on a subset of the Stack Dedup v1.2
 dataset covering 20 languages such as Java, Python, and C++ * [LLaVa-MPT]
 (https://github.com/haotian-liu/LLaVA#LLaVA-MPT-7b): Visual instruction tuning
 to get MPT multimodal capabilities * [ggml](https://github.com/ggerganov/ggml/
 tree/master): Optimized MPT version for efficient inference on consumer
 hardware * [GPT4All](https://gpt4all.io/index.html): locally running chat
@@ -64,55 +78,57 @@
 www.youtube.com/watch?v=DXpk9K7DgMo&t=3s) by [@jamesbriggs](https://
 www.youtube.com/@jamesbriggs) * [MPT-7B StoryWriter Intro](https://
 www.youtube.com/watch?v=O9Y_ZdsuKWQ) by [AItrepreneur](https://www.youtube.com/
 @Aitrepreneur) * [Fine-tuning MPT-7B on a single GPU](https://www.youtube.com/
 watch?v=KSlWkrByc0o&t=9s) by [@AIology2022](https://www.youtube.com/
 @AIology2022) * [How to Fine-tune MPT-7B-Instruct on Google Colab](https://
 youtu.be/3de0Utr9XnI) by [@VRSEN](https://www.youtube.com/@vrsen) Something
-missing? Contribute with a PR! # Latest News * [Blog: LLM Training and
-Inference with Intel Gaudi2 AI Accelerators](https://www.databricks.com/blog/
-llm-training-and-inference-intel-gaudi2-ai-accelerators) * [Blog: Training LLMs
-at Scale with AMD MI250 GPUs](https://www.databricks.com/blog/training-llms-
-scale-amd-mi250-gpus) * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML]
-(https://www.mosaicml.com/blog/amd-mi250) * [Blog: Announcing MPT-7B-8K: 8K
-Context Length for Document Understanding](https://www.mosaicml.com/blog/long-
-context-mpt-7b-8k) * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML]
-(https://www.mosaicml.com/blog/amd-mi250) * [Blog: MPT-30B: Raising the bar for
-open-source foundation models](https://www.mosaicml.com/blog/mpt-30b) * [Blog:
+missing? Contribute with a PR! # Latest News * [Blog: Introducing DBRX: A New
+State-of-the-Art Open LLM](https://www.databricks.com/blog/introducing-dbrx-
+new-state-art-open-llm) * [Blog: LLM Training and Inference with Intel Gaudi2
+AI Accelerators](https://www.databricks.com/blog/llm-training-and-inference-
+intel-gaudi2-ai-accelerators) * [Blog: Training LLMs at Scale with AMD MI250
+GPUs](https://www.databricks.com/blog/training-llms-scale-amd-mi250-gpus) *
+[Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://
+www.mosaicml.com/blog/amd-mi250) * [Blog: Announcing MPT-7B-8K: 8K Context
+Length for Document Understanding](https://www.mosaicml.com/blog/long-context-
+mpt-7b-8k) * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://
+www.mosaicml.com/blog/amd-mi250) * [Blog: MPT-30B: Raising the bar for open-
+source foundation models](https://www.mosaicml.com/blog/mpt-30b) * [Blog:
 Introducing MPT-7B](https://www.mosaicml.com/blog/mpt-7b) * [Blog: Benchmarking
 LLMs on H100](https://www.mosaicml.com/blog/coreweave-nvidia-h100-part-1) *
 [Blog: Blazingly Fast LLM Evaluation](https://www.mosaicml.com/blog/llm-
 evaluation-for-icl) * [Blog: GPT3 Quality for $500k](https://www.mosaicml.com/
 blog/gpt-3-quality-for-500k) * [Blog: Billion parameter GPT training made easy]
 (https://www.mosaicml.com/blog/billion-parameter-gpt-training-made-easy) #
 Hardware and Software Requirements This codebase has been tested with PyTorch
 2.2 with NVIDIA A100s and H100s. This codebase may also work on systems with
 other devices, such as consumer NVIDIA cards and AMD cards, but we are not
 actively testing these systems. If you have success/failure using LLM Foundry
 on other systems, please let us know in a Github issue and we will update the
 support matrix! | Device | Torch Version | Cuda Version | Status | | ----------
 ---- | ------------- | ------------ | ---------------------------- | | A100-
-40GB/80GB | 2.2.1 | 12.1 | :white_check_mark: Supported | | H100-80GB | 2.2.1 |
+40GB/80GB | 2.3.0 | 12.1 | :white_check_mark: Supported | | H100-80GB | 2.3.0 |
 12.1 | :white_check_mark: Supported | ## MosaicML Docker Images We highly
 recommend using our prebuilt Docker images. You can find them here: https://
 hub.docker.com/orgs/mosaicml/repositories. The `mosaicml/pytorch` images are
 pinned to specific PyTorch and CUDA versions, and are stable and rarely
 updated. The `mosaicml/llm-foundry` images are built with new tags upon every
 commit to the `main` branch. You can select a specific commit hash such as
-`mosaicml/llm-foundry:2.2.1_cu121_flash2-36ab1ba` or take the latest one using
-`mosaicml/llm-foundry:2.2.1_cu121_flash2-latest`. **Please Note:** The
+`mosaicml/llm-foundry:2.3.0_cu121_flash2-36ab1ba` or take the latest one using
+`mosaicml/llm-foundry:2.3.0_cu121_flash2-latest`. **Please Note:** The
 `mosaicml/llm-foundry` images do not come with the `llm-foundry` package
 preinstalled, just the dependencies. You will still need to `pip install llm-
 foundry` either from PyPi or from source. | Docker Image | Torch Version | Cuda
 Version | LLM Foundry dependencies installed? | | -----------------------------
 ------------------------- | ------------- | ----------------- | ---------------
--------------------- | | `mosaicml/pytorch:2.2.1_cu121-python3.11-ubuntu20.04`
-| 2.2.1 | 12.1 (Infiniband) | No | | `mosaicml/llm-foundry:2.2.1_cu121_flash2-
-latest` | 2.2.1 | 12.1 (Infiniband) | Yes | | `mosaicml/llm-foundry:
-2.2.1_cu121_flash2_aws-latest` | 2.2.1 | 12.1 (EFA) | Yes | # Installation This
+-------------------- | | `mosaicml/pytorch:2.3.0_cu121-python3.11-ubuntu20.04`
+| 2.3.0 | 12.1 (Infiniband) | No | | `mosaicml/llm-foundry:2.3.0_cu121_flash2-
+latest` | 2.3.0 | 12.1 (Infiniband) | Yes | | `mosaicml/llm-foundry:
+2.3.0_cu121_flash2_aws-latest` | 2.3.0 | 12.1 (EFA) | Yes | # Installation This
 assumes you already have PyTorch, CMake, and packaging installed. If not, you
 can install them with `pip install cmake packaging torch`. To get started,
 clone the repo and set up your environment. Instructions to do so differ
 slightly depending on whether you're using Docker. ### With Docker
 (recommended) We *strongly* recommend working with LLM Foundry inside a Docker
 container (see our recommended Docker image above). If you are doing so, follow
 these steps to clone the repo and install the requirements. ```bash git clone
@@ -193,15 +209,15 @@
 There are a few ways to register a new component: ### Python entrypoints You
 can specify registered components via a Python entrypoint if you are building
 your own package with registered components. For example, the following would
 register the `WandBLogger` class, under the key `wandb`, in the
 `llm_foundry.loggers` registry: ```yaml [build-system] requires =
 ["setuptools>=42", "wheel"] build-backend = "setuptools.build_meta" [project]
 name = "foundry_registry" version = "0.1.0" dependencies = [ "mosaicml", "llm-
-foundry", ] [project.entry-points."llm_foundry.loggers"] my_logger =
+foundry", ] [project.entry-points."llmfoundry_loggers"] my_logger =
 "foundry_registry.loggers:MyLogger" ``` ### Direct call to register You can
 also register a component directly in your code: ```python from
 composer.loggers import LoggerDestination from llmfoundry.registry import
 loggers class MyLogger(LoggerDestination): pass loggers.register("my_logger",
 func=MyLogger) ``` ### Decorators You can also use decorators to register
 components directly from your code: ```python from composer.loggers import
 LoggerDestination from llmfoundry.registry import loggers @loggers.register
```

### Comparing `llm-foundry-0.7.0/README.md` & `llm-foundry-0.9.0.dev0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,28 @@
     * `train/benchmarking` - profile training throughput and MFU
   * `inference/` - convert models to HuggingFace or ONNX format, and generate responses
     * `inference/benchmarking` - profile inference latency and throughput
   * `eval/` - evaluate LLMs on academic (or custom) in-context-learning tasks
 * `mcli/` - launch any of these workloads using [MCLI](https://docs.mosaicml.com/projects/mcli/en/latest/) and the [MosaicML platform](https://www.mosaicml.com/platform)
 * `TUTORIAL.md` - a deeper dive into the repo, example workflows, and FAQs
 
+# DBRX
+
+DBRX is a state-of-the-art open source LLM trained by Databricks Mosaic team. It uses the Mixture-of-Experts (MoE) architecture and was trained with optimized versions of [Composer](https://github.com/mosaicml/composer), LLM Foundry, and [MegaBlocks](https://github.com/databricks/megablocks). The model has 132B total parameters and 36B active parameters. We have released two DBRX models:
+
+
+| Model              | Context Length | Download                                           |
+| ------------------ | -------------- | -------------------------------------------------- |
+| DBRX Base          | 32768          | https://huggingface.co/databricks/dbrx-base        |
+| DBRX Instruct      | 32768          | https://huggingface.co/databricks/dbrx-instruct    |
+
+Our model weights and code are licensed for both researchers and commercial entities. The Databricks Open Source License can be found at [LICENSE](https://github.com/databricks/dbrx/LICENSE), and our Acceptable Use Policy can be found [here](https://www.databricks.com/legal/acceptable-use-policy-open-model).
+
+For more information about the DBRX models, see https://github.com/databricks/dbrx.
+
 # MPT
 
 Mosaic Pretrained Transformers (MPT) are GPT-style models with some special features -- Flash Attention for efficiency, ALiBi for context length extrapolation, and stability improvements to mitigate loss spikes. As part of MosaicML's Foundation series, we have open-sourced several MPT models:
 
 
 | Model              | Context Length | Download                                           | Commercial use? |
 | ------------------ | -------------- | -------------------------------------------------- | --------------- |
@@ -73,14 +87,15 @@
 * [MPT-7B StoryWriter Intro](https://www.youtube.com/watch?v=O9Y_ZdsuKWQ) by [AItrepreneur](https://www.youtube.com/@Aitrepreneur)
 * [Fine-tuning MPT-7B on a single GPU](https://www.youtube.com/watch?v=KSlWkrByc0o&t=9s) by [@AIology2022](https://www.youtube.com/@AIology2022)
 * [How to Fine-tune MPT-7B-Instruct on Google Colab](https://youtu.be/3de0Utr9XnI) by [@VRSEN](https://www.youtube.com/@vrsen)
 
 Something missing? Contribute with a PR!
 
 # Latest News
+* [Blog: Introducing DBRX: A New State-of-the-Art Open LLM](https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm)
 * [Blog: LLM Training and Inference with Intel Gaudi2 AI Accelerators](https://www.databricks.com/blog/llm-training-and-inference-intel-gaudi2-ai-accelerators)
 * [Blog: Training LLMs at Scale with AMD MI250 GPUs](https://www.databricks.com/blog/training-llms-scale-amd-mi250-gpus)
 * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://www.mosaicml.com/blog/amd-mi250)
 * [Blog: Announcing MPT-7B-8K: 8K Context Length for Document Understanding](https://www.mosaicml.com/blog/long-context-mpt-7b-8k)
 * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://www.mosaicml.com/blog/amd-mi250)
 * [Blog: MPT-30B: Raising the bar for open-source foundation models](https://www.mosaicml.com/blog/mpt-30b)
 * [Blog: Introducing MPT-7B](https://www.mosaicml.com/blog/mpt-7b)
@@ -94,32 +109,32 @@
 # Hardware and Software Requirements
 This codebase has been tested with PyTorch 2.2 with NVIDIA A100s and H100s.
 This codebase may also work on systems with other devices, such as consumer NVIDIA cards and AMD cards, but we are not actively testing these systems.
 If you have success/failure using LLM Foundry on other systems, please let us know in a Github issue and we will update the support matrix!
 
 | Device         | Torch Version | Cuda Version | Status                       |
 | -------------- | ------------- | ------------ | ---------------------------- |
-| A100-40GB/80GB | 2.2.1         | 12.1         | :white_check_mark: Supported |
-| H100-80GB      | 2.2.1         | 12.1         | :white_check_mark: Supported |
+| A100-40GB/80GB | 2.3.0         | 12.1         | :white_check_mark: Supported |
+| H100-80GB      | 2.3.0         | 12.1         | :white_check_mark: Supported |
 
 ## MosaicML Docker Images
 We highly recommend using our prebuilt Docker images. You can find them here: https://hub.docker.com/orgs/mosaicml/repositories.
 
 The `mosaicml/pytorch` images are pinned to specific PyTorch and CUDA versions, and are stable and rarely updated.
 
 The `mosaicml/llm-foundry` images are built with new tags upon every commit to the `main` branch.
-You can select a specific commit hash such as `mosaicml/llm-foundry:2.2.1_cu121_flash2-36ab1ba` or take the latest one using `mosaicml/llm-foundry:2.2.1_cu121_flash2-latest`.
+You can select a specific commit hash such as `mosaicml/llm-foundry:2.3.0_cu121_flash2-36ab1ba` or take the latest one using `mosaicml/llm-foundry:2.3.0_cu121_flash2-latest`.
 
 **Please Note:** The `mosaicml/llm-foundry` images do not come with the `llm-foundry` package preinstalled, just the dependencies. You will still need to `pip install llm-foundry` either from PyPi or from source.
 
 | Docker Image                                           | Torch Version | Cuda Version      | LLM Foundry dependencies installed? |
 | ------------------------------------------------------ | ------------- | ----------------- | ----------------------------------- |
-| `mosaicml/pytorch:2.2.1_cu121-python3.11-ubuntu20.04`  | 2.2.1         | 12.1 (Infiniband) | No                                  |
-| `mosaicml/llm-foundry:2.2.1_cu121_flash2-latest`       | 2.2.1         | 12.1 (Infiniband) | Yes                                 |
-| `mosaicml/llm-foundry:2.2.1_cu121_flash2_aws-latest`   | 2.2.1         | 12.1 (EFA)        | Yes                                 |
+| `mosaicml/pytorch:2.3.0_cu121-python3.11-ubuntu20.04`  | 2.3.0         | 12.1 (Infiniband) | No                                  |
+| `mosaicml/llm-foundry:2.3.0_cu121_flash2-latest`       | 2.3.0         | 12.1 (Infiniband) | Yes                                 |
+| `mosaicml/llm-foundry:2.3.0_cu121_flash2_aws-latest`   | 2.3.0         | 12.1 (EFA)        | Yes                                 |
 
 
 # Installation
 
 This assumes you already have PyTorch, CMake, and packaging installed. If not, you can install them with `pip install cmake packaging torch`.
 
 To get started, clone the repo and set up your environment. Instructions to do so differ slightly depending on whether you're using Docker.
@@ -287,15 +302,15 @@
 name = "foundry_registry"
 version = "0.1.0"
 dependencies = [
     "mosaicml",
     "llm-foundry",
 ]
 
-[project.entry-points."llm_foundry.loggers"]
+[project.entry-points."llmfoundry_loggers"]
 my_logger = "foundry_registry.loggers:MyLogger"
 ```
 
 ### Direct call to register
 
 You can also register a component directly in your code:
```

#### html2text {}

```diff
@@ -14,38 +14,52 @@
 HuggingFace and MPT models from 125M - 70B parameters * `train/benchmarking` -
 profile training throughput and MFU * `inference/` - convert models to
 HuggingFace or ONNX format, and generate responses * `inference/benchmarking` -
 profile inference latency and throughput * `eval/` - evaluate LLMs on academic
 (or custom) in-context-learning tasks * `mcli/` - launch any of these workloads
 using [MCLI](https://docs.mosaicml.com/projects/mcli/en/latest/) and the
 [MosaicML platform](https://www.mosaicml.com/platform) * `TUTORIAL.md` - a
-deeper dive into the repo, example workflows, and FAQs # MPT Mosaic Pretrained
-Transformers (MPT) are GPT-style models with some special features -- Flash
-Attention for efficiency, ALiBi for context length extrapolation, and stability
-improvements to mitigate loss spikes. As part of MosaicML's Foundation series,
-we have open-sourced several MPT models: | Model | Context Length | Download |
-Commercial use? | | ------------------ | -------------- | ---------------------
------------------------------ | --------------- | | MPT-30B | 8192 | https://
-huggingface.co/mosaicml/mpt-30b | Yes | | MPT-30B-Instruct | 8192 | https://
-huggingface.co/mosaicml/mpt-30b-instruct | Yes | | MPT-30B-Chat | 8192 | https:
-//huggingface.co/mosaicml/mpt-30b-chat | No | | MPT-7b-8k | 8192 | https://
-huggingface.co/mosaicml/mpt-7b-8k | Yes | | MPT-7b-8k-Chat | 8192 | https://
-huggingface.co/mosaicml/mpt-7b-8k-chat | No | | MPT-7B | 2048 | https://
-huggingface.co/mosaicml/mpt-7b | Yes | | MPT-7B-Instruct | 2048 | https://
-huggingface.co/mosaicml/mpt-7b-instruct | Yes | | MPT-7B-Chat | 2048 | https://
-huggingface.co/mosaicml/mpt-7b-chat | No | | MPT-7B-StoryWriter | 65536 |
-https://huggingface.co/mosaicml/mpt-7b-storywriter | Yes | To try out these
-models locally, [follow the instructions](https://github.com/mosaicml/llm-
-foundry/tree/main/scripts/inference#interactive-generation-with-modelgenerate)
-in `scripts/inference/README.md` to prompt HF models using our [hf_generate.py]
-(https://github.com/mosaicml/llm-foundry/blob/main/scripts/inference/
-hf_generate.py) or [hf_chat.py](https://github.com/mosaicml/llm-foundry/blob/
-main/scripts/inference/hf_chat.py) scripts. # MPT Community We've been
-overwhelmed by all the amazing work the community has put into MPT! Here we
-provide a few links to some of them: * [ReplitLM](https://github.com/replit/
+deeper dive into the repo, example workflows, and FAQs # DBRX DBRX is a state-
+of-the-art open source LLM trained by Databricks Mosaic team. It uses the
+Mixture-of-Experts (MoE) architecture and was trained with optimized versions
+of [Composer](https://github.com/mosaicml/composer), LLM Foundry, and
+[MegaBlocks](https://github.com/databricks/megablocks). The model has 132B
+total parameters and 36B active parameters. We have released two DBRX models: |
+Model | Context Length | Download | | ------------------ | -------------- | ---
+----------------------------------------------- | | DBRX Base | 32768 | https:/
+/huggingface.co/databricks/dbrx-base | | DBRX Instruct | 32768 | https://
+huggingface.co/databricks/dbrx-instruct | Our model weights and code are
+licensed for both researchers and commercial entities. The Databricks Open
+Source License can be found at [LICENSE](https://github.com/databricks/dbrx/
+LICENSE), and our Acceptable Use Policy can be found [here](https://
+www.databricks.com/legal/acceptable-use-policy-open-model). For more
+information about the DBRX models, see https://github.com/databricks/dbrx. #
+MPT Mosaic Pretrained Transformers (MPT) are GPT-style models with some special
+features -- Flash Attention for efficiency, ALiBi for context length
+extrapolation, and stability improvements to mitigate loss spikes. As part of
+MosaicML's Foundation series, we have open-sourced several MPT models: | Model
+| Context Length | Download | Commercial use? | | ------------------ | --------
+------ | -------------------------------------------------- | --------------- |
+| MPT-30B | 8192 | https://huggingface.co/mosaicml/mpt-30b | Yes | | MPT-30B-
+Instruct | 8192 | https://huggingface.co/mosaicml/mpt-30b-instruct | Yes | |
+MPT-30B-Chat | 8192 | https://huggingface.co/mosaicml/mpt-30b-chat | No | |
+MPT-7b-8k | 8192 | https://huggingface.co/mosaicml/mpt-7b-8k | Yes | | MPT-7b-
+8k-Chat | 8192 | https://huggingface.co/mosaicml/mpt-7b-8k-chat | No | | MPT-7B
+| 2048 | https://huggingface.co/mosaicml/mpt-7b | Yes | | MPT-7B-Instruct |
+2048 | https://huggingface.co/mosaicml/mpt-7b-instruct | Yes | | MPT-7B-Chat |
+2048 | https://huggingface.co/mosaicml/mpt-7b-chat | No | | MPT-7B-StoryWriter
+| 65536 | https://huggingface.co/mosaicml/mpt-7b-storywriter | Yes | To try out
+these models locally, [follow the instructions](https://github.com/mosaicml/
+llm-foundry/tree/main/scripts/inference#interactive-generation-with-
+modelgenerate) in `scripts/inference/README.md` to prompt HF models using our
+[hf_generate.py](https://github.com/mosaicml/llm-foundry/blob/main/scripts/
+inference/hf_generate.py) or [hf_chat.py](https://github.com/mosaicml/llm-
+foundry/blob/main/scripts/inference/hf_chat.py) scripts. # MPT Community We've
+been overwhelmed by all the amazing work the community has put into MPT! Here
+we provide a few links to some of them: * [ReplitLM](https://github.com/replit/
 replitLM): `replit-code-v1-3b` is a 2.7B Causal Language Model focused on Code
 Completion. The model has been trained on a subset of the Stack Dedup v1.2
 dataset covering 20 languages such as Java, Python, and C++ * [LLaVa-MPT]
 (https://github.com/haotian-liu/LLaVA#LLaVA-MPT-7b): Visual instruction tuning
 to get MPT multimodal capabilities * [ggml](https://github.com/ggerganov/ggml/
 tree/master): Optimized MPT version for efficient inference on consumer
 hardware * [GPT4All](https://gpt4all.io/index.html): locally running chat
@@ -55,55 +69,57 @@
 www.youtube.com/watch?v=DXpk9K7DgMo&t=3s) by [@jamesbriggs](https://
 www.youtube.com/@jamesbriggs) * [MPT-7B StoryWriter Intro](https://
 www.youtube.com/watch?v=O9Y_ZdsuKWQ) by [AItrepreneur](https://www.youtube.com/
 @Aitrepreneur) * [Fine-tuning MPT-7B on a single GPU](https://www.youtube.com/
 watch?v=KSlWkrByc0o&t=9s) by [@AIology2022](https://www.youtube.com/
 @AIology2022) * [How to Fine-tune MPT-7B-Instruct on Google Colab](https://
 youtu.be/3de0Utr9XnI) by [@VRSEN](https://www.youtube.com/@vrsen) Something
-missing? Contribute with a PR! # Latest News * [Blog: LLM Training and
-Inference with Intel Gaudi2 AI Accelerators](https://www.databricks.com/blog/
-llm-training-and-inference-intel-gaudi2-ai-accelerators) * [Blog: Training LLMs
-at Scale with AMD MI250 GPUs](https://www.databricks.com/blog/training-llms-
-scale-amd-mi250-gpus) * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML]
-(https://www.mosaicml.com/blog/amd-mi250) * [Blog: Announcing MPT-7B-8K: 8K
-Context Length for Document Understanding](https://www.mosaicml.com/blog/long-
-context-mpt-7b-8k) * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML]
-(https://www.mosaicml.com/blog/amd-mi250) * [Blog: MPT-30B: Raising the bar for
-open-source foundation models](https://www.mosaicml.com/blog/mpt-30b) * [Blog:
+missing? Contribute with a PR! # Latest News * [Blog: Introducing DBRX: A New
+State-of-the-Art Open LLM](https://www.databricks.com/blog/introducing-dbrx-
+new-state-art-open-llm) * [Blog: LLM Training and Inference with Intel Gaudi2
+AI Accelerators](https://www.databricks.com/blog/llm-training-and-inference-
+intel-gaudi2-ai-accelerators) * [Blog: Training LLMs at Scale with AMD MI250
+GPUs](https://www.databricks.com/blog/training-llms-scale-amd-mi250-gpus) *
+[Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://
+www.mosaicml.com/blog/amd-mi250) * [Blog: Announcing MPT-7B-8K: 8K Context
+Length for Document Understanding](https://www.mosaicml.com/blog/long-context-
+mpt-7b-8k) * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://
+www.mosaicml.com/blog/amd-mi250) * [Blog: MPT-30B: Raising the bar for open-
+source foundation models](https://www.mosaicml.com/blog/mpt-30b) * [Blog:
 Introducing MPT-7B](https://www.mosaicml.com/blog/mpt-7b) * [Blog: Benchmarking
 LLMs on H100](https://www.mosaicml.com/blog/coreweave-nvidia-h100-part-1) *
 [Blog: Blazingly Fast LLM Evaluation](https://www.mosaicml.com/blog/llm-
 evaluation-for-icl) * [Blog: GPT3 Quality for $500k](https://www.mosaicml.com/
 blog/gpt-3-quality-for-500k) * [Blog: Billion parameter GPT training made easy]
 (https://www.mosaicml.com/blog/billion-parameter-gpt-training-made-easy) #
 Hardware and Software Requirements This codebase has been tested with PyTorch
 2.2 with NVIDIA A100s and H100s. This codebase may also work on systems with
 other devices, such as consumer NVIDIA cards and AMD cards, but we are not
 actively testing these systems. If you have success/failure using LLM Foundry
 on other systems, please let us know in a Github issue and we will update the
 support matrix! | Device | Torch Version | Cuda Version | Status | | ----------
 ---- | ------------- | ------------ | ---------------------------- | | A100-
-40GB/80GB | 2.2.1 | 12.1 | :white_check_mark: Supported | | H100-80GB | 2.2.1 |
+40GB/80GB | 2.3.0 | 12.1 | :white_check_mark: Supported | | H100-80GB | 2.3.0 |
 12.1 | :white_check_mark: Supported | ## MosaicML Docker Images We highly
 recommend using our prebuilt Docker images. You can find them here: https://
 hub.docker.com/orgs/mosaicml/repositories. The `mosaicml/pytorch` images are
 pinned to specific PyTorch and CUDA versions, and are stable and rarely
 updated. The `mosaicml/llm-foundry` images are built with new tags upon every
 commit to the `main` branch. You can select a specific commit hash such as
-`mosaicml/llm-foundry:2.2.1_cu121_flash2-36ab1ba` or take the latest one using
-`mosaicml/llm-foundry:2.2.1_cu121_flash2-latest`. **Please Note:** The
+`mosaicml/llm-foundry:2.3.0_cu121_flash2-36ab1ba` or take the latest one using
+`mosaicml/llm-foundry:2.3.0_cu121_flash2-latest`. **Please Note:** The
 `mosaicml/llm-foundry` images do not come with the `llm-foundry` package
 preinstalled, just the dependencies. You will still need to `pip install llm-
 foundry` either from PyPi or from source. | Docker Image | Torch Version | Cuda
 Version | LLM Foundry dependencies installed? | | -----------------------------
 ------------------------- | ------------- | ----------------- | ---------------
--------------------- | | `mosaicml/pytorch:2.2.1_cu121-python3.11-ubuntu20.04`
-| 2.2.1 | 12.1 (Infiniband) | No | | `mosaicml/llm-foundry:2.2.1_cu121_flash2-
-latest` | 2.2.1 | 12.1 (Infiniband) | Yes | | `mosaicml/llm-foundry:
-2.2.1_cu121_flash2_aws-latest` | 2.2.1 | 12.1 (EFA) | Yes | # Installation This
+-------------------- | | `mosaicml/pytorch:2.3.0_cu121-python3.11-ubuntu20.04`
+| 2.3.0 | 12.1 (Infiniband) | No | | `mosaicml/llm-foundry:2.3.0_cu121_flash2-
+latest` | 2.3.0 | 12.1 (Infiniband) | Yes | | `mosaicml/llm-foundry:
+2.3.0_cu121_flash2_aws-latest` | 2.3.0 | 12.1 (EFA) | Yes | # Installation This
 assumes you already have PyTorch, CMake, and packaging installed. If not, you
 can install them with `pip install cmake packaging torch`. To get started,
 clone the repo and set up your environment. Instructions to do so differ
 slightly depending on whether you're using Docker. ### With Docker
 (recommended) We *strongly* recommend working with LLM Foundry inside a Docker
 container (see our recommended Docker image above). If you are doing so, follow
 these steps to clone the repo and install the requirements. ```bash git clone
@@ -184,15 +200,15 @@
 There are a few ways to register a new component: ### Python entrypoints You
 can specify registered components via a Python entrypoint if you are building
 your own package with registered components. For example, the following would
 register the `WandBLogger` class, under the key `wandb`, in the
 `llm_foundry.loggers` registry: ```yaml [build-system] requires =
 ["setuptools>=42", "wheel"] build-backend = "setuptools.build_meta" [project]
 name = "foundry_registry" version = "0.1.0" dependencies = [ "mosaicml", "llm-
-foundry", ] [project.entry-points."llm_foundry.loggers"] my_logger =
+foundry", ] [project.entry-points."llmfoundry_loggers"] my_logger =
 "foundry_registry.loggers:MyLogger" ``` ### Direct call to register You can
 also register a component directly in your code: ```python from
 composer.loggers import LoggerDestination from llmfoundry.registry import
 loggers class MyLogger(LoggerDestination): pass loggers.register("my_logger",
 func=MyLogger) ``` ### Decorators You can also use decorators to register
 components directly from your code: ```python from composer.loggers import
 LoggerDestination from llmfoundry.registry import loggers @loggers.register
```

### Comparing `llm-foundry-0.7.0/llm_foundry.egg-info/PKG-INFO` & `llm-foundry-0.9.0.dev0/llm_foundry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-foundry
-Version: 0.7.0
+Version: 0.9.0.dev0
 Summary: LLM Foundry
 Home-page: https://github.com/mosaicml/llm-foundry/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,16 +13,16 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: databricks
 Provides-Extra: tensorboard
 Provides-Extra: gpu-flash2
 Provides-Extra: gpu
 Provides-Extra: peft
-Provides-Extra: olmo
 Provides-Extra: openai
+Provides-Extra: megablocks
 Provides-Extra: all-cpu
 Provides-Extra: all
 Provides-Extra: all-flash2
 License-File: LICENSE
 
 
 
@@ -54,14 +54,28 @@
     * `train/benchmarking` - profile training throughput and MFU
   * `inference/` - convert models to HuggingFace or ONNX format, and generate responses
     * `inference/benchmarking` - profile inference latency and throughput
   * `eval/` - evaluate LLMs on academic (or custom) in-context-learning tasks
 * `mcli/` - launch any of these workloads using [MCLI](https://docs.mosaicml.com/projects/mcli/en/latest/) and the [MosaicML platform](https://www.mosaicml.com/platform)
 * `TUTORIAL.md` - a deeper dive into the repo, example workflows, and FAQs
 
+# DBRX
+
+DBRX is a state-of-the-art open source LLM trained by Databricks Mosaic team. It uses the Mixture-of-Experts (MoE) architecture and was trained with optimized versions of [Composer](https://github.com/mosaicml/composer), LLM Foundry, and [MegaBlocks](https://github.com/databricks/megablocks). The model has 132B total parameters and 36B active parameters. We have released two DBRX models:
+
+
+| Model              | Context Length | Download                                           |
+| ------------------ | -------------- | -------------------------------------------------- |
+| DBRX Base          | 32768          | https://huggingface.co/databricks/dbrx-base        |
+| DBRX Instruct      | 32768          | https://huggingface.co/databricks/dbrx-instruct    |
+
+Our model weights and code are licensed for both researchers and commercial entities. The Databricks Open Source License can be found at [LICENSE](https://github.com/databricks/dbrx/LICENSE), and our Acceptable Use Policy can be found [here](https://www.databricks.com/legal/acceptable-use-policy-open-model).
+
+For more information about the DBRX models, see https://github.com/databricks/dbrx.
+
 # MPT
 
 Mosaic Pretrained Transformers (MPT) are GPT-style models with some special features -- Flash Attention for efficiency, ALiBi for context length extrapolation, and stability improvements to mitigate loss spikes. As part of MosaicML's Foundation series, we have open-sourced several MPT models:
 
 
 | Model              | Context Length | Download                                           | Commercial use? |
 | ------------------ | -------------- | -------------------------------------------------- | --------------- |
@@ -91,14 +105,15 @@
 * [MPT-7B StoryWriter Intro](https://www.youtube.com/watch?v=O9Y_ZdsuKWQ) by [AItrepreneur](https://www.youtube.com/@Aitrepreneur)
 * [Fine-tuning MPT-7B on a single GPU](https://www.youtube.com/watch?v=KSlWkrByc0o&t=9s) by [@AIology2022](https://www.youtube.com/@AIology2022)
 * [How to Fine-tune MPT-7B-Instruct on Google Colab](https://youtu.be/3de0Utr9XnI) by [@VRSEN](https://www.youtube.com/@vrsen)
 
 Something missing? Contribute with a PR!
 
 # Latest News
+* [Blog: Introducing DBRX: A New State-of-the-Art Open LLM](https://www.databricks.com/blog/introducing-dbrx-new-state-art-open-llm)
 * [Blog: LLM Training and Inference with Intel Gaudi2 AI Accelerators](https://www.databricks.com/blog/llm-training-and-inference-intel-gaudi2-ai-accelerators)
 * [Blog: Training LLMs at Scale with AMD MI250 GPUs](https://www.databricks.com/blog/training-llms-scale-amd-mi250-gpus)
 * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://www.mosaicml.com/blog/amd-mi250)
 * [Blog: Announcing MPT-7B-8K: 8K Context Length for Document Understanding](https://www.mosaicml.com/blog/long-context-mpt-7b-8k)
 * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://www.mosaicml.com/blog/amd-mi250)
 * [Blog: MPT-30B: Raising the bar for open-source foundation models](https://www.mosaicml.com/blog/mpt-30b)
 * [Blog: Introducing MPT-7B](https://www.mosaicml.com/blog/mpt-7b)
@@ -112,32 +127,32 @@
 # Hardware and Software Requirements
 This codebase has been tested with PyTorch 2.2 with NVIDIA A100s and H100s.
 This codebase may also work on systems with other devices, such as consumer NVIDIA cards and AMD cards, but we are not actively testing these systems.
 If you have success/failure using LLM Foundry on other systems, please let us know in a Github issue and we will update the support matrix!
 
 | Device         | Torch Version | Cuda Version | Status                       |
 | -------------- | ------------- | ------------ | ---------------------------- |
-| A100-40GB/80GB | 2.2.1         | 12.1         | :white_check_mark: Supported |
-| H100-80GB      | 2.2.1         | 12.1         | :white_check_mark: Supported |
+| A100-40GB/80GB | 2.3.0         | 12.1         | :white_check_mark: Supported |
+| H100-80GB      | 2.3.0         | 12.1         | :white_check_mark: Supported |
 
 ## MosaicML Docker Images
 We highly recommend using our prebuilt Docker images. You can find them here: https://hub.docker.com/orgs/mosaicml/repositories.
 
 The `mosaicml/pytorch` images are pinned to specific PyTorch and CUDA versions, and are stable and rarely updated.
 
 The `mosaicml/llm-foundry` images are built with new tags upon every commit to the `main` branch.
-You can select a specific commit hash such as `mosaicml/llm-foundry:2.2.1_cu121_flash2-36ab1ba` or take the latest one using `mosaicml/llm-foundry:2.2.1_cu121_flash2-latest`.
+You can select a specific commit hash such as `mosaicml/llm-foundry:2.3.0_cu121_flash2-36ab1ba` or take the latest one using `mosaicml/llm-foundry:2.3.0_cu121_flash2-latest`.
 
 **Please Note:** The `mosaicml/llm-foundry` images do not come with the `llm-foundry` package preinstalled, just the dependencies. You will still need to `pip install llm-foundry` either from PyPi or from source.
 
 | Docker Image                                           | Torch Version | Cuda Version      | LLM Foundry dependencies installed? |
 | ------------------------------------------------------ | ------------- | ----------------- | ----------------------------------- |
-| `mosaicml/pytorch:2.2.1_cu121-python3.11-ubuntu20.04`  | 2.2.1         | 12.1 (Infiniband) | No                                  |
-| `mosaicml/llm-foundry:2.2.1_cu121_flash2-latest`       | 2.2.1         | 12.1 (Infiniband) | Yes                                 |
-| `mosaicml/llm-foundry:2.2.1_cu121_flash2_aws-latest`   | 2.2.1         | 12.1 (EFA)        | Yes                                 |
+| `mosaicml/pytorch:2.3.0_cu121-python3.11-ubuntu20.04`  | 2.3.0         | 12.1 (Infiniband) | No                                  |
+| `mosaicml/llm-foundry:2.3.0_cu121_flash2-latest`       | 2.3.0         | 12.1 (Infiniband) | Yes                                 |
+| `mosaicml/llm-foundry:2.3.0_cu121_flash2_aws-latest`   | 2.3.0         | 12.1 (EFA)        | Yes                                 |
 
 
 # Installation
 
 This assumes you already have PyTorch, CMake, and packaging installed. If not, you can install them with `pip install cmake packaging torch`.
 
 To get started, clone the repo and set up your environment. Instructions to do so differ slightly depending on whether you're using Docker.
@@ -305,15 +320,15 @@
 name = "foundry_registry"
 version = "0.1.0"
 dependencies = [
     "mosaicml",
     "llm-foundry",
 ]
 
-[project.entry-points."llm_foundry.loggers"]
+[project.entry-points."llmfoundry_loggers"]
 my_logger = "foundry_registry.loggers:MyLogger"
 ```
 
 ### Direct call to register
 
 You can also register a component directly in your code:
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: llm-foundry Version: 0.7.0 Summary: LLM Foundry
-Home-page: https://github.com/mosaicml/llm-foundry/ Author: MosaicML Author-
-email: team@mosaicml.com Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1 Name: llm-foundry Version: 0.9.0.dev0 Summary: LLM
+Foundry Home-page: https://github.com/mosaicml/llm-foundry/ Author: MosaicML
+Author-email: team@mosaicml.com Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
 dev Provides-Extra: databricks Provides-Extra: tensorboard Provides-Extra: gpu-
-flash2 Provides-Extra: gpu Provides-Extra: peft Provides-Extra: olmo Provides-
-Extra: openai Provides-Extra: all-cpu Provides-Extra: all Provides-Extra: all-
-flash2 License-File: LICENSE
+flash2 Provides-Extra: gpu Provides-Extra: peft Provides-Extra: openai
+Provides-Extra: megablocks Provides-Extra: all-cpu Provides-Extra: all
+Provides-Extra: all-flash2 License-File: LICENSE
           _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _P_a_c_k_a_g_e_ _V_e_r_s_i_o_n_]_[_C_h_a_t_ _@_ _S_l_a_c_k_]_[_L_i_c_e_n_s_e_]
 
 # LLM Foundry This repository contains code for training, finetuning,
 evaluating, and deploying LLMs for inference with [Composer](https://
 github.com/mosaicml/composer) and the [MosaicML platform](https://
 forms.mosaicml.com/
 demo?utm_source=github.com&utm_medium=referral&utm_campaign=llm-foundry).
@@ -23,38 +23,52 @@
 HuggingFace and MPT models from 125M - 70B parameters * `train/benchmarking` -
 profile training throughput and MFU * `inference/` - convert models to
 HuggingFace or ONNX format, and generate responses * `inference/benchmarking` -
 profile inference latency and throughput * `eval/` - evaluate LLMs on academic
 (or custom) in-context-learning tasks * `mcli/` - launch any of these workloads
 using [MCLI](https://docs.mosaicml.com/projects/mcli/en/latest/) and the
 [MosaicML platform](https://www.mosaicml.com/platform) * `TUTORIAL.md` - a
-deeper dive into the repo, example workflows, and FAQs # MPT Mosaic Pretrained
-Transformers (MPT) are GPT-style models with some special features -- Flash
-Attention for efficiency, ALiBi for context length extrapolation, and stability
-improvements to mitigate loss spikes. As part of MosaicML's Foundation series,
-we have open-sourced several MPT models: | Model | Context Length | Download |
-Commercial use? | | ------------------ | -------------- | ---------------------
------------------------------ | --------------- | | MPT-30B | 8192 | https://
-huggingface.co/mosaicml/mpt-30b | Yes | | MPT-30B-Instruct | 8192 | https://
-huggingface.co/mosaicml/mpt-30b-instruct | Yes | | MPT-30B-Chat | 8192 | https:
-//huggingface.co/mosaicml/mpt-30b-chat | No | | MPT-7b-8k | 8192 | https://
-huggingface.co/mosaicml/mpt-7b-8k | Yes | | MPT-7b-8k-Chat | 8192 | https://
-huggingface.co/mosaicml/mpt-7b-8k-chat | No | | MPT-7B | 2048 | https://
-huggingface.co/mosaicml/mpt-7b | Yes | | MPT-7B-Instruct | 2048 | https://
-huggingface.co/mosaicml/mpt-7b-instruct | Yes | | MPT-7B-Chat | 2048 | https://
-huggingface.co/mosaicml/mpt-7b-chat | No | | MPT-7B-StoryWriter | 65536 |
-https://huggingface.co/mosaicml/mpt-7b-storywriter | Yes | To try out these
-models locally, [follow the instructions](https://github.com/mosaicml/llm-
-foundry/tree/main/scripts/inference#interactive-generation-with-modelgenerate)
-in `scripts/inference/README.md` to prompt HF models using our [hf_generate.py]
-(https://github.com/mosaicml/llm-foundry/blob/main/scripts/inference/
-hf_generate.py) or [hf_chat.py](https://github.com/mosaicml/llm-foundry/blob/
-main/scripts/inference/hf_chat.py) scripts. # MPT Community We've been
-overwhelmed by all the amazing work the community has put into MPT! Here we
-provide a few links to some of them: * [ReplitLM](https://github.com/replit/
+deeper dive into the repo, example workflows, and FAQs # DBRX DBRX is a state-
+of-the-art open source LLM trained by Databricks Mosaic team. It uses the
+Mixture-of-Experts (MoE) architecture and was trained with optimized versions
+of [Composer](https://github.com/mosaicml/composer), LLM Foundry, and
+[MegaBlocks](https://github.com/databricks/megablocks). The model has 132B
+total parameters and 36B active parameters. We have released two DBRX models: |
+Model | Context Length | Download | | ------------------ | -------------- | ---
+----------------------------------------------- | | DBRX Base | 32768 | https:/
+/huggingface.co/databricks/dbrx-base | | DBRX Instruct | 32768 | https://
+huggingface.co/databricks/dbrx-instruct | Our model weights and code are
+licensed for both researchers and commercial entities. The Databricks Open
+Source License can be found at [LICENSE](https://github.com/databricks/dbrx/
+LICENSE), and our Acceptable Use Policy can be found [here](https://
+www.databricks.com/legal/acceptable-use-policy-open-model). For more
+information about the DBRX models, see https://github.com/databricks/dbrx. #
+MPT Mosaic Pretrained Transformers (MPT) are GPT-style models with some special
+features -- Flash Attention for efficiency, ALiBi for context length
+extrapolation, and stability improvements to mitigate loss spikes. As part of
+MosaicML's Foundation series, we have open-sourced several MPT models: | Model
+| Context Length | Download | Commercial use? | | ------------------ | --------
+------ | -------------------------------------------------- | --------------- |
+| MPT-30B | 8192 | https://huggingface.co/mosaicml/mpt-30b | Yes | | MPT-30B-
+Instruct | 8192 | https://huggingface.co/mosaicml/mpt-30b-instruct | Yes | |
+MPT-30B-Chat | 8192 | https://huggingface.co/mosaicml/mpt-30b-chat | No | |
+MPT-7b-8k | 8192 | https://huggingface.co/mosaicml/mpt-7b-8k | Yes | | MPT-7b-
+8k-Chat | 8192 | https://huggingface.co/mosaicml/mpt-7b-8k-chat | No | | MPT-7B
+| 2048 | https://huggingface.co/mosaicml/mpt-7b | Yes | | MPT-7B-Instruct |
+2048 | https://huggingface.co/mosaicml/mpt-7b-instruct | Yes | | MPT-7B-Chat |
+2048 | https://huggingface.co/mosaicml/mpt-7b-chat | No | | MPT-7B-StoryWriter
+| 65536 | https://huggingface.co/mosaicml/mpt-7b-storywriter | Yes | To try out
+these models locally, [follow the instructions](https://github.com/mosaicml/
+llm-foundry/tree/main/scripts/inference#interactive-generation-with-
+modelgenerate) in `scripts/inference/README.md` to prompt HF models using our
+[hf_generate.py](https://github.com/mosaicml/llm-foundry/blob/main/scripts/
+inference/hf_generate.py) or [hf_chat.py](https://github.com/mosaicml/llm-
+foundry/blob/main/scripts/inference/hf_chat.py) scripts. # MPT Community We've
+been overwhelmed by all the amazing work the community has put into MPT! Here
+we provide a few links to some of them: * [ReplitLM](https://github.com/replit/
 replitLM): `replit-code-v1-3b` is a 2.7B Causal Language Model focused on Code
 Completion. The model has been trained on a subset of the Stack Dedup v1.2
 dataset covering 20 languages such as Java, Python, and C++ * [LLaVa-MPT]
 (https://github.com/haotian-liu/LLaVA#LLaVA-MPT-7b): Visual instruction tuning
 to get MPT multimodal capabilities * [ggml](https://github.com/ggerganov/ggml/
 tree/master): Optimized MPT version for efficient inference on consumer
 hardware * [GPT4All](https://gpt4all.io/index.html): locally running chat
@@ -64,55 +78,57 @@
 www.youtube.com/watch?v=DXpk9K7DgMo&t=3s) by [@jamesbriggs](https://
 www.youtube.com/@jamesbriggs) * [MPT-7B StoryWriter Intro](https://
 www.youtube.com/watch?v=O9Y_ZdsuKWQ) by [AItrepreneur](https://www.youtube.com/
 @Aitrepreneur) * [Fine-tuning MPT-7B on a single GPU](https://www.youtube.com/
 watch?v=KSlWkrByc0o&t=9s) by [@AIology2022](https://www.youtube.com/
 @AIology2022) * [How to Fine-tune MPT-7B-Instruct on Google Colab](https://
 youtu.be/3de0Utr9XnI) by [@VRSEN](https://www.youtube.com/@vrsen) Something
-missing? Contribute with a PR! # Latest News * [Blog: LLM Training and
-Inference with Intel Gaudi2 AI Accelerators](https://www.databricks.com/blog/
-llm-training-and-inference-intel-gaudi2-ai-accelerators) * [Blog: Training LLMs
-at Scale with AMD MI250 GPUs](https://www.databricks.com/blog/training-llms-
-scale-amd-mi250-gpus) * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML]
-(https://www.mosaicml.com/blog/amd-mi250) * [Blog: Announcing MPT-7B-8K: 8K
-Context Length for Document Understanding](https://www.mosaicml.com/blog/long-
-context-mpt-7b-8k) * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML]
-(https://www.mosaicml.com/blog/amd-mi250) * [Blog: MPT-30B: Raising the bar for
-open-source foundation models](https://www.mosaicml.com/blog/mpt-30b) * [Blog:
+missing? Contribute with a PR! # Latest News * [Blog: Introducing DBRX: A New
+State-of-the-Art Open LLM](https://www.databricks.com/blog/introducing-dbrx-
+new-state-art-open-llm) * [Blog: LLM Training and Inference with Intel Gaudi2
+AI Accelerators](https://www.databricks.com/blog/llm-training-and-inference-
+intel-gaudi2-ai-accelerators) * [Blog: Training LLMs at Scale with AMD MI250
+GPUs](https://www.databricks.com/blog/training-llms-scale-amd-mi250-gpus) *
+[Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://
+www.mosaicml.com/blog/amd-mi250) * [Blog: Announcing MPT-7B-8K: 8K Context
+Length for Document Understanding](https://www.mosaicml.com/blog/long-context-
+mpt-7b-8k) * [Blog: Training LLMs with AMD MI250 GPUs and MosaicML](https://
+www.mosaicml.com/blog/amd-mi250) * [Blog: MPT-30B: Raising the bar for open-
+source foundation models](https://www.mosaicml.com/blog/mpt-30b) * [Blog:
 Introducing MPT-7B](https://www.mosaicml.com/blog/mpt-7b) * [Blog: Benchmarking
 LLMs on H100](https://www.mosaicml.com/blog/coreweave-nvidia-h100-part-1) *
 [Blog: Blazingly Fast LLM Evaluation](https://www.mosaicml.com/blog/llm-
 evaluation-for-icl) * [Blog: GPT3 Quality for $500k](https://www.mosaicml.com/
 blog/gpt-3-quality-for-500k) * [Blog: Billion parameter GPT training made easy]
 (https://www.mosaicml.com/blog/billion-parameter-gpt-training-made-easy) #
 Hardware and Software Requirements This codebase has been tested with PyTorch
 2.2 with NVIDIA A100s and H100s. This codebase may also work on systems with
 other devices, such as consumer NVIDIA cards and AMD cards, but we are not
 actively testing these systems. If you have success/failure using LLM Foundry
 on other systems, please let us know in a Github issue and we will update the
 support matrix! | Device | Torch Version | Cuda Version | Status | | ----------
 ---- | ------------- | ------------ | ---------------------------- | | A100-
-40GB/80GB | 2.2.1 | 12.1 | :white_check_mark: Supported | | H100-80GB | 2.2.1 |
+40GB/80GB | 2.3.0 | 12.1 | :white_check_mark: Supported | | H100-80GB | 2.3.0 |
 12.1 | :white_check_mark: Supported | ## MosaicML Docker Images We highly
 recommend using our prebuilt Docker images. You can find them here: https://
 hub.docker.com/orgs/mosaicml/repositories. The `mosaicml/pytorch` images are
 pinned to specific PyTorch and CUDA versions, and are stable and rarely
 updated. The `mosaicml/llm-foundry` images are built with new tags upon every
 commit to the `main` branch. You can select a specific commit hash such as
-`mosaicml/llm-foundry:2.2.1_cu121_flash2-36ab1ba` or take the latest one using
-`mosaicml/llm-foundry:2.2.1_cu121_flash2-latest`. **Please Note:** The
+`mosaicml/llm-foundry:2.3.0_cu121_flash2-36ab1ba` or take the latest one using
+`mosaicml/llm-foundry:2.3.0_cu121_flash2-latest`. **Please Note:** The
 `mosaicml/llm-foundry` images do not come with the `llm-foundry` package
 preinstalled, just the dependencies. You will still need to `pip install llm-
 foundry` either from PyPi or from source. | Docker Image | Torch Version | Cuda
 Version | LLM Foundry dependencies installed? | | -----------------------------
 ------------------------- | ------------- | ----------------- | ---------------
--------------------- | | `mosaicml/pytorch:2.2.1_cu121-python3.11-ubuntu20.04`
-| 2.2.1 | 12.1 (Infiniband) | No | | `mosaicml/llm-foundry:2.2.1_cu121_flash2-
-latest` | 2.2.1 | 12.1 (Infiniband) | Yes | | `mosaicml/llm-foundry:
-2.2.1_cu121_flash2_aws-latest` | 2.2.1 | 12.1 (EFA) | Yes | # Installation This
+-------------------- | | `mosaicml/pytorch:2.3.0_cu121-python3.11-ubuntu20.04`
+| 2.3.0 | 12.1 (Infiniband) | No | | `mosaicml/llm-foundry:2.3.0_cu121_flash2-
+latest` | 2.3.0 | 12.1 (Infiniband) | Yes | | `mosaicml/llm-foundry:
+2.3.0_cu121_flash2_aws-latest` | 2.3.0 | 12.1 (EFA) | Yes | # Installation This
 assumes you already have PyTorch, CMake, and packaging installed. If not, you
 can install them with `pip install cmake packaging torch`. To get started,
 clone the repo and set up your environment. Instructions to do so differ
 slightly depending on whether you're using Docker. ### With Docker
 (recommended) We *strongly* recommend working with LLM Foundry inside a Docker
 container (see our recommended Docker image above). If you are doing so, follow
 these steps to clone the repo and install the requirements. ```bash git clone
@@ -193,15 +209,15 @@
 There are a few ways to register a new component: ### Python entrypoints You
 can specify registered components via a Python entrypoint if you are building
 your own package with registered components. For example, the following would
 register the `WandBLogger` class, under the key `wandb`, in the
 `llm_foundry.loggers` registry: ```yaml [build-system] requires =
 ["setuptools>=42", "wheel"] build-backend = "setuptools.build_meta" [project]
 name = "foundry_registry" version = "0.1.0" dependencies = [ "mosaicml", "llm-
-foundry", ] [project.entry-points."llm_foundry.loggers"] my_logger =
+foundry", ] [project.entry-points."llmfoundry_loggers"] my_logger =
 "foundry_registry.loggers:MyLogger" ``` ### Direct call to register You can
 also register a component directly in your code: ```python from
 composer.loggers import LoggerDestination from llmfoundry.registry import
 loggers class MyLogger(LoggerDestination): pass loggers.register("my_logger",
 func=MyLogger) ``` ### Decorators You can also use decorators to register
 components directly from your code: ```python from composer.loggers import
 LoggerDestination from llmfoundry.registry import loggers @loggers.register
```

### Comparing `llm-foundry-0.7.0/llm_foundry.egg-info/SOURCES.txt` & `llm-foundry-0.9.0.dev0/llm_foundry.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,37 +5,47 @@
 llm_foundry.egg-info/PKG-INFO
 llm_foundry.egg-info/SOURCES.txt
 llm_foundry.egg-info/dependency_links.txt
 llm_foundry.egg-info/entry_points.txt
 llm_foundry.egg-info/requires.txt
 llm_foundry.egg-info/top_level.txt
 llmfoundry/__init__.py
+llmfoundry/layers_registry.py
 llmfoundry/registry.py
 llmfoundry/algorithms/__init__.py
 llmfoundry/callbacks/__init__.py
 llmfoundry/callbacks/async_eval_callback.py
 llmfoundry/callbacks/curriculum_learning_callback.py
 llmfoundry/callbacks/eval_gauntlet_callback.py
+llmfoundry/callbacks/eval_output_logging_callback.py
 llmfoundry/callbacks/fdiff_callback.py
 llmfoundry/callbacks/hf_checkpointer.py
+llmfoundry/callbacks/log_mbmoe_tok_per_expert_callback.py
 llmfoundry/callbacks/monolithic_ckpt_callback.py
 llmfoundry/callbacks/resumption_callbacks.py
 llmfoundry/callbacks/scheduled_gc_callback.py
 llmfoundry/cli/__init__.py
 llmfoundry/cli/cli.py
 llmfoundry/cli/registry_cli.py
 llmfoundry/data/__init__.py
 llmfoundry/data/data.py
 llmfoundry/data/dataloader.py
 llmfoundry/data/packing.py
 llmfoundry/data/text_data.py
+llmfoundry/data/utils.py
 llmfoundry/data/finetuning/__init__.py
 llmfoundry/data/finetuning/collator.py
 llmfoundry/data/finetuning/dataloader.py
 llmfoundry/data/finetuning/tasks.py
+llmfoundry/eval/__init__.py
+llmfoundry/eval/datasets/__init__.py
+llmfoundry/eval/datasets/in_context_learning_evaluation.py
+llmfoundry/eval/datasets/utils.py
+llmfoundry/eval/metrics/__init__.py
+llmfoundry/eval/metrics/nlp.py
 llmfoundry/interfaces/__init__.py
 llmfoundry/interfaces/callback_with_config.py
 llmfoundry/loggers/__init__.py
 llmfoundry/metrics/__init__.py
 llmfoundry/metrics/token_acc.py
 llmfoundry/models/__init__.py
 llmfoundry/models/hf/__init__.py
@@ -47,23 +57,27 @@
 llmfoundry/models/inference_api_wrapper/fmapi.py
 llmfoundry/models/inference_api_wrapper/interface.py
 llmfoundry/models/inference_api_wrapper/openai_causal_lm.py
 llmfoundry/models/layers/__init__.py
 llmfoundry/models/layers/attention.py
 llmfoundry/models/layers/blocks.py
 llmfoundry/models/layers/custom_embedding.py
+llmfoundry/models/layers/dmoe.py
 llmfoundry/models/layers/fc.py
 llmfoundry/models/layers/ffn.py
+llmfoundry/models/layers/layer_builders.py
 llmfoundry/models/layers/norm.py
 llmfoundry/models/mpt/__init__.py
 llmfoundry/models/mpt/configuration_mpt.py
 llmfoundry/models/mpt/modeling_mpt.py
 llmfoundry/models/utils/__init__.py
 llmfoundry/models/utils/act_ckpt.py
+llmfoundry/models/utils/config_moe_args.py
 llmfoundry/models/utils/meta_init_context.py
+llmfoundry/models/utils/mpt_param_count.py
 llmfoundry/models/utils/param_init_fns.py
 llmfoundry/optim/__init__.py
 llmfoundry/optim/adaptive_lion.py
 llmfoundry/optim/lion.py
 llmfoundry/optim/outlier_detection.py
 llmfoundry/optim/scheduler.py
 llmfoundry/tokenizers/__init__.py
```

### Comparing `llm-foundry-0.7.0/llm_foundry.egg-info/requires.txt` & `llm-foundry-0.9.0.dev0/llm_foundry.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,121 @@
-mosaicml[gcs,libcloud,oci,wandb]<0.22,>=0.21.1
-mlflow<3,>=2.10
+mosaicml[gcs,libcloud,oci,wandb]<0.23,>=0.22.0
+mlflow<2.13,>=2.12.1
 accelerate<0.26,>=0.25
-transformers<4.39,>=4.38.2
-mosaicml-streaming<0.8,>=0.7.4
-torch<2.3,>=2.2.1
-datasets<2.17,>=2.16
+transformers<4.41,>=4.40
+mosaicml-streaming<0.8,>=0.7.5
+torch<2.4,>=2.3.0
+datasets<2.20,>=2.19
 fsspec==2023.6.0
 sentencepiece==0.1.97
 einops==0.7.0
 omegaconf<3,>=2.2.3
 slack-sdk<4
 mosaicml-cli<1,>=0.6.10
 onnx==1.14.0
 onnxruntime==1.15.1
 boto3<2,>=1.21.45
-huggingface-hub<1.0,>=0.17.0
+huggingface-hub<0.23,>=0.19.0
 beautifulsoup4<5,>=4.12.2
 tenacity<9,>=8.2.3
 catalogue<3,>=2
 typer[all]<1
 
 [all]
-pyright==1.1.256
 pytest_codeblocks<0.17,>=0.16.1
-pre-commit<4,>=3.4.0
-toml<0.11,>=0.10.2
-mosaicml[databricks]<0.22,>=0.21.1
+lz4<5,>=4
 pytest<8,>=7.2.1
-mosaicml[tensorboard]<0.22,>=0.21.1
-flash-attn==2.5.0
-hf_transfer==0.1.3
+pyright==1.1.256
+mosaicml[tensorboard]<0.23,>=0.22.0
+flash-attn==2.5.8
+pytest-cov<5,>=4
+grouped-gemm==0.1.4
 databricks-connect==14.1.0
-openai==1.3.8
+coverage[toml]==7.4.4
 tiktoken==0.4.0
-mosaicml[peft]<0.22,>=0.21.1
-ai2-olmo>0.2.4
-lz4<5,>=4
-packaging<23,>=21
-pytest-cov<5,>=4
+hf_transfer==0.1.3
+mosaicml[databricks]<0.23,>=0.22.0
+megablocks==0.5.1
+pre-commit<4,>=3.4.0
+openai==1.3.8
+toml<0.11,>=0.10.2
 databricks-sql-connector<4,>=3
+mosaicml[peft]<0.23,>=0.22.0
+packaging<23,>=21
 
 [all-cpu]
-pyright==1.1.256
 pytest_codeblocks<0.17,>=0.16.1
 pre-commit<4,>=3.4.0
-toml<0.11,>=0.10.2
-mosaicml[databricks]<0.22,>=0.21.1
-pytest<8,>=7.2.1
-mosaicml[tensorboard]<0.22,>=0.21.1
-hf_transfer==0.1.3
-databricks-connect==14.1.0
 openai==1.3.8
-tiktoken==0.4.0
-mosaicml[peft]<0.22,>=0.21.1
-ai2-olmo>0.2.4
 lz4<5,>=4
-packaging<23,>=21
+pytest<8,>=7.2.1
+pyright==1.1.256
+mosaicml[tensorboard]<0.23,>=0.22.0
+tiktoken==0.4.0
+toml<0.11,>=0.10.2
 pytest-cov<5,>=4
+hf_transfer==0.1.3
+databricks-connect==14.1.0
+coverage[toml]==7.4.4
+mosaicml[databricks]<0.23,>=0.22.0
+mosaicml[peft]<0.23,>=0.22.0
 databricks-sql-connector<4,>=3
+packaging<23,>=21
 
 [all-flash2]
-pyright==1.1.256
 pytest_codeblocks<0.17,>=0.16.1
-pre-commit<4,>=3.4.0
-toml<0.11,>=0.10.2
-mosaicml[databricks]<0.22,>=0.21.1
+lz4<5,>=4
 pytest<8,>=7.2.1
-mosaicml[tensorboard]<0.22,>=0.21.1
-flash-attn==2.5.0
-hf_transfer==0.1.3
+pyright==1.1.256
+mosaicml[tensorboard]<0.23,>=0.22.0
+flash-attn==2.5.8
+pytest-cov<5,>=4
+grouped-gemm==0.1.4
 databricks-connect==14.1.0
-openai==1.3.8
+coverage[toml]==7.4.4
 tiktoken==0.4.0
-mosaicml[peft]<0.22,>=0.21.1
-ai2-olmo>0.2.4
-lz4<5,>=4
-packaging<23,>=21
-pytest-cov<5,>=4
+hf_transfer==0.1.3
+mosaicml[databricks]<0.23,>=0.22.0
+megablocks==0.5.1
+pre-commit<4,>=3.4.0
+openai==1.3.8
+toml<0.11,>=0.10.2
 databricks-sql-connector<4,>=3
+mosaicml[peft]<0.23,>=0.22.0
+packaging<23,>=21
 
 [databricks]
-mosaicml[databricks]<0.22,>=0.21.1
+mosaicml[databricks]<0.23,>=0.22.0
 databricks-sql-connector<4,>=3
 databricks-connect==14.1.0
 lz4<5,>=4
 
 [dev]
+coverage[toml]==7.4.4
 pre-commit<4,>=3.4.0
 pytest<8,>=7.2.1
 pytest_codeblocks<0.17,>=0.16.1
 pytest-cov<5,>=4
 pyright==1.1.256
 toml<0.11,>=0.10.2
 packaging<23,>=21
 hf_transfer==0.1.3
 
 [gpu]
-flash-attn==2.5.0
+flash-attn==2.5.8
 
 [gpu-flash2]
-flash-attn==2.5.0
+flash-attn==2.5.8
 
-[olmo]
-ai2-olmo>0.2.4
+[megablocks]
+megablocks==0.5.1
+grouped-gemm==0.1.4
 
 [openai]
 openai==1.3.8
 tiktoken==0.4.0
 
 [peft]
-mosaicml[peft]<0.22,>=0.21.1
+mosaicml[peft]<0.23,>=0.22.0
 
 [tensorboard]
-mosaicml[tensorboard]<0.22,>=0.21.1
+mosaicml[tensorboard]<0.23,>=0.22.0
```

### Comparing `llm-foundry-0.7.0/llmfoundry/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,60 +8,67 @@
 warnings.filterwarnings('ignore', category=UserWarning, module='bitsandbytes')
 
 import logging
 
 from llmfoundry.utils.logging_utils import SpecificWarningFilter
 
 # Filter out Hugging Face warning for not using a pinned revision of the model
-hf_dynamic_modules_logger = logging.getLogger(
-    'transformers.dynamic_module_utils')
+logger = logging.getLogger('transformers.dynamic_module_utils')
 new_files_warning_filter = SpecificWarningFilter(
-    'A new version of the following files was downloaded from')
+    'A new version of the following files was downloaded from',
+)
 
-hf_dynamic_modules_logger.addFilter(new_files_warning_filter)
+logger.addFilter(new_files_warning_filter)
 
-from llmfoundry import algorithms, callbacks, loggers, optim, registry, utils
-from llmfoundry.data import (ConcatTokensDataset, NoConcatDataset,
-                             Seq2SeqFinetuningCollator,
-                             build_finetuning_dataloader)
-from llmfoundry.models.hf import ComposerHFCausalLM, ComposerHFT5
-from llmfoundry.models.layers.attention import (
-    MultiheadAttention, attn_bias_shape, build_alibi_bias, build_attn_bias,
-    flash_attn_fn, scaled_multihead_dot_product_attention)
-from llmfoundry.models.layers.blocks import MPTBlock
-from llmfoundry.models.layers.ffn import FFN_CLASS_REGISTRY, MPTMLP, build_ffn
-from llmfoundry.models.mpt import (ComposerMPTCausalLM, MPTConfig,
-                                   MPTForCausalLM, MPTModel, MPTPreTrainedModel)
-from llmfoundry.tokenizers import TiktokenTokenizerWrapper
+from llmfoundry import (
+    algorithms,
+    callbacks,
+    cli,
+    data,
+    eval,
+    interfaces,
+    loggers,
+    metrics,
+    models,
+    optim,
+    tokenizers,
+    utils,
+)
+from llmfoundry.data import StreamingFinetuningDataset, StreamingTextDataset
+from llmfoundry.eval import InContextLearningDataset, InContextLearningMetric
+from llmfoundry.models.hf import ComposerHFCausalLM
+from llmfoundry.models.mpt import (
+    ComposerMPTCausalLM,
+    MPTConfig,
+    MPTForCausalLM,
+    MPTModel,
+    MPTPreTrainedModel,
+)
+from llmfoundry.optim import DecoupledLionW
 
 __all__ = [
-    'build_finetuning_dataloader',
-    'Seq2SeqFinetuningCollator',
-    'MPTBlock',
-    'FFN_CLASS_REGISTRY',
-    'MPTMLP',
-    'build_ffn',
+    'StreamingFinetuningDataset',
+    'StreamingTextDataset',
+    'InContextLearningDataset',
+    'InContextLearningMetric',
+    'ComposerHFCausalLM',
     'MPTConfig',
     'MPTPreTrainedModel',
     'MPTModel',
     'MPTForCausalLM',
     'ComposerMPTCausalLM',
-    'ComposerHFCausalLM',
-    'ComposerHFT5',
-    'scaled_multihead_dot_product_attention',
-    'flash_attn_fn',
-    'MultiheadAttention',
-    'NoConcatDataset',
-    'ConcatTokensDataset',
-    'attn_bias_shape',
-    'build_attn_bias',
-    'build_alibi_bias',
-    'optim',
-    'utils',
-    'loggers',
+    'DecoupledLionW',
     'algorithms',
     'callbacks',
-    'TiktokenTokenizerWrapper',
-    'registry',
+    'cli',
+    'data',
+    'eval',
+    'interfaces',
+    'loggers',
+    'metrics',
+    'models',
+    'optim',
+    'tokenizers',
+    'utils',
 ]
 
-__version__ = '0.7.0'
+__version__ = '0.9.0.dev0'
```

### Comparing `llm-foundry-0.7.0/llmfoundry/callbacks/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
-from composer.callbacks import (EarlyStopper, Generate, LRMonitor,
-                                MemoryMonitor, MemorySnapshot, OOMObserver,
-                                OptimizerMonitor, RuntimeEstimator,
-                                SpeedMonitor)
+from composer.callbacks import (
+    EarlyStopper,
+    Generate,
+    LRMonitor,
+    MemoryMonitor,
+    MemorySnapshot,
+    OOMObserver,
+    OptimizerMonitor,
+    RuntimeEstimator,
+    SpeedMonitor,
+)
 
 from llmfoundry.callbacks.async_eval_callback import AsyncEval
 from llmfoundry.callbacks.curriculum_learning_callback import CurriculumLearning
 from llmfoundry.callbacks.eval_gauntlet_callback import EvalGauntlet
+from llmfoundry.callbacks.eval_output_logging_callback import EvalOutputLogging
 from llmfoundry.callbacks.fdiff_callback import FDiffMetrics
 from llmfoundry.callbacks.hf_checkpointer import HuggingFaceCheckpointer
+from llmfoundry.callbacks.log_mbmoe_tok_per_expert_callback import \
+    MegaBlocksMoE_TokPerExpert
 from llmfoundry.callbacks.monolithic_ckpt_callback import \
     MonolithicCheckpointSaver
-from llmfoundry.callbacks.resumption_callbacks import (GlobalLRScaling,
-                                                       LayerFreezing)
+from llmfoundry.callbacks.resumption_callbacks import (
+    GlobalLRScaling,
+    LayerFreezing,
+)
 from llmfoundry.callbacks.scheduled_gc_callback import ScheduledGarbageCollector
 from llmfoundry.registry import callbacks, callbacks_with_config
 
 callbacks.register('lr_monitor', func=LRMonitor)
 callbacks.register('memory_monitor', func=MemoryMonitor)
 callbacks.register('memory_snapshot', func=MemorySnapshot)
 callbacks.register('speed_monitor', func=SpeedMonitor)
@@ -29,22 +41,25 @@
 callbacks.register('fdiff_metrics', func=FDiffMetrics)
 callbacks.register('hf_checkpointer', func=HuggingFaceCheckpointer)
 callbacks.register('global_lr_scaling', func=GlobalLRScaling)
 callbacks.register('layer_freezing', func=LayerFreezing)
 callbacks.register('mono_checkpoint_saver', func=MonolithicCheckpointSaver)
 callbacks.register('scheduled_gc', func=ScheduledGarbageCollector)
 callbacks.register('oom_observer', func=OOMObserver)
+callbacks.register('eval_output_logging', func=EvalOutputLogging)
+callbacks.register('mbmoe_tok_per_expert', func=MegaBlocksMoE_TokPerExpert)
 
 callbacks_with_config.register('async_eval', func=AsyncEval)
 callbacks_with_config.register('curriculum_learning', func=CurriculumLearning)
 
 __all__ = [
     'FDiffMetrics',
     'MonolithicCheckpointSaver',
     'GlobalLRScaling',
     'LayerFreezing',
     'ScheduledGarbageCollector',
     'EvalGauntlet',
     'HuggingFaceCheckpointer',
+    'MegaBlocksMoE_TokPerExpert',
     'AsyncEval',
     'CurriculumLearning',
 ]
```

### Comparing `llm-foundry-0.7.0/llmfoundry/callbacks/async_eval_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/async_eval_callback.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,29 @@
 from collections import Counter
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from composer.callbacks import CheckpointSaver
 from composer.core import Event, State, Time, Timestamp, TimeUnit
 from composer.loggers import Logger
-from composer.loggers.mosaicml_logger import (MOSAICML_PLATFORM_ENV_VAR,
-                                              RUN_NAME_ENV_VAR)
+from composer.loggers.mosaicml_logger import (
+    MOSAICML_PLATFORM_ENV_VAR,
+    RUN_NAME_ENV_VAR,
+)
 from composer.utils import dist
 from composer.utils.file_helpers import list_remote_objects
 from composer.utils.misc import create_interval_scheduler
 
 from llmfoundry.interfaces import CallbackWithConfig
 from mcli import Run, RunConfig, create_run, get_run
 
 log = logging.getLogger(__name__)
 
+__all__ = ['AsyncEval']
+
 REQUIRED_PARAMS_FOR_EVAL = {
     'device_eval_batch_size',
     'icl_tasks',  # only required for eval, may not be specified in pure training
     'max_seq_len',
     'model',  # converted into models
     'tokenizer',  # converted into models
 }
@@ -59,23 +63,25 @@
         current_interval: The current interval string of the training run
 
     Returns:
         The new run name
     """
     name_without_uuid_suffix = training_run_name.rsplit('-', 1)[0]
 
-    max_length = MAX_RUN_NAME_BASE_LENGTH - len(RUN_NAME_PREFIX) - len(
-        current_interval) - 2
+    max_length = MAX_RUN_NAME_BASE_LENGTH - len(
+        RUN_NAME_PREFIX,
+    ) - len(current_interval) - 2
 
     # A run name that is too long will fail a createRun call
     if len(name_without_uuid_suffix) > max_length:
         new_name = name_without_uuid_suffix[:max_length]
         log.warning(
             f'Training run name {name_without_uuid_suffix} may be too long,' +
-            f' truncating to {new_name}')
+            f' truncating to {new_name}',
+        )
         name_without_uuid_suffix = new_name
 
     return f'{RUN_NAME_PREFIX}-{current_interval}-{name_without_uuid_suffix}'
 
 
 def get_eval_parameters(
     parameters: Dict[str, Any],
@@ -101,15 +107,15 @@
             subset_keys[key] = parameters[key]
         elif key in REQUIRED_PARAMS_FOR_EVAL:
             subset_keys[key] = parameters[key]
             looking_for.remove(key)
 
     if looking_for:
         raise Exception(
-            f'Missing the following required parameters for async eval: {looking_for}'
+            f'Missing the following required parameters for async eval: {looking_for}',
         )
 
     for logger, config in subset_keys.get('loggers', {}).items():
         if logger == 'wandb':
             config['group'] = config.pop('name', training_run_name)
 
         # mlflow currently does not support grouping, so this will just launch
@@ -120,45 +126,50 @@
 
     model_name = model.get('name', None)
     if not model_name:
         raise Exception(f'Async evaluation requires "name" keys for models')
     new_models = {
         'model_name': model_name,
         'model': model,
-        'load_path': checkpoint
+        'load_path': checkpoint,
     }
 
     tokenizer = subset_keys.pop('tokenizer', None)
     if tokenizer is not None:
         new_models['tokenizer'] = tokenizer
     subset_keys['models'] = [new_models]
     return subset_keys
 
 
-def validate_interval(interval: Union[str, int, Time],
-                      save_interval: Union[str, int, Time]) -> Time:
+def validate_interval(
+    interval: Union[str, int, Time],
+    save_interval: Union[str, int, Time],
+) -> Time:
 
     new_save_interval = Time.from_input(save_interval, TimeUnit.EPOCH)
     async_interval = Time.from_input(interval, TimeUnit.EPOCH)
 
     if new_save_interval.unit != async_interval.unit:
         raise ValueError(
-            'Save interval and async eval interval must be in the same unit')
+            'Save interval and async eval interval must be in the same unit',
+        )
     if async_interval < new_save_interval:
         raise ValueError(
-            'Async eval interval must be equal or greater (less frequent) than save interval'
+            'Async eval interval must be equal or greater (less frequent) than save interval',
         )
     if async_interval.value % new_save_interval.value != 0:
         raise ValueError(
-            'Async eval interval must be a multiple of save interval')
+            'Async eval interval must be a multiple of save interval',
+        )
     return async_interval
 
 
 def validate_eval_run_config(
-        eval_run_config: Optional[Dict[str, Any]]) -> Dict[str, Any]:
+    eval_run_config: Optional[Dict[str, Any]],
+) -> Dict[str, Any]:
 
     if not eval_run_config:
         return {}
 
     run_config = eval_run_config.copy()
 
     supported_keys = {'image', 'command', 'compute', 'scheduling'}
@@ -166,15 +177,16 @@
     for key in run_config:
         if key not in supported_keys:
             found_unsupported.add(key)
 
     if found_unsupported:
         raise ValueError(
             f'Unsupported eval run config keys found: {", ".join(found_unsupported)}'
-            + f'. Supported keys: {supported_keys}')
+            + f'. Supported keys: {supported_keys}',
+        )
 
     return run_config
 
 
 CHECKS_PER_INTERVAL = 4
 
 
@@ -204,49 +216,53 @@
             All fields are optional, but if specified, must be valid for a mcli run config. We
             provide this optional config to give you the most flexibility in customizing the eval
             run, but it is recommended to use the default values unless you have a specific use case
     """
 
     def __init__(
         self,
-        training_params: Dict[str, Any],
+        train_config: Dict[str, Any],
         interval: Union[str, int, Time],
         eval_run_config: Optional[Dict[str, Any]] = None,
     ):
 
         # Run these during init to fail fast in any of the error cases
         for required in ('save_interval', 'save_folder'):
-            if required not in training_params:
+            if required not in train_config:
                 raise ValueError(f'{required} required for async eval')
 
-        if '/' in training_params.get('save_filename', ''):
+        if '/' in train_config.get('save_filename', ''):
             raise ValueError(
-                'AsyncEval not supported for save_filename that includes a path'
+                'AsyncEval not supported for save_filename that includes a path',
             )
 
-        self.checkpoint_save_folder = training_params['save_folder']
-        self.training_params = training_params
+        self.checkpoint_save_folder = train_config['save_folder']
+        self.training_params = train_config
         self.eval_run_config = validate_eval_run_config(eval_run_config)
 
         self.current_run = self._get_current_run()
         get_eval_parameters(
-            parameters=training_params,
+            parameters=train_config,
             checkpoint='test',
             training_run_name=self.current_run.name,
         )
 
         # Validate the interval (how often to launch eval runs)
-        self.interval = validate_interval(interval,
-                                          self.training_params['save_interval'])
+        self.interval = validate_interval(
+            interval,
+            self.training_params['save_interval'],
+        )
 
         # Configures how often to check for new checkpoints. This is semi-arbitrary;
         # really we just want to check often enough to pull relevant checkpoints
         # but not so often that we're constantly checking
-        check_interval_value = max(self.interval.value // CHECKS_PER_INTERVAL,
-                                   1)
+        check_interval_value = max(
+            self.interval.value // CHECKS_PER_INTERVAL,
+            1,
+        )
         self.check_interval = Time(check_interval_value, self.interval.unit)
 
         # Keep track of checkpoints that have already been evaled
         # Format: {eval_timestamp: (checkpoint, run_name)}
         self.checkpoints_evaled: Dict[Time, Tuple[str, str]] = {}
 
         # Scheduling is based on the check interval, while _get_checkpoints_and_launch_runs
@@ -254,16 +270,18 @@
         self.is_at_check_interval = create_interval_scheduler(
             self.check_interval,
             # There is a custom close to ensure that the final checkpoint
             # (which is the most important) is evaled after it is written
             include_end_of_training=False,
         )
 
-        log.info('Initialized AsyncEval callback. Will generate runs at ' +
-                 f'interval {interval}, checking at {self.check_interval}')
+        log.info(
+            'Initialized AsyncEval callback. Will generate runs at ' +
+            f'interval {interval}, checking at {self.check_interval}',
+        )
 
     def state_dict(self) -> Dict[str, Any]:
         checkpoints_evaled = []
         for eval_ts, (checkpoint, run_name) in self.checkpoints_evaled.items():
             eval_ts_dict = {
                 'value': eval_ts.value,
                 'unit': eval_ts.unit.value,
@@ -278,15 +296,15 @@
         previous_checkpoints_evaled = state_dict.get('checkpoints_evaled', [])
         if previous_checkpoints_evaled:
             for (eval_ts, checkpoint, run_name) in previous_checkpoints_evaled:
                 eval_ts = Time(eval_ts['value'], TimeUnit(eval_ts['unit']))
                 self.checkpoints_evaled[eval_ts] = (checkpoint, run_name)
 
             log.info(
-                f'Loaded previous checkpoints evaled: {self.checkpoints_evaled}'
+                f'Loaded previous checkpoints evaled: {self.checkpoints_evaled}',
             )
 
     @staticmethod
     def _get_ready_sharded_checkpoints(
         checkpointer_checkpoints: Dict[str, Timestamp],
         remote_files: List[str],
     ) -> Dict[str, Timestamp]:
@@ -312,20 +330,20 @@
         checkpoints_to_eval = {}
         for checkpoint, checkpoint_ts in checkpointer_checkpoints.items():
             # eg {save_folder}/ep0-ba1/file.blah.
             checkpoint_ts_path = Path(checkpoint).parts[-2]
 
             # expecting one shard per gpu + 1 for metadata
             expected_shard_count = dist.get_world_size() + 1
-            if remote_file_group_counts[
-                    checkpoint_ts_path] != expected_shard_count:
+            if remote_file_group_counts[checkpoint_ts_path
+                                       ] != expected_shard_count:
                 log.debug(
                     f'Checkpoint {checkpoint} not fully uploaded (missing shards '
                     +
-                    f'{remote_file_group_counts[checkpoint_ts_path]}/{expected_shard_count}), skipping'
+                    f'{remote_file_group_counts[checkpoint_ts_path]}/{expected_shard_count}), skipping',
                 )
                 continue
 
             checkpoints_to_eval[checkpoint_ts_path] = checkpoint_ts
 
         return checkpoints_to_eval
 
@@ -351,15 +369,16 @@
         for checkpoint, checkpoint_ts in checkpointer_checkpoints.items():
             # This assumes checkpoint_ts_path is unique per checkpoint,
             # eg the default {save_folder}/ep0-ba1-rank0.pt
             checkpoint_ts_path = Path(checkpoint).parts[-1]
 
             if checkpoint not in unique_remote_checkpoints:
                 log.debug(
-                    f'Checkpoint {checkpoint} not fully uploaded, skipping')
+                    f'Checkpoint {checkpoint} not fully uploaded, skipping',
+                )
                 continue
 
             checkpoints_to_eval[checkpoint_ts_path] = checkpoint_ts
         return checkpoints_to_eval
 
     def _get_checkpoints_and_launch_runs(self, state: State):
         """Get the latest checkpoint from the training run.
@@ -373,51 +392,57 @@
         checkpointer = None
         for callback in state.callbacks:
             if isinstance(callback, CheckpointSaver):
                 if checkpointer is None:
                     checkpointer = callback
                 else:
                     log.warning(
-                        'Multiple checkpoint savers found. Using the first one')
+                        'Multiple checkpoint savers found. Using the first one',
+                    )
 
         if not checkpointer:
             warnings.warn('No checkpoint saver callback found. Skipping eval')
             return
 
         if not checkpointer.all_saved_checkpoints_to_timestamp:
             log.debug(
-                'No saved checkpoints found on the checkpointer. Skipping eval')
+                'No saved checkpoints found on the checkpointer. Skipping eval',
+            )
             return
 
         log.debug(
             f'Found {len(checkpointer.all_saved_checkpoints_to_timestamp)} ' +
-            f'checkpoints: {checkpointer.all_saved_checkpoints_to_timestamp}')
+            f'checkpoints: {checkpointer.all_saved_checkpoints_to_timestamp}',
+        )
 
         remote_checkpoints = list_remote_objects(self.checkpoint_save_folder)
 
         if not remote_checkpoints:
             log.debug('No saved checkpoints found yet on remote. Skipping eval')
             return
 
         if state.fsdp_sharded_state_dict_enabled:
             checkpoints_to_eval = self._get_ready_sharded_checkpoints(
                 checkpointer.all_saved_checkpoints_to_timestamp,
-                remote_checkpoints)
+                remote_checkpoints,
+            )
         else:
             checkpoints_to_eval = self._get_ready_single_checkpoints(
                 checkpointer.all_saved_checkpoints_to_timestamp,
-                remote_checkpoints)
+                remote_checkpoints,
+            )
 
         for checkpoint_interval_path, checkpoint_timestamp in checkpoints_to_eval.items(
         ):
             checkpoint_ts = checkpoint_timestamp.get(self.interval.unit)
             if checkpoint_ts.value % self.interval.value != 0:
                 log.debug(
                     f'Checkpoint {checkpoint_interval_path} ({checkpoint_ts}) is '
-                    + f'not at an eval interval ({self.interval}), skipping')
+                    + f'not at an eval interval ({self.interval}), skipping',
+                )
                 continue
             if checkpoint_ts in self.checkpoints_evaled:
                 continue  # Skip checkpoints that have already been evaled
 
             full_checkpoint_path = f'{self.checkpoint_save_folder}/{checkpoint_interval_path}'
             eval_run = self.launch_run(full_checkpoint_path, checkpoint_ts)
             self.checkpoints_evaled[checkpoint_ts] = (
@@ -448,44 +473,48 @@
         # Eval any remaining checkpoints
         self._get_checkpoints_and_launch_runs(state)
 
         # Eval the latest checkpoint
         latest_timestamp = state.timestamp.get(self.interval.unit)
         if latest_timestamp not in self.checkpoints_evaled:
             save_latest_filename = self.training_params.get(
-                'save_latest_filename', None)
+                'save_latest_filename',
+                None,
+            )
 
             if not save_latest_filename:
                 rank = dist.get_global_rank()
                 save_latest_filename = f'latest-rank{rank}.pt'
 
             checkpoint = f'{self.checkpoint_save_folder}/{save_latest_filename}'
 
             eval_run = self.launch_run(checkpoint, latest_timestamp)
-            self.checkpoints_evaled[latest_timestamp] = (checkpoint,
-                                                         eval_run.name)
+            self.checkpoints_evaled[latest_timestamp] = (
+                checkpoint,
+                eval_run.name,
+            )
 
         log.info(
-            f'AsyncEval callback finished. Launched {len(self.checkpoints_evaled)} eval runs:'
+            f'AsyncEval callback finished. Launched {len(self.checkpoints_evaled)} eval runs:',
         )
         for checkpoint_ts, (checkpoint,
                             run_name) in self.checkpoints_evaled.items():
             log.info(f'  {checkpoint_ts}: {checkpoint}, {run_name}')
 
     def _get_current_run(self) -> Run:
         if os.environ.get(MOSAICML_PLATFORM_ENV_VAR,
                           'false').lower() == 'false':
             raise RuntimeError(
-                'AsyncEval callback is only supported when running on the MosaicML platform'
+                'AsyncEval callback is only supported when running on the MosaicML platform',
             )
 
         run_name = os.environ.get(RUN_NAME_ENV_VAR, None)
         if not run_name:
             raise RuntimeError(
-                'RUN_NAME environment variable must be set to use the AsyncEval callback'
+                'RUN_NAME environment variable must be set to use the AsyncEval callback',
             )
 
         # Allows the MapiException to be raised if the run doesn't exist
         return get_run(run_name, include_details=True)
 
     def launch_run(self, checkpoint: str, current_interval: Time) -> Run:
         """Launch a new eval run.
@@ -536,15 +565,16 @@
             # behaviors because its not using custom repos or branches specified
             # in the training run. For this reason, we'll log a warning
             version = f'v{latest_foundry_version}'
             log.warning(
                 'No github integration found for llm-foundry. Adding installation '
                 + f'to eval run for latest foundry release ({version}). ' +
                 'To use a fork, custom branch, or custom version, configure ' +
-                'llm-foundry installation through a github integration')
+                'llm-foundry installation through a github integration',
+            )
             integrations.append({
                 'integration_type': 'git_repo',
                 'git_repo': 'mosaicml/llm-foundry',
                 'git_branch': version,
                 'pip_install': '-e .[gpu]',
                 'ssh_clone': False,
             })
```

### Comparing `llm-foundry-0.7.0/llmfoundry/callbacks/curriculum_learning_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/curriculum_learning_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,68 +16,74 @@
 from torch.utils.data import DataLoader
 
 from llmfoundry.interfaces import CallbackWithConfig
 from llmfoundry.utils.warnings import experimental_class
 
 log = logging.getLogger(__name__)
 
+__all__ = ['CurriculumLearning']
+
 
 @experimental_class('CurriculumLearning callback')
 class CurriculumLearning(CallbackWithConfig):
     """Starts an epoch with a different dataset when resuming from a checkpoint.
 
     Args:
         dataset_index (int): The index of the dataset currently being used.
         current_dataset_config (Dict): The configuration of the dataset currently
             being used.
     """
 
-    def __init__(self, dataset_index: int, train_config: Dict):
+    def __init__(self, train_config: Dict, dataset_index: int):
         self.dataset_index = dataset_index
         self.saved_dataset_index = 0
         self.all_dataset_configs = []
         self.current_dataset_state = {}
         # The current dataset config is resolved and passed in train.py
-        self.current_dataset_config = train_config['dataloader']
+        self.current_dataset_config = train_config['train_loader']
 
     def before_load(self, state: State, logger: Logger):
         del logger
 
         # Save the current dataset state so we can restore it correctly
         # if we are resuming with a new dataset.
         train_loader = state.train_dataloader
         # Check if we are using a DataLoader and StreamingDataset
         if not isinstance(train_loader, DataLoader):
             raise ValueError(
                 f'CurriculumLearning callback can only be used with a train ',
-                f'dataloader of type DataLoader, but got {type(train_loader)}.')
+                f'dataloader of type DataLoader, but got {type(train_loader)}.',
+            )
         dataset = train_loader.dataset
         if not isinstance(dataset, StreamingDataset):
             raise ValueError(
                 f'CurriculumLearning callback only supports StreamingDataset ',
                 f'because it requires loading and saving dataset state. ',
-                f'Instead, got a dataset of type {type(dataset)}')
+                f'Instead, got a dataset of type {type(dataset)}',
+            )
         assert isinstance(dataset, StreamingDataset)
         # Save the current dataset state so we can restore it if needed.
         self.current_dataset_state = dataset.state_dict(  # type: ignore
             num_samples=0, from_beginning=False)
 
     def after_load(self, state: State, logger: Logger):
         del logger
 
         # As saved_dataset_index is loaded from state_dict, this only runs when
         # a user explicitly increments the dataset_index and not on any other
         # resumption, including autoresume.
         train_loader = state._train_dataloader
         assert isinstance(
             train_loader,
-            DataLoader), 'CurriculumLearning callback requires a DataLoader.'
+            DataLoader,
+        ), 'CurriculumLearning callback requires a DataLoader.'
         dataset = train_loader.dataset
         assert isinstance(
-            dataset, StreamingDataset
+            dataset,
+            StreamingDataset,
         ), 'CurriculumLearning callback requires a StreamingDataset.'
         if self.saved_dataset_index < self.dataset_index:
             # Ignore the dataset state that was read in from the checkpoint, and
             # replace with the new dataset state. This preserves resumption info.
             if self.current_dataset_state['epoch'] < 0:
                 # Make sure the epoch in the loaded state dict is not negative.
                 # Since `__iter__` has not yet been called on the dataset, the
@@ -95,13 +101,13 @@
         elif self.dataset_index == 0 and len(self.all_dataset_configs) == 0:
             # Make sure to track our current dataset config if we are just starting training.
             self.all_dataset_configs.append(self.current_dataset_config)
 
     def state_dict(self):
         return {
             'dataset_index': self.dataset_index,
-            'all_dataset_configs': self.all_dataset_configs
+            'all_dataset_configs': self.all_dataset_configs,
         }
 
     def load_state_dict(self, state: Dict[str, Any]):
         self.saved_dataset_index = state.get('dataset_index', 0)
         self.all_dataset_configs = state.get('all_dataset_configs', [])
```

### Comparing `llm-foundry-0.7.0/llmfoundry/callbacks/eval_gauntlet_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/eval_gauntlet_callback.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 
 class Weighting(Enum):
     EQUAL = 1
     SAMPLE_SZ = 2
     LOG_SAMPLE_SZ = 3
 
 
-def calculate_named_averages(average_names: Dict[str, list],
-                             category_scores: Dict[str, float]):
+def calculate_named_averages(
+    average_names: Dict[str, list],
+    category_scores: Dict[str, float],
+):
     """Calculates the named averages based off the raw category scores.
 
     For each named average, take a simple average of all the category scores associated with that named average.
 
     Args:
         average_names (dict[str, list]):  Contains a mapping of named averages to which category scores that average should consist of.
         category_scores (dict[str, float]): Contains the raw scores corresponding to each category.
@@ -36,16 +38,17 @@
     for avg_name, category_list in average_names.items():
         composite_subset = {
             category: score
             for category, score in category_scores.items()
             if category in category_list
         }
         if len(composite_subset.values()) > 0:
-            average_scores[avg_name] = sum(composite_subset.values()) / len(
-                composite_subset.values())
+            average_scores[avg_name] = sum(
+                composite_subset.values(),
+            ) / len(composite_subset.values())
         else:
             average_scores[avg_name] = 0
 
     return average_scores
 
 
 class EvalGauntlet(Callback):
@@ -68,33 +71,36 @@
                                           from the performance on each individual benchmark before aggregating.
         rescale_accuracy (bool): Flag determining whether to rescale the accuracy on each benchmark
                                  by (1-random_baseline_accuracy) before aggregating. Using this ensures that all benchmarks max out at 1.0.
         benchmark_sizes (Optional[dict]): Optional data on benchmark sizes, used when not relying on equal weighting.
         averages (Optional[dict]): Optional dictionary specifying a mapping from a average names to lists of categories used produce each named average.
     """
 
-    def __init__(self,
-                 logger_keys: list,
-                 categories: dict,
-                 weighting: str = 'EQUAL',
-                 subtract_random_baseline: bool = True,
-                 rescale_accuracy: bool = True,
-                 benchmark_sizes: Optional[dict] = None,
-                 averages: Optional[dict] = None):
+    def __init__(
+        self,
+        logger_keys: list,
+        categories: dict,
+        weighting: str = 'EQUAL',
+        subtract_random_baseline: bool = True,
+        rescale_accuracy: bool = True,
+        benchmark_sizes: Optional[dict] = None,
+        averages: Optional[dict] = None,
+    ):
         if isinstance(logger_keys, dict):
             raise ValueError(
-                'logger_keys now requires a list type as input, not a dict')
+                'logger_keys now requires a list type as input, not a dict',
+            )
         if weighting != Weighting.EQUAL and benchmark_sizes is None:
             raise Exception(
-                'When not using equal weighting, you must provide the benchmark sizes.'
+                'When not using equal weighting, you must provide the benchmark sizes.',
             )
 
         if rescale_accuracy and not subtract_random_baseline:
             raise Exception(
-                'Only use accuracy rescaling in conjunction with subtracting random baseline accuracy.'
+                'Only use accuracy rescaling in conjunction with subtracting random baseline accuracy.',
             )
 
         self.categories = categories
         self.category_names = [conf.get('name') for conf in self.categories]
         self.weighting = Weighting[weighting]
         self.subtract_random_baseline = subtract_random_baseline
         self.rescale_accuracy = rescale_accuracy
@@ -102,16 +108,20 @@
         for category in self.categories:
             for benchmark in category['benchmarks']:
                 bench_name = f"{benchmark['name']}/{benchmark['num_fewshot']}-shot"
 
                 if self.weighting != Weighting.EQUAL:
                     assert benchmark_sizes is not None
                     cumulative_samples = max(
-                        sum(count for name, count in benchmark_sizes.items()
-                            if name.startswith(bench_name)), 1)
+                        sum(
+                            count for name, count in benchmark_sizes.items()
+                            if name.startswith(bench_name)
+                        ),
+                        1,
+                    )
                 else:
                     cumulative_samples = -1  # pyright
 
                 weight = None
                 if self.weighting == Weighting.EQUAL:
                     weight = 1
                 elif self.weighting == Weighting.SAMPLE_SZ:
@@ -127,15 +137,15 @@
         else:
             # if no averages spec provided, simply average everything
             self.averages['default_average'] = self.category_names
 
         for avg_name in self.averages:
             if avg_name in self.category_names:
                 raise ValueError(
-                    f'Found average name `{avg_name}` used as category name. Average names and category names must be non-overlapping.'
+                    f'Found average name `{avg_name}` used as category name. Average names and category names must be non-overlapping.',
                 )
 
     def extract_metrics_from_state(self, state: State) -> Dict[str, float]:
         results = {}
 
         for key in self.logger_keys:
 
@@ -168,45 +178,50 @@
             missing_metrics = []
             category_scores[category['name']] = []
             for benchmark in category['benchmarks']:
                 key = f"{benchmark['name']}/{benchmark['num_fewshot']}-shot"
 
                 if key not in computed_metrics:
                     log.warning(
-                        f'Could not find results for benchmark: {benchmark}.')
+                        f'Could not find results for benchmark: {benchmark}.',
+                    )
                     missing_metrics.append(key)
                 else:
                     score = computed_metrics[key]
 
                     if self.subtract_random_baseline:
                         score -= benchmark['random_baseline']
 
                     if self.rescale_accuracy and self.subtract_random_baseline:
                         score /= 1.0 - benchmark['random_baseline']
 
                     category_scores[category['name']].append({
                         'name': benchmark['name'],
                         'score': score,
-                        'weighting': benchmark['weighting']
+                        'weighting': benchmark['weighting'],
                     })
 
             if len(missing_metrics) > 0:
                 log.warning(
-                    f"Removing category `{category['name']}` from scores because benchmarks were missing: {missing_metrics}"
+                    f"Removing category `{category['name']}` from scores because benchmarks were missing: {missing_metrics}",
                 )
                 del category_scores[category['name']]
                 continue
             total_weight = sum(
-                k['weighting'] for k in category_scores[category['name']])
+                k['weighting'] for k in category_scores[category['name']]
+            )
             category_scores[category['name']] = sum(
                 k['score'] * (k['weighting'] / total_weight)
-                for k in category_scores[category['name']])
+                for k in category_scores[category['name']]
+            )
 
-        named_averages = calculate_named_averages(self.averages,
-                                                  category_scores)
+        named_averages = calculate_named_averages(
+            self.averages,
+            category_scores,
+        )
         category_scores.update(named_averages)
         category_scores = {
             f'icl/metrics/eval_gauntlet/{k}': v
             for k, v in category_scores.items()
         }
         if logger is not None:
             logger.log_metrics(category_scores)
```

### Comparing `llm-foundry-0.7.0/llmfoundry/callbacks/fdiff_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/fdiff_callback.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,46 +4,52 @@
 """Monitor rate of change of loss."""
 from __future__ import annotations
 
 import torch
 from composer.core import Callback, State
 from composer.loggers import Logger
 
+__all__ = ['FDiffMetrics']
+
 
 class FDiffMetrics(Callback):
     """Rate of change of metrics.
 
     tracks and plots the rate of change of metrics effectively taking the
     numerical derivative of the metrics
     """
 
-    def __init__(self,
-                 diff_train_metrics: bool = False,
-                 diff_eval_metrics: bool = True):
+    def __init__(
+        self,
+        diff_train_metrics: bool = False,
+        diff_eval_metrics: bool = True,
+    ):
         self.diff_train_metrics = diff_train_metrics
         self.diff_eval_metrics = diff_eval_metrics
 
         self.train_prev_loss = None
         self.train_prev_metric = {}
         self.eval_prev_metric = {}
 
     def batch_end(self, state: State, logger: Logger) -> None:
         if self.diff_train_metrics:
             if not isinstance(state.loss, torch.Tensor):
                 raise NotImplementedError('Multiple losses not supported yet')
             loss = state.loss.item()
             if self.train_prev_loss:
-                logger.log_metrics(
-                    {'loss/train/total_fdiff': loss - self.train_prev_loss})
+                logger.log_metrics({
+                    'loss/train/total_fdiff': loss - self.train_prev_loss,
+                })
             self.train_prev_loss = loss
 
             for k in self.train_prev_metric.keys():
                 logger.log_metrics({
                     f'metrics/train/{k}_fdiff':
-                        state.train_metric_values[k] - self.train_prev_metric[k]
+                        state.train_metric_values[k] -
+                        self.train_prev_metric[k],
                 })
 
             for k in state.train_metric_values.keys():
                 value = state.train_metric_values[k]
                 self.train_prev_metric[k] = value
 
     def eval_end(self, state: State, logger: Logger) -> None:
@@ -55,13 +61,13 @@
 
             for k in metrics:
                 mkey = '/'.join(['metrics', evaluator, k])
                 if mkey in self.eval_prev_metric.keys():
                     logger.log_metrics({
                         f'{mkey}_fdiff':
                             state.eval_metric_values[k] -
-                            self.eval_prev_metric[mkey]
+                            self.eval_prev_metric[mkey],
                     })
 
             for k in metrics:
                 mkey = '/'.join(['metrics', evaluator, k])
                 self.eval_prev_metric[mkey] = state.eval_metric_values[k]
```

### Comparing `llm-foundry-0.7.0/llmfoundry/callbacks/hf_checkpointer.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/hf_checkpointer.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,79 +3,126 @@
 
 import contextlib
 import copy
 import logging
 import math
 import os
 import re
+import shutil
 import tempfile
+import time
+from multiprocessing.context import SpawnProcess
 from pathlib import Path
-from typing import Any, Dict, Optional, Sequence, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
+import numpy as np
 import torch
+import torch.nn as nn
 from composer.core import Callback, Event, State, Time, TimeUnit
 from composer.core.state import fsdp_state_dict_type_context
 from composer.loggers import Logger, MLFlowLogger
 from composer.models import HuggingFaceModel
-from composer.utils import (dist, format_name_with_dist_and_time,
-                            maybe_create_remote_uploader_downloader_from_uri,
-                            parse_uri)
+from composer.utils import (
+    dist,
+    format_name_with_dist_and_time,
+    maybe_create_remote_uploader_downloader_from_uri,
+    parse_uri,
+)
 from composer.utils.misc import create_interval_scheduler
 from mlflow.transformers import _fetch_model_card, _write_license_information
+from packaging import version
 from transformers import PreTrainedModel, PreTrainedTokenizerBase
 
 from llmfoundry.models.mpt import MPTConfig, MPTForCausalLM
 from llmfoundry.models.utils import init_empty_weights
 from llmfoundry.utils.huggingface_hub_utils import \
     edit_files_for_hf_compatibility
 
 log = logging.getLogger(__name__)
 
+__all__ = ['HuggingFaceCheckpointer']
+
 _LICENSE_FILE_PATTERN = re.compile(r'license(\.[a-z]+|$)', re.IGNORECASE)
 
 
 def _maybe_get_license_filename(
-        local_dir: str,
-        pretrained_model_name: Optional[str] = None) -> Optional[str]:
+    local_dir: str,
+    pretrained_model_name: Optional[str] = None,
+) -> Optional[str]:
     """Returns the name of the license file if it exists in the local_dir.
 
     Note: This is intended to be consistent with the code in MLflow.
     https://github.com/mlflow/mlflow/blob/5d13d6ec620a02de9a5e31201bf1becdb9722ea5/mlflow/transformers/__init__.py#L1152
 
     Since LLM Foundry supports local model files being used rather than fetching the files from the Hugging Face Hub,
     MLflow's logic to fetch and write the license information on model save is not applicable; it will try to search for
     a Hugging Face repo named after the local path. However, the user can provide the original pretrained model name,
     in which case this function will use that to fetch the correct license information.
 
     If the license file does not exist, returns None.
     """
     try:
-        license_filename = next(file for file in os.listdir(local_dir)
-                                if _LICENSE_FILE_PATTERN.search(file))
+        license_filename = next(
+            file for file in os.listdir(local_dir)
+            if _LICENSE_FILE_PATTERN.search(file)
+        )
 
         # If a pretrained model name is provided, replace the license file with the correct info from HF Hub.
         if pretrained_model_name is not None:
             log.info(
-                f'Overwriting license file {license_filename} with license info for model {pretrained_model_name} from Hugging Face Hub'
+                f'Overwriting license file {license_filename} with license info for model {pretrained_model_name} from Hugging Face Hub',
             )
             os.remove(os.path.join(local_dir, license_filename))
             model_card = _fetch_model_card(pretrained_model_name)
 
             local_dir_path = Path(local_dir).absolute()
-            _write_license_information(pretrained_model_name, model_card,
-                                       local_dir_path)
-            license_filename = next(file for file in os.listdir(local_dir)
-                                    if _LICENSE_FILE_PATTERN.search(file))
+            _write_license_information(
+                pretrained_model_name,
+                model_card,
+                local_dir_path,
+            )
+            license_filename = next(
+                file for file in os.listdir(local_dir)
+                if _LICENSE_FILE_PATTERN.search(file)
+            )
 
         return license_filename
 
     except StopIteration:
         return None
 
 
+def _register_model_with_run_id_multiprocess(
+    mlflow_logger: MLFlowLogger,
+    composer_logging_level: int,
+    model_uri: str,
+    name: str,
+    await_creation_for: int,
+):
+    """Call MLFlowLogger.register_model_with_run_id.
+
+    Used mainly to register from a child process.
+    """
+    # Setup logging for child process. This ensures that any logs from composer are surfaced.
+    if composer_logging_level > 0:
+        # If logging_level is 0, then the composer logger was unset.
+        logging.basicConfig(
+            format=
+            f'%(asctime)s: rank{dist.get_global_rank()}[%(process)d][%(threadName)s]: %(levelname)s: %(name)s: %(message)s',
+        )
+        logging.getLogger('composer').setLevel(composer_logging_level)
+
+    # Register model.
+    mlflow_logger.register_model_with_run_id(
+        model_uri=model_uri,
+        name=name,
+        await_creation_for=await_creation_for,
+    )
+
+
 class HuggingFaceCheckpointer(Callback):
     """Save a huggingface formatted checkpoint during training.
 
     Args:
         save_folder (str): Top level folder to save checkpoints to (can be a
             URI). It is likely that this would be the same as your save_folder.
         save_interval: Union[str, int, Time]: The interval describing how often
@@ -99,23 +146,23 @@
             and signature intended for text generation is also included under the
             keys ``input_example`` and ``signature``.
         flatten_imports (Sequence[str]): A sequence of import prefixes that will
             be flattened when editing MPT files.
     """
 
     def __init__(
-            self,
-            save_folder: str,
-            save_interval: Union[str, int, Time],
-            huggingface_folder_name: str = 'ba{batch}',
-            precision: str = 'float32',
-            overwrite: bool = True,
-            mlflow_registered_model_name: Optional[str] = None,
-            mlflow_logging_config: Optional[dict] = None,
-            flatten_imports: Sequence[str] = ('llmfoundry',),
+        self,
+        save_folder: str,
+        save_interval: Union[str, int, Time],
+        huggingface_folder_name: str = 'ba{batch}',
+        precision: str = 'float32',
+        overwrite: bool = True,
+        mlflow_registered_model_name: Optional[str] = None,
+        mlflow_logging_config: Optional[dict] = None,
+        flatten_imports: Sequence[str] = ('llmfoundry',),
     ):
         _, _, self.save_dir_format_str = parse_uri(save_folder)
         self.overwrite = overwrite
         self.precision = precision
         self.dtype = {
             'float32': torch.float32,
             'float16': torch.float16,
@@ -124,104 +171,171 @@
         self.flatten_imports = flatten_imports
 
         # mlflow config setup
         self.mlflow_registered_model_name = mlflow_registered_model_name
         if mlflow_logging_config is None:
             mlflow_logging_config = {}
         if self.mlflow_registered_model_name is not None:
-            import numpy as np
-
             # Both the metadata and the task are needed in order for mlflow
             # and databricks optimized model serving to work
             passed_metadata = mlflow_logging_config.get('metadata', {})
             mlflow_logging_config['metadata'] = passed_metadata
             mlflow_logging_config.setdefault('task', 'llm/v1/completions')
 
             default_input_example = {
-                'prompt': np.array(['What is Machine Learning?'])
+                'prompt': np.array(['What is Machine Learning?']),
             }
-            is_chat = mlflow_logging_config['task'].endswith(
-                'chat') or mlflow_logging_config['metadata'].get(
-                    'task', '').endswith('chat')
+            is_chat = mlflow_logging_config['task'].endswith('chat') or (
+                mlflow_logging_config['metadata'] is not None and
+                mlflow_logging_config['metadata'].get('task',
+                                                      '').endswith('chat')
+            )
             if is_chat:
                 default_input_example = {
-                    'messages':
-                        np.array([{
-                            'role': 'user',
-                            'content': 'What is Machine Learning?'
-                        }])
+                    'messages': [{
+                        'role': 'user',
+                        'content': 'What is Machine Learning?',
+                    }],
                 }
-                mlflow_logging_config.setdefault('example_no_conversion', True)
-            mlflow_logging_config.setdefault('input_example',
-                                             default_input_example)
+            mlflow_logging_config.setdefault(
+                'input_example',
+                default_input_example,
+            )
 
         self.mlflow_logging_config = mlflow_logging_config
 
         self.huggingface_folder_name_fstr = os.path.join(
-            'huggingface', huggingface_folder_name)
-
-        self.save_interval: Time = Time.from_input(save_interval,
-                                                   TimeUnit.EPOCH)
+            'huggingface',
+            huggingface_folder_name,
+        )
+
+        self.save_interval: Time = Time.from_input(
+            save_interval,
+            TimeUnit.EPOCH,
+        )
         self.check_interval = create_interval_scheduler(
-            self.save_interval, include_end_of_training=True)
+            self.save_interval,
+            include_end_of_training=True,
+        )
         self.remote_ud = maybe_create_remote_uploader_downloader_from_uri(
-            save_folder, loggers=[])
+            save_folder,
+            loggers=[],
+        )
         if self.remote_ud is not None:
             self.remote_ud._num_concurrent_uploads = 4
 
         self.last_checkpoint_batch: Optional[Time] = None
         self.mlflow_loggers = []
 
+        self.child_processes: List[SpawnProcess] = []
+        # Temporary save directory used by child_processes.
+        self.temp_save_dir = None
+
     def run_event(self, event: Event, state: State, logger: Logger) -> None:
         # The interval scheduler handles only returning True for the appropriate events
         if state.get_elapsed_duration() is not None and self.check_interval(
-                state,
-                event) and self.last_checkpoint_batch != state.timestamp.batch:
+            state,
+            event,
+        ) and self.last_checkpoint_batch != state.timestamp.batch:
             self._save_checkpoint(state, logger)
         elif event == Event.INIT:
             if not isinstance(state.model, HuggingFaceModel):
                 raise ValueError(
                     f'`HuggingFaceCheckpointer` is only compatible with `HuggingFaceModel`s. '
-                    + f'Got {type(state.model)} instead.')
+                    + f'Got {type(state.model)} instead.',
+                )
             if self.remote_ud is not None:
                 self.remote_ud.init(state, logger)
                 state.callbacks.append(self.remote_ud)
 
             if self.mlflow_registered_model_name is not None:
                 self.mlflow_loggers = [
                     logger_destination
                     for logger_destination in logger.destinations
                     if isinstance(logger_destination, MLFlowLogger)
                 ]
                 if len(self.mlflow_loggers) == 0:
                     raise ValueError(
                         f'`mlflow_registered_model_name` was set, but no `MLFlowLogger` was found in the `logger.destinations` list. '
                         +
-                        'Please add an `MLFlowLogger` or set `mlflow_registered_model_name` to `None`.'
+                        'Please add an `MLFlowLogger` or set `mlflow_registered_model_name` to `None`.',
                     )
 
                 import mlflow
                 mlflow.environment_variables.MLFLOW_HUGGINGFACE_MODEL_MAX_SHARD_SIZE.set(
-                    '5GB')
+                    '1GB',
+                )
+        elif event == Event.FIT_END:
+            # Wait for all child processes spawned by the callback to finish.
+            timeout = 3600
+            wait_start = time.time()
+            while not self._all_child_processes_done():
+                wait_time = time.time() - wait_start
+                if wait_time > timeout:
+                    raise TimeoutError(
+                        f'Waited {wait_time} seconds for child processes to complete. Exceeded timeout of {timeout} seconds.',
+                    )
+                time.sleep(2)
+
+            # Clean up temporary save directory; all processes are done with it.
+            if self.temp_save_dir is not None:
+                shutil.rmtree(self.temp_save_dir)
 
     def _is_last_batch(self, state: State):
         elapsed_duration = state.get_elapsed_duration()
         if elapsed_duration is not None and elapsed_duration >= 1.0:
             return True
 
         assert state.max_duration is not None  # for pyright
+
+        epoch_complete = state.dataloader_len == state.timestamp.batch_in_epoch
+        second_to_last_epoch = state.max_duration.unit == TimeUnit.EPOCH and (
+            state.timestamp.epoch == state.max_duration.value - 1
+        )
+        # If the save interval is specified as exactly the same number of batches as the total duration,
+        # but the max duration is specified in epochs, we need a special case to identify we are on the last batch
+        # and should write the mlflow checkpoint. This should occur on the last batch of the final epoch.
+        if self.save_interval.unit == TimeUnit.BATCH and second_to_last_epoch and epoch_complete:
+            return True
+
         # If the save interval is specified as 1dur, and the max duration is in epoch units
         # we need a special case to identify we are on the last batch and should write the mlflow checkpoint
         if self.save_interval.unit == TimeUnit.DURATION and self.save_interval.value == 1 and state.max_duration.unit == TimeUnit.EPOCH:
             assert state.dataloader_len is not None  # for pyright
             return int(state.timestamp.batch) % math.ceil(
-                state.max_duration.value * state.dataloader_len) == 0
+                state.max_duration.value * state.dataloader_len,
+            ) == 0
 
         return False
 
+    def _all_child_processes_done(self) -> bool:
+        not_done = any(process.is_alive() for process in self.child_processes)
+        x = torch.tensor(1 if not_done else 0).to(device='cuda')
+        dist.all_reduce(x, reduce_operation='MAX')
+        return x.item() == 0
+
+    def transform_model_and_tokenizer(
+        self,
+        model: PreTrainedModel,
+        tokenizer: PreTrainedTokenizerBase,
+    ) -> Tuple[PreTrainedModel, PreTrainedTokenizerBase]:
+        """Transform the model and tokenizer before saving.
+
+        This allows a subclass to modify the model and tokenizer before saving. The base class implementation will
+        make no modifications.
+
+        Args:
+            model (PreTrainedModel): The model to be transformed.
+            tokenizer (PreTrainedTokenizerBase): The tokenizer to be transformed.
+
+        Returns:
+            Tuple[PreTrainedModel, PreTrainedTokenizerBase]: The transformed model and tokenizer.
+        """
+        return model, tokenizer
+
     def _save_checkpoint(self, state: State, logger: Logger):
         del logger  # unused
 
         self.last_checkpoint_batch = state.timestamp.batch
 
         log.info('Saving HuggingFace formatted checkpoint')
 
@@ -229,164 +343,252 @@
         CONFIG_MAPPING._extra_content['mpt'] = MPTConfig
         MPTConfig.register_for_auto_class()
         MPTForCausalLM.register_for_auto_class('AutoModelForCausalLM')
 
         save_dir = format_name_with_dist_and_time(
             str(
                 Path(self.save_dir_format_str) /
-                self.huggingface_folder_name_fstr), state.run_name,
-            state.timestamp)
-        dir_context_mgr = tempfile.TemporaryDirectory(
-        ) if self.remote_ud is not None else contextlib.nullcontext(
-            enter_result=save_dir)
-
-        with dir_context_mgr as temp_save_dir:
-            assert isinstance(temp_save_dir,
-                              str)  # pyright doesn't know about enter_result
-
-            log.debug('Gathering state dict')
-            from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
-
-            if state.is_model_ddp:
-                composer_model = state.model.module
-                original_model: PreTrainedModel = state.model.module.model
-                state_dict_model = state.model.module.model
-                original_tokenizer = state.model.module.tokenizer
-            elif isinstance(state.model.model, FSDP):
-                composer_model = state.model
-                original_model: PreTrainedModel = state.model.model.module
-                state_dict_model = state.model.model
-                original_tokenizer = state.model.tokenizer
-            else:
-                composer_model = state.model
-                original_model: PreTrainedModel = state.model.model
-                state_dict_model = state.model.model
-                original_tokenizer = state.model.tokenizer
+                self.huggingface_folder_name_fstr,
+            ),
+            state.run_name,
+            state.timestamp,
+        )
+
+        # Use a temporary directory if save_dir is remote.
+        use_temp_dir = self.remote_ud is not None
+        temp_save_dir = tempfile.mkdtemp() if use_temp_dir else save_dir
+
+        log.debug('Gathering state dict')
+        from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
+
+        if state.is_model_ddp:
+            composer_model = state.model.module
+            original_model: PreTrainedModel = state.model.module.model
+            state_dict_model = state.model.module.model
+            original_tokenizer = state.model.module.tokenizer
+        elif isinstance(state.model.model, FSDP):
+            composer_model = state.model
+            original_model: PreTrainedModel = state.model.model.module
+            state_dict_model = state.model.model
+            original_tokenizer = state.model.tokenizer
+        else:
+            composer_model = state.model
+            original_model: PreTrainedModel = state.model.model
+            state_dict_model = state.model.model
+            original_tokenizer = state.model.tokenizer
+
+        if version.parse(torch.__version__) > version.parse('2.2.9'):
+            from torch.distributed._tensor import DTensor
+            from torch.distributed.checkpoint.state_dict import (
+                StateDictOptions,
+                get_model_state_dict,
+            )
+            cpu_offload = True
 
-            state_dict_context = fsdp_state_dict_type_context(
-                original_model, state_dict_type='full') if (
-                    (not state.is_model_ddp) and isinstance(
-                        state_dict_model, FSDP)) else contextlib.nullcontext()
+            # Add a dtensor->cpu tensor hook to avoid CUDA OOM
+            def dtensor_to_tensor_hook(
+                module: nn.Module,
+                state_dict: Dict[str, Any],
+                prefix: str,
+                *args: Any,
+            ) -> Dict[str, Any]:
+                dtensor_fqns = []
+                for fqn in state_dict.keys():
+                    tensor = state_dict[fqn]
+                    if isinstance(tensor, DTensor):
+                        dtensor_fqns.append(fqn)
+                        tensor = tensor.full_tensor()  # type: ignore
+                        if dist.get_global_rank() == 0:
+                            if cpu_offload:
+                                tensor = tensor.cpu()
+                            state_dict[fqn] = tensor
+                if dist.get_global_rank() != 0:
+                    for fqn in dtensor_fqns:
+                        del state_dict[fqn]
+                return state_dict
+
+            hooks = []
+            for _, module in state_dict_model.named_modules():
+                if isinstance(module, FSDP):
+                    hooks.append(
+                        module.
+                        _register_state_dict_hook(dtensor_to_tensor_hook),
+                    )
 
+            state_dict = get_model_state_dict(
+                state_dict_model,
+                options=StateDictOptions(
+                    full_state_dict=True,
+                    cpu_offload=cpu_offload,
+                ),
+            )
+            for hook in hooks:
+                hook.remove()
+        else:
+            state_dict_context = fsdp_state_dict_type_context(
+                original_model,
+                state_dict_type='full',
+            ) if ((not state.is_model_ddp) and
+                  isinstance(state_dict_model,
+                             FSDP)) else contextlib.nullcontext()
             with state_dict_context:
                 state_dict = state_dict_model.state_dict()
 
-                # convert the state dict to the requested precision
-                for k, v in state_dict.items():
-                    if isinstance(v, torch.Tensor):
-                        state_dict[k] = v.to(dtype=self.dtype)
-
-            if dist.get_global_rank() == 0:
-                log.debug('Saving Hugging Face checkpoint in global rank 0')
-
-                copied_config = copy.deepcopy(original_model.config)
-                if copied_config.model_type == 'mpt':
-                    copied_config.attn_config['attn_impl'] = 'torch'
-                    copied_config.init_device = 'cpu'
-
-                log.debug(f'Creating new model instance')
-
-                if composer_model.using_peft:
-                    # We don't use meta here because the state dict does not contain the full
-                    # model, only the adapter weights.
-                    active_adapter = original_model.active_adapter
-                    base_model = original_model.get_base_model()
-                    new_base_model_instance = type(base_model)(copied_config)
-
-                    new_model_instance = type(original_model)(
-                        new_base_model_instance,
-                        original_model.peft_config[active_adapter])
-                    new_model_instance.to(dtype=self.dtype)
-                else:
-                    # First create the model instance on meta device to avoid the
-                    # initialization cost.
-                    with init_empty_weights():
-                        new_model_instance = type(original_model)(copied_config)
-
-                # Then load the state dict in with "assign" so that the state dict
-                # is loaded properly even though the model is initially on meta device.
-                new_model_instance.load_state_dict(state_dict, assign=True)
-                del state_dict
+        # Convert the state dict to the requested precis
+        for k, v in state_dict.items():
+            if isinstance(v, torch.Tensor):
+                state_dict[k] = v.to(dtype=self.dtype)
+
+        new_model_instance = None  # Need this for pyright because variable could be unbound
+
+        if dist.get_global_rank() == 0:
+            log.debug('Saving Hugging Face checkpoint in global rank 0')
+
+            # Edit HF config before building 2nd model copy
+            copied_config = copy.deepcopy(original_model.config)
+            if copied_config.model_type == 'mpt':
+                copied_config.attn_config['attn_impl'] = 'torch'
+                copied_config.init_device = 'cpu'
+                if 'moe_world_size' in getattr(copied_config, 'ffn_config', {}):
+                    copied_config.ffn_config['moe_world_size'] = 1
+
+            log.debug(f'Creating new model instance')
+
+            if composer_model.using_peft:
+                # We don't use meta here because the state dict does not contain the full
+                # model, only the adapter weights.
+                active_adapter = original_model.active_adapter
+                base_model = original_model.get_base_model()
+                new_base_model_instance = type(base_model)(copied_config)
+
+                new_model_instance = type(original_model)(
+                    new_base_model_instance,
+                    original_model.peft_config[active_adapter],
+                )
+                new_model_instance.to(dtype=self.dtype)
+            else:
+                # First create the model instance on meta device to avoid the
+                # initialization cost.
+                with init_empty_weights():
+                    new_model_instance = type(original_model)(copied_config)
+                    new_model_instance.generation_config.update(
+                        **original_model.generation_config.to_dict(),
+                    )
+
+            # Then load the state dict in with "assign" so that the state dict
+            # is loaded properly even though the model is initially on meta device.
+            new_model_instance.load_state_dict(state_dict, assign=True)
+            del state_dict
+
+            # Transform the model and tokenizer before saving
+            new_model_instance, original_tokenizer = self.transform_model_and_tokenizer(
+                new_model_instance,
+                original_tokenizer,
+            )
+
+            log.debug('Saving Hugging Face checkpoint to disk')
+            new_model_instance.save_pretrained(temp_save_dir)
+            if original_tokenizer is not None:
+                assert isinstance(original_tokenizer, PreTrainedTokenizerBase)
+                original_tokenizer.save_pretrained(temp_save_dir)
+
+            # Only need to edit files for MPT because it has custom code
+            if original_model.config.model_type == 'mpt':
+                log.debug('Editing MPT files for HuggingFace compatibility')
+                edit_files_for_hf_compatibility(
+                    temp_save_dir,
+                    self.flatten_imports,
+                )
+
+            if self.remote_ud is not None:
+                for filename in os.listdir(temp_save_dir):
+                    remote_file_name = os.path.join(save_dir, filename)
+                    remote_file_uri = self.remote_ud.remote_backend.get_uri(
+                        remote_file_name,
+                    )
+                    log.info(
+                        f'Uploading HuggingFace formatted checkpoint to {remote_file_uri}',
+                    )
+                    self.remote_ud.upload_file(
+                        state=state,
+                        remote_file_name=remote_file_name,
+                        file_path=Path(os.path.join(temp_save_dir, filename)),
+                        overwrite=self.overwrite,
+                    )
+
+        dist.barrier()
 
-                log.debug('Saving Hugging Face checkpoint to disk')
-                new_model_instance.save_pretrained(temp_save_dir)
+        if dist.get_global_rank() == 0:
+            if self.mlflow_registered_model_name and self._is_last_batch(state):
+                components = {'model': new_model_instance}
                 if original_tokenizer is not None:
-                    assert isinstance(original_tokenizer,
-                                      PreTrainedTokenizerBase)
-                    original_tokenizer.save_pretrained(temp_save_dir)
-
-                # Only need to edit files for MPT because it has custom code
-                if original_model.config.model_type == 'mpt':
-                    log.debug('Editing MPT files for HuggingFace compatibility')
-                    edit_files_for_hf_compatibility(
-                        temp_save_dir,
-                        self.flatten_imports,
-                    )
-
-                if self.remote_ud is not None:
-                    for filename in os.listdir(temp_save_dir):
-                        remote_file_name = os.path.join(save_dir, filename)
-                        remote_file_uri = self.remote_ud.remote_backend.get_uri(
-                            remote_file_name)
-                        log.info(
-                            f'Uploading HuggingFace formatted checkpoint to {remote_file_uri}'
-                        )
-                        self.remote_ud.upload_file(
-                            state=state,
-                            remote_file_name=remote_file_name,
-                            file_path=Path(os.path.join(temp_save_dir,
-                                                        filename)),
-                            overwrite=self.overwrite,
-                        )
+                    components['tokenizer'] = original_tokenizer
 
-                if self.mlflow_registered_model_name and self._is_last_batch(
-                        state):
-                    components = {'model': new_model_instance}
-                    if original_tokenizer is not None:
-                        components['tokenizer'] = original_tokenizer
-
-                    log.debug('Logging Hugging Face model to MLFlow')
-                    for i, mlflow_logger in enumerate(self.mlflow_loggers):
-                        log.debug(
-                            f'Registering model to UC at {mlflow_logger.model_registry_prefix}.{self.mlflow_registered_model_name}'
-                        )
-                        local_save_path = str(
-                            Path(temp_save_dir) / f'mlflow_save_{i}')
+                log.debug('Logging Hugging Face model to MLFlow')
+                for i, mlflow_logger in enumerate(self.mlflow_loggers):
+                    log.debug(
+                        f'Registering model to UC at {mlflow_logger.model_registry_prefix}.{self.mlflow_registered_model_name}',
+                    )
+                    local_save_path = str(
+                        Path(temp_save_dir) / f'mlflow_save_{i}',
+                    )
 
-                        # TODO: Remove after mlflow fixes the bug that makes this necessary
-                        import mlflow
-                        mlflow.store._unity_catalog.registry.rest_store.get_feature_dependencies = lambda *args, **kwargs: ''
-                        model_saving_kwargs: Dict[str, Any] = {
-                            'path': local_save_path
-                        }
-                        if composer_model.using_peft:
-                            model_saving_kwargs['flavor'] = 'peft'
-                            model_saving_kwargs[
-                                'save_pretrained_dir'] = temp_save_dir
-                            model_saving_kwargs[
-                                'metadata'] = self.mlflow_logging_config[
-                                    'metadata']
-                        else:
-                            model_saving_kwargs['flavor'] = 'transformers'
-                            model_saving_kwargs[
-                                'transformers_model'] = components
-                            model_saving_kwargs.update(
-                                self.mlflow_logging_config)
-
-                        mlflow_logger.save_model(**model_saving_kwargs)
-
-                        # Upload the license file generated by mlflow during the model saving.
-                        license_filename = _maybe_get_license_filename(
-                            local_save_path,
-                            self.mlflow_logging_config['metadata'].get(
-                                'pretrained_model_name', None))
-                        if license_filename is not None:
-                            mlflow_logger._mlflow_client.log_artifact(
-                                mlflow_logger._run_id,
-                                os.path.join(local_save_path, license_filename),
-                            )
-
-                        mlflow_logger.register_model_with_run_id(
-                            model_uri=local_save_path,
-                            name=self.mlflow_registered_model_name,
-                            await_creation_for=3600,
+                    # TODO: Remove after mlflow fixes the bug that makes this necessary
+                    import mlflow
+                    mlflow.store._unity_catalog.registry.rest_store.get_feature_dependencies = lambda *args, **kwargs: ''
+                    model_saving_kwargs: Dict[str, Any] = {
+                        'path': local_save_path,
+                    }
+                    if composer_model.using_peft:
+                        model_saving_kwargs['flavor'] = 'peft'
+                        model_saving_kwargs['save_pretrained_dir'
+                                           ] = temp_save_dir
+                        model_saving_kwargs[
+                            'metadata'] = self.mlflow_logging_config['metadata']
+                    else:
+                        model_saving_kwargs['flavor'] = 'transformers'
+                        model_saving_kwargs['transformers_model'] = components
+                        model_saving_kwargs.update(self.mlflow_logging_config)
+
+                    mlflow_logger.save_model(**model_saving_kwargs)
+
+                    # Upload the license file generated by mlflow during the model saving.
+                    license_filename = _maybe_get_license_filename(
+                        local_save_path,
+                        self.mlflow_logging_config['metadata'].get(
+                            'pretrained_model_name',
+                            None,
+                        ),
+                    )
+                    if license_filename is not None:
+                        mlflow_logger._mlflow_client.log_artifact(
+                            mlflow_logger._run_id,
+                            os.path.join(local_save_path, license_filename),
                         )
+
+                    # Spawn a new process to register the model.
+                    process = SpawnProcess(
+                        target=_register_model_with_run_id_multiprocess,
+                        kwargs={
+                            'mlflow_logger':
+                                mlflow_logger,
+                            'composer_logging_level':
+                                logging.getLogger('composer').level,
+                            'model_uri':
+                                local_save_path,
+                            'name':
+                                self.mlflow_registered_model_name,
+                            'await_creation_for':
+                                3600,
+                        },
+                    )
+                    process.start()
+                    self.child_processes.append(process)
+
+                    # Save the temporary directory to be cleaned up later.
+                    if use_temp_dir:
+                        self.temp_save_dir = temp_save_dir
+            else:
+                # Clean up the temporary directory if we don't need to register to mlflow.
+                if use_temp_dir:
+                    shutil.rmtree(temp_save_dir)
+        dist.barrier()
```

### Comparing `llm-foundry-0.7.0/llmfoundry/callbacks/monolithic_ckpt_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/monolithic_ckpt_callback.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,49 +4,61 @@
 import contextlib
 import os
 import tempfile
 from pathlib import Path
 
 import torch
 from composer.core import Callback, State
-from composer.core.state import (fsdp_get_optim_state_dict,
-                                 fsdp_state_dict_type_context)
+from composer.core.state import (
+    fsdp_get_optim_state_dict,
+    fsdp_state_dict_type_context,
+)
 from composer.loggers import Logger
 from composer.loggers.remote_uploader_downloader import RemoteUploaderDownloader
-from composer.utils import (dist, format_name_with_dist_and_time, parse_uri,
-                            reproducibility)
+from composer.utils import (
+    dist,
+    format_name_with_dist_and_time,
+    parse_uri,
+    reproducibility,
+)
+
+__all__ = ['MonolithicCheckpointSaver']
 
 
 class MonolithicCheckpointSaver(Callback):
     """Save a monolithic checkpoint every N batches.
 
     Args:
         save_folder (str): Folder to save checkpoints to (can be a URI)
         batch_interval (int): Number of batches between checkpoints.
         filename (str): Filename to save checkpoints to.
         overwrite (bool): Whether to overwrite previous checkpoints.
         keep_optimizers (bool): Whether to save the optimizer state in the monolithic checkpoint.
     """
 
-    def __init__(self,
-                 save_folder: str,
-                 batch_interval: int,
-                 filename: str = 'ep{epoch}-ba{batch}.pt',
-                 overwrite: bool = False,
-                 keep_optimizers: bool = False):
+    def __init__(
+        self,
+        save_folder: str,
+        batch_interval: int,
+        filename: str = 'ep{epoch}-ba{batch}.pt',
+        overwrite: bool = False,
+        keep_optimizers: bool = False,
+    ):
         self.backend, self.bucket_name, self.save_dir_format_str = parse_uri(
-            save_folder)
+            save_folder,
+        )
         self.filename_format_str = filename
         self.batch_interval = batch_interval
         self.upload_to_object_store = (self.backend != '')
         self.overwrite = overwrite
         self.keep_optimizers = keep_optimizers
         if self.upload_to_object_store:
             self.remote_ud = RemoteUploaderDownloader(
-                bucket_uri=f'{self.backend}://{self.bucket_name}')
+                bucket_uri=f'{self.backend}://{self.bucket_name}',
+            )
         else:
             self.remote_ud = None
 
     def init(self, state: State, logger: Logger) -> None:
         if self.upload_to_object_store and self.remote_ud is not None:
             self.remote_ud.init(state, logger)
             # updated_logger_destinations = [*logger.destinations, new_remote_ud]
@@ -60,56 +72,67 @@
     def fit_end(self, state: State, logger: Logger) -> None:
         if state.timestamp.batch.value % self.batch_interval != 0:
             self._save_checkpoint(state, logger)
 
     def _save_checkpoint(self, state: State, logger: Logger) -> None:
         del logger  # unused
 
-        filename = format_name_with_dist_and_time(self.filename_format_str,
-                                                  state.run_name,
-                                                  state.timestamp)
-        save_dir = format_name_with_dist_and_time(self.save_dir_format_str,
-                                                  state.run_name,
-                                                  state.timestamp)
+        filename = format_name_with_dist_and_time(
+            self.filename_format_str,
+            state.run_name,
+            state.timestamp,
+        )
+        save_dir = format_name_with_dist_and_time(
+            self.save_dir_format_str,
+            state.run_name,
+            state.timestamp,
+        )
         dir_context_mgr = tempfile.TemporaryDirectory(
         ) if self.upload_to_object_store else contextlib.nullcontext(
-            enter_result=save_dir)
+            enter_result=save_dir,
+        )
         with dir_context_mgr as temp_save_dir:
             # pyright doesn't know about enter_result
             assert isinstance(temp_save_dir, str)
 
             save_path = str(Path(temp_save_dir) / Path(filename))
             dirname = os.path.dirname(save_path)
             if dirname:
                 os.makedirs(dirname, exist_ok=True)
             state_dict = {
                 'state': state.state_dict(),
-                'rng': reproducibility.get_rng_state()
+                'rng': reproducibility.get_rng_state(),
             }
             # Remove sharded model and optimizer state dicts
             state_dict['state'].pop('optimizers')
             state_dict['state'].pop('model')
 
             # Add in unsharded model params.
-            with fsdp_state_dict_type_context(state.model,
-                                              state_dict_type='full'):
+            with fsdp_state_dict_type_context(
+                state.model,
+                state_dict_type='full',
+            ):
                 state_dict['state']['model'] = state.model.state_dict()
 
             # Add in unsharded optimizer state dict.
             if self.keep_optimizers:
                 optimizer = state.optimizers[0]
                 state_dict['state']['optimizers'] = {
                     type(optimizer).__qualname__:
-                        fsdp_get_optim_state_dict(state.model,
-                                                  optimizer,
-                                                  state_dict_type='full')
+                        fsdp_get_optim_state_dict(
+                            state.model,
+                            optimizer,
+                            state_dict_type='full',
+                        ),
                 }
             if dist.get_global_rank() == 0:
                 torch.save(state_dict, save_path)
 
             if self.upload_to_object_store and self.remote_ud is not None and dist.get_global_rank(
             ) == 0:
                 remote_file_name = str(Path(save_dir) / Path(filename))
-                self.remote_ud.upload_file(state=state,
-                                           remote_file_name=remote_file_name,
-                                           file_path=Path(save_path),
-                                           overwrite=self.overwrite)
+                self.remote_ud.upload_file(
+                    state=state,
+                    remote_file_name=remote_file_name,
+                    file_path=Path(save_path),
+                    overwrite=self.overwrite,
+                )
```

### Comparing `llm-foundry-0.7.0/llmfoundry/callbacks/resumption_callbacks.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/resumption_callbacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 
 import logging
 from typing import List
 
 from composer.core import Callback, State
 from composer.loggers import Logger
 
+from llmfoundry.utils.warnings import experimental_class
+
 __all__ = [
     'GlobalLRScaling',
     'LayerFreezing',
 ]
 
 log = logging.getLogger(__name__)
 
 
+@experimental_class('GlobalLRScaling')
 class GlobalLRScaling(Callback):
     """GlobalLRScaling.
 
     This callback can be applied upon resuming a model checkpoint. Upon
     fit_start it will multiply the base LR by `lr_scale` and set the WD to be.
 
     `wd_pct` * `lr`.
@@ -40,22 +43,24 @@
         for optimizer in state.optimizers:
             for group in optimizer.param_groups:
                 group['lr'] *= self.lr_scale
                 group['weight_decay'] = group['lr'] * self.wd_pct
                 if 'initial_lr' in group:
                     group['initial_lr'] *= self.lr_scale
                 log.info(
-                    f"Set LR and WD to {group['lr']}, {group['weight_decay']}")
+                    f"Set LR and WD to {group['lr']}, {group['weight_decay']}",
+                )
 
         for scheduler in state.schedulers:
             scheduler.base_lrs = [
                 self.lr_scale * lr for lr in scheduler.base_lrs
             ]
 
 
+@experimental_class('LayerFreezing')
 class LayerFreezing(Callback):
     """LayerFreezing.
 
     This callback can be applied upon resuming a model checkpoint. Upon
     fit_start it freeze the layers specified in `layer_names`. If using
     activation checkpointing, please set the
     `activation_checkpointing_reentrant` flag in `fsdp_config` to false.
@@ -66,24 +71,25 @@
 
     def __init__(self, layer_names: List[str]):
         self.layer_names = set(layer_names)
 
     def fit_start(self, state: State, logger: Logger) -> None:
         del logger  # unused
 
-        model_layers = set(name for name, _ in state.model.named_parameters())
+        model_layers = {name for name, _ in state.model.named_parameters()}
         for layer in self.layer_names:
             if layer not in model_layers:
                 raise Exception(
-                    f'Attempted to freeze layer not found in model: {layer}\nAvailable layers: {model_layers}'
+                    f'Attempted to freeze layer not found in model: {layer}\nAvailable layers: {model_layers}',
                 )
 
         successful_freeze = False
         for name, p in state.model.named_parameters():
             if p.requires_grad and name in self.layer_names:
                 p.requires_grad = False
                 log.debug(f'Froze layer: {name}\nParam: {p}')
                 successful_freeze = True
 
         if not successful_freeze:
             raise Exception(
-                f"Tried to run LayerFreezing but didn't freeze any layers")
+                f"Tried to run LayerFreezing but didn't freeze any layers",
+            )
```

### Comparing `llm-foundry-0.7.0/llmfoundry/callbacks/scheduled_gc_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/scheduled_gc_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import gc
 from typing import Optional
 
 import torch
 from composer.core import Callback, State
 from composer.loggers import Logger
 
+__all__ = ['ScheduledGarbageCollector']
+
 
 def gc_cuda():
     """Garbage collect Torch (CUDA) memory."""
     gc.collect()
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
```

### Comparing `llm-foundry-0.7.0/llmfoundry/cli/registry_cli.py` & `llm-foundry-0.9.0.dev0/llmfoundry/cli/registry_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     registry_attrs = [getattr(registry, name) for name in registry_attr_names]
     available_registries = [
         r for r in registry_attrs if isinstance(r, TypedRegistry)
     ]
 
     if group is not None and group not in registry_attr_names:
         console.print(
-            f'Group {group} not found in registry. Run `llmfoundry registry get` to see available groups.'
+            f'Group {group} not found in registry. Run `llmfoundry registry get` to see available groups.',
         )
         return []
 
     if group is not None:
         available_registries = [getattr(registry, group)]
 
     return available_registries
@@ -40,16 +40,19 @@
     Args:
         group (Optional[str], optional): The group to get. If not provided, all groups will be shown. Defaults to None.
     """
     available_registries = _get_registries(group)
 
     table = Table('Registry', 'Description', 'Options', show_lines=True)
     for r in available_registries:
-        table.add_row('.'.join(r.namespace), r.description,
-                      ', '.join(r.get_all()))
+        table.add_row(
+            '.'.join(r.namespace),
+            r.description,
+            ', '.join(r.get_all()),
+        )
 
     console.print(table)
 
 
 @app.command()
 def find(group: str, name: str):
     """Find a registry entry by name.
@@ -62,11 +65,15 @@
     if not available_registries:
         return
 
     r = available_registries[0]
     find_output = r.find(name)
 
     table = Table('Module', 'File', 'Line number', 'Docstring')
-    table.add_row(find_output['module'], find_output['file'],
-                  str(find_output['line_no']), find_output['docstring'])
+    table.add_row(
+        find_output['module'],
+        find_output['file'],
+        str(find_output['line_no']),
+        find_output['docstring'],
+    )
 
     console.print(table)
```

### Comparing `llm-foundry-0.7.0/llmfoundry/data/data.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,23 +7,30 @@
 from typing import Dict, Iterable, Union
 
 import datasets as hf_datasets
 import numpy as np
 from torch.utils.data import IterableDataset
 from transformers import PreTrainedTokenizerBase
 
+__all__ = [
+    'ConcatTokensDataset',
+    'NoConcatDataset',
+]
+
 
 class NoConcatDataset(IterableDataset):
     """An IterableDataset that returns text samples for MDSWriter.
 
     Returns dicts of {'text': bytes}
     """
 
-    def __init__(self, hf_dataset: Union[hf_datasets.IterableDataset,
-                                         hf_datasets.Dataset]):
+    def __init__(
+        self,
+        hf_dataset: Union[hf_datasets.IterableDataset, hf_datasets.Dataset],
+    ):
         self.hf_dataset = hf_dataset
 
     def __iter__(self) -> Iterable[Dict[str, bytes]]:
         for sample in self.hf_dataset:
             # convert to bytes to store in MDS binary format
             yield {'text': sample['text'].encode('utf-8')}
 
@@ -64,54 +71,64 @@
         self.tokenizer = tokenizer
         os.environ['TOKENIZERS_PARALLELISM'] = 'false'
         self.max_length = max_length
         self.bos_text = bos_text
         self.eos_text = eos_text
         self.should_wrap = not no_wrap
 
-        self.bos_tokens = self.tokenizer(self.bos_text,
-                                         truncation=False,
-                                         padding=False,
-                                         add_special_tokens=False)['input_ids']
+        self.bos_tokens = self.tokenizer(
+            self.bos_text,
+            truncation=False,
+            padding=False,
+            add_special_tokens=False,
+        )['input_ids']
         if len(self.bos_tokens) > 1:
             warnings.warn(
                 f'You specified --concat_tokens with --bos_text, but your BOS text is not tokenizing to one token\
-                , instead we got {self.bos_tokens}. Quit if this was in error.')
+                , instead we got {self.bos_tokens}. Quit if this was in error.',
+            )
 
-        self.eos_tokens = self.tokenizer(self.eos_text,
-                                         truncation=False,
-                                         padding=False,
-                                         add_special_tokens=False)['input_ids']
+        self.eos_tokens = self.tokenizer(
+            self.eos_text,
+            truncation=False,
+            padding=False,
+            add_special_tokens=False,
+        )['input_ids']
         if len(self.eos_tokens) > 1:
             warnings.warn(
                 f'You specified --concat_tokens with --eos_text, but your EOS text is not tokenizing to one token\
-                , instead we got {self.eos_tokens}. Quit if this was in error.')
+                , instead we got {self.eos_tokens}. Quit if this was in error.',
+            )
 
         eos_text_provided = self.eos_text != ''
         bos_text_provided = self.bos_text != ''
         test_text = self.tokenizer('')
-        if len(test_text['input_ids']) > 0 and (eos_text_provided or
-                                                bos_text_provided):
+        if len(
+            test_text['input_ids'],
+        ) > 0 and (eos_text_provided or bos_text_provided):
             message = 'both eos and bos' if eos_text_provided and bos_text_provided else (
-                'eos_text' if eos_text_provided else 'bos_text')
+                'eos_text' if eos_text_provided else 'bos_text'
+            )
             warnings.warn(
                 f'The provided tokenizer adds special tokens, but you also specified {message}. This may result '
                 +
-                'in duplicated special tokens. Please be sure this is what you intend.'
+                'in duplicated special tokens. Please be sure this is what you intend.',
             )
 
     def __iter__(self) -> Iterable[Dict[str, bytes]]:
 
         buffer = []
         for sample in self.hf_dataset:
-            encoded = self.tokenizer(sample['text'],
-                                     truncation=False,
-                                     padding=False)
+            encoded = self.tokenizer(
+                sample['text'],
+                truncation=False,
+                padding=False,
+            )
             iids = encoded['input_ids']
             buffer = buffer + self.bos_tokens + iids + self.eos_tokens
             while len(buffer) >= self.max_length:
                 concat_sample = buffer[:self.max_length]
                 buffer = buffer[self.max_length:] if self.should_wrap else []
                 yield {
                     # convert to bytes to store in MDS binary format
-                    'tokens': np.asarray(concat_sample).tobytes()
+                    'tokens': np.asarray(concat_sample).tobytes(),
                 }
```

### Comparing `llm-foundry-0.7.0/llmfoundry/data/dataloader.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/dataloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Dataloader builder utilities."""
 
+from typing import Union
+
 from composer import DataSpec
 from omegaconf import DictConfig
 from transformers import PreTrainedTokenizerBase
 
 from llmfoundry import registry
 from llmfoundry.utils.registry_utils import construct_from_registry
 
+__all__ = [
+    'build_dataloader',
+]
+
 
-def build_dataloader(cfg: DictConfig, tokenizer: PreTrainedTokenizerBase,
-                     device_batch_size: int) -> DataSpec:
+def build_dataloader(
+    cfg: DictConfig,
+    tokenizer: PreTrainedTokenizerBase,
+    device_batch_size: Union[int, float],
+) -> DataSpec:
     """Builds a dataloader from a config.
 
     Args:
         cfg (DictConfig): An omegaconf dictionary used to configure the loader.
         tokenizer (PreTrainedTokenizerBase): The tokenizer that the model will use.
         device_batch_size (int): The size of the batches (number of examples)
             that the dataloader will produce.
     """
     kwargs = {
         'cfg': cfg,
         'tokenizer': tokenizer,
-        'device_batch_size': device_batch_size
+        'device_batch_size': device_batch_size,
     }
 
     return construct_from_registry(
         name=cfg.name,
         registry=registry.dataloaders,
         partial_function=False,
         pre_validation_function=None,
```

### Comparing `llm-foundry-0.7.0/llmfoundry/data/finetuning/collator.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/collator.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,88 +6,103 @@
 from typing import Any, Dict, List, Optional, Union
 
 import torch
 from transformers import PreTrainedTokenizer, PreTrainedTokenizerFast
 
 log = logging.getLogger(__name__)
 
+__all__ = [
+    'Seq2SeqFinetuningCollator',
+]
+
 # HuggingFace hardcodes the ignore index to -100
 _HF_IGNORE_INDEX = -100
 
 TokenizedExample = Dict[str, List[Dict[str, List[int]]]]
 
 
 def ensure_list(x: Union[List, torch.Tensor]) -> List:
     if isinstance(x, torch.Tensor):
         x = list(x.flatten())
     assert isinstance(x, list)
     return x
 
 
-def validate_target_settings(target_prompts: str, target_responses: str,
-                             decoder_only_format: bool):
+def validate_target_settings(
+    target_prompts: str,
+    target_responses: str,
+    decoder_only_format: bool,
+):
     """Raises an error if target settings are invalid."""
-    if (not decoder_only_format) and (target_prompts != 'none' or
-                                      target_responses != 'last'):
+    if (not decoder_only_format
+       ) and (target_prompts != 'none' or target_responses != 'last'):
         raise ValueError(
-            f'When using encoder_decoder format, you must use target_prompts="none" and target_responses="last".'
+            f'When using encoder_decoder format, you must use target_prompts="none" and target_responses="last".',
         )
 
     if target_responses not in {'all', 'last'}:
         raise ValueError(
-            f'target_responses must be either "last" or "all" but {target_responses=}'
+            f'target_responses must be either "last" or "all" but {target_responses=}',
         )
 
     if target_prompts.startswith('length>='):
         cutoff = target_prompts[8:]
         if not cutoff.isdigit():
             raise ValueError(
                 f'target_prompts starts with "length>=" but the rest of the string is not digits ({target_prompts=}). ' +\
                 'To use this configuration option, set target_prompts "length>=XX" where "XX" is a positive integer indicating ' +\
-                'the length cutoff. Prompts of at least XX tokens in length will be treated as targets.'
+                'the length cutoff. Prompts of at least XX tokens in length will be treated as targets.',
             )
         cutoff = int(cutoff)
         if cutoff <= 0:
             raise ValueError(
-                f'You are trying to set the target_prompts length cutoff to a negative number {cutoff=}. This is not allowed.'
+                f'You are trying to set the target_prompts length cutoff to a negative number {cutoff=}. This is not allowed.',
             )
     elif target_prompts not in {'all', 'none'}:
         raise ValueError(
-            f'target_prompts must either be "all", "none" or "length>=XX" where "XX" is a positive integer, but {target_prompts=}'
+            f'target_prompts must either be "all", "none" or "length>=XX" where "XX" is a positive integer, but {target_prompts=}',
         )
 
 
 ###### Functions to implement target_prompts and target_responses choices #####
-def _sequence_to_labels_all(sequence: list[int],
-                            is_last_turn: bool,
-                            cutoff: Optional[int] = None) -> list[int]:
+def _sequence_to_labels_all(
+    sequence: list[int],
+    is_last_turn: bool,
+    cutoff: Optional[int] = None,
+) -> list[int]:
     del is_last_turn, cutoff  # unused
     return sequence
 
 
-def _sequence_to_labels_none(sequence: list[int],
-                             is_last_turn: bool,
-                             cutoff: Optional[int] = None) -> list[int]:
+def _sequence_to_labels_none(
+    sequence: list[int],
+    is_last_turn: bool,
+    cutoff: Optional[int] = None,
+) -> list[int]:
     del is_last_turn, cutoff  # unused
     return [_HF_IGNORE_INDEX] * len(sequence)
 
 
-def _sequence_to_labels_last(sequence: list[int],
-                             is_last_turn: bool,
-                             cutoff: Optional[int] = None) -> list[int]:
+def _sequence_to_labels_last(
+    sequence: list[int],
+    is_last_turn: bool,
+    cutoff: Optional[int] = None,
+) -> list[int]:
     del cutoff  # unused
     if is_last_turn:
         return sequence
     else:
         return [_HF_IGNORE_INDEX] * len(sequence)
 
 
-def _sequence_to_labels_cutoff(sequence: list[int],
-                               is_last_turn: bool,
-                               cutoff: Optional[int] = None) -> list[int]:
+def _sequence_to_labels_cutoff(
+    sequence: list[int],
+    is_last_turn: bool,
+    cutoff: Optional[int] = None,
+) -> list[int]:
     del is_last_turn  # unused
     if cutoff is None:
         raise ValueError('input ``cutoff`` must be provided')
     if len(sequence) >= cutoff:
         return sequence
     else:
         return [_HF_IGNORE_INDEX] * len(sequence)
@@ -98,26 +113,29 @@
     'none': _sequence_to_labels_none,
     'last': _sequence_to_labels_last,
     'length': _sequence_to_labels_cutoff,
 }
 
 
 def stitch_turns_decoder_only(
-        example_turns: list[dict[str, list[int]]],
-        target_prompts: str,
-        target_responses: str,
-        eos_token_id: Optional[int] = None,
-        validate: bool = False) -> tuple[list[int], list[int]]:
+    example_turns: list[dict[str, list[int]]],
+    target_prompts: str,
+    target_responses: str,
+    eos_token_id: Optional[int] = None,
+    validate: bool = False,
+) -> tuple[list[int], list[int]]:
     target_prompts = target_prompts.lower()
     target_responses = target_responses.lower()
 
     if validate:
-        validate_target_settings(target_prompts,
-                                 target_responses,
-                                 decoder_only_format=True)
+        validate_target_settings(
+            target_prompts,
+            target_responses,
+            decoder_only_format=True,
+        )
 
     if target_prompts.startswith('length'):
         prompt_cutoff = int(target_prompts.split('>=')[-1])
         prompt_to_target = _TARGET_POLICY_LOOKUP['length']
     else:
         prompt_cutoff = None
         prompt_to_target = _TARGET_POLICY_LOOKUP[target_prompts]
@@ -140,15 +158,15 @@
         input_ids += target
         # Extend the labels, with values depending on the loss-generating policies
         labels += prompt_to_target(context, is_last_turn, prompt_cutoff)
         labels += response_to_target(target, is_last_turn)
 
     if len(input_ids) != len(labels):
         raise ValueError(
-            f'input_ids and labels should be the same length, {len(input_ids)=}, {len(labels)=}'
+            f'input_ids and labels should be the same length, {len(input_ids)=}, {len(labels)=}',
         )
     return input_ids, labels
 
 
 def stitch_turns_encoder_decoder(
     example_turns: list[dict[str, list[int]]],
     eos_token_id: Optional[int] = None,
@@ -232,37 +250,40 @@
         illegal_keys = [
             'input_ids',
             'labels',
             'attention_mask',
             'decoder_input_ids',
             'decoder_attention_mask',
         ]
-        found_keys = []
-        for illegal_key in illegal_keys:
-            if illegal_key in self.batch_metadata:
-                found_keys.append(illegal_key)
+        found_keys = [
+            illegal_key for illegal_key in illegal_keys
+            if illegal_key in self.batch_metadata
+        ]
         if found_keys:
             raise ValueError(
                 f'The following keys are in batch_metadata but are not allowed: {", ".join(found_keys)}.\n' +\
                 f'You cannot use keys that are used directly by the models. The prohibited keys are:\n' +\
-                f'{", ".join(illegal_keys)}'
+                f'{", ".join(illegal_keys)}',
             )
 
         if (max_seq_len % 8) != 0:
             log.warning(
-                'For performance, a max_seq_len as a multiple of 8 is recommended.'
+                'For performance, a max_seq_len as a multiple of 8 is recommended.',
             )
 
         if self.tokenizer.pad_token_id is None:
             raise ValueError(
-                f'{self.__class__.__name__} requires that the tokenizer has the pad token set, but it is None'
+                f'{self.__class__.__name__} requires that the tokenizer has the pad token set, but it is None',
             )
 
-        validate_target_settings(self.target_prompts, self.target_responses,
-                                 self.decoder_only_format)
+        validate_target_settings(
+            self.target_prompts,
+            self.target_responses,
+            self.decoder_only_format,
+        )
         if self.target_prompts.startswith('length'):
             self.prompt_cutoff = int(self.target_prompts.split('>=')[-1])
             self.prompt_to_target = _TARGET_POLICY_LOOKUP['length']
         else:
             self.prompt_cutoff = None
             self.prompt_to_target = _TARGET_POLICY_LOOKUP[self.target_prompts]
         self.response_to_target = _TARGET_POLICY_LOOKUP[self.target_responses]
@@ -272,15 +293,15 @@
         self._warned_target = False
 
     def __call__(self,
                  examples: List[TokenizedExample]) -> Dict[str, torch.Tensor]:
         for check_key in ['input_ids', 'labels']:
             if check_key not in examples[0]['turns'][0]:
                 raise KeyError(
-                    f'Examples returned by dataset do not include required key: {check_key}'
+                    f'Examples returned by dataset do not include required key: {check_key}',
                 )
 
         if self.decoder_only_format:
             batch = self._process_and_batch_decoder_only(examples)
         else:
             batch = self._process_and_batch_encoder_decoder(examples)
 
@@ -290,15 +311,17 @@
             k: torch.tensor([v] * batch_size)
             for k, v in self.batch_metadata.items()
         })
 
         return batch
 
     def _process_and_batch_decoder_only(
-            self, examples: List[TokenizedExample]) -> Dict[str, torch.Tensor]:
+        self,
+        examples: List[TokenizedExample],
+    ) -> Dict[str, torch.Tensor]:
         # Steps explained in comments
         processed_examples = []
         for example in examples:
             input_ids, labels = stitch_turns_decoder_only(
                 example_turns=example['turns'],
                 target_prompts=self.target_prompts,
                 target_responses=self.target_responses,
@@ -315,22 +338,22 @@
                 if len([l for l in labels if l != _HF_IGNORE_INDEX]) == 0:
                     raise ValueError(
                         f'Truncating to max_seq_len={self.max_seq_len} has removed all loss-generating tokens. ' +\
                         f'Pre-truncation sequence length was {orig_size}. ' +\
                         'This sample should have been filtered out before reaching the collator. If using ' +\
                         'pre-tokenized streaming data, this may have resulted from using different ' +\
                         '``target_prompts``, ``target_responses``, or ``max_seq_len`` ' +\
-                        'settings when preparing the streaming dataset than what are currently being used.'
+                        'settings when preparing the streaming dataset than what are currently being used.',
                     )
 
                 # Still issue a warning when truncating
                 if not self._warned_truncated:
                     warnings.warn(
                         f'Truncating sequence of length={orig_size} to fit max_seq_len={self.max_seq_len}. ' +\
-                        f'If truncation is a problem, consider increasing max_seq_len.'
+                        f'If truncation is a problem, consider increasing max_seq_len.',
                     )
                     self._warned_truncated = True
 
             attention_mask = [1] * len(input_ids)
 
             # Annoyingly, we need to pad everything but input_ids
             # and attention_mask ourselves
@@ -377,15 +400,17 @@
                 batch[k] = v[:, -keep_tokens:].contiguous()
             else:
                 batch[k] = v[:, :keep_tokens].contiguous()
 
         return batch
 
     def _process_and_batch_encoder_decoder(
-            self, examples: List[TokenizedExample]) -> Dict[str, torch.Tensor]:
+        self,
+        examples: List[TokenizedExample],
+    ) -> Dict[str, torch.Tensor]:
         # The encoder-decoder case is has some gotchas.
         # Steps are explained in comments.
         processed_examples = []
         for example in examples:
             context, target = stitch_turns_encoder_decoder(
                 example_turns=example['turns'],
                 eos_token_id=self.tokenizer.eos_token_id,
@@ -431,22 +456,26 @@
             padding='max_length',
             max_length=self.max_seq_len,
             return_tensors='pt',
         )
         # We're still missing decoder_input_ids and decoder_attention_mask
         batch['decoder_input_ids'] = torch.cat([
             torch.full((len(processed_examples), 1),
-                       self.tokenizer.pad_token_id), batch['labels'][:, :-1]
+                       self.tokenizer.pad_token_id),
+            batch['labels'][:, :-1],
         ],
                                                dim=1)
         batch['decoder_input_ids'].masked_fill_(
             batch['decoder_input_ids'] == _HF_IGNORE_INDEX,
-            self.tokenizer.pad_token_id)
+            self.tokenizer.pad_token_id,
+        )
         batch['decoder_attention_mask'] = torch.not_equal(
-            batch['labels'], _HF_IGNORE_INDEX)
+            batch['labels'],
+            _HF_IGNORE_INDEX,
+        )
 
         # This logic prevents trimming on at least the first batch
         if not (self._allow_pad_trimming and self._seen_first_batch):
             self._seen_first_batch = True
             return batch
         self._seen_first_batch = True
```

### Comparing `llm-foundry-0.7.0/llmfoundry/data/finetuning/dataloader.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/dataloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,37 +7,51 @@
 import torch
 from composer.core.data_spec import DataSpec
 from composer.utils import dist, get_file, parse_uri
 from omegaconf import DictConfig
 from torch.utils.data import DataLoader
 from transformers import PreTrainedTokenizerBase
 
-from llmfoundry.data.finetuning.collator import (Seq2SeqFinetuningCollator,
-                                                 validate_target_settings)
-from llmfoundry.data.finetuning.tasks import (DOWNLOADED_FT_DATASETS_DIRPATH,
-                                              SUPPORTED_EXTENSIONS,
-                                              dataset_constructor)
+from llmfoundry import registry
+from llmfoundry.data.finetuning.collator import (
+    Seq2SeqFinetuningCollator,
+    validate_target_settings,
+)
+from llmfoundry.data.finetuning.tasks import (
+    DOWNLOADED_FT_DATASETS_DIRPATH,
+    SUPPORTED_EXTENSIONS,
+    dataset_constructor,
+)
 from llmfoundry.data.packing import BinPackCollator, auto_packing_ratio
-from llmfoundry.data.text_data import build_streams, get_tokens_per_batch_func
-from llmfoundry.utils.exceptions import (MissingHuggingFaceURLSplitError,
-                                         NotEnoughDatasetSamplesError)
+from llmfoundry.data.text_data import build_streams
+from llmfoundry.utils.exceptions import (
+    MissingHuggingFaceURLSplitError,
+    NotEnoughDatasetSamplesError,
+)
+from llmfoundry.utils.registry_utils import construct_from_registry
 
 log = logging.getLogger(__name__)
 
+__all__ = [
+    'build_finetuning_dataloader',
+]
+
 # HuggingFace hardcodes the ignore index to -100
 _HF_IGNORE_INDEX = -100
 
 # Default settings to use for target responses and target prompts
 _DEFAULT_TARGET_RESPONSES = 'last'
 _DEFAULT_TARGET_PROMPTS = 'none'
 
 
-def build_finetuning_dataloader(cfg: DictConfig,
-                                tokenizer: PreTrainedTokenizerBase,
-                                device_batch_size: int) -> DataSpec:
+def build_finetuning_dataloader(
+    cfg: DictConfig,
+    tokenizer: PreTrainedTokenizerBase,
+    device_batch_size: Union[int, float],
+) -> DataSpec:
     """Builds a finetuning dataloader for training or evaluating.
 
     The underlying dataset can be built through one of two code paths:
         1. As a HuggingFace dataset, via `datasets.load_dataset(...)`
         2. As a streaming dataset
     You will need to set slightly different dataset config fields depending
     on which you intend to use, as explained below.
@@ -116,15 +130,15 @@
                 using the streaming codepath.
             ---
             See :class:`DataLoader` for standard argument options to the pytorch
                 dataloader, such as `cfg.drop_last`, `cfg.num_workers`, etc.
         tokenizer (transformers.PreTrainedTokenizer): The tokenizer used to
             prepare the data from raw text. Any missing sentinel tokens will
             be added by the collator.
-        device_batch_size (int): The size of the batches (number of examples)
+        device_batch_size (int, float): The size of the batches (number of examples)
             that the dataloader will produce.
 
     Returns:
         A pytorch dataloader
 
     Note:
         You can run the script inside `scripts/misc/profile_packing.py` to quickly test the
@@ -133,21 +147,41 @@
     """
     _validate_config(cfg.dataset)
 
     # Use EOS as the pad token if none exists
     if tokenizer.pad_token is None:
         tokenizer.pad_token = tokenizer.eos_token
 
-    collate_fn, dataloader_batch_size = _build_collate_fn(
-        cfg, tokenizer, device_batch_size)
+    replication_factor, dataset_batch_size = construct_from_registry(
+        name='dataset_replication_validator',
+        registry=registry.dataset_replication_validators,
+        partial_function=False,
+        kwargs={
+            'cfg': cfg,
+            'tokenizer': tokenizer,
+            'device_batch_size': device_batch_size,
+        },
+    )
+
+    collate_fn, dataloader_batch_size = construct_from_registry(
+        name='finetuning_collator',
+        registry=registry.collators,
+        partial_function=False,
+        kwargs={
+            'cfg': cfg,
+            'tokenizer': tokenizer,
+            'dataset_batch_size': dataset_batch_size,
+        },
+    )
 
     dataset = None  # for pyright
     sampler = None
-    if cfg.dataset.get('remote') is not None or cfg.dataset.get(
-            'streams') is not None:
+    if cfg.dataset.get(
+        'remote',
+    ) is not None or cfg.dataset.get('streams') is not None:
         # Build streaming dataloader
         streams = build_streams(cfg.dataset)
         dataset = dataset_constructor.build_from_streaming(
             tokenizer=tokenizer,
             streams=streams,
             local=cfg.dataset.get('local', None),
             remote=cfg.dataset.get('remote', None),
@@ -157,81 +191,100 @@
             validate_hash=cfg.dataset.get('validate_hash', None),
             keep_zip=cfg.dataset.get('keep_zip', False),
             epoch_size=cfg.dataset.get('epoch_size', None),
             predownload=cfg.dataset.get('predownload', None),
             cache_limit=cfg.dataset.get('cache_limit', None),
             partition_algo=cfg.dataset.get('partition_algo', 'relaxed'),
             num_canonical_nodes=cfg.dataset.get('num_canonical_nodes', None),
-            batch_size=device_batch_size,
+            batch_size=dataset_batch_size,
             shuffle=cfg.dataset.get('shuffle', False),
             shuffle_algo=cfg.dataset.get('shuffle_algo', 'py1e'),
             shuffle_seed=cfg.dataset.get('shuffle_seed', 9176),
             shuffle_block_size=cfg.dataset.get('shuffle_block_size', None),
             sampling_method=cfg.dataset.get('sampling_method', 'balanced'),
             sampling_granularity=cfg.dataset.get('sampling_granularity', 1),
             batching_method=cfg.dataset.get('batching_method', 'random'),
             max_seq_len=cfg.dataset.max_seq_len,
+            allow_unsafe_types=cfg.dataset.get('allow_unsafe_types', False),
+            replication=replication_factor,
         )
 
     else:
         # Build HF dataloader
         dataset_name_or_path = cfg.dataset.hf_name
         split = cfg.dataset.get('split')
         if split is None:
             raise MissingHuggingFaceURLSplitError()
 
         # If dataset is a remote path, download it first.
         backend, _, _ = parse_uri(dataset_name_or_path)
         if backend not in ['', None]:
             dataset_name_or_path = _download_remote_hf_dataset(
-                remote_path=dataset_name_or_path, split=split)
+                remote_path=dataset_name_or_path,
+                split=split,
+            )
             split = split.replace('-', '_')
 
         # Get the preprocessing function.
         proto_preprocessing_fn = cfg.dataset.get('preprocessing_fn')
         if isinstance(proto_preprocessing_fn, (dict, DictConfig)):
             preprocessing_fn = dataset_constructor.get_preprocessing_fn_from_dict(
-                dict(proto_preprocessing_fn))
+                dict(proto_preprocessing_fn),
+            )
         else:
             preprocessing_fn = dataset_constructor.get_preprocessing_fn_from_str(
-                proto_preprocessing_fn, dataset_name_or_path)
+                proto_preprocessing_fn,
+                dataset_name_or_path,
+            )
 
         # Build dataset from HF.
         dataset = dataset_constructor.build_from_hf(
             dataset_name=dataset_name_or_path,
             split=split,
             safe_load=cfg.dataset.get('safe_load', False),
             max_seq_len=cfg.dataset.max_seq_len,
             preprocessing_fn=preprocessing_fn,
             tokenizer=tokenizer,
-            target_prompts=cfg.dataset.get('target_prompts',
-                                           _DEFAULT_TARGET_PROMPTS),
-            target_responses=cfg.dataset.get('target_responses',
-                                             _DEFAULT_TARGET_RESPONSES),
+            target_prompts=cfg.dataset.get(
+                'target_prompts',
+                _DEFAULT_TARGET_PROMPTS,
+            ),
+            target_responses=cfg.dataset.get(
+                'target_responses',
+                _DEFAULT_TARGET_RESPONSES,
+            ),
             decoder_only_format=cfg.dataset.decoder_only_format,
-            hf_kwargs=cfg.dataset.get('hf_kwargs', {}))
+            hf_kwargs=cfg.dataset.get('hf_kwargs', {}),
+        )
 
         # Ensure dataset is large enough.
         if cfg.drop_last:
-            world_size = dist.get_world_size()
+            world_size = dist.get_world_size() // replication_factor
             minimum_dataset_size = world_size * dataloader_batch_size
             if hasattr(dataset, '__len__'):
                 full_dataset_size = len(dataset)
                 if full_dataset_size < minimum_dataset_size:
                     raise NotEnoughDatasetSamplesError(
                         dataset_name=cfg.dataset.hf_name,
                         split=split,
                         dataloader_batch_size=dataloader_batch_size,
                         world_size=world_size,
                         full_dataset_size=full_dataset_size,
-                        minimum_dataset_size=minimum_dataset_size)
+                        minimum_dataset_size=minimum_dataset_size,
+                    )
         # Initialize sampler.
-        sampler = dist.get_sampler(dataset,
-                                   drop_last=cfg.drop_last,
-                                   shuffle=cfg.dataset.shuffle)
+        sampler = dist.get_sampler(
+            dataset,
+            drop_last=cfg.drop_last,
+            shuffle=cfg.dataset.shuffle,
+            num_replicas=dist.get_world_size() //
+            replication_factor if replication_factor > 1 else None,
+            rank=dist.get_global_rank() //
+            replication_factor if replication_factor > 1 else None,
+        )
 
     assert dataset is not None  # for pyright
     dl = DataLoader(
         dataset,
         collate_fn=collate_fn,
         batch_size=dataloader_batch_size,
         drop_last=cfg.drop_last,
@@ -239,17 +292,23 @@
         num_workers=cfg.num_workers,
         pin_memory=cfg.get('pin_memory', True),
         prefetch_factor=cfg.get('prefetch_factor', 2),
         persistent_workers=cfg.get('persistent_workers', True),
         timeout=cfg.get('timeout', 0),
     )
 
-    token_counting_func = get_tokens_per_batch_func()
-
-    return DataSpec(dataloader=dl, get_num_tokens_in_batch=token_counting_func)
+    return construct_from_registry(
+        name='data_spec',
+        registry=registry.data_specs,
+        partial_function=False,
+        kwargs={
+            'dl': dl,
+            'dataset_cfg': cfg.dataset,
+        },
+    )
 
 
 def _validate_config(dataset_cfg: DictConfig) -> None:
     """Validates the dataset configuration.
 
     Makes sure that the dataset is properly configured for either
     a HuggingFace dataset or a streaming dataset. Must be valid for one or
@@ -260,90 +319,102 @@
 
     Raises:
         ValueError: If the dataset configuration does not meet the requirements.
     """
     if dataset_cfg.get('hf_name') is not None:
         # Using the HuggingFace dataset codepath
         illegal_keys = ['local', 'remote']
-        discovered_illegal_keys = []
-        for key in illegal_keys:
-            if dataset_cfg.get(key) is not None:
-                discovered_illegal_keys.append('`' + key + '`')
+        discovered_illegal_keys = [
+            '`' + key + '`'
+            for key in illegal_keys
+            if dataset_cfg.get(key) is not None
+        ]
         if discovered_illegal_keys:
             raise ValueError(
                 'The dataset config sets a value for `hf_name` as well as the ' +\
                 f'following keys: {", ".join(discovered_illegal_keys)}.\n' +\
                 'Those keys are used when building from a streaming dataset, but ' +\
-                'setting `hf_name` instructs the dataset to build from a HuggingFace dataset.'
+                'setting `hf_name` instructs the dataset to build from a HuggingFace dataset.',
             )
     elif dataset_cfg.get('remote') is not None:
         # Using the streaming dataset codepath
         illegal_keys = ['hf_name', 'hf_kwargs', 'preprocessing_fn', 'safe_load']
         discovered_illegal_keys = []
         for key in illegal_keys:
             if dataset_cfg.get(key) is not None:
                 discovered_illegal_keys.append('`' + key + '`')
         if discovered_illegal_keys:
             raise ValueError(
                 'The dataset config sets a value for `remote` as well as the ' +\
                 f'following keys: {", ".join(discovered_illegal_keys)}.\n' +\
                 'Those keys are used when building from a HuggingFace dataset, but ' +\
-                'setting `remote` instructs the dataset to build from a streaming dataset.'
+                'setting `remote` instructs the dataset to build from a streaming dataset.',
             )
         if dataset_cfg.get('local') is None:
             raise ValueError(
                 'Using a streaming dataset requires setting both `remote` and `local`, ' +\
-                'but dataset.local is None.'
+                'but dataset.local is None.',
             )
     elif dataset_cfg.get('streams') is not None:
         # Using the streaming dataset codepath
         illegal_keys = ['hf_name', 'hf_kwargs', 'preprocessing_fn', 'safe_load']
         discovered_illegal_keys = []
         for key in illegal_keys:
             if dataset_cfg.get(key) is not None:
                 discovered_illegal_keys.append('`' + key + '`')
         if discovered_illegal_keys:
             raise ValueError(
                 'The dataset config sets a value for `streams` as well as the ' +\
                 f'following keys: {", ".join(discovered_illegal_keys)}.\n' +\
                 'Those keys are used when building from a HuggingFace dataset, but ' +\
-                'setting `streams` instructs the dataset to build from a streaming dataset.'
+                'setting `streams` instructs the dataset to build from a streaming dataset.',
             )
         illegal_keys = ['remote', 'local']
         discovered_illegal_keys = []
         for key in illegal_keys:
             if dataset_cfg.get(key) is not None:
                 discovered_illegal_keys.append('`' + key + '`')
         if discovered_illegal_keys:
             raise ValueError(
                 'The dataset config sets a value for `streams` as well as the ' +\
                 f'following keys: {", ".join(discovered_illegal_keys)}.\n' +\
                 'Please either use single stream (set remote/local only) ' +\
-                'or put remote/local under streams'
+                'or put remote/local under streams',
             )
 
     else:
         raise ValueError(
             'In the dataset config, you must set `hf_name` to use a HuggingFace ' +\
             'dataset, or set `remote` to use a streaming dataset, or set ' +\
-            '`streams` to use multiple streaming datasets,  but all were None.'
+            '`streams` to use multiple streaming datasets,  but all were None.',
         )
-    if dataset_cfg.get('max_seq_len') is None:
+    max_seq_len = dataset_cfg.get('max_seq_len')
+    if max_seq_len is None:
         raise ValueError(
-            'In the dataset config, you must set the `max_seq_len`')
+            'In the dataset config, you must set the `max_seq_len`',
+        )
+
+    if max_seq_len != int(max_seq_len):
+        raise ValueError('max_seq_len must be an integer')
+    dataset_cfg['max_seq_len'] = int(max_seq_len)
 
     # Raise an error if the target_prompts + target_responses + decoder_only_format settings
     # are invalid
     target_responses = str(
-        dataset_cfg.get('target_responses', _DEFAULT_TARGET_RESPONSES)).lower()
+        dataset_cfg.get('target_responses', _DEFAULT_TARGET_RESPONSES),
+    ).lower()
     target_prompts = str(
-        dataset_cfg.get('target_prompts', _DEFAULT_TARGET_PROMPTS)).lower()
+        dataset_cfg.get('target_prompts', _DEFAULT_TARGET_PROMPTS),
+    ).lower()
     decoder_only_format = dataset_cfg.decoder_only_format
-    validate_target_settings(target_prompts, target_responses,
-                             decoder_only_format)
+    validate_target_settings(
+        target_prompts,
+        target_responses,
+        decoder_only_format,
+    )
 
 
 def _download_remote_hf_dataset(remote_path: str, split: str) -> str:
     """Downloads a dataset from a remote object store.
 
     This function supports 'jsonl', 'csv', and 'parquet' file formats for the dataset. It will attempt to download
     the dataset, then once it is downloaded, convert it into HuggingFace ``datasets`` format, and then return this
@@ -371,38 +442,45 @@
     )
     os.makedirs(finetune_dir, exist_ok=True)
     for extension in SUPPORTED_EXTENSIONS:
         name = f'{remote_path.strip("/")}/{split}{extension}'
         destination = str(
             os.path.abspath(
                 os.path.join(
-                    finetune_dir, 'data',
-                    f'{hf_formatted_split}-00000-of-00001{extension}')))
+                    finetune_dir,
+                    'data',
+                    f'{hf_formatted_split}-00000-of-00001{extension}',
+                ),
+            ),
+        )
 
         # Since we don't know exactly what the extension will be, since it is one of a list
         # use a signal file to wait for instead of the desired file
         signal_file_path = os.path.join(
-            finetune_dir, f'.node_{dist.get_node_rank()}_local_rank0_completed')
+            finetune_dir,
+            f'.node_{dist.get_node_rank()}_local_rank0_completed',
+        )
         if dist.get_local_rank() == 0:
             try:
                 get_file(path=name, destination=destination, overwrite=True)
             except FileNotFoundError as e:
                 if extension == SUPPORTED_EXTENSIONS[-1]:
                     files_searched = [
                         f'{cfg.dataset.hf_name}/{cfg.dataset.split}{ext}'
                         for ext in SUPPORTED_EXTENSIONS
                     ]
                     raise FileNotFoundError(
                         f'Could not find a file with any of ' + \
                         f'the supported extensions: {SUPPORTED_EXTENSIONS}\n' + \
-                        f'at {files_searched}'
+                        f'at {files_searched}',
                     ) from e
                 else:
                     log.debug(
-                        f'Could not find {name}, looking for another extension')
+                        f'Could not find {name}, looking for another extension',
+                    )
                 continue
 
             os.makedirs(os.path.dirname(signal_file_path), exist_ok=True)
             with open(signal_file_path, 'wb') as f:
                 f.write(b'local_rank0_completed_download')
 
         # Avoid the collective call until the local rank zero has finished trying to download the dataset
@@ -415,61 +493,70 @@
         if dist.get_local_rank() == 0:
             os.remove(signal_file_path)
         dist.barrier()
         break
     return finetune_dir
 
 
-def _build_collate_fn(
-    dataloader_cfg: DictConfig, tokenizer: PreTrainedTokenizerBase,
-    device_batch_size: int
+def build_collate_fn(
+    dataloader_cfg: DictConfig,
+    tokenizer: PreTrainedTokenizerBase,
+    device_batch_size: int,
 ) -> Tuple[Union[Seq2SeqFinetuningCollator, BinPackCollator], int]:
     dataset_cfg = dataloader_cfg.dataset
     max_seq_len = dataset_cfg.max_seq_len
 
     collate_fn = Seq2SeqFinetuningCollator(
         tokenizer=tokenizer,
         max_seq_len=max_seq_len,
         decoder_only_format=dataset_cfg.decoder_only_format,
-        target_responses=dataset_cfg.get('target_responses',
-                                         _DEFAULT_TARGET_RESPONSES),
-        target_prompts=dataset_cfg.get('target_prompts',
-                                       _DEFAULT_TARGET_PROMPTS),
+        target_responses=dataset_cfg.get(
+            'target_responses',
+            _DEFAULT_TARGET_RESPONSES,
+        ),
+        target_prompts=dataset_cfg.get(
+            'target_prompts',
+            _DEFAULT_TARGET_PROMPTS,
+        ),
         allow_pad_trimming=dataset_cfg.get('allow_pad_trimming', False),
     )
 
     packing_ratio = dataset_cfg.get('packing_ratio')
     max_leftover_bins_to_keep = dataset_cfg.get('max_leftover_bins_to_keep')
     if packing_ratio is None:
         if max_leftover_bins_to_keep is not None:
             raise ValueError(
                 'dataset.max_leftover_bins_to_keep has been defined, ' +\
                 'but dataset.packing_ratio has not been set. Please set ' +\
                 'the latter to turn on packing or remove the former from the config.')
         return collate_fn, device_batch_size
 
     if packing_ratio == 'auto':
-        packing_ratio = auto_packing_ratio(dataloader_cfg, tokenizer,
-                                           device_batch_size)
+        packing_ratio = auto_packing_ratio(
+            dataloader_cfg,
+            tokenizer,
+            device_batch_size,
+        )
 
     if isinstance(packing_ratio, str):
         raise ValueError(
             'dataset.packing_ratio must be a float or "auto", but it was set to '
-            + f'{packing_ratio}.')
+            + f'{packing_ratio}.',
+        )
 
     log.info(f'Using packing ratio {packing_ratio}')
 
     if packing_ratio == 1.0:
         return collate_fn, device_batch_size
     elif packing_ratio < 1.0:
         raise ValueError('packing_ratio must be >= 1, if supplied')
 
     if not dataset_cfg.decoder_only_format:
         raise NotImplementedError(
-            'On-the-fly packing is currently only supported for decoder-only formats.'
+            'On-the-fly packing is currently only supported for decoder-only formats.',
         )
 
     collate_fn = BinPackCollator(
         collator=collate_fn,
         target_batch_size=device_batch_size,
         max_seq_len=max_seq_len,
         pad_token_id=tokenizer.pad_token_id,
@@ -511,24 +598,27 @@
                 'none',
         },
         'drop_last': False,
         'num_workers': 0,
         'pin_memory': False,
         'prefetch_factor': None,
         'persistent_workers': False,
-        'timeout': 0
+        'timeout': 0,
     })
 
     tokenizer_name = 'EleutherAI/gpt-neox-20b'
     tokenizer_kwargs = {'model_max_length': cfg.dataset.max_seq_len}
     tokenizer = build_tokenizer(tokenizer_name, tokenizer_kwargs)
 
     device_batch_size = 1
-    dataloader = build_finetuning_dataloader(cfg, tokenizer,
-                                             device_batch_size).dataloader
+    dataloader = build_finetuning_dataloader(
+        cfg,
+        tokenizer,
+        device_batch_size,
+    ).dataloader
 
     packing = cfg.dataset.get('packing_ratio') is not None
 
     for i, batch in enumerate(dataloader):
         if i >= 5:
             break
         print(f'-----Batch {i}-----')
@@ -541,68 +631,94 @@
             print(f'--- Sample {j} ---')
             if cfg.dataset.decoder_only_format:
                 if packing:
                     for subseq in range(int(batch['sequence_id'][j].max()) + 1):
                         is_subseq = batch['sequence_id'][j] == subseq
                         print(
                             '\033[93m{}\033[00m\n'.format('INPUT IDS:'),
-                            tokenizer.decode(batch['input_ids'][
-                                j,
-                                torch.logical_and(
-                                    is_subseq, batch['attention_mask'][j] ==
-                                    1)],
-                                             skip_special_tokens=False,
-                                             clean_up_tokenization_spaces=True))
+                            tokenizer.decode(
+                                batch['input_ids'][
+                                    j,
+                                    torch.logical_and(
+                                        is_subseq,
+                                        batch['attention_mask'][j] == 1,
+                                    )],
+                                skip_special_tokens=False,
+                                clean_up_tokenization_spaces=True,
+                            ),
+                        )
                         context = torch.logical_and(
                             batch['attention_mask'][j] == 1,
-                            batch['labels'][j] == _HF_IGNORE_INDEX)
+                            batch['labels'][j] == _HF_IGNORE_INDEX,
+                        )
                         print(
                             '\033[92m{}\033[00m\n'.format('CONTEXT:  '),
-                            tokenizer.decode(batch['input_ids'][
-                                j, torch.logical_and(is_subseq, context)],
-                                             skip_special_tokens=False,
-                                             clean_up_tokenization_spaces=True))
+                            tokenizer.decode(
+                                batch['input_ids'][
+                                    j, torch.logical_and(is_subseq, context)],
+                                skip_special_tokens=False,
+                                clean_up_tokenization_spaces=True,
+                            ),
+                        )
                         print(
                             '\033[91m{}\033[00m\n'.format('TARGET:   '),
-                            tokenizer.decode(batch['input_ids'][
-                                j,
-                                torch.logical_and(
-                                    is_subseq,
-                                    batch['labels'][j] != _HF_IGNORE_INDEX)],
-                                             skip_special_tokens=False,
-                                             clean_up_tokenization_spaces=True))
+                            tokenizer.decode(
+                                batch['input_ids'][
+                                    j,
+                                    torch.logical_and(
+                                        is_subseq,
+                                        batch['labels'][j] != _HF_IGNORE_INDEX,
+                                    )],
+                                skip_special_tokens=False,
+                                clean_up_tokenization_spaces=True,
+                            ),
+                        )
                 else:
                     print(
                         '\033[93m{}\033[00m\n'.format('INPUT IDS:'),
                         tokenizer.decode(
                             batch['input_ids'][j,
                                                batch['attention_mask'][j] == 1],
                             skip_special_tokens=False,
-                            clean_up_tokenization_spaces=True))
+                            clean_up_tokenization_spaces=True,
+                        ),
+                    )
                     context = torch.logical_and(
                         batch['attention_mask'][j] == 1,
-                        batch['labels'][j] == _HF_IGNORE_INDEX)
+                        batch['labels'][j] == _HF_IGNORE_INDEX,
+                    )
                     print(
                         '\033[92m{}\033[00m\n'.format('CONTEXT:  '),
-                        tokenizer.decode(batch['input_ids'][j, context],
-                                         skip_special_tokens=False,
-                                         clean_up_tokenization_spaces=True))
+                        tokenizer.decode(
+                            batch['input_ids'][j, context],
+                            skip_special_tokens=False,
+                            clean_up_tokenization_spaces=True,
+                        ),
+                    )
                     print(
                         '\033[91m{}\033[00m\n'.format('TARGET:   '),
-                        tokenizer.decode(batch['input_ids'][
-                            j, batch['labels'][j] != _HF_IGNORE_INDEX],
-                                         skip_special_tokens=False,
-                                         clean_up_tokenization_spaces=True))
+                        tokenizer.decode(
+                            batch['input_ids'][
+                                j, batch['labels'][j] != _HF_IGNORE_INDEX],
+                            skip_special_tokens=False,
+                            clean_up_tokenization_spaces=True,
+                        ),
+                    )
             else:
                 print(
                     '\033[92m{}\033[00m\n'.format('CONTEXT:  '),
                     tokenizer.decode(
                         batch['input_ids'][j, batch['attention_mask'][j] == 1],
                         skip_special_tokens=False,
-                        clean_up_tokenization_spaces=True))
+                        clean_up_tokenization_spaces=True,
+                    ),
+                )
                 print(
                     '\033[91m{}\033[00m\n'.format('TARGET:   '),
-                    tokenizer.decode(batch['labels'][
-                        j, batch['decoder_attention_mask'][j] == 1],
-                                     skip_special_tokens=False,
-                                     clean_up_tokenization_spaces=True))
+                    tokenizer.decode(
+                        batch['labels'][j, batch['decoder_attention_mask'][j] ==
+                                        1],
+                        skip_special_tokens=False,
+                        clean_up_tokenization_spaces=True,
+                    ),
+                )
         print('   ')
```

### Comparing `llm-foundry-0.7.0/llmfoundry/data/finetuning/tasks.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,59 +34,85 @@
 import importlib
 import logging
 import os
 import warnings
 from collections.abc import Mapping
 from functools import partial
 from pathlib import Path
-from typing import (Any, Callable, Dict, List, Literal, Optional, Sequence,
-                    Tuple, Union, cast)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+    cast,
+)
 
 import datasets as hf_datasets
+import datasets.exceptions as hf_exceptions
 import huggingface_hub as hf_hub
 import numpy as np
 from composer.utils import dist
 from streaming import Stream, StreamingDataset
 from transformers import PreTrainedTokenizerBase
 
-from llmfoundry.data.finetuning.collator import (_HF_IGNORE_INDEX,
-                                                 stitch_turns_decoder_only,
-                                                 stitch_turns_encoder_decoder)
+from llmfoundry.data.finetuning.collator import (
+    _HF_IGNORE_INDEX,
+    stitch_turns_decoder_only,
+    stitch_turns_encoder_decoder,
+)
 # yapf: disable
-from llmfoundry.utils.exceptions import (ConsecutiveRepeatedChatRolesError,
-                                         IncorrectMessageKeyQuantityError,
-                                         InvalidContentTypeError,
-                                         InvalidFileExtensionError,
-                                         InvalidLastChatMessageRoleError,
-                                         InvalidPromptResponseKeysError,
-                                         InvalidPromptTypeError,
-                                         InvalidResponseTypeError,
-                                         InvalidRoleError,
-                                         NotEnoughChatDataError,
-                                         TooManyKeysInExampleError,
-                                         UnableToProcessPromptResponseError,
-                                         UnknownExampleTypeError)
+from llmfoundry.utils.exceptions import (
+    ALLOWED_MESSAGES_KEYS,
+    ALLOWED_PROMPT_KEYS,
+    ALLOWED_RESPONSE_KEYS,
+    ConsecutiveRepeatedChatRolesError,
+    IncorrectMessageKeyQuantityError,
+    InvalidContentTypeError,
+    InvalidFileExtensionError,
+    InvalidLastChatMessageRoleError,
+    InvalidPromptResponseKeysError,
+    InvalidPromptTypeError,
+    InvalidResponseTypeError,
+    InvalidRoleError,
+    MisconfiguredHfDatasetError,
+    NotEnoughChatDataError,
+    UnableToProcessPromptResponseError,
+    UnknownExampleTypeError,
+)
 #  yapf: enable
 from llmfoundry.utils.logging_utils import SpecificWarningFilter
 
 log = logging.getLogger(__name__)
 
-__all__ = ['dataset_constructor']
+__all__ = [
+    'dataset_constructor',
+    'tokenize_formatted_example',
+    'is_valid_ift_example',
+    'StreamingFinetuningDataset',
+]
 
-_ALLOWED_RESPONSE_KEYS = {'response', 'completion'}
-_ALLOWED_PROMPT_KEYS = {'prompt'}
-_ALLOWED_MESSAGES_KEYS = {'messages'}
 _ALLOWED_ROLE_KEYS = {'role'}
 _ALLOWED_CONTENT_KEYS = {'content'}
-_ALLOWED_ROLES = {'user', 'assistant', 'system'}
+_ALLOWED_ROLES = {'user', 'assistant', 'system', 'tool'}
 _ALLOWED_LAST_MESSAGE_ROLES = {'assistant'}
 DOWNLOADED_FT_DATASETS_DIRPATH = os.path.abspath(
-    os.path.join(os.path.realpath(__file__), os.pardir, os.pardir, os.pardir,
-                 '.downloaded_finetuning'))
-SUPPORTED_EXTENSIONS = ['.csv', '.jsonl', '.parquet']
+    os.path.join(
+        os.path.realpath(__file__),
+        os.pardir,
+        os.pardir,
+        os.pardir,
+        '.downloaded_finetuning',
+    ),
+)
+SUPPORTED_EXTENSIONS = ['.csv', '.json', '.jsonl', '.parquet']
 
 PromptResponseDict = Mapping[str, str]
 ChatFormattedDict = Mapping[str, List[Dict[str, str]]]
 Example = Union[PromptResponseDict, ChatFormattedDict]
 ExampleType = Literal['prompt_response', 'chat']
 TokenizedExample = Dict[str, List[Dict[str, List[int]]]]
 
@@ -101,20 +127,28 @@
         ExampleType: The type of the input example, which can be either 'chat' for multi-way chat formatted conversation or 'prompt_response' for instruction-response pair.
 
     Raises:
         KeyError: If the example type is unknown.
     """
     if not isinstance(example, Mapping):
         raise TypeError(
-            f'Expected example to be a Mapping, but found {type(example)}')
-    if any(allowed_message_key in example
-           for allowed_message_key in _ALLOWED_MESSAGES_KEYS):
+            f'Expected example to be a Mapping, but found {type(example)}',
+        )
+    if (
+        len(example.keys()) == 1 and any(
+            allowed_message_key in example
+            for allowed_message_key in ALLOWED_MESSAGES_KEYS
+        )
+    ):
         return 'chat'
-    elif any(p in example for p in _ALLOWED_PROMPT_KEYS) and any(
-            r in example for r in _ALLOWED_RESPONSE_KEYS):
+    elif (
+        len(example.keys()) == 2 and
+        any(p in example for p in ALLOWED_PROMPT_KEYS) and
+        any(r in example for r in ALLOWED_RESPONSE_KEYS)
+    ):
         return 'prompt_response'
     else:
         raise UnknownExampleTypeError(example)
 
 
 def _is_empty_or_nonexistent(dirpath: str) -> bool:
     """Check if a directory is empty or non-existent.
@@ -127,59 +161,64 @@
     """
     return not os.path.isdir(dirpath) or len(os.listdir(dirpath)) == 0
 
 
 def _get_key(dictionary: Mapping[str, Any], allowed_keys: set[str]):
     if not isinstance(dictionary, Mapping):
         raise TypeError(
-            f'Expected dictionary to be a mapping, but found {type(dictionary)}'
+            f'Expected dictionary to be a mapping, but found {type(dictionary)}',
         )
     desired_keys = allowed_keys.intersection(dictionary.keys())
-    if len(desired_keys) != 1:
-        raise TooManyKeysInExampleError(allowed_keys, desired_keys)
     return list(desired_keys)[0]
 
 
 def _validate_chat_formatted_example(example: ChatFormattedDict):
     if not isinstance(example, Mapping):
         raise TypeError(
-            f'Expected example to be a mapping, but found {type(example)}')
-    messages = example[_get_key(example, _ALLOWED_MESSAGES_KEYS)]
+            f'Expected example to be a mapping, but found {type(example)}',
+        )
+    messages = example[_get_key(example, ALLOWED_MESSAGES_KEYS)]
     if not isinstance(messages, List):
         raise TypeError(
-            f'Expected messages to be an iterable, but found {type(messages)}')
+            f'Expected messages to be an iterable, but found {type(messages)}',
+        )
     if len(messages) <= 1:
         raise NotEnoughChatDataError()
 
     last_message = messages[-1]
     role_key = _get_key(last_message, _ALLOWED_ROLE_KEYS)
     last_role = last_message[role_key]
     if last_role not in _ALLOWED_LAST_MESSAGE_ROLES:
-        raise InvalidLastChatMessageRoleError(last_role,
-                                              _ALLOWED_LAST_MESSAGE_ROLES)
+        raise InvalidLastChatMessageRoleError(
+            last_role,
+            _ALLOWED_LAST_MESSAGE_ROLES,
+        )
 
     last_message_role = None
     for message in messages:
         role_key, content_key = _get_key(message, _ALLOWED_ROLE_KEYS), _get_key(
-            message, _ALLOWED_CONTENT_KEYS)
+            message,
+            _ALLOWED_CONTENT_KEYS,
+        )
         if len(message.keys()) != 2:
             raise IncorrectMessageKeyQuantityError(list(message.keys()))
         if message[role_key] not in _ALLOWED_ROLES:
             raise InvalidRoleError(message[role_key], _ALLOWED_ROLES)
         if not isinstance(message[content_key], str):
             raise InvalidContentTypeError(type(message[content_key]))
         if last_message_role is not None and last_message_role == message[
-                role_key]:
+            role_key]:
             raise ConsecutiveRepeatedChatRolesError(last_message_role)
         last_message_role = message[role_key]
 
 
 def _slice_chat_formatted_example(
-        example: ChatFormattedDict,
-        tokenizer: PreTrainedTokenizerBase) -> List[Tuple[str, str]]:
+    example: ChatFormattedDict,
+    tokenizer: PreTrainedTokenizerBase,
+) -> List[Tuple[str, str]]:
     """Slices chat example into a list of templated prompt, response turns.
 
     Note: Assistant messages mark the end of chat turns. So there are as many turns as there are
         assistant messages in the chat example.
 
     Args:
         example (ChatFormattedDict): The chat example containing the messages.
@@ -189,90 +228,106 @@
         List[Tuple[str, str]]: A list of templated prompt and response string pairs, one pair per chat turn.
 
     Raises:
         ValueError: If any chat turn in the example has less than two messages or if the last message is not from the assistant.
         KeyError: If a message does not have a role or content.
     """
     _validate_chat_formatted_example(example)
-    messages = example[_get_key(example, _ALLOWED_MESSAGES_KEYS)]
+    messages = example[_get_key(example, ALLOWED_MESSAGES_KEYS)]
 
     last_message = messages[-1]
     if last_message['role'] != 'assistant':
-        raise InvalidLastChatMessageRoleError(last_message['role'],
-                                              set(['assistant']))
+        raise InvalidLastChatMessageRoleError(
+            last_message['role'],
+            set('assistant'),
+        )
 
     def slice_out_last_turn(
-            messages_through_current_turn: List[Dict[str, str]],
-            conversation_through_previous_turn: str) -> Tuple[str, str]:
+        messages_through_current_turn: List[Dict[str, str]],
+        conversation_through_previous_turn: str,
+    ) -> Tuple[str, str]:
         full_conversation = tokenizer.apply_chat_template(
-            messages_through_current_turn, tokenize=False)
+            messages_through_current_turn,
+            tokenize=False,
+        )
         prompt_with_history = tokenizer.apply_chat_template(
             messages_through_current_turn[:-1],
             tokenize=False,
-            add_generation_prompt=True)
+            add_generation_prompt=True,
+        )
         if conversation_through_previous_turn != full_conversation[:len(
-                conversation_through_previous_turn)]:
+            conversation_through_previous_turn,
+        )]:
             raise ValueError(
-                f'The full conversation must start with the conversation through the previous turn. {conversation_through_previous_turn=}, {full_conversation=}'
+                f'The full conversation must start with the conversation through the previous turn. {conversation_through_previous_turn=}, {full_conversation=}',
             )
         if conversation_through_previous_turn != prompt_with_history[:len(
-                conversation_through_previous_turn)]:
+            conversation_through_previous_turn,
+        )]:
             raise ValueError(
-                f'The prompt_with_histry must start with the conversation through the previous turn. {conversation_through_previous_turn=}, {prompt_with_history=}'
+                f'The prompt_with_history must start with the conversation through the previous turn. {conversation_through_previous_turn=}, {prompt_with_history=}',
             )
         if prompt_with_history != full_conversation[:len(prompt_with_history)]:
             raise ValueError(
-                f'prompt_with_history must be the first part of the full conversation. {prompt_with_history=}, {full_conversation=}'
+                f'prompt_with_history must be the first part of the full conversation. {prompt_with_history=}, {full_conversation=}',
             )
         prompt = prompt_with_history[len(conversation_through_previous_turn):]
         response = full_conversation[len(prompt_with_history):]
         return prompt, response
 
     templated_prompt_response_turns: List[Tuple[str, str]] = []
     conversation_through_previous_turn = ''
     for idx, message in enumerate(messages):
         if message['role'] == 'assistant':
             prompt, response = slice_out_last_turn(
-                messages[:idx + 1], conversation_through_previous_turn)
+                messages[:idx + 1],
+                conversation_through_previous_turn,
+            )
             templated_prompt_response_turns.append((prompt, response))
             conversation_through_previous_turn += prompt
             conversation_through_previous_turn += response
 
     return templated_prompt_response_turns
 
 
-def _tokenize_with_bos_removal(tokenizer: PreTrainedTokenizerBase, text: str,
-                               text_target: str) -> Dict[str, List[int]]:
+def _tokenize_with_bos_removal(
+    tokenizer: PreTrainedTokenizerBase,
+    text: str,
+    text_target: str,
+) -> Dict[str, List[int]]:
     """Tokenizes the prompt and response using the provided tokenizer.
 
     Args:
         tokenizer (PreTrainedTokenizerBase): The tokenizer to use for tokenization.
         text (str): The prompt to tokenize.
         text_target (str): The response to tokenize.
 
     Returns:
         Dict[str, List[int]]: The tokenized text and text_target.
     """
-    tokenized_sample = tokenizer(text=text,
-                                 text_target=text_target,
-                                 padding=False,
-                                 truncation=False)
+    tokenized_sample = tokenizer(
+        text=text,
+        text_target=text_target,
+        padding=False,
+        truncation=False,
+    )
 
     # Remove the BOS token from the start of the labels if it was automatically added
     if hasattr(tokenizer, 'add_bos_token') and tokenizer.add_bos_token:
         if tokenizer.bos_token_id is not None and tokenized_sample['labels'][
-                0] == tokenizer.bos_token_id:
+            0] == tokenizer.bos_token_id:
             tokenized_sample['labels'] = tokenized_sample['labels'][1:]
 
     return tokenized_sample
 
 
 def _tokenize_chat_formatted_example(
-        example: ChatFormattedDict,
-        tokenizer: PreTrainedTokenizerBase) -> TokenizedExample:
+    example: ChatFormattedDict,
+    tokenizer: PreTrainedTokenizerBase,
+) -> TokenizedExample:
     """Tokenizes a chat-formatted example using the provided tokenizer.
 
     Args:
         example (ChatFormattedDict): The chat-formatted example to tokenize.
         tokenizer (PreTrainedTokenizerBase): The tokenizer to use for tokenization.
 
     Returns:
@@ -282,38 +337,34 @@
     # special tokens are expected to be added via the tokenizer's chat template. So,
     # we instead expect the prompt/response outputs of `_slice_chat_formatted_example`
     # (which calls `apply_chat_template`) to have the correct special tokens already.
     # We disable padding and truncation because those are handled in the collator, which needs to
     # be able to assume that none of the tokens are pad tokens.
     return {
         'turns': [
-            tokenizer(text=prompt,
-                      text_target=response,
-                      add_special_tokens=False,
-                      padding=False,
-                      truncation=False)
-            for prompt, response in _slice_chat_formatted_example(
-                example, tokenizer)
-        ]
+            tokenizer(
+                text=prompt,
+                text_target=response,
+                add_special_tokens=False,
+                padding=False,
+                truncation=False,
+            ) for prompt, response in
+            _slice_chat_formatted_example(example, tokenizer)
+        ],
     }
 
 
 def _tokenize_prompt_response_formatted_example(
-        example: PromptResponseDict,
-        tokenizer: PreTrainedTokenizerBase) -> TokenizedExample:
+    example: PromptResponseDict,
+    tokenizer: PreTrainedTokenizerBase,
+) -> TokenizedExample:
     """Tokenize a formatted example and validate expected keys."""
     example_keys = set(example.keys())
-    prompt_keys = example_keys.intersection(_ALLOWED_PROMPT_KEYS)
-    response_keys = example_keys.intersection(_ALLOWED_RESPONSE_KEYS)
-
-    if len(prompt_keys) != 1:
-        raise TooManyKeysInExampleError(_ALLOWED_PROMPT_KEYS, prompt_keys)
-
-    if len(response_keys) != 1:
-        raise TooManyKeysInExampleError(_ALLOWED_RESPONSE_KEYS, response_keys)
+    prompt_keys = example_keys.intersection(ALLOWED_PROMPT_KEYS)
+    response_keys = example_keys.intersection(ALLOWED_RESPONSE_KEYS)
 
     prompt_key = prompt_keys.pop()
     response_key = response_keys.pop()
     prompt = example[prompt_key]
     response = example[response_key]
     if not isinstance(prompt, str):
         raise InvalidPromptTypeError(type(prompt))
@@ -329,22 +380,23 @@
     # be able to assume that none of the tokens are pad tokens.
     return {
         'turns': [
             _tokenize_with_bos_removal(
                 tokenizer=tokenizer,
                 text=prompt,
                 text_target=response,
-            )
-        ]
+            ),
+        ],
     }
 
 
 def tokenize_formatted_example(
-        example: Example,
-        tokenizer: PreTrainedTokenizerBase) -> TokenizedExample:
+    example: Example,
+    tokenizer: PreTrainedTokenizerBase,
+) -> TokenizedExample:
     """Tokenizes a formatted example using the provided tokenizer.
 
     Args:
         example (Example): The input example to be tokenized.
         tokenizer (PreTrainedTokenizerBase): The tokenizer to be used for tokenization.
 
     Returns:
@@ -356,24 +408,32 @@
     example_format = _get_example_type(example)
 
     if example_format == 'chat':
         chat_example = cast(ChatFormattedDict, example)
         return _tokenize_chat_formatted_example(chat_example, tokenizer)
     elif example_format == 'prompt_response':
         prompt_response_example: PromptResponseDict = cast(
-            PromptResponseDict, example)
+            PromptResponseDict,
+            example,
+        )
         return _tokenize_prompt_response_formatted_example(
-            prompt_response_example, tokenizer)
+            prompt_response_example,
+            tokenizer,
+        )
     else:
-        raise UnknownExampleTypeError(example)
+        raise NotImplementedError
 
 
-def is_valid_ift_example(max_seq_len: int, target_prompts: str,
-                         target_responses: str, decoder_only_format: bool,
-                         example: TokenizedExample) -> bool:
+def is_valid_ift_example(
+    max_seq_len: int,
+    target_prompts: str,
+    target_responses: str,
+    decoder_only_format: bool,
+    example: TokenizedExample,
+) -> bool:
     """Check if the example is a valid ift example.
 
     This function confirms that none of the ``input_ids`` and ``labels`` fields
     are empty in any of the turns within the example.
 
     This function also prepares the final input_ids and labels
     of the (potentially multi-turn) example, using the target settings
@@ -408,35 +468,40 @@
             example_turns=example['turns'],
             target_prompts=target_prompts,
             target_responses=target_responses,
         )
 
     else:
         input_ids, labels = stitch_turns_encoder_decoder(
-            example_turns=example['turns'],)
+            example_turns=example['turns'],
+        )
     input_ids = input_ids[:max_seq_len]
     labels = labels[:max_seq_len]
 
     if len(input_ids) == 0:
         return False
 
     if len([label for label in labels if label != _HF_IGNORE_INDEX]) == 0:
         return False
 
     return True
 
 
-def _stream_remote_local_validate(remote: Optional[str], local: Optional[str],
-                                  split: Optional[str]):
+def _stream_remote_local_validate(
+    remote: Optional[str],
+    local: Optional[str],
+    split: Optional[str],
+):
     if remote is None or (local == remote):
         if local is not None and os.path.isdir(local):
             contents = set(os.listdir(local))
             if split is not None and split not in contents:
                 raise ValueError(
-                    f'Local directory {local} does not contain split {split}')
+                    f'Local directory {local} does not contain split {split}',
+                )
 
 
 class StreamingFinetuningDataset(StreamingDataset):
     """Finetuning dataset with flexible tokenization using StreamingDataset.
 
     Args:
         tokenizer (Tokenizer): The name of the HuggingFace tokenizer to use to
@@ -486,53 +551,66 @@
             Defaults to ``balanced``.
         sampling_granularity (int): When picking samples for a stream's final partial repeat,
             how many samples to pick from the same shard at a time (``1`` for evenly balanced
             across shards, ``1000`` to pick 1000 samples from the same shard at a time, etc).
             Defaults to ``1``.
         batching_method (str): Which batching method to use, either ``random``, ``stratified``, or
             ``per_stream``. Defaults to ``random``.
+        allow_unsafe_types (bool): If a shard contains Pickle, which allows arbitrary code
+            execution during deserialization, whether to keep going if ``True`` or raise an error
+            if ``False``. Defaults to ``False``.
+        replication (int, optional): Determines how many consecutive devices will receive the same
+            samples. Useful for training with tensor or sequence parallelism, where multiple
+            devices need to see the same partition of the dataset. Defaults to ``None``.
     """
 
-    def __init__(self,
-                 tokenizer: PreTrainedTokenizerBase,
-                 streams: Optional[Sequence[Stream]] = None,
-                 local: Optional[str] = None,
-                 remote: Optional[str] = None,
-                 split: Optional[str] = None,
-                 download_retry: int = 2,
-                 download_timeout: float = 60,
-                 validate_hash: Optional[str] = None,
-                 keep_zip: bool = False,
-                 epoch_size: Optional[Union[int, str]] = None,
-                 predownload: Optional[int] = None,
-                 cache_limit: Optional[Union[int, str]] = None,
-                 partition_algo: str = 'relaxed',
-                 num_canonical_nodes: Optional[int] = None,
-                 batch_size: Optional[int] = None,
-                 shuffle: bool = False,
-                 shuffle_algo: str = 'py1e',
-                 shuffle_seed: int = 9176,
-                 shuffle_block_size: Optional[int] = None,
-                 sampling_method: str = 'balanced',
-                 sampling_granularity: int = 1,
-                 batching_method: str = 'random',
-                 max_seq_len: int = 2048,
-                 **kwargs: Any):
+    def __init__(
+        self,
+        tokenizer: PreTrainedTokenizerBase,
+        streams: Optional[Sequence[Stream]] = None,
+        local: Optional[str] = None,
+        remote: Optional[str] = None,
+        split: Optional[str] = None,
+        download_retry: int = 2,
+        download_timeout: float = 60,
+        validate_hash: Optional[str] = None,
+        keep_zip: bool = False,
+        epoch_size: Optional[Union[int, str]] = None,
+        predownload: Optional[int] = None,
+        cache_limit: Optional[Union[int, str]] = None,
+        partition_algo: str = 'relaxed',
+        num_canonical_nodes: Optional[int] = None,
+        batch_size: Optional[int] = None,
+        shuffle: bool = False,
+        shuffle_algo: str = 'py1e',
+        shuffle_seed: int = 9176,
+        shuffle_block_size: Optional[int] = None,
+        sampling_method: str = 'balanced',
+        sampling_granularity: int = 1,
+        batching_method: str = 'random',
+        max_seq_len: int = 2048,
+        allow_unsafe_types: bool = False,
+        replication: Optional[int] = None,
+        **kwargs: Any,
+    ):
 
         if len(kwargs) > 0:
             raise ValueError(
-                f'StreamingFinetuningDataset() got an unexpected keyword argument: {kwargs}'
+                f'StreamingFinetuningDataset() got an unexpected keyword argument: {kwargs}',
             )
 
         if streams is None:
             _stream_remote_local_validate(remote, local, split)
         else:
             for stream in streams:
-                _stream_remote_local_validate(stream.remote, stream.local,
-                                              split)
+                _stream_remote_local_validate(
+                    stream.remote,
+                    stream.local,
+                    split,
+                )
 
         super().__init__(
             streams=streams,
             local=local,
             remote=remote,
             split=split,
             download_retry=download_retry,
@@ -548,14 +626,16 @@
             shuffle=shuffle,
             shuffle_algo=shuffle_algo,
             shuffle_seed=shuffle_seed,
             shuffle_block_size=shuffle_block_size,
             sampling_method=sampling_method,
             sampling_granularity=sampling_granularity,
             batching_method=batching_method,
+            allow_unsafe_types=allow_unsafe_types,
+            replication=replication,
         )
 
         self.tokenizer = tokenizer
         self.max_seq_len = max_seq_len
 
     # How to process a sample
     def __getitem__(self, idx: int) -> Dict[str, Any]:
@@ -564,26 +644,28 @@
             # Already tokenized in latest format
             return sample
         if 'input_ids' in sample:
             # Already tokenized data (old format)
             if isinstance(sample['input_ids'], bytes):
                 sample['input_ids'] = np.frombuffer(
                     sample['input_ids'],
-                    dtype=np.int64)[:self.max_seq_len].tolist().copy()
+                    dtype=np.int64,
+                )[:self.max_seq_len].tolist().copy()
                 sample['labels'] = np.frombuffer(
                     sample['labels'],
-                    dtype=np.int64)[:self.max_seq_len].tolist().copy()
+                    dtype=np.int64,
+                )[:self.max_seq_len].tolist().copy()
             elif isinstance(sample['input_ids'], np.ndarray):
-                sample['input_ids'] = sample[
-                    'input_ids'][:self.max_seq_len].tolist().copy()
+                sample['input_ids'] = sample['input_ids'][:self.max_seq_len
+                                                         ].tolist().copy()
                 sample['labels'] = sample['labels'][:self.max_seq_len].tolist(
                 ).copy()
             else:
                 raise ValueError(
-                    f'Expect input_ids to be bytes or numpy.ndarray type, but got {type(sample["input_ids"])}'
+                    f'Expect input_ids to be bytes or numpy.ndarray type, but got {type(sample["input_ids"])}',
                 )
             # Convert to latest format by wrapping sample as a "turn"
             return {'turns': [sample]}
         return tokenize_formatted_example(sample, tokenizer=self.tokenizer)
 
 
 class DatasetConstructor:
@@ -593,15 +675,15 @@
 
     def register(self, *names: str) -> Callable[[Callable], Callable]:
         """Decorator for registering preprocessing functions."""
 
         def _register_func(name: str, func: Callable) -> None:
             if name in self._task_preprocessing_registry:
                 raise ValueError(
-                    f'A tokenization function has already been registered with {name=}.'
+                    f'A tokenization function has already been registered with {name=}.',
                 )
             self._task_preprocessing_registry[name] = func
             return
 
         def wrapper(func: Callable) -> Callable:
             for name in names:
                 _register_func(name, func)
@@ -610,17 +692,17 @@
         return wrapper
 
     def print_registered_tasks(self) -> None:
         tasks = sorted(self._task_preprocessing_registry.keys())
         log.info('\n'.join(tasks))
 
     def get_preprocessing_fn_from_dict(
-            self,
-            mapping: Dict[str,
-                          str]) -> Callable[[Dict[str, Any]], Dict[str, str]]:
+        self,
+        mapping: Dict[str, str],
+    ) -> Callable[[Dict[str, Any]], Example]:
         """Get a preprocessing function from a dictionary.
 
         The dictionary maps column names in the dataset to "prompt" and "response".
         For example,
             ```yaml
             preprocessing_fn:
                 prompt: text
@@ -639,24 +721,24 @@
         """
 
         def _preprocessor(example: Dict[str, Any]) -> Dict[str, str]:
             if list(mapping.keys()) != ['prompt', 'response']:
                 raise InvalidPromptResponseKeysError(mapping, example)
             return {
                 'prompt': example[mapping['prompt']],
-                'response': example[mapping['response']]
+                'response': example[mapping['response']],
             }
 
         return _preprocessor
 
     def get_preprocessing_fn_from_str(
         self,
         preprocessor: Optional[str],
-        dataset_name: Optional[str] = None
-    ) -> Optional[Callable[[Dict[str, Any]], Dict[str, str]]]:
+        dataset_name: Optional[str] = None,
+    ) -> Optional[Callable[[Dict[str, Any]], Example]]:
         """Get a preprocessing function from a string.
 
         String can be either a registered function or an import path.
 
         Args:
             preprocessor (Optional[str]): The name of the preprocessing function, or an import path.
             dataset_name (Optional[str]): The dataset name to look up in the registry.
@@ -668,46 +750,52 @@
             ValueError: If the preprocessing function import from the provided string fails.
         """
         if preprocessor is None:
             if dataset_name is None:
                 return None
             if dataset_name in self._task_preprocessing_registry:
                 log.info(
-                    f'Re-formatting dataset with "{dataset_name}" preprocessing function.'
+                    f'Re-formatting dataset with "{dataset_name}" preprocessing function.',
                 )
                 return self._task_preprocessing_registry[dataset_name]
             else:
                 log.info('No preprocessor was supplied and no preprocessing function ' +\
                         f'is registered for dataset name "{dataset_name}". No additional ' +\
                         'preprocessing will be applied. If the dataset is already formatted ' +\
                         'correctly, you can ignore this message.')
                 return None
         if preprocessor in self._task_preprocessing_registry:
             log.info(
-                f'Re-formatting dataset with "{preprocessor}" preprocessing function.'
+                f'Re-formatting dataset with "{preprocessor}" preprocessing function.',
             )
             return self._task_preprocessing_registry[preprocessor]
 
         try:
             import_path, function_name = preprocessor.split(':', maxsplit=1)
             module = importlib.import_module(import_path)
             preprocessing_fn = getattr(module, function_name)
         except Exception as e:
             raise ValueError(
-                f'Failed to import preprocessing function from string = {preprocessor}.'
+                f'Failed to import preprocessing function from string = {preprocessor}.',
             ) from e
 
         return preprocessing_fn
 
     def build_from_hf(
-        self, dataset_name: str, split: str, safe_load: bool, max_seq_len: int,
-        preprocessing_fn: Optional[Callable[[dict[str, Any]], dict[str, str]]],
-        tokenizer: PreTrainedTokenizerBase, target_prompts: str,
-        target_responses: str, decoder_only_format: bool, hf_kwargs: Dict[str,
-                                                                          Any]
+        self,
+        dataset_name: str,
+        split: str,
+        safe_load: bool,
+        max_seq_len: int,
+        preprocessing_fn: Optional[Callable[[dict[str, Any]], Example]],
+        tokenizer: PreTrainedTokenizerBase,
+        target_prompts: str,
+        target_responses: str,
+        decoder_only_format: bool,
+        hf_kwargs: Dict[str, Any],
     ) -> Union[hf_datasets.DatasetDict, hf_datasets.Dataset,
                hf_datasets.IterableDatasetDict, hf_datasets.IterableDataset]:
         """Load a HuggingFace Datasets, preprocess, and tokenize.
 
         Note: This function will drop examples where the prompt is longer than the max_seq_len
 
         Args:
@@ -725,69 +813,83 @@
         # can just read them.
         if dist.get_local_rank() != 0:
             log.debug('Waiting for local_rank 0 to finish data prep')
             with dist.local_rank_zero_download_and_wait(signal_file_path):
                 pass
 
         hf_tokenization_logger = logging.getLogger(
-            'transformers.tokenization_utils_base')
+            'transformers.tokenization_utils_base',
+        )
         sequence_length_warning_filter = SpecificWarningFilter(
-            'Token indices sequence length is longer than the specified maximum sequence length'
+            'Token indices sequence length is longer than the specified maximum sequence length',
         )
 
         # We will trim examples later in the collate_fn, so we want to silence this warning from Hugging Face
         hf_tokenization_logger.addFilter(sequence_length_warning_filter)
 
         error: Optional[Exception] = None
         filtered_dataset = None
         try:
             if safe_load:
                 if not os.path.isdir(dataset_name):
                     # dataset_name is not a local dir path, download if needed.
                     local_dataset_dir = os.path.join(
-                        DOWNLOADED_FT_DATASETS_DIRPATH, dataset_name)
+                        DOWNLOADED_FT_DATASETS_DIRPATH,
+                        dataset_name,
+                    )
 
                     if _is_empty_or_nonexistent(dirpath=local_dataset_dir):
                         # Safely load a dataset from HF Hub with restricted file types.
                         hf_hub.snapshot_download(
                             dataset_name,
                             repo_type='dataset',
                             allow_patterns=[
                                 '*' + ext for ext in SUPPORTED_EXTENSIONS
                             ],
                             token=hf_kwargs.get('token', None),
                             revision=hf_kwargs.get('revision', None),
                             local_dir_use_symlinks=False,
-                            local_dir=local_dataset_dir)
+                            local_dir=local_dataset_dir,
+                        )
                         if _is_empty_or_nonexistent(dirpath=local_dataset_dir):
                             raise InvalidFileExtensionError(
-                                dataset_name, SUPPORTED_EXTENSIONS)
+                                dataset_name,
+                                SUPPORTED_EXTENSIONS,
+                            )
                     # Set dataset_name to the downloaded location.
                     dataset_name = local_dataset_dir
 
                 # dataset_name is a local dir path. Use the abspath to prevent confusion.
                 dataset_name = os.path.abspath(dataset_name)
 
                 # Ensure that the local dir contains only allowed file types.
                 dataset_files = [
                     f for _, _, files in os.walk(dataset_name) for f in files
                 ]
                 if not all(
-                        Path(f).suffix in SUPPORTED_EXTENSIONS
-                        for f in dataset_files):
-                    raise InvalidFileExtensionError(dataset_name,
-                                                    SUPPORTED_EXTENSIONS)
-
-            dataset = hf_datasets.load_dataset(dataset_name,
-                                               split=split,
-                                               **hf_kwargs)
+                    Path(f).suffix in SUPPORTED_EXTENSIONS
+                    for f in dataset_files
+                ):
+                    raise InvalidFileExtensionError(
+                        dataset_name,
+                        SUPPORTED_EXTENSIONS,
+                    )
+
+            dataset = hf_datasets.load_dataset(
+                dataset_name,
+                split=split,
+                **hf_kwargs,
+            )
 
             def dataset_mapper(example: Dict):
                 if preprocessing_fn is not None:
-                    example = preprocessing_fn(example)
+                    return tokenize_formatted_example(
+                        preprocessing_fn(example),
+                        tokenizer,
+                    )
                 return tokenize_formatted_example(example, tokenizer)
 
             detected_cpu_count = os.cpu_count() or 1
             detected_cpus_with_margin = detected_cpu_count - 8
             num_cpus_to_use = max(1, detected_cpus_with_margin)
 
             columns_to_remove = list(dataset[0].keys())
@@ -796,26 +898,31 @@
                 batched=False,
                 remove_columns=columns_to_remove,
                 num_proc=num_cpus_to_use,
                 desc='Tokenizing dataset',
             )
 
             filtered_dataset = tokenized_dataset.filter(
-                partial(is_valid_ift_example, max_seq_len, target_prompts,
-                        target_responses, decoder_only_format),
+                partial(
+                    is_valid_ift_example,
+                    max_seq_len,
+                    target_prompts,
+                    target_responses,
+                    decoder_only_format,
+                ),
                 num_proc=num_cpus_to_use,
                 desc='Filtering out long prompts',
             )
 
             examples_removed = len(tokenized_dataset) - len(filtered_dataset)
             if examples_removed > 0:
                 warnings.warn(
                     f'Dropped {examples_removed} examples where the prompt was longer than {max_seq_len}, '
                     +
-                    'the prompt or response was empty, or the response was all padding tokens.'
+                    'the prompt or response was empty, or the response was all padding tokens.',
                 )
         except Exception as e:
             error = e
         # Now local rank 0 indicates to the other ranks that it is done
         if dist.get_local_rank() == 0:
             log.debug('Local rank 0 finished data prep')
             with open(signal_file_path, 'wb') as f:
@@ -824,46 +931,55 @@
         # All ranks sync up at this barrier, having completed data processing
         dist.barrier()
 
         # Last, local rank 0 cleans up the signal file
         if dist.get_local_rank() == 0:
             os.remove(signal_file_path)
 
+        if isinstance(error, hf_exceptions.DatasetGenerationError):
+            log.error('Huggingface DatasetGenerationError during data prep.')
+            raise MisconfiguredHfDatasetError(
+                dataset_name=dataset_name,
+                split=split,
+            )
         if error is not None:
             log.error('Error during data prep')
             raise error
         log.debug('All ranks finished data prep')
 
         hf_tokenization_logger.removeFilter(sequence_length_warning_filter)
 
         assert filtered_dataset is not None
         return filtered_dataset
 
-    def build_from_streaming(self, *args: Any,
-                             **kwargs: Any) -> StreamingFinetuningDataset:
+    def build_from_streaming(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> StreamingFinetuningDataset:
         return StreamingFinetuningDataset(*args, **kwargs)
 
 
 dataset_constructor = DatasetConstructor()
 
 
 @dataset_constructor.register('tatsu-lab/alpaca')
-def alpaca_preprocessing_function(inp: Dict) -> Dict[str, str]:
+def alpaca_preprocessing_function(inp: Dict) -> PromptResponseDict:
     """Split out prompt/response from text."""
     try:
         prompt, response = inp['text'].split('### Response:')
         prompt += '### Response:'
     except Exception as e:
         raise UnableToProcessPromptResponseError(inp) from e
 
     return {'prompt': prompt, 'response': response}
 
 
 @dataset_constructor.register('HuggingFaceH4/databricks_dolly_15k')
-def dolly_preprocessing_function(inp: Dict) -> Dict[str, str]:
+def dolly_preprocessing_function(inp: Dict) -> PromptResponseDict:
     """Format the text string."""
     PROMPT_FORMAT = 'Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:\n{instruction}\n\n### Response:\n'
     try:
         if inp['input'] != '':
             instruction = inp['instruction'] + '\n' + inp['input']
         else:
             instruction = inp['instruction']
@@ -871,30 +987,50 @@
         response = inp['output']
     except Exception as e:
         raise UnableToProcessPromptResponseError(inp) from e
     return {'prompt': prompt, 'response': response}
 
 
 @dataset_constructor.register('bigscience/P3')
-def p3_preprocessing_function(inp: Dict) -> Dict[str, str]:
+def p3_preprocessing_function(inp: Dict) -> PromptResponseDict:
     """Format the already-split example."""
     return {
         'prompt': inp['inputs'] + ':',
         'response': inp['targets'],
     }
 
 
 # Muennighoff's P3 and flan datasets share a similar convention
 @dataset_constructor.register('Muennighoff/P3', 'Muennighoff/flan')
-def muennighoff_tokenize_function(inp: Dict) -> Dict[str, str]:
+def muennighoff_tokenize_function(inp: Dict) -> PromptResponseDict:
     """Format the already-split example."""
     try:
         prompt: str = inp['inputs']
         response: str = inp['targets']
         # Put a space before the response if needed
         transitions = (' ', '\n', '\t')
-        if not (prompt.endswith(transitions) or
-                response.startswith(transitions)):
+        if not (
+            prompt.endswith(transitions) or response.startswith(transitions)
+        ):
             response = ' ' + response
     except Exception as e:
         raise UnableToProcessPromptResponseError(inp) from e
     return {'prompt': prompt, 'response': response}
+
+
+@dataset_constructor.register('teknium/OpenHermes-2.5')
+def shareGPT_format_preprocessor(inp: Dict) -> ChatFormattedDict:
+    """Convert from ShareGPT format to our chat format."""
+    role_map = {
+        'human': 'user',
+        'gpt': 'assistant',
+    }
+    try:
+        conversation = inp['conversations']
+        messages: List[Dict[str, str]] = []
+        for message in conversation:
+            role: str = role_map.get(message['from'], message['from'])
+            content: str = message['value']
+            messages.append({'role': role, 'content': content})
+    except Exception as e:
+        raise UnableToProcessPromptResponseError(inp) from e
+    return {'messages': messages}
```

### Comparing `llm-foundry-0.7.0/llmfoundry/data/packing.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/packing.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,39 @@
 
 import logging
 import tempfile
 from typing import Callable, Dict, Iterable, List, Literal, Optional, Tuple
 
 import numpy as np
 import torch
+from composer.utils import dist
 from omegaconf import DictConfig
 from transformers import PreTrainedTokenizerBase
 
 log = logging.getLogger(__name__)
 
+__all__ = [
+    'BinPackCollator',
+    'auto_packing_ratio',
+    'profile_packing',
+]
+
 
 class BinPackCollator:
     """Utility collator for packing to reduce padding."""
 
-    def __init__(self,
-                 collator: Callable,
-                 target_batch_size: int,
-                 max_seq_len: int,
-                 pad_token_id: int,
-                 padding_side: Literal['left', 'right'],
-                 max_leftover_bins_to_keep: Optional[int] = None):
+    def __init__(
+        self,
+        collator: Callable,
+        target_batch_size: int,
+        max_seq_len: int,
+        pad_token_id: int,
+        padding_side: Literal['left', 'right'],
+        max_leftover_bins_to_keep: Optional[int] = None,
+    ):
         self.base_collator = collator
         self.out_size = int(target_batch_size)
         self.max_seq_len = int(max_seq_len)
         self.pad_token_id = int(pad_token_id)
         self.padding_side = padding_side
 
         if self.out_size <= 0:
@@ -34,35 +43,38 @@
         if self.max_seq_len <= 0:
             raise ValueError(f'{max_seq_len=} must be >0.')
         if self.pad_token_id < 0:
             raise ValueError(f'{pad_token_id=} must be >=0.')
 
         if max_leftover_bins_to_keep is not None and max_leftover_bins_to_keep < 0:
             raise ValueError(
-                f'{max_leftover_bins_to_keep=} must be >=0 or None.')
+                f'{max_leftover_bins_to_keep=} must be >=0 or None.',
+            )
         self.max_leftover_bins_to_keep = max_leftover_bins_to_keep
 
         self.n_packed_tokens = 0
         self.n_total_tokens = 0
         self.n_packed_examples = 0
 
         self._leftover_bins: List[Tuple[int, Dict[str, torch.Tensor]]] = []
 
     @property
     def waste(self) -> float:
         return 1 - (self.n_packed_tokens / self.n_total_tokens)
 
     @property
     def efficiency(self) -> float:
-        return self.n_packed_tokens / (self.max_seq_len *
-                                       self.n_packed_examples)
+        return self.n_packed_tokens / (
+            self.max_seq_len * self.n_packed_examples
+        )
 
     def __call__(
-            self,
-            examples: List[Dict[str, torch.Tensor]]) -> Dict[str, torch.Tensor]:
+        self,
+        examples: List[Dict[str, torch.Tensor]],
+    ) -> Dict[str, torch.Tensor]:
         batch = self.base_collator(examples)
         return self.pack(batch)
 
     def pack(self, batch: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         assert 'attention_mask' in batch
         assert 'input_ids' in batch
 
@@ -73,17 +85,19 @@
                 'attention_mask',
                 'sequence_id',
             ]
         # Cut everything down to size
         sizes, trimmed_examples = _trim_batch(batch)
         return self._pack_trimmed_examples(trimmed_examples, sizes)
 
-    def _pack_trimmed_examples(self, trimmed_examples: List[Dict[str,
-                                                                 torch.Tensor]],
-                               sizes: List[int]) -> Dict[str, torch.Tensor]:
+    def _pack_trimmed_examples(
+        self,
+        trimmed_examples: List[Dict[str, torch.Tensor]],
+        sizes: List[int],
+    ) -> Dict[str, torch.Tensor]:
         """Packs trimmed examples into fixed-size bins and repads them.
 
         Args:
             trimmed_examples (List[Dict[str, torch.Tensor]]): A list of trimmed examples.
             sizes (List[int]): The sizes of the trimmed examples.
 
         Returns:
@@ -99,23 +113,25 @@
         )
         self.n_packed_tokens += n_packed_tokens
         self.n_total_tokens += n_total_tokens
         self.n_packed_examples += self.out_size
         self._leftover_bins = leftover_bins[:self.max_leftover_bins_to_keep]
 
         # Re-pad to max_seq_len and batch
-        batch = _repad(packed_examples,
-                       max_seq_len=self.max_seq_len,
-                       pad_token_id=self.pad_token_id,
-                       padding_side=self.padding_side)
+        batch = _repad(
+            packed_examples,
+            max_seq_len=self.max_seq_len,
+            pad_token_id=self.pad_token_id,
+            padding_side=self.padding_side,
+        )
         return batch
 
 
 def _trim_batch(
-    batch: Dict[str, torch.Tensor]
+    batch: Dict[str, torch.Tensor],
 ) -> Tuple[List[int], List[Dict[str, torch.Tensor]]]:
     """Trims padding off all examples in batch.
 
     Args:
         batch (Dict[str, torch.Tensor]): Batch of padded data with tensors as values.
 
     Returns:
@@ -139,76 +155,83 @@
     trim_example = {k: v[keep] for k, v in example.items()}
     trim_example['sequence_id'] = torch.zeros_like(trim_example['input_ids'])
 
     return size, trim_example
 
 
 def _combine_in_place(
-        example: Dict[str, torch.Tensor],
-        add_on: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
+    example: Dict[str, torch.Tensor],
+    add_on: Dict[str, torch.Tensor],
+) -> Dict[str, torch.Tensor]:
     if 'labels' in add_on:
         # Prevents the last token in example from being trained to
         # predict the first token in add_on, which would make no sense.
         add_on['labels'][0] = -100
 
     for k in example.keys():
         if k == 'sequence_id':
-            example[k] = torch.cat(
-                [example[k], add_on[k] + 1 + torch.max(example[k])])
+            example[k] = torch.cat([
+                example[k],
+                add_on[k] + 1 + torch.max(example[k]),
+            ])
         else:
             example[k] = torch.cat([example[k], add_on[k]])
     return example
 
 
 def _first_fit_bin_packing(
-    sizes: List[int], examples: List[Dict[str, torch.Tensor]], num_bins: int,
-    max_bin_size: int, existing_bins: List[Tuple[int, Dict[str, torch.Tensor]]]
+    sizes: List[int],
+    examples: List[Dict[str, torch.Tensor]],
+    num_bins: int,
+    max_bin_size: int,
+    existing_bins: List[Tuple[int, Dict[str, torch.Tensor]]],
 ) -> Tuple[List[Dict[str, torch.Tensor]], int, int, List[Tuple[int, Dict[
-        str, torch.Tensor]]]]:
+    str, torch.Tensor]]]]:
 
     # Will contain tuples (bin_size_size, packed_example)
     bins: List[Tuple[int, Dict[str, torch.Tensor]]] = existing_bins
 
     starting_total_bin_sizes = sum([bin_size for bin_size, _ in bins])
 
-    sizes_and_examples = [
-        (size, example) for size, example in zip(sizes, examples)
-    ]
-    sorted_sizes_and_examples = sorted(sizes_and_examples,
-                                       key=lambda x: x[0],
-                                       reverse=True)
+    sizes_and_examples = list(zip(sizes, examples))
+    sorted_sizes_and_examples = sorted(
+        sizes_and_examples,
+        key=lambda x: x[0],
+        reverse=True,
+    )
 
     required_num_examples = max(0, num_bins - len(bins))
     num_examples = len(sizes)
     if num_examples < required_num_examples:
         for size, example in sorted_sizes_and_examples:
             # Can't keep packing. All remaining items get their own bin.
             bins.append((size, example))
 
         total_bin_sizes = sum([bin_size for bin_size, _ in bins])
         total_new_bin_sizes = total_bin_sizes - starting_total_bin_sizes
         total_example_sizes = sum(sizes)
         if total_new_bin_sizes != total_example_sizes:
             raise AssertionError(
-                f'Error in packing. {total_example_sizes=} does not equal {total_new_bin_sizes=}.'
+                f'Error in packing. {total_example_sizes=} does not equal {total_new_bin_sizes=}.',
             )
 
         sorted_bins = sorted(bins, key=lambda x: x[0], reverse=True)
         bin_sizes, packed_examples = [], []
         for bin_size, packed_example in sorted_bins:
             bin_sizes.append(bin_size)
             packed_examples.append(packed_example)
 
         # Return:
         #  - the num_bins largest packed examples
         #  - the total tokens in those examples
         #  - the total size of all new examples
         #  - leftover bins
         return packed_examples[:num_bins], sum(
-            bin_sizes[:num_bins]), sum(sizes), sorted_bins[num_bins:]
+            bin_sizes[:num_bins],
+        ), sum(sizes), sorted_bins[num_bins:]
 
     # Go through each item from longest to shortest.
     # Note: all items will either go into an existing or new bin.
     for i, (size, example) in enumerate(sorted_sizes_and_examples):
         # If we can't keep packing, all remaining items get their own bin.
         required_num_examples = max(0, num_bins - len(bins))
         n_remaining = num_examples - i
@@ -233,34 +256,39 @@
             bins.append((size, example))
 
     total_bin_sizes = sum([bin_size for bin_size, _ in bins])
     total_new_bin_sizes = total_bin_sizes - starting_total_bin_sizes
     total_example_sizes = sum(sizes)
     if total_new_bin_sizes != total_example_sizes:
         raise AssertionError(
-            f'Error in packing. {total_example_sizes=} does not equal {total_new_bin_sizes=}.'
+            f'Error in packing. {total_example_sizes=} does not equal {total_new_bin_sizes=}.',
         )
 
     sorted_bins = sorted(bins, key=lambda x: x[0], reverse=True)
     bin_sizes, packed_examples = [], []
     for bin_size, packed_example in sorted_bins:
         bin_sizes.append(bin_size)
         packed_examples.append(packed_example)
 
     # Return:
     #  - the num_bins largest packed examples
     #  - the total tokens in those examples
     #  - the total size of all new examples
     #  - leftover bins
     return packed_examples[:num_bins], sum(
-        bin_sizes[:num_bins]), sum(sizes), sorted_bins[num_bins:]
+        bin_sizes[:num_bins],
+    ), sum(sizes), sorted_bins[num_bins:]
 
 
-def _repad(packed_examples: List[Dict[str, torch.Tensor]], max_seq_len: int,
-           pad_token_id: int, padding_side: str) -> Dict[str, torch.Tensor]:
+def _repad(
+    packed_examples: List[Dict[str, torch.Tensor]],
+    max_seq_len: int,
+    pad_token_id: int,
+    padding_side: str,
+) -> Dict[str, torch.Tensor]:
 
     def pad_tensor(tensor: torch.Tensor, pad_value: int):
         if len(tensor) == max_seq_len:
             return tensor
         t = torch.full((max_seq_len,),
                        pad_value,
                        dtype=tensor.dtype,
@@ -285,18 +313,20 @@
         batch[key] = torch.stack([
             pad_tensor(example[key], pad_vals[key])
             for example in packed_examples
         ])
     return batch
 
 
-def auto_packing_ratio(dataloader_cfg: DictConfig,
-                       tokenizer: PreTrainedTokenizerBase,
-                       device_batch_size: int,
-                       num_packing_ratios: int = 20) -> float:
+def auto_packing_ratio(
+    dataloader_cfg: DictConfig,
+    tokenizer: PreTrainedTokenizerBase,
+    device_batch_size: int,
+    num_packing_ratios: int = 20,
+) -> float:
     """Find a packing ratio that minimizes padding with zero waste.
 
     By packing examples, we can increase training efficiency, training on more data with less batches.
     However, in practice, the selected packing_ratio may produce some waste because profiling is done on only
     a subset of the dataset.
 
     We select a min_ratio of 1 and a max_ratio that is the max_seq_len / 100, and profile up to
@@ -311,56 +341,67 @@
         num_packing_ratio (int): The number of packing ratios to try.
 
     Returns:
         A packing ratio that minimizes padding while maintaining zero waste.
     """
     from composer.utils import dist, get_device, reproducibility
 
+    log.debug('Searching for optimal packing ratio.')
+
     # Stash the rng state to restore later.
     rng_state = reproducibility.get_rng_state()
     # Set the seed so that auto packing is deterministic.
     reproducibility.seed_all(0)
 
     max_seq_len = dataloader_cfg.dataset.max_seq_len
     # If max_seq_len is very small, skip profiling and select packing ratio of 1.
     if max_seq_len <= 100:
         return 1
 
     min_ratio = 1
     max_ratio = max_seq_len / 100
-    profiling_results = profile_packing(dataloader_cfg, tokenizer, min_ratio,
-                                        max_ratio, num_packing_ratios,
-                                        device_batch_size)
+    profiling_results = profile_packing(
+        dataloader_cfg,
+        tokenizer,
+        min_ratio,
+        max_ratio,
+        num_packing_ratios,
+        device_batch_size,
+    )
 
     # Obtain the maximum packing_ratio/minimum padding that has no waste.
     # profiling_results are sorted from smallest to largest packing_ratio.
     packing_ratio = 1
     for packing_ratio_candidate, _, waste in profiling_results:
         if waste is None or waste > 0:
             break
         packing_ratio = packing_ratio_candidate
 
     # Select the minimum packing ratio across all ranks.
     if dist.is_available() and dist.is_initialized():
         device = get_device(None)
         packing_ratio_tensor = device.tensor_to_device(
-            torch.tensor(packing_ratio))
+            torch.tensor(packing_ratio),
+        )
         dist.all_reduce(packing_ratio_tensor, reduce_operation='MIN')
         packing_ratio = packing_ratio_tensor.item()
 
     # Restore rng state.
     reproducibility.load_rng_state(rng_state)
 
     return packing_ratio
 
 
 def profile_packing(
-    dataloader_cfg: DictConfig, tokenizer: PreTrainedTokenizerBase,
-    min_ratio: float, max_ratio: float, num_packing_ratios: int,
-    device_batch_size: int
+    dataloader_cfg: DictConfig,
+    tokenizer: PreTrainedTokenizerBase,
+    min_ratio: float,
+    max_ratio: float,
+    num_packing_ratios: int,
+    device_batch_size: int,
 ) -> Iterable[Tuple[float, Optional[float], Optional[float]]]:
     """Generator function that profiles example packing across packing ratios.
 
     Args:
         dataloader_cfg (DictConfig): The dataloader configuration for profiling.
         tokenizer (PreTrainedTokenizerBase): The tokenizer for profiling.
         min_ratio (float): Smallest packing_ratio to test. Must be >=1.
@@ -372,45 +413,68 @@
         An iterable of tuples of packing ratio, padding, and waste, sorted by smallest to largest packing ratio.
     """
     import copy
 
     from llmfoundry.data.dataloader import build_dataloader
 
     max_seq_len = dataloader_cfg.dataset.get('max_seq_len')
-    max_leftovers_to_keep = dataloader_cfg.dataset.get('max_leftovers_to_keep',
-                                                       None)
+    max_leftovers_to_keep = dataloader_cfg.dataset.get(
+        'max_leftovers_to_keep',
+        None,
+    )
 
-    # Turn off packing for the dataloader (we want raw, pre-packed examples)
+    # Turn off packing and sequence parallelism for the dataloader (we want raw, pre-packed, full-length examples)
     dataloader_cfg = copy.deepcopy(dataloader_cfg)
     dataloader_cfg.dataset.packing_ratio = 1.0
+    dataloader_cfg.dataset.auto_packing_replication = dataloader_cfg.dataset.get(
+        'seq_parallel_replication',
+        1,
+    ) or 1
+    dataloader_cfg.dataset.seq_parallel_replication = 1
     dataloader_cfg.drop_last = False
     dataloader_cfg.num_workers = 0
     dataloader_cfg.prefetch_factor = None
     dataloader_cfg.persistent_workers = False
 
     # If streaming dataset, use a temporary local folder for profiling
+    local_rank_zero = dist.get_global_rank() - dist.get_local_rank()
     if dataloader_cfg.dataset.get('remote') is not None:
-        dataloader_cfg.dataset.local = tempfile.TemporaryDirectory().name
+        tmp_path_to_broadcast = tempfile.TemporaryDirectory().name
+        gathered_paths = dist.all_gather_object(tmp_path_to_broadcast)
+        tmp_path = gathered_paths[local_rank_zero]
+        dataloader_cfg.dataset.local = tmp_path
+
+    if dataloader_cfg.dataset.get('streams') is not None:
+        for stream_config in dataloader_cfg.dataset.streams.values():
+            tmp_path_to_broadcast = tempfile.TemporaryDirectory().name
+            gathered_paths = dist.all_gather_object(tmp_path_to_broadcast)
+            tmp_path = gathered_paths[local_rank_zero]
+            stream_config.local = tmp_path
 
     # Determine the packing_ratio values we'll try
     packing_ratios, raw_batch_sizes = [], []
-    for packing_ratio in np.linspace(min_ratio,
-                                     max_ratio,
-                                     num_packing_ratios,
-                                     endpoint=True):
+    for packing_ratio in np.linspace(
+        min_ratio,
+        max_ratio,
+        num_packing_ratios,
+        endpoint=True,
+    ):
         packing_ratio = np.round(10 * packing_ratio) / 10
         raw_batch_size = int(packing_ratio * device_batch_size)
         if raw_batch_size not in raw_batch_sizes:
             packing_ratios.append(packing_ratio)
             raw_batch_sizes.append(raw_batch_size)
 
     n_profile_examples = max(raw_batch_sizes) * 100
 
-    train_dataspec = build_dataloader(dataloader_cfg, tokenizer,
-                                      n_profile_examples)
+    train_dataspec = build_dataloader(
+        dataloader_cfg,
+        tokenizer,
+        n_profile_examples,
+    )
     train_dataloader = train_dataspec.dataloader
 
     # Get a bunch of raw examples
     big_batch = next(iter(train_dataloader))
 
     # Cut everything down to size
     sizes, trimmed_examples = _trim_batch(big_batch)
@@ -422,31 +486,40 @@
         # Create the packing collator.
         packer = BinPackCollator(
             collator=lambda x: x,
             target_batch_size=device_batch_size,
             max_seq_len=max_seq_len,
             pad_token_id=0,  # <-- Doesn't need to be correct for profiling
             padding_side='left',  # <-- Doesn't need to be correct for profiling
-            max_leftover_bins_to_keep=max_leftovers_to_keep)
+            max_leftover_bins_to_keep=max_leftovers_to_keep,
+        )
 
         # Simulate feeding the packing collator a bunch of data
         for idx in range(0, len(trimmed_examples_copy), raw_batch_size):
             batch = trimmed_examples_copy[idx:idx + raw_batch_size]
             if len(batch) < device_batch_size:
                 continue
-            packer._pack_trimmed_examples(batch,
-                                          sizes[idx:idx + raw_batch_size])
+            packer._pack_trimmed_examples(
+                batch,
+                sizes[idx:idx + raw_batch_size],
+            )
 
         if packer.n_packed_examples == 0:
             log.debug(
-                'No examples packed during profiling. Dataset is smaller than device batch size.'
+                'No examples packed during profiling. Dataset is smaller than device batch size.',
             )
             return None, None
 
         # Return the padding and waste stats over that bunch of data
         padding_percent = 100 * (1 - packer.efficiency)
         waste_percent = 100 * packer.waste
         return padding_percent, waste_percent
 
-    for packing_ratio, raw_batch_size in zip(packing_ratios, raw_batch_sizes):
+    log.debug('Profiling packing ratios')
+    total_packing_ratios = min(len(packing_ratios), len(raw_batch_sizes))
+    for i, (packing_ratio,
+            raw_batch_size) in enumerate(zip(packing_ratios, raw_batch_sizes)):
+        log.debug(
+            f'Progress [{i}/{total_packing_ratios}]: Profiling packing ratio {packing_ratio}',
+        )
         padding, waste = profile(raw_batch_size)
         yield (packing_ratio, padding, waste)
```

### Comparing `llm-foundry-0.7.0/llmfoundry/data/text_data.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/text_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Build a StreamingTextDataset dataset and dataloader for training."""
 
+import inspect
 import os
 from itertools import islice
-from typing import (Any, Callable, Dict, List, Mapping, Optional, Sequence,
-                    Union, cast)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Mapping,
+    Optional,
+    Sequence,
+    Union,
+    cast,
+)
 
 import numpy as np
 import torch
-import transformers
 from composer.core.data_spec import DataSpec
-from composer.core.types import Batch
 from omegaconf import DictConfig
 from omegaconf import OmegaConf as om
 from streaming import Stream, StreamingDataset
 from torch.utils.data import DataLoader
 from transformers import PreTrainedTokenizerBase
 
+from llmfoundry import registry
+from llmfoundry.utils.registry_utils import construct_from_registry
+
+__all__ = [
+    'StreamingTextDataset',
+    'build_text_dataloader',
+    'ConcatenatedSequenceCollatorWrapper',
+]
+
 
 class StreamingTextDataset(StreamingDataset):
     """Generic text dataset using MosaicML's StreamingDataset.
 
     Args:
         tokenizer (Tokenizer): HuggingFace tokenizer to
             tokenize samples.
@@ -76,53 +92,63 @@
             Defaults to ``balanced``.
         sampling_granularity (int): When picking samples for a stream's final partial repeat,
             how many samples to pick from the same shard at a time (``1`` for evenly balanced
             across shards, ``1000`` to pick 1000 samples from the same shard at a time, etc).
             Defaults to ``1``.
         batching_method (str): Which batching method to use, either ``random``, ``stratified``, or
             ``per_stream``. Defaults to ``random``.
+        allow_unsafe_types (bool): If a shard contains Pickle, which allows arbitrary code
+            execution during deserialization, whether to keep going if ``True`` or raise an error
+            if ``False``. Defaults to ``False``.
+        replication (int, optional): Determines how many consecutive devices will receive the same
+            samples. Useful for training with tensor or sequence parallelism, where multiple
+            devices need to see the same partition of the dataset. Defaults to ``None``.
     """
 
-    def __init__(self,
-                 tokenizer: PreTrainedTokenizerBase,
-                 max_seq_len: int,
-                 streams: Optional[Sequence[Stream]] = None,
-                 remote: Optional[str] = None,
-                 local: Optional[str] = None,
-                 split: Optional[str] = None,
-                 download_retry: int = 2,
-                 download_timeout: float = 60,
-                 validate_hash: Optional[str] = None,
-                 keep_zip: bool = False,
-                 epoch_size: Optional[Union[int, str]] = None,
-                 predownload: Optional[int] = None,
-                 cache_limit: Optional[Union[int, str]] = None,
-                 partition_algo: str = 'relaxed',
-                 num_canonical_nodes: Optional[int] = None,
-                 batch_size: Optional[int] = None,
-                 shuffle: bool = False,
-                 shuffle_algo: str = 'py1e',
-                 shuffle_seed: int = 9176,
-                 shuffle_block_size: Optional[int] = None,
-                 sampling_method: str = 'balanced',
-                 sampling_granularity: int = 1,
-                 batching_method: str = 'random',
-                 **kwargs: Any):
+    def __init__(
+        self,
+        tokenizer: PreTrainedTokenizerBase,
+        max_seq_len: int,
+        streams: Optional[Sequence[Stream]] = None,
+        remote: Optional[str] = None,
+        local: Optional[str] = None,
+        split: Optional[str] = None,
+        download_retry: int = 2,
+        download_timeout: float = 60,
+        validate_hash: Optional[str] = None,
+        keep_zip: bool = False,
+        epoch_size: Optional[Union[int, str]] = None,
+        predownload: Optional[int] = None,
+        cache_limit: Optional[Union[int, str]] = None,
+        partition_algo: str = 'relaxed',
+        num_canonical_nodes: Optional[int] = None,
+        batch_size: Optional[int] = None,
+        shuffle: bool = False,
+        shuffle_algo: str = 'py1e',
+        shuffle_seed: int = 9176,
+        shuffle_block_size: Optional[int] = None,
+        sampling_method: str = 'balanced',
+        sampling_granularity: int = 1,
+        batching_method: str = 'random',
+        allow_unsafe_types: bool = False,
+        replication: Optional[int] = None,
+        **kwargs: Any,
+    ):
 
         if len(kwargs) > 0:
             raise ValueError(
-                f'StreamingTextDataset() got an unexpected keyword argument: {kwargs}'
+                f'StreamingTextDataset() got an unexpected keyword argument: {kwargs}',
             )
 
         if local is not None and (remote is None or (local == remote)):
             if os.path.isdir(local):
                 contents = set(os.listdir(local))
                 if split not in contents:
                     raise ValueError(
-                        f'local directory {local} does not contain split {split}'
+                        f'local directory {local} does not contain split {split}',
                     )
 
         # TODO: discover where yamls are being converted incorrect, but temporary workaround
         if isinstance(shuffle_block_size, float):
             shuffle_block_size = int(shuffle_block_size)
 
         # Build Dataset
@@ -144,47 +170,55 @@
             shuffle=shuffle,
             shuffle_algo=shuffle_algo,
             shuffle_seed=shuffle_seed,
             shuffle_block_size=shuffle_block_size,
             sampling_method=sampling_method,
             sampling_granularity=sampling_granularity,
             batching_method=batching_method,
+            allow_unsafe_types=allow_unsafe_types,
+            replication=replication,
         )
         self.tokenizer = tokenizer
         self.max_seq_len = max_seq_len
 
     # How to tokenize a text sample to a token sample
-    def _tokenize(self, text_sample: Mapping) -> Dict[str, List[int]]:
+    def _tokenize(self, text_sample: Mapping) -> Dict[str, list[int]]:
         if self.tokenizer._pad_token is None:
             # Some tokenizers (e.g. GPT2 tokenizer) have no padding token which causes bugs
             raise RuntimeError(
-                'If tokenizing on-the-fly, tokenizer must have a pad_token_id')
+                'If tokenizing on-the-fly, tokenizer must have a pad_token_id',
+            )
 
-        return self.tokenizer(text_sample['text'],
-                              truncation=True,
-                              padding='max_length',
-                              max_length=self.max_seq_len)
+        return self.tokenizer(
+            text_sample['text'],
+            truncation=True,
+            padding='max_length',
+            max_length=self.max_seq_len,
+        )
 
-    def _read_binary_tokenized_sample(self, sample: Dict[str,
-                                                         Any]) -> torch.Tensor:
+    def _read_binary_tokenized_sample(
+        self,
+        sample: Dict[str, Any],
+    ) -> torch.Tensor:
         return torch.from_numpy(
             np.frombuffer(sample['tokens'],
-                          dtype=np.int64)[:self.max_seq_len].copy())
+                          dtype=np.int64)[:self.max_seq_len].copy(),
+        )
 
     # How to process a sample
     def __getitem__(self,
-                    idx: int) -> Union[Dict[str, List[int]], torch.Tensor]:
+                    idx: int) -> Union[Dict[str, list[int]], torch.Tensor]:
         sample = super().__getitem__(idx)
         if 'text' in sample:
             token_sample = self._tokenize(sample)
         elif 'tokens' in sample:
             token_sample = self._read_binary_tokenized_sample(sample)
         else:
             raise RuntimeError(
-                'StreamingTextDataset needs samples to have a `text` or `tokens` column'
+                'StreamingTextDataset needs samples to have a `text` or `tokens` column',
             )
         return token_sample
 
 
 class ConcatenatedSequenceCollatorWrapper:
     """Collator wrapper to add sequence_id to batch."""
 
@@ -193,37 +227,39 @@
         base_collator: Callable,
         eos_token_id: Optional[int] = None,
         bos_token_id: Optional[int] = None,
     ):
         self.base_collator = base_collator
         if (eos_token_id is None) and (bos_token_id is None):
             raise ValueError(
-                'Must supply a value for either eos_token_id or bos_token_id, but got None for both.'
+                'Must supply a value for either eos_token_id or bos_token_id, but got None for both.',
             )
         if (eos_token_id is not None) and (bos_token_id is not None):
             raise ValueError(
                 'Cannot use *both* EOS and BOS tokens for detecting sequence boundaries. ' +\
                 'Please supply `eos_token_id` if sequences end with an EOS token, or use ' +\
-                '`bos_token_id` if sequences start with a BOS token.'
+                '`bos_token_id` if sequences start with a BOS token.',
             )
 
         if eos_token_id is None:
             self.split_token_id = cast(int, bos_token_id)
             self.bos_mode = True
         else:
             self.split_token_id = eos_token_id
             self.bos_mode = False
 
-    def __call__(self, examples: List[Any]) -> Dict[str, torch.Tensor]:
+    def __call__(self, examples: list[Any]) -> Dict[str, torch.Tensor]:
         batch = self.base_collator(examples)
         batch['sequence_id'] = self.get_sequence_id_from_batch(batch)
         return batch
 
     def get_sequence_id_from_batch(
-            self, batch: Dict[str, torch.Tensor]) -> torch.Tensor:
+        self,
+        batch: Dict[str, torch.Tensor],
+    ) -> torch.Tensor:
         is_separator = torch.eq(batch['input_ids'], self.split_token_id)
         cumulative_sep = torch.cumsum(is_separator,
                                       dim=1).to(batch['input_ids'].dtype)
         # If separator token is bos, we're already done
         if self.bos_mode:
             return cumulative_sep
 
@@ -234,156 +270,138 @@
 
 def build_streams(dataset_cfg: DictConfig):
     streams_dict = dataset_cfg.pop('streams', None)
     # build streams
     streams = None
     if streams_dict is not None:
         streams = []
-        for _, stream in streams_dict.items():
+        for stream in streams_dict.values():
             # stream is the streams kwargs
             # fwd all kwargs with **stream allows streaming to check args
             streams.append(Stream(**stream))
     return streams
 
 
 def build_text_dataloader(
     cfg: DictConfig,
     tokenizer: PreTrainedTokenizerBase,
-    device_batch_size: int,
+    device_batch_size: Union[int, float],
 ) -> DataSpec:
     assert cfg.name == 'text', f'Tried to build text dataloader with cfg.name={cfg.name}'
 
     # get kwargs
-    mlm_probability = cfg.dataset.pop('mlm_probability', None)
-    eos_token_id = cfg.dataset.pop('eos_token_id', None)
-    bos_token_id = cfg.dataset.pop('bos_token_id', None)
+    cfg.dataset['replication'], dataset_batch_size = construct_from_registry(
+        name='dataset_replication_validator',
+        registry=registry.dataset_replication_validators,
+        partial_function=False,
+        kwargs={
+            'cfg': cfg,
+            'tokenizer': tokenizer,
+            'device_batch_size': device_batch_size,
+        },
+    )
 
     streams = build_streams(cfg.dataset)
 
+    valid_streaming_text_dataset_parameters = inspect.signature(
+        StreamingTextDataset,
+    ).parameters
+
+    dataset_config_subset_for_streaming_text_dataset = {
+        k: v
+        for k, v in cfg.dataset.items()
+        if k in valid_streaming_text_dataset_parameters
+    }
+
     # build dataset potentially with streams
     dataset = StreamingTextDataset(
         tokenizer=tokenizer,
         streams=streams,
-        batch_size=device_batch_size,
-        **cfg.dataset,
+        batch_size=dataset_batch_size,
+        **dataset_config_subset_for_streaming_text_dataset,
     )
 
-    collate_fn = transformers.DataCollatorForLanguageModeling(
-        tokenizer=dataset.tokenizer,
-        mlm=mlm_probability is not None,
-        mlm_probability=mlm_probability)
-
-    if (eos_token_id is not None) or (bos_token_id is not None):
-        # Note: Will raise an error if both are non-None
-        collate_fn = ConcatenatedSequenceCollatorWrapper(
-            base_collator=collate_fn,
-            eos_token_id=eos_token_id,
-            bos_token_id=bos_token_id)
+    collate_fn, dataloader_batch_size = construct_from_registry(
+        name='text_collator',
+        registry=registry.collators,
+        partial_function=False,
+        kwargs={
+            'cfg': cfg,
+            'tokenizer': dataset.tokenizer,
+            'dataset_batch_size': dataset_batch_size,
+        },
+    )
 
     dl = DataLoader(
         dataset,
         collate_fn=collate_fn,
-        batch_size=device_batch_size,
+        batch_size=dataloader_batch_size,
         drop_last=cfg.drop_last,
         num_workers=cfg.num_workers,
         pin_memory=cfg.get('pin_memory', True),
         prefetch_factor=cfg.get('prefetch_factor', 2),
         persistent_workers=cfg.get('persistent_workers', True),
         timeout=cfg.get('timeout', 0),
     )
 
-    # If we pretokenized, we may not have padding, in which case the
-    # tokenizer may not have a pad_token_id. In this case, we can
-    # just use the default token counting function. This is correct
-    # because we do not support training on pretokenized data with padding,
-    # and if tokenizing on the fly, we require that the tokenizer has a pad token.
-    token_counting_func = None
-    if tokenizer.pad_token_id is not None:
-        token_counting_func = get_tokens_per_batch_func()
-
-    return DataSpec(dataloader=dl, get_num_tokens_in_batch=token_counting_func)
-
-
-def get_tokens_per_batch_func(
-        decoder_only: bool = True) -> Callable[[Batch], int]:
-    """Returns a callable that counts the number of tokens in a batch.
-
-    Args:
-        pad_token_id (int): The id of the padding token.
-        decoder_only (bool, optional): Whether to expect the batch to just contain ``input_ids`` (decoder only)
-            or to also contain ``decoder_input_ids`` (encoder decoder). Defaults to ``True``.
-
-    Returns:
-        Callable[[Batch], int]: A callable that counts the number of tokens in a batch.
-    """
-
-    def get_num_samples_in_batch(batch: Batch) -> int:
-        if not isinstance(batch, Mapping) or ('attention_mask' not in batch and
-                                              'input_ids' not in batch):
-            raise ValueError(
-                'get_tokens_per_batch_func() requires a batch with an attention_mask key or an input_ids key'
-            )
-
-        if not decoder_only and 'decoder_attention_mask' not in batch:
-            raise ValueError(
-                'get_tokens_per_batch_func() for encoder decoder requires a batch with a decoder_attention_mask key'
-            )
-
-        # Count number of non padding tokens in batch
-        if 'attention_mask' in batch:
-            input_ids_tokens = int(torch.sum(batch['attention_mask']).item())
-        else:
-            input_ids_tokens = batch['input_ids'].numel()
-
-        # For encoder decoder models only
-        decoder_input_ids_tokens = 0
-        if not decoder_only:
-            decoder_input_ids_tokens = int(
-                torch.sum(batch['decoder_attention_mask']).item())
-
-        return input_ids_tokens + decoder_input_ids_tokens
-
-    return get_num_samples_in_batch
+    return construct_from_registry(
+        name='data_spec',
+        registry=registry.data_specs,
+        partial_function=False,
+        kwargs={
+            'dl': dl,
+            'dataset_cfg': cfg.dataset,
+        },
+    )
 
 
 # Helpful to test if your dataloader is working locally
 # Run `python data.py  --local_path [local] [--remote_path remote, optional]` and verify that batches are printed out
 if __name__ == '__main__':
     import argparse
 
     from llmfoundry.utils.builders import build_tokenizer
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('--tokenizer',
-                        type=str,
-                        default='EleutherAI/gpt-neox-20b',
-                        help='the name of the tokenizer to use')
-    parser.add_argument('--local_path',
-                        type=str,
-                        required=True,
-                        help='the path to the local copy of the dataset')
+    parser.add_argument(
+        '--tokenizer',
+        type=str,
+        default='EleutherAI/gpt-neox-20b',
+        help='the name of the tokenizer to use',
+    )
+    parser.add_argument(
+        '--local_path',
+        type=str,
+        required=True,
+        help='the path to the local copy of the dataset',
+    )
     parser.add_argument(
         '--remote_path',
         type=str,
         default=None,
-        help='the path to the remote copy to stream from (optional)')
-    parser.add_argument('--split',
-                        type=str,
-                        default='val',
-                        help='which split of the dataset to use')
-    parser.add_argument('--max_seq_len',
-                        type=int,
-                        default=32,
-                        help='max sequence length to test')
+        help='the path to the remote copy to stream from (optional)',
+    )
+    parser.add_argument(
+        '--split',
+        type=str,
+        default='val',
+        help='which split of the dataset to use',
+    )
+    parser.add_argument(
+        '--max_seq_len',
+        type=int,
+        default=32,
+        help='max sequence length to test',
+    )
 
     args = parser.parse_args()
 
     if args.remote_path is not None:
         print(
-            f'Reading {args.split} split from {args.local_path} <- streamed from <- {args.remote_path}'
+            f'Reading {args.split} split from {args.local_path} <- streamed from <- {args.remote_path}',
         )
     else:
         print(f'Reading {args.split} split from {args.local_path}')
 
     cfg = {
         'name': 'text',
         'dataset': {
```

### Comparing `llm-foundry-0.7.0/llmfoundry/loggers/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/loggers/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Copyright 2024 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
-from composer.loggers import (InMemoryLogger, MLFlowLogger, TensorboardLogger,
-                              WandBLogger)
+from composer.loggers import (
+    InMemoryLogger,
+    MLFlowLogger,
+    TensorboardLogger,
+    WandBLogger,
+)
 
 from llmfoundry.registry import loggers
 
 loggers.register('wandb', func=WandBLogger)
 loggers.register('tensorboard', func=TensorboardLogger)
 loggers.register('inmemory', func=InMemoryLogger)
-loggers.register('in_memory_logger',
-                 func=InMemoryLogger)  # for backwards compatibility
+loggers.register(
+    'in_memory_logger',
+    func=InMemoryLogger,
+)  # for backwards compatibility
 loggers.register('mlflow', func=MLFlowLogger)
```

### Comparing `llm-foundry-0.7.0/llmfoundry/metrics/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/metrics/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 # Copyright 2024 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
-from composer.metrics import (InContextLearningCodeEvalAccuracy,
-                              InContextLearningLMAccuracy,
-                              InContextLearningLMExpectedCalibrationError,
-                              InContextLearningMCExpectedCalibrationError,
-                              InContextLearningMultipleChoiceAccuracy,
-                              InContextLearningQAAccuracy, MaskedAccuracy)
-from composer.metrics.nlp import LanguageCrossEntropy, LanguagePerplexity
-
+from composer.metrics import (
+    LanguageCrossEntropy,
+    LanguagePerplexity,
+    MaskedAccuracy,
+)
+
+from llmfoundry.eval.metrics import (
+    InContextLearningGenerationExactMatchAccuracy,
+    InContextLearningLMAccuracy,
+    InContextLearningLMExpectedCalibrationError,
+    InContextLearningMCExpectedCalibrationError,
+    InContextLearningMultipleChoiceAccuracy,
+)
 from llmfoundry.metrics.token_acc import TokenAccuracy
 from llmfoundry.registry import metrics
 
 metrics.register('token_accuracy', func=TokenAccuracy)
 metrics.register('lm_accuracy', func=InContextLearningLMAccuracy)
-metrics.register('lm_expected_calibration_error',
-                 func=InContextLearningLMExpectedCalibrationError)
-metrics.register('mc_expected_calibration_error',
-                 func=InContextLearningMCExpectedCalibrationError)
+metrics.register(
+    'lm_expected_calibration_error',
+    func=InContextLearningLMExpectedCalibrationError,
+)
+metrics.register(
+    'mc_expected_calibration_error',
+    func=InContextLearningMCExpectedCalibrationError,
+)
 metrics.register('mc_accuracy', func=InContextLearningMultipleChoiceAccuracy)
-metrics.register('qa_accuracy', func=InContextLearningQAAccuracy)
-metrics.register('code_eval_accuracy', func=InContextLearningCodeEvalAccuracy)
+metrics.register(
+    'qa_accuracy',
+    func=InContextLearningGenerationExactMatchAccuracy,
+)
 metrics.register('language_cross_entropy', func=LanguageCrossEntropy)
 metrics.register('language_perplexity', func=LanguagePerplexity)
 metrics.register('masked_accuracy', func=MaskedAccuracy)
 
 DEFAULT_CAUSAL_LM_TRAIN_METRICS = [
     'language_cross_entropy',
     'language_perplexity',
@@ -36,30 +47,25 @@
     'language_perplexity',
     'token_accuracy',
     'lm_accuracy',
     'lm_expected_calibration_error',
     'mc_expected_calibration_error',
     'mc_accuracy',
     'qa_accuracy',
-    'code_eval_accuracy',
 ]
 
 DEFAULT_ENC_DEC_METRICS = [
     'language_cross_entropy',
     'masked_accuracy',
 ]
 
 __all__ = [
     'TokenAccuracy',
     'InContextLearningLMAccuracy',
     'InContextLearningLMExpectedCalibrationError',
     'InContextLearningMCExpectedCalibrationError',
     'InContextLearningMultipleChoiceAccuracy',
-    'InContextLearningQAAccuracy',
-    'InContextLearningCodeEvalAccuracy',
-    'LanguageCrossEntropy',
-    'LanguagePerplexity',
-    'MaskedAccuracy',
+    'InContextLearningGenerationExactMatchAccuracy',
     'DEFAULT_CAUSAL_LM_TRAIN_METRICS',
     'DEFAULT_CAUSAL_LM_EVAL_METRICS',
     'DEFAULT_ENC_DEC_METRICS',
 ]
```

### Comparing `llm-foundry-0.7.0/llmfoundry/metrics/token_acc.py` & `llm-foundry-0.9.0.dev0/llmfoundry/metrics/token_acc.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,25 +21,31 @@
         dist_sync_on_step (bool, optional): Synchronize metric state across processes at
             each forward() before returning the value at the step. Default: False.
     """
 
     # Ensures torchmetrics calls update only once
     full_state_update = False
 
-    def __init__(self,
-                 ignore_index: int = -100,
-                 dist_sync_on_step: bool = False):
+    def __init__(
+        self,
+        ignore_index: int = -100,
+        dist_sync_on_step: bool = False,
+    ):
         super().__init__(dist_sync_on_step=dist_sync_on_step)
         self.ignore_index = ignore_index
-        self.add_state('correct_tokens',
-                       default=torch.tensor(0),
-                       dist_reduce_fx='sum')
-        self.add_state('total_tokens',
-                       default=torch.tensor(0),
-                       dist_reduce_fx='sum')
+        self.add_state(
+            'correct_tokens',
+            default=torch.tensor(0),
+            dist_reduce_fx='sum',
+        )
+        self.add_state(
+            'total_tokens',
+            default=torch.tensor(0),
+            dist_reduce_fx='sum',
+        )
 
     def update(self, preds: torch.Tensor, target: torch.Tensor):
         """Updates the internal state with results from a new batch.
 
         Args:
             preds (~torch.Tensor): The predictions from the model, a Tensor of logits.
             target (~torch.Tensor): A Tensor of ground-truth token values.
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 from llmfoundry.models.hf import ComposerHFCausalLM, ComposerHFT5
-from llmfoundry.models.inference_api_wrapper import (FMAPICasualLMEvalWrapper,
-                                                     FMAPIChatAPIEvalWrapper,
-                                                     OpenAICausalLMEvalWrapper,
-                                                     OpenAIChatAPIEvalWrapper)
-from llmfoundry.models.mpt import (ComposerMPTCausalLM, MPTConfig,
-                                   MPTForCausalLM, MPTModel, MPTPreTrainedModel)
+from llmfoundry.models.inference_api_wrapper import (
+    FMAPICasualLMEvalWrapper,
+    FMAPIChatAPIEvalWrapper,
+    OpenAICausalLMEvalWrapper,
+    OpenAIChatAPIEvalWrapper,
+)
+from llmfoundry.models.mpt import (
+    ComposerMPTCausalLM,
+    MPTConfig,
+    MPTForCausalLM,
+    MPTModel,
+    MPTPreTrainedModel,
+)
 from llmfoundry.registry import models
 
 models.register('mpt_causal_lm', func=ComposerMPTCausalLM)
 models.register('hf_causal_lm', func=ComposerHFCausalLM)
 models.register('hf_t5', func=ComposerHFT5)
 models.register('openai_causal_lm', func=OpenAICausalLMEvalWrapper)
 models.register('fmapi_causal_lm', func=FMAPICasualLMEvalWrapper)
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/hf/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/hf/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 from llmfoundry.models.hf.hf_causal_lm import ComposerHFCausalLM
-from llmfoundry.models.hf.hf_fsdp import (prepare_hf_causal_lm_model_for_fsdp,
-                                          prepare_hf_enc_dec_model_for_fsdp,
-                                          prepare_hf_model_for_fsdp)
+from llmfoundry.models.hf.hf_fsdp import (
+    prepare_hf_causal_lm_model_for_fsdp,
+    prepare_hf_enc_dec_model_for_fsdp,
+    prepare_hf_model_for_fsdp,
+)
 from llmfoundry.models.hf.hf_t5 import ComposerHFT5
+from llmfoundry.models.hf.model_wrapper import HuggingFaceModelWithFSDP
 
 __all__ = [
     'ComposerHFCausalLM',
     'ComposerHFT5',
     'prepare_hf_causal_lm_model_for_fsdp',
     'prepare_hf_enc_dec_model_for_fsdp',
     'prepare_hf_model_for_fsdp',
+    'HuggingFaceModelWithFSDP',
 ]
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/hf/hf_causal_lm.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/hf/hf_causal_lm.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,32 +2,40 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """Implements a Hugging Causal LM wrapped inside a :class:`.ComposerModel`."""
 
 import logging
 import os
 import warnings
-from typing import TYPE_CHECKING, Any, Dict, Mapping
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Tuple, Union
 
 from composer.models.huggingface import peft_installed
 from composer.utils import dist
 from omegaconf import DictConfig
-from transformers import (AutoConfig, AutoModelForCausalLM, PreTrainedModel,
-                          PreTrainedTokenizerBase)
-
-from llmfoundry.metrics import (DEFAULT_CAUSAL_LM_EVAL_METRICS,
-                                DEFAULT_CAUSAL_LM_TRAIN_METRICS)
+from torchmetrics import Metric
+from transformers import (
+    AutoConfig,
+    AutoModelForCausalLM,
+    PretrainedConfig,
+    PreTrainedModel,
+    PreTrainedTokenizerBase,
+)
+
+from llmfoundry.metrics import (
+    DEFAULT_CAUSAL_LM_EVAL_METRICS,
+    DEFAULT_CAUSAL_LM_TRAIN_METRICS,
+)
 from llmfoundry.models.hf.hf_fsdp import hf_get_init_device
 from llmfoundry.models.hf.model_wrapper import HuggingFaceModelWithFSDP
 from llmfoundry.models.layers.attention import is_flash_v2_installed
 from llmfoundry.models.utils import init_empty_weights
-from llmfoundry.utils.config_utils import pop_config
+from llmfoundry.utils.config_utils import get_hf_config_value, pop_config
 
 if TYPE_CHECKING:
-    from peft import PeftConfig
+    from peft import PeftConfig, PeftModel
 
 __all__ = ['ComposerHFCausalLM']
 
 log = logging.getLogger(__name__)
 
 
 class ComposerHFCausalLM(HuggingFaceModelWithFSDP):
@@ -55,70 +63,130 @@
             cfg.use_train_metrics (bool, optional): Whether to use training metrics. Default: ``True``.
             cfg.load_in_8bit (bool, optional): Whether to load the model in 8-bit mode. Default: ``False``.
             cfg.init_device (str, optional): Which device to initialize the model on. Default: ``'cpu'``.
             cfg.use_flash_attention_2 (bool, optional): Whether to use flash-attention 2. Default: ``False``.
         tokenizer (PreTrainedTokenizer): The tokenizer that the model will use.
     """
 
-    def __init__(self, om_model_config: DictConfig,
-                 tokenizer: PreTrainedTokenizerBase):
+    def __init__(
+        self,
+        om_model_config: DictConfig,
+        tokenizer: PreTrainedTokenizerBase,
+    ):
+        model = ComposerHFCausalLM.build_inner_model(om_model_config)
+
+        train_metrics, eval_metrics = ComposerHFCausalLM.build_metrics(
+            om_model_config,
+        )
+
+        peft_config_dict = pop_config(
+            om_model_config,
+            'peft_config',
+            must_exist=False,
+            convert=True,
+        )
+        if peft_config_dict is not None and not peft_installed:
+            raise ValueError(
+                'PEFT is not installed, but peft_config was passed. Please install LLM Foundry with the peft extra to use peft_config.',
+            )
+
+        peft_config = None
+        if peft_config_dict is not None:
+            peft_config = self._get_peft_config(peft_config_dict)
+
+        # Set up config args for the model construction and base classes
+        init_device = om_model_config.get('init_device', 'cpu')
+
+        super().__init__(
+            model=model,
+            shift_labels=True,
+            tokenizer=tokenizer,
+            metrics=train_metrics,
+            eval_metrics=eval_metrics,
+            init_device=init_device,
+            peft_config=peft_config,
+        )
+
+    @staticmethod
+    def build_metrics(
+        om_model_config: DictConfig,
+    ) -> Tuple[List[Metric], List[Metric]]:
+        """Builds the training and evaluation metrics for the model.
+
+        Args:
+            om_model_config (DictConfig): The model configuration. See `__init__` for details on allowed keys.
+        """
         from llmfoundry.utils.builders import build_metric
 
+        use_train_metrics = om_model_config.get('use_train_metrics', True)
+        train_metric_names = DEFAULT_CAUSAL_LM_TRAIN_METRICS + om_model_config.get(
+            'additional_train_metrics',
+            [],
+        )
+        train_metrics = [
+            build_metric(metric, {}) for metric in train_metric_names
+        ] if use_train_metrics else []
+        eval_metric_names = DEFAULT_CAUSAL_LM_EVAL_METRICS + om_model_config.get(
+            'additional_eval_metrics',
+            [],
+        )
+        eval_metrics = [
+            build_metric(metric, {}) for metric in eval_metric_names
+        ]
+
+        return train_metrics, eval_metrics
+
+    @staticmethod
+    def build_inner_model(
+        om_model_config: DictConfig,
+        prepare_for_fsdp: bool = False,
+    ) -> Union[PreTrainedModel, 'PeftModel']:
+        """Builds the inner model for the ComposerHFCausalLM.
+
+        Args:
+            om_model_config (DictConfig): The model configuration. See `__init__` for details on allowed keys.
+            prepare_for_fsdp (bool): Whether to prepare the model for FSDP wrapping. Default: ``False``.
+        """
         pretrained_model_name_or_path = om_model_config.pretrained_model_name_or_path
         pretrained_lora_id_or_path = om_model_config.get(
-            'pretrained_lora_id_or_path', None)
+            'pretrained_lora_id_or_path',
+            None,
+        )
 
         if not om_model_config.get(
-                'trust_remote_code', True
+            'trust_remote_code',
+            True,
         ) and pretrained_model_name_or_path.startswith('mosaicml/mpt'):
             raise ValueError(
                 'trust_remote_code must be set to True for MPT models. Without this, the MPT model code will come from the transformers library, '
                 +
-                'which is significantly slower and not compatible with the LLM foundry training code, rather than the code release by MosaicML.'
+                'which is significantly slower and not compatible with the LLM foundry training code, rather than the code release by MosaicML.',
             )
 
         # Set up Hugging Face args
         trust_remote_code = om_model_config.get('trust_remote_code', True)
         use_auth_token = om_model_config.get('use_auth_token', False)
-        use_flash_attention_2 = om_model_config.get('use_flash_attention_2',
-                                                    False)
+        use_flash_attention_2 = om_model_config.get(
+            'use_flash_attention_2',
+            False,
+        )
         load_in_8bit = om_model_config.get('load_in_8bit', False)
 
         # Set up config args for the model construction and base classes
         init_device = om_model_config.get('init_device', 'cpu')
         # Resolve "mixed" init device to either "cpu" or "meta"
         resolved_init_device = hf_get_init_device(init_device)
         requested_attention_implementation = 'flash_attention_2' if use_flash_attention_2 else 'eager'
 
         if use_flash_attention_2 and not is_flash_v2_installed():
             raise ValueError(
                 'use_flash_attention_2 is set to True, but flash-attention 2 is not installed. '
-                + 'Please `pip install llm-foundry[gpu]`.')
-
-        peft_config_dict = pop_config(om_model_config,
-                                      'peft_config',
-                                      must_exist=False,
-                                      convert=True)
-        if peft_config_dict is not None and not peft_installed:
-            raise ValueError(
-                'PEFT is not installed, but peft_config was passed. Please install LLM Foundry with the peft extra to use peft_config.'
+                + 'Please `pip install llm-foundry[gpu]`.',
             )
 
-        use_train_metrics = om_model_config.get('use_train_metrics', True)
-        train_metric_names = DEFAULT_CAUSAL_LM_TRAIN_METRICS + om_model_config.get(
-            'additional_train_metrics', [])
-        train_metrics = [
-            build_metric(metric, {}) for metric in train_metric_names
-        ] if use_train_metrics else []
-        eval_metric_names = DEFAULT_CAUSAL_LM_EVAL_METRICS + om_model_config.get(
-            'additional_eval_metrics', [])
-        eval_metrics = [
-            build_metric(metric, {}) for metric in eval_metric_names
-        ]
-
         # Construct the Hugging Face config to use
         config = AutoConfig.from_pretrained(
             pretrained_model_name_or_path,
             trust_remote_code=trust_remote_code,
             use_auth_token=use_auth_token,
             attn_implementation=requested_attention_implementation,
             use_cache=
@@ -126,59 +194,82 @@
         )
 
         # This is not ideal, however Hugging Face's _autoset_attn_implementation function
         # forces you to load the model in fp16/bf16 if you want to use flash attention. Rather than loading
         # the model and then casting it back to fp32, we are monkeypatching their check.
         # https://github.com/huggingface/transformers/issues/28052
         def _autoset_attn_implementation_monkeypatch(
-                cls,  # type: ignore
-                config,  # type: ignore
-                *args,  # type: ignore
-                **kwargs):  # type: ignore
+            cls,  # type: ignore
+            config,  # type: ignore
+            *args,  # type: ignore
+            **kwargs,  # type: ignore
+        ):  # type: ignore
             config._attn_implementation = requested_attention_implementation
             return config
 
         PreTrainedModel._autoset_attn_implementation = classmethod(
-            _autoset_attn_implementation_monkeypatch)
+            _autoset_attn_implementation_monkeypatch,
+        )
 
         # set config overrides
         for k, v in om_model_config.get('config_overrides', {}).items():
             if not hasattr(config, k):
                 raise ValueError(
-                    f'config does not have attribute "{k}" to override ({k}: {v}).'
+                    f'config does not have attribute "{k}" to override ({k}: {v}).',
                 )
 
             attr = getattr(config, k)
             # attempt to disallow typos in nested configs
             if isinstance(attr, Mapping):
                 extra_keys = [_k for _k in v.keys() if _k not in attr.keys()]
                 if extra_keys:
                     raise ValueError(
                         f'Config dict override got unknown keys. ' +
                         f'Extra keys: {extra_keys}. ' +
-                        f'Expected (a subset of) keys: {list(attr.keys())}.')
+                        f'Expected (a subset of) keys: {list(attr.keys())}.',
+                    )
                 getattr(config, k).update(v)
             # necessary case to allow for rope_scaling to be overriden in llama config
             elif attr is None and isinstance(v, Mapping):
                 setattr(config, k, {})
                 getattr(config, k).update(v)
+            elif isinstance(attr, PretrainedConfig):
+                if not isinstance(v, Mapping):
+                    raise ValueError(
+                        f'Expected a dictionary for config override {k}, but got {v}.',
+                    )
+
+                for _k, _v in v.items():
+                    if not hasattr(attr, _k):
+                        raise ValueError(
+                            f'config does not have attribute "{_k}" to override ({k}: {_k}: {_v}).',
+                        )
+                    setattr(attr, _k, _v)
             else:
                 setattr(config, k, v)
 
+        if hasattr(config, 'attn_config') and get_hf_config_value(
+            config.attn_config,
+            'seq_parallel_world_size',
+        ) is not None:
+            raise NotImplementedError(
+                'Sequence Parallelism is not supported for HuggingFace models.',
+            )
+
         # We need to have all non-zero local ranks be not-pretrained
         # Rank 0 will still be pretrained, and distribute the weights appropriately
         if dist.get_local_rank() != 0 and init_device == 'mixed':
             om_model_config.pretrained = False
 
         # If the HuggingFace model is coming from a local folder, Hugging Face copies the modules into the
         # transformers modules cache. On particular systems, this operation seems to cause contention between
         # the different processes. To avoid this contention, we first create the model (on meta device) on local rank
         # zero. This will set up the transformers model cache and avoid the future contention.
-        if dist.get_local_rank() == 0 and os.path.isdir(
-                pretrained_model_name_or_path):
+        if dist.get_local_rank(
+        ) == 0 and os.path.isdir(pretrained_model_name_or_path):
             with init_empty_weights(include_buffers=False):
                 with warnings.catch_warnings():
                     warnings.simplefilter('ignore', UserWarning)
                     AutoModelForCausalLM.from_pretrained(
                         pretrained_model_name_or_path,
                         trust_remote_code=trust_remote_code,
                         use_auth_token=use_auth_token,
@@ -201,24 +292,25 @@
                 model = AutoModelForCausalLM.from_config(
                     config,
                     trust_remote_code=trust_remote_code,
                 )
         elif resolved_init_device == 'meta':
             if om_model_config.pretrained:
                 raise ValueError(
-                    'Setting cfg.pretrained=True is not supported when init_device="meta".'
+                    'Setting cfg.pretrained=True is not supported when init_device="meta".',
                 )
             with init_empty_weights(include_buffers=False):
                 model = AutoModelForCausalLM.from_config(
                     config,
                     trust_remote_code=trust_remote_code,
                 )
         else:
             raise ValueError(
-                f'init_device="{init_device}" must be either "cpu" or "meta".')
+                f'init_device="{init_device}" must be either "cpu" or "meta".',
+            )
 
         signal_file_path = f'.node_{dist.get_node_rank()}_local_rank0_completed'
         if dist.get_local_rank() == 0:
             with open(signal_file_path, 'wb') as f:
                 f.write(b'local_rank0_completed_download')
 
         # Avoid the collective call until the local rank zero has finished trying to download the checkpoint
@@ -231,49 +323,41 @@
             os.remove(signal_file_path)
 
         # Hugging Face's weight tying does not succeed if the model is inited on meta device
         # so we manually apply the weight tying here
         if model.config.tie_word_embeddings and resolved_init_device == 'meta':
             model.tie_weights()
 
-        peft_config = None
-        if peft_config_dict is not None:
-            peft_config = self._get_peft_config(peft_config_dict)
-
         if pretrained_lora_id_or_path is not None:
             if not peft_installed:
                 raise ValueError(
-                    'PEFT is not installed, but lora_id_or_path was passed. Please install LLM Foundry with the peft extra to use lora_id_or_path.'
+                    'PEFT is not installed, but lora_id_or_path was passed. Please install LLM Foundry with the peft extra to use lora_id_or_path.',
                 )
             from peft import PeftModelForCausalLM
             model = PeftModelForCausalLM.from_pretrained(
-                model, pretrained_lora_id_or_path)
+                model,
+                pretrained_lora_id_or_path,
+            )
 
-        super().__init__(
-            model=model,
-            shift_labels=True,
-            tokenizer=tokenizer,
-            metrics=train_metrics,
-            eval_metrics=eval_metrics,
-            init_device=init_device,
-            peft_config=peft_config,
-        )
+        if prepare_for_fsdp:
+            ComposerHFCausalLM.prepare_inner_model(model, init_device)
+        return model
 
     @staticmethod
     def _get_peft_config(peft_config_dict: Dict[str, Any]) -> 'PeftConfig':
         if peft_installed:
             from peft import LoraConfig
             peft_type = peft_config_dict.get('peft_type', '')
             if peft_type.upper() != 'LORA':
                 raise ValueError(
-                    f'Only LORA is supported for peft_type, but got {peft_type}.'
+                    f'Only LORA is supported for peft_type, but got {peft_type}.',
                 )
             task_type = peft_config_dict.get('task_type', '')
             if task_type.upper() != 'CAUSAL_LM':
                 raise ValueError(
-                    f'Only CAUSAL_LM is supported for task_type, but got {task_type}.'
+                    f'Only CAUSAL_LM is supported for task_type, but got {task_type}.',
                 )
             return LoraConfig(**peft_config_dict)
         else:
             raise ValueError(
-                'PEFT is not installed, but peft_config was passed. Please install LLM Foundry with the peft extra to use peft_config.'
+                'PEFT is not installed, but peft_config was passed. Please install LLM Foundry with the peft extra to use peft_config.',
             )
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/hf/hf_fsdp.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/hf/hf_fsdp.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 from composer.models.huggingface import maybe_get_underlying_model
 from transformers import PreTrainedModel
 from transformers.models.opt.modeling_opt import OPTDecoder
 
 if TYPE_CHECKING:
     from peft import PeftModel
 
+__all__ = [
+    'prepare_hf_model_for_fsdp',
+    'prepare_hf_causal_lm_model_for_fsdp',
+    'prepare_hf_enc_dec_model_for_fsdp',
+]
+
 
 # helper functions
 def rhasattr(obj: Any, attr: str) -> bool:
     """A chain-able attribute version of hasattr.
 
     For example, to check if
     `obj` has the attribute `foo.bar.baz`, you can use:
@@ -65,20 +71,24 @@
         - transformer: (GPT2LMHeadModel, GPTJConfig)
         - model.decoder: (OPTConfig, BloomConfig)
         - gpt_neox: (GPTNeoXConfig)
     """
     if hasattr(model, 'get_decoder'):
         return model.get_decoder()
 
-    decoder_attrs = ('transformer', 'model.decoder', 'gpt_neox',
-                     'model.transformer')
+    decoder_attrs = (
+        'transformer',
+        'model.decoder',
+        'gpt_neox',
+        'model.transformer',
+    )
     causal_base_model = findattr(model, decoder_attrs)
     if causal_base_model is None:
         raise ValueError(
-            f'Unable to FSDP-wrap model {model}. Please open a github issue to add support.'
+            f'Unable to FSDP-wrap model {model}. Please open a github issue to add support.',
         )
     return causal_base_model
 
 
 def hf_get_hidden_layers(model: PreTrainedModel) -> Any:
     """Returns the hidden layers of the specified model.
 
@@ -96,15 +106,15 @@
         'layers',  # GPTNeoX, Llama, ProphetNet, Marian (from encoder)
         'block',  # T5, BART, Pegasus (from encoder)
         'blocks',  # MPT
     )
     layers = findattr(model, hidden_layers_attrs)
     if layers is None:
         raise ValueError(
-            f'Unable to find hidden layer for {model}. Model must have one of the following attributes: {hidden_layers_attrs}'
+            f'Unable to find hidden layer for {model}. Model must have one of the following attributes: {hidden_layers_attrs}',
         )
     return layers
 
 
 def hf_get_init_device(init_device: Optional[str]) -> Optional[str]:
     """Returns the appropriate device to initialize models."""
     from composer.utils import dist
@@ -114,41 +124,43 @@
         return 'meta'
     return init_device
 
 
 # /end helper functions
 
 
-def prepare_hf_model_for_fsdp(model: PreTrainedModel,
-                              init_device: Optional[str]) -> None:
+def prepare_hf_model_for_fsdp(
+    model: PreTrainedModel,
+    init_device: Optional[str],
+) -> None:
     """FSDP wrap a HuggingFace model.
 
     Call specific functions
     """
     if model.config.is_encoder_decoder:
         prepare_hf_enc_dec_model_for_fsdp(model, init_device)
     else:
         # many common decoder-only model do not set the flag
         # model.config.is_decoder, so we can't trust it
         prepare_hf_causal_lm_model_for_fsdp(model, init_device)
 
 
-def prepare_hf_causal_lm_model_for_fsdp(model: Union[PreTrainedModel,
-                                                     'PeftModel'],
-                                        init_device: Optional[str]) -> None:
+def prepare_hf_causal_lm_model_for_fsdp(
+    model: Union[PreTrainedModel, 'PeftModel'],
+    init_device: Optional[str],
+) -> None:
     """FSDP wrap a HuggingFace decoder.
 
     Wrap any model for FSDP which follows one of the 3 existing conventions from
     HuggingFace for decoder-only LLMs.
     """
     causal_base_model = hf_get_causal_base_model(model)
 
     # OPT and olmo have an extra layer of wrapping, so special case here
-    if isinstance(causal_base_model,
-                  OPTDecoder) or model.config.model_type == 'olmo':
+    if isinstance(causal_base_model, OPTDecoder):
         underlying_model = maybe_get_underlying_model(model)
         underlying_model.model._fsdp_wrap = False
     model_block = hf_get_hidden_layers(causal_base_model)
     lm_head = model.get_output_embeddings()
     # Try to get input embeddings from the transformer backbone
     # and then from the XXXForCausalLM
     try:
@@ -156,22 +168,23 @@
     except:
         tied_embeddings = model.get_input_embeddings()
 
     modules = {
         'base_model': causal_base_model,
         'model_block': model_block,
         'lm_head': lm_head,
-        'tied_embeddings': tied_embeddings
+        'tied_embeddings': tied_embeddings,
     }
 
     for mod_name, module in modules.items():
         if module is None:
             raise ValueError(
                 f'Unable to FSDP-wrap this model! `{mod_name}` does not ' +
-                'follow common layer/weight naming conventions.')
+                'follow common layer/weight naming conventions.',
+            )
     block_type = type(model_block[0])
 
     # When using the HF LM models,
     # the weights of the self.lm_head and self.transformer.wte are tied.
     # This tying occurs inside the `self.post_init()` function.
     # This is a hurdle for FSDP because they need to be in the same FSDP block
     # These lines ensures that both modules stay together in the top-most block when
@@ -185,28 +198,33 @@
     # TODO: Revisit this if we enforce use_orig_params=True, which seems to support
     # mixed frozen/unfrozen FSDP modules
     if hasattr(model, 'peft_type') and model.peft_type is not None:
         peft_type = model.peft_type.lower()
         active_adapters = [adapter.lower() for adapter in model.active_adapters]
         for name, module in model.named_modules():
             if peft_type in name.lower() and any(
-                    adapter in name.lower() for adapter in active_adapters):
+                adapter in name.lower() for adapter in active_adapters
+            ):
                 has_parameters = next(module.parameters(), None) is not None
                 has_buffers = next(module.buffers(), None) is not None
                 if has_parameters or has_buffers:
                     module._fsdp_wrap = True
 
     # FSDP Wrap and Activation Checkpoint every model block
     model.fsdp_wrap_fn = lambda module: isinstance(module, block_type)
     model.activation_checkpointing_fn = lambda module: isinstance(
-        module, block_type)
+        module,
+        block_type,
+    )
 
 
-def prepare_hf_enc_dec_model_for_fsdp(model: PreTrainedModel,
-                                      init_device: Optional[str]) -> None:
+def prepare_hf_enc_dec_model_for_fsdp(
+    model: PreTrainedModel,
+    init_device: Optional[str],
+) -> None:
     """Wrap an encoder/decoder HF model.
 
     This works for T5, BART, Pegasus, PegasusX, but not all enc/dec (ProphetNet)
     You have model.shared, model.encoder, model.decoder and model.lm_head, where
     model.shared are the embeddings which are tied to model.lm_head, and
     model.shared == model.encoder.embed_tokens and model.shared ==
     model.decoder.embed_tokens
@@ -221,37 +239,42 @@
 
     modules = {
         'encoder': encoder,
         'decoder': decoder,
         'encoder_block': encoder_block,
         'decoder_block': decoder_block,
         'lm_head': lm_head,
-        'tied_embeddings': tied_embeddings
+        'tied_embeddings': tied_embeddings,
     }
 
     for mod_name, module in modules.items():
         if module is None:
             raise ValueError(
                 f'Unable to FSDP-wrap this model! `{mod_name}` does not ' +
-                'follow common layer/weight naming conventions.')
+                'follow common layer/weight naming conventions.',
+            )
     decoder_block_type = type(decoder_block[0])
     encoder_block_type = type(encoder_block[0])
 
     if model.config.tie_word_embeddings:
         # it is possible to train an enc/dec without tied embeddings, hence the check
         tied_embeddings._fsdp_wrap = False
         encoder._fsdp_wrap = False
         decoder._fsdp_wrap = False
         lm_head._fsdp_wrap = False
 
     # FSDP Wrap and Activation Checkpoint every decoder block
     model.fsdp_wrap_fn = lambda module: isinstance(module, decoder_block_type)
     model.activation_checkpointing_fn = lambda module: isinstance(
-        module, decoder_block_type)
+        module,
+        decoder_block_type,
+    )
 
     if encoder_block_type == decoder_block_type:
         return
 
-    # need to wrap encoder blocks separately for ProhpetNet and Marian
+    # need to wrap encoder blocks separately for ProphetNet and Marian
     model.fsdp_wrap_fn = lambda module: isinstance(module, encoder_block_type)
     model.activation_checkpointing_fn = lambda module: isinstance(
-        module, encoder_block_type)
+        module,
+        encoder_block_type,
+    )
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/hf/hf_t5.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/hf/hf_t5.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 
 from __future__ import annotations
 
 from typing import Mapping
 
 from composer.utils import dist
 from omegaconf import DictConfig
-from transformers import (AutoConfig, PreTrainedTokenizerBase,
-                          T5ForConditionalGeneration)
+from transformers import (
+    AutoConfig,
+    PreTrainedTokenizerBase,
+    T5ForConditionalGeneration,
+)
 
 from llmfoundry.metrics import DEFAULT_ENC_DEC_METRICS
 from llmfoundry.models.hf.hf_fsdp import hf_get_init_device
 from llmfoundry.models.hf.model_wrapper import HuggingFaceModelWithFSDP
 from llmfoundry.models.utils import init_empty_weights
 from llmfoundry.utils.warnings import experimental_class
 
@@ -40,39 +43,43 @@
                 cfg.config_overrides must be compatible with the pre-trained weights.
             cfg.init_device ('cpu' | 'meta'): Which device, 'cpu' or 'meta', to
                 initialize the model on. Currently, `meta` is only supported when
                 cfg.pretrained is ``False``. Default: ``'cpu'``.
         tokenizer (PreTrainedTokenizer): The tokenizer that the model will use.
     """
 
-    def __init__(self, om_model_config: DictConfig,
-                 tokenizer: PreTrainedTokenizerBase):
+    def __init__(
+        self,
+        om_model_config: DictConfig,
+        tokenizer: PreTrainedTokenizerBase,
+    ):
         from llmfoundry.utils.builders import build_metric
 
         config = AutoConfig.from_pretrained(
             om_model_config.pretrained_model_name_or_path,
             trust_remote_code=om_model_config.get('trust_remote_code', True),
             use_auth_token=om_model_config.get('use_auth_token', False),
         )
 
         # set config overrides
         for k, v in om_model_config.get('config_overrides', {}).items():
             if not hasattr(config, k):
                 raise ValueError(
-                    f'config does not have attribute "{k}" to override ({k}: {v}).'
+                    f'config does not have attribute "{k}" to override ({k}: {v}).',
                 )
 
             attr = getattr(config, k)
             if isinstance(attr, Mapping):
                 extra_keys = [_k for _k in v.keys() if _k not in attr.keys()]
                 if extra_keys:
                     raise ValueError(
                         f'Config dict override got unknown keys. ' +
                         f'Extra keys: {extra_keys}. ' +
-                        f'Expected (a subset of) keys: {list(attr.keys())}.')
+                        f'Expected (a subset of) keys: {list(attr.keys())}.',
+                    )
                 getattr(config, k).update(v)
             else:
                 setattr(config, k, v)
 
         if not config.is_encoder_decoder:
             raise ValueError(f'Model type "hf_t5" currently only supports T5 models ' +\
                              f'using configs where `is_encoder_decoder` is ``True``.')
@@ -88,32 +95,34 @@
         if dist.get_local_rank() != 0 and init_device == 'mixed':
             om_model_config.pretrained = False
 
         if resolved_init_device == 'cpu':
             if om_model_config.pretrained:
                 model = T5ForConditionalGeneration.from_pretrained(
                     om_model_config.pretrained_model_name_or_path,
-                    config=config)
+                    config=config,
+                )
             else:
                 model = T5ForConditionalGeneration(config)
         elif resolved_init_device == 'meta':
             if om_model_config.pretrained:
                 raise ValueError(
-                    'Setting cfg.pretrained=True is not supported when init_device="meta".'
+                    'Setting cfg.pretrained=True is not supported when init_device="meta".',
                 )
             with init_empty_weights(include_buffers=False):
                 model = T5ForConditionalGeneration(config)
         else:
             raise ValueError(
-                f'init_device="{init_device}" must be either "cpu" or "meta".')
+                f'init_device="{init_device}" must be either "cpu" or "meta".',
+            )
 
         metrics = [
             build_metric(metric, {}) for metric in DEFAULT_ENC_DEC_METRICS +
             om_model_config.get('additional_train_metrics', [])
         ]
 
-        composer_model = super().__init__(model=model,
-                                          tokenizer=tokenizer,
-                                          metrics=metrics,
-                                          init_device=init_device)
-
-        return composer_model
+        super().__init__(
+            model=model,
+            tokenizer=tokenizer,
+            metrics=metrics,
+            init_device=init_device,
+        )
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/hf/model_wrapper.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/hf/model_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,75 +2,91 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """Re-usable :class:`.ComposerModel` for LLM HF Models."""
 
 from __future__ import annotations
 
 from collections import UserDict
-from typing import TYPE_CHECKING, List, Mapping, Optional
+from typing import TYPE_CHECKING, List, Mapping, Optional, Union
 
 import transformers
 from composer.models.huggingface import HuggingFaceModel
 from torchmetrics import Metric
 from transformers import PreTrainedTokenizerBase
 from transformers.utils.generic import ModelOutput
 
 from llmfoundry.models.hf.hf_fsdp import prepare_hf_model_for_fsdp
 
 if TYPE_CHECKING:
-    from peft import PeftConfig
+    from peft import PeftConfig, PeftModel
+
+__all__ = ['HuggingFaceModelWithFSDP']
 
 # HuggingFace hardcodes the ignore index to -100
 _HF_IGNORE_INDEX = -100
 
 
 class HuggingFaceModelWithFSDP(HuggingFaceModel):
     """Wrapper around HuggingFaceModel.
 
     Handles preparation for FSDP wrapping.
     """
 
-    def __init__(self,
-                 model: transformers.PreTrainedModel,
-                 tokenizer: Optional[PreTrainedTokenizerBase] = None,
-                 metrics: Optional[List[Metric]] = None,
-                 eval_metrics: Optional[List[Metric]] = None,
-                 shift_labels: bool = False,
-                 init_device: Optional[str] = None,
-                 peft_config: Optional['PeftConfig'] = None):
+    def __init__(
+        self,
+        model: Union[transformers.PreTrainedModel, 'PeftModel'],
+        tokenizer: Optional[PreTrainedTokenizerBase] = None,
+        metrics: Optional[List[Metric]] = None,
+        eval_metrics: Optional[List[Metric]] = None,
+        shift_labels: bool = False,
+        init_device: Optional[str] = None,
+        peft_config: Optional['PeftConfig'] = None,
+    ):
         super().__init__(
             model,
             tokenizer,
             use_logits=True,
             metrics=metrics,
             eval_metrics=eval_metrics,
             shift_labels=shift_labels,
             peft_config=peft_config,
             should_save_peft_only=True,
         )
 
-        # Note: We need to add the FSDP related attributes to the model AFTER the super init,
-        # so that the (possible) embedding resizing doesn't destroy them
-        prepare_hf_model_for_fsdp(self.model, init_device)
-
-        # This provides support for meta initialization when using FSDP
-        self.model.param_init_fn = lambda module: self.model._init_weights(
-            module)
+        self.prepare_inner_model(self.model, init_device)
 
     def forward(self, batch: Mapping):
         if isinstance(batch, dict) or isinstance(batch, UserDict):
             # Further input validation is left to the huggingface forward call
             batch = {
                 k: v for k, v in batch.items() if k in self.model_forward_args
             }
             output = self.model(**batch)  # type: ignore (thirdparty)
         else:
             raise ValueError(
-                'Unexpected batch type. Expected a dictionary with keys corresponding to the inputs to the forward function of the Huggingface model'
+                'Unexpected batch type. Expected a dictionary with keys corresponding to the inputs to the forward function of the Huggingface model',
             )
         return output
 
     def loss(self, outputs: ModelOutput, batch: Mapping):
         if self.config.use_return_dict:
             return outputs['loss']
         # loss is at index 0 in the output tuple, logits are at index 1
         return outputs[:2]
+
+    @staticmethod
+    def prepare_inner_model(
+        model: Union[transformers.PreTrainedModel, 'PeftModel'],
+        init_device: Optional[str] = None,
+    ):
+        """Prepare the inner model for FSDP wrapping.
+
+        Args:
+            model: The model to prepare.
+            init_device: The device to initialize the model on.
+        """
+        # Note: We need to add the FSDP related attributes to the model AFTER the super init,
+        # so that the (possible) embedding resizing doesn't destroy them
+        prepare_hf_model_for_fsdp(model, init_device)
+
+        # This provides support for meta initialization when using FSDP
+        model.param_init_fn = lambda module: model._init_weights(module)
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/inference_api_wrapper/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 from llmfoundry.models.inference_api_wrapper.fmapi import (
-    FMAPICasualLMEvalWrapper, FMAPIChatAPIEvalWrapper)
+    FMAPICasualLMEvalWrapper,
+    FMAPIChatAPIEvalWrapper,
+    FMAPIEvalInterface,
+)
 from llmfoundry.models.inference_api_wrapper.interface import \
     InferenceAPIEvalWrapper
 from llmfoundry.models.inference_api_wrapper.openai_causal_lm import (
-    OpenAICausalLMEvalWrapper, OpenAIChatAPIEvalWrapper)
+    OpenAICausalLMEvalWrapper,
+    OpenAIChatAPIEvalWrapper,
+    OpenAIEvalInterface,
+)
 
 __all__ = [
     'OpenAICausalLMEvalWrapper',
     'OpenAIChatAPIEvalWrapper',
+    'OpenAIEvalInterface',
     'InferenceAPIEvalWrapper',
     'FMAPICasualLMEvalWrapper',
     'FMAPIChatAPIEvalWrapper',
+    'FMAPIEvalInterface',
 ]
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/inference_api_wrapper/fmapi.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/fmapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 import time
 
 import requests
 from omegaconf import DictConfig
 from transformers import AutoTokenizer
 
 from llmfoundry.models.inference_api_wrapper.openai_causal_lm import (
-    OpenAICausalLMEvalWrapper, OpenAIChatAPIEvalWrapper, OpenAIEvalInterface)
+    OpenAICausalLMEvalWrapper,
+    OpenAIChatAPIEvalWrapper,
+    OpenAIEvalInterface,
+)
 
 __all__ = [
     'FMAPICasualLMEvalWrapper',
     'FMAPIChatAPIEvalWrapper',
+    'FMAPIEvalInterface',
 ]
 
 log = logging.getLogger(__name__)
 
 
 class FMAPIEvalInterface(OpenAIEvalInterface):
 
@@ -33,35 +37,37 @@
         while True:
             try:
                 requests.get(ping_url)
                 log.info(f'Endpoint {ping_url} is ready')
                 break
             except requests.exceptions.ConnectionError:
                 log.debug(
-                    f'Endpoint {ping_url} not ready yet. Sleeping {sleep_s} seconds'
+                    f'Endpoint {ping_url} not ready yet. Sleeping {sleep_s} seconds',
                 )
                 time.sleep(sleep_s)
                 waited_s += sleep_s
 
             if waited_s >= timeout_s:
                 raise TimeoutError(
-                    f'Endpoint {ping_url} did not become read after {waited_s:,} seconds, exiting'
+                    f'Endpoint {ping_url} did not become read after {waited_s:,} seconds, exiting',
                 )
 
     def __init__(self, om_model_config: DictConfig, tokenizer: AutoTokenizer):
         is_local = om_model_config.pop('local', False)
         if is_local:
-            base_url = os.environ.get('MOSAICML_MODEL_ENDPOINT',
-                                      'http://0.0.0.0:8080/v2')
+            base_url = os.environ.get(
+                'MOSAICML_MODEL_ENDPOINT',
+                'http://0.0.0.0:8080/v2',
+            )
             om_model_config['base_url'] = base_url
             self.block_until_ready(base_url)
 
         if 'base_url' not in om_model_config:
             raise ValueError(
-                'Must specify base_url or use local=True in model_cfg for FMAPIsEvalWrapper'
+                'Must specify base_url or use local=True in model_cfg for FMAPIsEvalWrapper',
             )
 
         super().__init__(om_model_config, tokenizer)
 
 
 class FMAPICasualLMEvalWrapper(FMAPIEvalInterface, OpenAICausalLMEvalWrapper):
     """Databricks Foundational Model API wrapper for causal LM models."""
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/inference_api_wrapper/interface.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 from typing import Any, Optional
 
 import torch
 from composer.core.types import Batch
-from composer.metrics import InContextLearningMetric
 from composer.models import ComposerModel
 from omegaconf import DictConfig
 from torchmetrics import Metric
 from transformers import AutoTokenizer
 
+from llmfoundry.eval.metrics import InContextLearningMetric
 from llmfoundry.metrics import DEFAULT_CAUSAL_LM_EVAL_METRICS
 
+__all__ = ['InferenceAPIEvalWrapper']
+
 
 class InferenceAPIEvalWrapper(ComposerModel):
 
     def __init__(self, om_model_config: DictConfig, tokenizer: AutoTokenizer):
         from llmfoundry.utils.builders import build_metric
 
         self.tokenizer = tokenizer
@@ -48,55 +50,64 @@
 
     def eval_forward(self, batch: Batch, outputs: Optional[Any] = None):
         padding_tok = self.tokenizer.pad_token_id if self.tokenizer.pad_token_id else self.tokenizer.eos_token_id
         # If the batch mode is generate, we will generate a requested number of tokens using the underlying
         # model's generate function. Extra generation kwargs can be passed in via the batch. Strings will
         # be returned from eval_forward
         output_logits_batch = []
-        for tokens, cont_idxs in zip(batch['input_ids'],
-                                     batch['continuation_indices']):
+        for tokens, cont_idxs in zip(
+            batch['input_ids'],
+            batch['continuation_indices'],
+        ):
 
             seqlen = tokens.shape[0]
             tokens = tokens.tolist()
             cont_idxs = cont_idxs.tolist()
             expected_cont_tokens = tokens[cont_idxs[0]:cont_idxs[-1] + 1]
             output_logits = torch.nn.functional.one_hot(
                 torch.tensor(tokens[1:cont_idxs[0]]),
-                num_classes=len(self.tokenizer))
+                num_classes=len(self.tokenizer),
+            )
             for i in range(len(expected_cont_tokens)):
                 # decode one token at a time
-                prompt = self.tokenizer.decode(tokens[:cont_idxs[0]] +
-                                               expected_cont_tokens[0:i])
+                prompt = self.tokenizer.decode(
+                    tokens[:cont_idxs[0]] + expected_cont_tokens[0:i],
+                )
                 next_logit_tensor = self.get_next_token_logit_tensor(prompt)
                 if next_logit_tensor is None:
                     continue
-                output_logits = torch.cat(
-                    [output_logits,
-                     next_logit_tensor.reshape(1, -1)])
+                output_logits = torch.cat([
+                    output_logits,
+                    next_logit_tensor.reshape(1, -1),
+                ])
             padding = torch.nn.functional.one_hot(
                 torch.full((seqlen - output_logits.shape[0],), padding_tok),
-                num_classes=len(self.tokenizer))
+                num_classes=len(self.tokenizer),
+            )
             output_logits = torch.cat([output_logits, padding])
             output_logits_batch.append(output_logits)
 
         return torch.stack(output_logits_batch).to(batch['input_ids'].device)
 
     def update_metric(self, batch: Any, outputs: Any, metric: Metric) -> None:
         batch = self.rebatch(batch)
         self.labels = batch.pop('labels')
         self.labels[:, :-1] = self.labels[:, 1:].clone()
         self.labels[:, -1] = -100
-        if isinstance(metric, InContextLearningMetric) and batch.get(
-                'mode', None) == 'icl_task':
+        if isinstance(
+            metric,
+            InContextLearningMetric,
+        ) and batch.get('mode', None) == 'icl_task':
             assert self.labels is not None
             metric.update(batch, outputs, self.labels)
         else:
             raise NotImplementedError(
-                'Inference API wrapper only supports InContextLearningMetrics and mode=icl_task'
+                'Inference API wrapper only supports InContextLearningMetrics and mode=icl_task',
             )
 
     def forward(self):
         raise NotImplementedError(
-            "Inference API wrapper doesn't support forward")
+            "Inference API wrapper doesn't support forward",
+        )
 
     def loss(self):
         raise NotImplementedError("Inference API wrapper doesn't support loss")
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/inference_api_wrapper/openai_causal_lm.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/openai_causal_lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,50 +19,55 @@
 
 from llmfoundry.models.inference_api_wrapper.interface import \
     InferenceAPIEvalWrapper
 
 __all__ = [
     'OpenAICausalLMEvalWrapper',
     'OpenAIChatAPIEvalWrapper',
+    'OpenAIEvalInterface',
 ]
 
 if TYPE_CHECKING:
     from openai.types.chat.chat_completion import ChatCompletion
     from openai.types.completion import Completion
     from openai.types.completion_choice import Logprobs
 
 MAX_RETRIES = 10
 
 
 class OpenAIEvalInterface(InferenceAPIEvalWrapper):
 
-    def __init__(self, om_model_config: DictConfig,
-                 tokenizer: AutoTokenizer) -> None:
+    def __init__(
+        self,
+        om_model_config: DictConfig,
+        tokenizer: AutoTokenizer,
+    ) -> None:
         super().__init__(om_model_config, tokenizer)
         try:
             import openai
         except ImportError as e:
             raise MissingConditionalImportError(
                 extra_deps_group='openai',
                 conda_package='openai',
-                conda_channel='conda-forge') from e
+                conda_channel='conda-forge',
+            ) from e
 
         api_key = os.environ.get('OPENAI_API_KEY')
         base_url = om_model_config.get('base_url')
         if base_url is None:
             # Using OpenAI default, where the API key is required
             if api_key is None:
                 raise ValueError(
-                    'No OpenAI API Key found. Ensure it is saved as an environmental variable called OPENAI_API_KEY.'
+                    'No OpenAI API Key found. Ensure it is saved as an environmental variable called OPENAI_API_KEY.',
                 )
 
         else:
             # Using a custom base URL, where the API key may not be required
             log.info(
-                f'Making request to custom base URL: {base_url}{"" if api_key is not None else " (no API key set)"}'
+                f'Making request to custom base URL: {base_url}{"" if api_key is not None else " (no API key set)"}',
             )
             api_key = 'placeholder'  # This cannot be None
 
         self.client = openai.OpenAI(base_url=base_url, api_key=api_key)
         if 'version' in om_model_config:
             self.model_name = om_model_config['version']
         else:
@@ -81,102 +86,123 @@
     def try_generate_completion(self, prompt: str, num_tokens: int):
         try:
             from openai import APITimeoutError, RateLimitError
         except ImportError as e:
             raise MissingConditionalImportError(
                 extra_deps_group='openai',
                 conda_package='openai',
-                conda_channel='conda-forge') from e
+                conda_channel='conda-forge',
+            ) from e
         tries = 0
         completion = None
         delay = 1
         while tries < MAX_RETRIES:
             tries += 1
             try:
                 completion = self.generate_completion(prompt, num_tokens)
                 break
             except RateLimitError as e:
                 if 'You exceeded your current quota' in str(
-                        e._message):  # pyright: ignore
+                    e._message,
+                ):  # pyright: ignore
                     raise e
                 delay *= 2 * (1 + random.random())
                 sleep(delay)
                 continue
             except APITimeoutError as e:
                 delay *= 2 * (1 + random.random())
                 sleep(delay)
                 continue
 
         return completion
 
 
 class OpenAIChatAPIEvalWrapper(OpenAIEvalInterface):
 
-    def __init__(self, om_model_config: DictConfig,
-                 tokenizer: AutoTokenizer) -> None:
+    def __init__(
+        self,
+        om_model_config: DictConfig,
+        tokenizer: AutoTokenizer,
+    ) -> None:
         super().__init__(om_model_config, tokenizer)
 
         self.generate_completion = lambda prompt, num_tokens: self.client.chat.completions.create(
             model=self.model_name,
             messages=[{
                 'role':
                     'system',
                 'content':
-                    om_model_config.get('system_role_prompt',
-                                        'Please complete the following text: ')
+                    om_model_config.get(
+                        'system_role_prompt',
+                        'Please complete the following text: ',
+                    ),
             }, {
                 'role': 'user',
-                'content': prompt
+                'content': prompt,
             }],
             max_tokens=num_tokens,
-            temperature=0.0)
+            temperature=0.0,
+        )
 
     def retokenize(self, tokens: List[int], cont_idxs: List[int]):
         """Chat API will never respond with a word-initial space.
 
         If the continuation tokens begin with a word initial space, we need to
         re-tokenize with the space removed.
         """
         original_len = len(tokens)
         retokenized_continuation = self.tokenizer(
-            self.tokenizer.decode(tokens[cont_idxs[0]:cont_idxs[-1] +
-                                         1]).strip())['input_ids']
+            self.tokenizer.decode(
+                tokens[cont_idxs[0]:cont_idxs[-1] + 1],
+            ).strip(),
+        )['input_ids']
 
         # replace the original continuation with the retokenized continuation + padding
         padding = [tokens[-1]] * (
-            len(tokens) - len(tokens[:cont_idxs[0]] + retokenized_continuation))
+            len(tokens) - len(tokens[:cont_idxs[0]] + retokenized_continuation)
+        )
         tokens = tokens[:cont_idxs[0]] + retokenized_continuation + padding
 
         if len(tokens) > original_len:
             # this only happens if we were already at max seq len and the continuation got LARGER
             tokens = tokens[-original_len:]
             cont_idxs = list(
-                range(original_len - len(retokenized_continuation),
-                      original_len))
+                range(
+                    original_len - len(retokenized_continuation),
+                    original_len,
+                ),
+            )
         else:
             cont_idxs = list(
-                range(cont_idxs[0],
-                      cont_idxs[0] + len(retokenized_continuation)))
+                range(
+                    cont_idxs[0],
+                    cont_idxs[0] + len(retokenized_continuation),
+                ),
+            )
         return torch.tensor(tokens), torch.tensor(cont_idxs)
 
     def rebatch(self, batch: Batch):
         """Chat API tokenization has different behavior than GPT3.
 
         Model responses will never begin with spaces even if the continuation is
         expected to, so we need to retokenize the input to account for that.
         """
         new_batch: Dict[str, Union[List[torch.Tensor], torch.Tensor]] = {
             'input_ids': [],
             'continuation_indices': [],
-            'labels': []
+            'labels': [],
         }
-        for tokens, cont_idxs in zip(batch['input_ids'],
-                                     batch['continuation_indices']):
-            tokens, cont_idxs = self.retokenize(tokens.tolist(),
-                                                cont_idxs.tolist())
+        for tokens, cont_idxs in zip(
+            batch['input_ids'],
+            batch['continuation_indices'],
+        ):
+            tokens, cont_idxs = self.retokenize(
+                tokens.tolist(),
+                cont_idxs.tolist(),
+            )
 
             assert isinstance(new_batch['input_ids'], list)
             new_batch['input_ids'].append(tokens)
             assert isinstance(new_batch['labels'], list)
             new_batch['labels'].append(tokens)
             assert isinstance(new_batch['continuation_indices'], list)
             new_batch['continuation_indices'].append(cont_idxs)
@@ -194,47 +220,54 @@
         # Override the base class because Chat's API always strips spacing from model outputs resulting in different tokens
         # than what the continuation would expect.
         # Get around this issue by retokenizing the batch to remove spacing from the continuation as well as
         # decoding the whole continuation at once.
         padding_tok = self.tokenizer.pad_token_id if self.tokenizer.pad_token_id else self.tokenizer.eos_token_id
         output_logits_batch = []
         batch = self.rebatch(batch)
-        for tokens, cont_idxs in zip(batch['input_ids'],
-                                     batch['continuation_indices']):
+        for tokens, cont_idxs in zip(
+            batch['input_ids'],
+            batch['continuation_indices'],
+        ):
 
             seqlen = tokens.shape[0]
             tokens = tokens.tolist()
             cont_idxs = cont_idxs.tolist()
             expected_cont_tokens = tokens[cont_idxs[0]:cont_idxs[-1] + 1]
             output_logits = torch.nn.functional.one_hot(
                 torch.tensor(tokens[1:cont_idxs[0]]),
-                num_classes=len(self.tokenizer))
+                num_classes=len(self.tokenizer),
+            )
 
             prompt = self.tokenizer.decode(tokens[:cont_idxs[0]])
             next_logit_tensor = self.get_next_token_logit_tensor(
-                prompt, num_tokens=len(expected_cont_tokens))
+                prompt,
+                num_tokens=len(expected_cont_tokens),
+            )
 
             if next_logit_tensor is not None:
                 output_logits = torch.cat([output_logits, next_logit_tensor])
             padding = torch.nn.functional.one_hot(
                 torch.full((seqlen - output_logits.shape[0],), padding_tok),
-                num_classes=len(self.tokenizer))
+                num_classes=len(self.tokenizer),
+            )
             output_logits = torch.cat([output_logits, padding])
             output_logits_batch.append(output_logits)
 
         return torch.stack(output_logits_batch).to(batch['input_ids'].device)
 
     def process_result(self, completion: Optional['ChatCompletion']):
         if completion is None:
             raise ValueError("Couldn't generate model output")
 
         if len(completion.choices) > 0:
             tensors = []
             for t in self.tokenizer(
-                    completion.choices[0].message.content)['input_ids']:
+                completion.choices[0].message.content,
+            )['input_ids']:
                 # Not real logprobs
                 tensor = torch.tensor([0] * (len(self.tokenizer)))
                 tensor[t] = 1.0
                 tensors.append(tensor)
 
             if len(tensors) == 0:
                 return None
@@ -243,37 +276,42 @@
             # the model sometimes stops early even though we are still requesting tokens!
             # not sure if there's a fix
             return None
 
 
 class OpenAICausalLMEvalWrapper(OpenAIEvalInterface):
 
-    def __init__(self, om_model_config: DictConfig,
-                 tokenizer: AutoTokenizer) -> None:
+    def __init__(
+        self,
+        om_model_config: DictConfig,
+        tokenizer: AutoTokenizer,
+    ) -> None:
         super().__init__(om_model_config, tokenizer)
         self.generate_completion = lambda prompt, num_tokens: self.client.completions.create(
             model=self.model_name,
             prompt=prompt,
             max_tokens=num_tokens,
             logprobs=5,
-            temperature=0.0)
+            temperature=0.0,
+        )
 
     def process_result(self, completion: Optional['Completion']):
         if completion is None:
             raise ValueError("Couldn't generate model output")
 
         if TYPE_CHECKING:
             assert isinstance(completion, Completion)
             assert isinstance(completion.choices[0].logprobs, Logprobs)
             assert isinstance(completion.choices[0].logprobs.top_logprobs, list)
 
         if len(completion.choices[0].logprobs.top_logprobs[0]) > 0:
             # Construct tensor of shape (vocab_size,) with logprobs for each token
             tokenizer_logprobs = dict(
-                completion.choices[0].logprobs.top_logprobs[0])
+                completion.choices[0].logprobs.top_logprobs[0],
+            )
             tensor = torch.tensor([min(tokenizer_logprobs.values()) - 1] *
                                   (len(self.tokenizer)))
             for k in tokenizer_logprobs:
                 encoding = self.tokenizer(k)['input_ids']
                 tensor[encoding[0]] = tokenizer_logprobs[k]
             return tensor
         else:
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/layers/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/layers/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,61 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 from llmfoundry.models.layers.attention import (
-    ATTN_CLASS_REGISTRY, GroupedQueryAttention, MultiheadAttention,
-    MultiQueryAttention, attn_bias_shape, build_alibi_bias, build_attn_bias,
-    flash_attn_fn, scaled_multihead_dot_product_attention)
-from llmfoundry.models.layers.blocks import MPTBlock
+    GroupedQueryAttention,
+    MultiheadAttention,
+    MultiQueryAttention,
+    attn_bias_shape,
+    build_alibi_bias,
+    build_attn_bias,
+    check_alibi_support,
+    flash_attn_fn,
+    scaled_multihead_dot_product_attention,
+)
+from llmfoundry.models.layers.blocks import FusedNormAttentionNorm, MPTBlock
 from llmfoundry.models.layers.custom_embedding import SharedEmbedding
-from llmfoundry.models.layers.fc import FC_CLASS_REGISTRY
-from llmfoundry.models.layers.ffn import FFN_CLASS_REGISTRY, MPTMLP, build_ffn
-from llmfoundry.models.layers.norm import NORM_CLASS_REGISTRY, LPLayerNorm
+from llmfoundry.models.layers.dmoe import DroplessMLP, LearnedRouter, dMoE
+from llmfoundry.models.layers.fc import *
+from llmfoundry.models.layers.ffn import MPTGLU, MPTMLP
+from llmfoundry.models.layers.layer_builders import (
+    build_attention_layer,
+    build_fc,
+    build_ffn,
+    build_norm,
+)
+from llmfoundry.models.layers.norm import (
+    LPLayerNorm,
+    LPRMSNorm,
+    RMSNorm,
+    TritonRMSNorm,
+    rms_norm,
+)
 
 __all__ = [
     'scaled_multihead_dot_product_attention',
     'flash_attn_fn',
     'MultiheadAttention',
     'MultiQueryAttention',
     'GroupedQueryAttention',
     'attn_bias_shape',
     'build_attn_bias',
     'build_alibi_bias',
-    'ATTN_CLASS_REGISTRY',
-    'MPTMLP',
+    'check_alibi_support',
     'MPTBlock',
-    'NORM_CLASS_REGISTRY',
-    'LPLayerNorm',
-    'FC_CLASS_REGISTRY',
+    'FusedNormAttentionNorm',
     'SharedEmbedding',
-    'FFN_CLASS_REGISTRY',
+    'dMoE',
+    'LearnedRouter',
+    'DroplessMLP',
+    'MPTMLP',
+    'MPTGLU',
+    'build_attention_layer',
     'build_ffn',
+    'build_fc',
+    'build_norm',
+    'LPLayerNorm',
+    'LPRMSNorm',
+    'RMSNorm',
+    'TritonRMSNorm',
+    'rms_norm',
 ]
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/layers/attention.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/layers/attention.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,31 @@
 import torch
 import torch.nn as nn
 import transformers
 from einops import rearrange
 from packaging import version
 from torch import nn
 
-from llmfoundry.models.layers.fc import FC_CLASS_REGISTRY
-from llmfoundry.models.layers.norm import NORM_CLASS_REGISTRY
+from llmfoundry.layers_registry import (
+    attention_classes,
+    attention_implementations,
+)
+from llmfoundry.models.layers.layer_builders import build_fc, build_norm
+
+__all__ = [
+    'scaled_multihead_dot_product_attention',
+    'flash_attn_fn',
+    'MultiheadAttention',
+    'MultiQueryAttention',
+    'GroupedQueryAttention',
+    'attn_bias_shape',
+    'build_attn_bias',
+    'build_alibi_bias',
+    'check_alibi_support',
+]
 
 
 def is_flash_v2_installed(v2_version: str = '2.0.0'):
     assert version.parse(v2_version) >= version.parse('2.0.0')
     try:
         import flash_attn as flash_attn
     except:
@@ -37,28 +52,32 @@
 
 def is_transformers_version_gte(hf_version: str) -> bool:
     return version.parse(transformers.__version__) >= version.parse(hf_version)
 
 
 def check_alibi_support(attention_impl: str) -> bool:
     return attention_impl != 'flash' or is_flash_v2_installed(
-        v2_version='v2.4.2')
+        v2_version='v2.4.2',
+    )
 
 
 from transformers.models.llama.modeling_llama import apply_rotary_pos_emb
 
 
-def _reset_is_causal(num_query_tokens: int, num_key_tokens: int,
-                     original_is_causal: bool) -> bool:
+def _reset_is_causal(
+    num_query_tokens: int,
+    num_key_tokens: int,
+    original_is_causal: bool,
+) -> bool:
     # disable causal when it is not needed
     # necessary for flash for generation with kv_cache
     if original_is_causal and num_query_tokens != num_key_tokens:
         if num_query_tokens != 1:
             raise NotImplementedError(
-                'MPT does not support query and key with different number of tokens, unless number of query tokens is 1.'
+                'MPT does not support query and key with different number of tokens, unless number of query tokens is 1.',
             )
         else:
             return False
     return original_is_causal
 
 
 def repeat_kv_for_gqa(hidden: torch.Tensor, n_rep: int) -> torch.Tensor:
@@ -130,64 +149,71 @@
 
     if attn_bias is not None:
         # clamp to 0 necessary for torch 2.0 compile()
         _s_q = max(0, attn_bias.size(2) - s_q)
         _s_k = max(0, attn_bias.size(3) - s_k)
         attn_bias = attn_bias[:, :, _s_q:, _s_k:]
 
-        if (attn_bias.size(-1) != 1 and
-                attn_bias.size(-1) != s_k) or (attn_bias.size(-2) != 1 and
-                                               attn_bias.size(-2) != s_q):
+        if (attn_bias.size(-1) != 1 and attn_bias.size(-1) != s_k
+           ) or (attn_bias.size(-2) != 1 and attn_bias.size(-2) != s_q):
             raise RuntimeError(
-                f'attn_bias (shape: {attn_bias.shape}) is expected to broadcast to shape: {attn_weight.shape}.'
+                f'attn_bias (shape: {attn_bias.shape}) is expected to broadcast to shape: {attn_weight.shape}.',
             )
         attn_weight = attn_weight + attn_bias
 
     min_val = torch.finfo(q.dtype).min
 
     if key_padding_mask is not None:
         if attn_bias is not None:
             warnings.warn(
                 'Propagating key_padding_mask to the attention module ' +\
                 'and applying it within the attention module can cause ' +\
                 'unnecessary computation/memory usage. Consider integrating ' +\
                 'into attn_bias once and passing that to each attention ' +\
-                'module instead.'
+                'module instead.',
             )
         attn_weight = attn_weight.masked_fill(
-            ~key_padding_mask.view((b, 1, 1, s_k)), min_val)
+            ~key_padding_mask.view((b, 1, 1, s_k)),
+            min_val,
+        )
 
     if is_causal and (not q.size(2) == 1):
         s = max(s_q, s_k)
         causal_mask = attn_weight.new_ones(s, s, dtype=torch.float32)
         causal_mask = causal_mask.tril()
         causal_mask = causal_mask.to(torch.bool)
         causal_mask = ~causal_mask
         causal_mask = causal_mask[-s_q:, -s_k:]
-        attn_weight = attn_weight.masked_fill(causal_mask.view(1, 1, s_q, s_k),
-                                              min_val)
+        attn_weight = attn_weight.masked_fill(
+            causal_mask.view(1, 1, s_q, s_k),
+            min_val,
+        )
 
     attn_weight = torch.softmax(attn_weight, dim=-1)
 
     if dropout_p:
-        attn_weight = torch.nn.functional.dropout(attn_weight,
-                                                  p=dropout_p,
-                                                  training=training,
-                                                  inplace=True)
+        attn_weight = torch.nn.functional.dropout(
+            attn_weight,
+            p=dropout_p,
+            training=training,
+            inplace=True,
+        )
 
     out = attn_weight.to(v.dtype).matmul(v)
     out = rearrange(out, 'b h s d -> b s (h d)')
 
     if needs_weights:
         return out, attn_weight, past_key_value
     return out, None, past_key_value
 
 
-def check_valid_inputs(*tensors: torch.Tensor,
-                       valid_dtypes: Optional[list[torch.dtype]] = None):
+def check_valid_inputs(
+    *tensors: torch.Tensor,
+    valid_dtypes: Optional[list[torch.dtype]] = None,
+):
     if valid_dtypes is None:
         valid_dtypes = [torch.float16, torch.bfloat16]
     for tensor in tensors:
         if tensor.dtype not in valid_dtypes:
             raise TypeError(f'{tensor.dtype=} must be in {valid_dtypes=}.')
         if not tensor.is_cuda:
             raise TypeError(f'Inputs must be cuda tensors ({tensor.is_cuda=}).')
@@ -219,15 +245,16 @@
     del key_padding_mask
     if flash_attn_padding_info is None:
         raise ValueError('flash_attn_padding_info is required for flash attn.')
     try:
         from flash_attn import bert_padding, flash_attn_interface  # type: ignore # yapf: disable # isort: skip
     except:
         raise RuntimeError(
-            'Please install flash-attn==1.0.9 or flash-attn==2.3.6')
+            'Please install flash-attn==1.0.9 or flash-attn==2.3.6',
+        )
 
     check_valid_inputs(query, key, value)
 
     if past_key_value is not None:
         if len(past_key_value) != 0:
             key = torch.cat([past_key_value[0], key], dim=1)
             value = torch.cat([past_key_value[1], value], dim=1)
@@ -244,58 +271,72 @@
     indices_v = flash_attn_padding_info['indices_v']
     cu_seqlens_q = flash_attn_padding_info['cu_seqlens_q']
     cu_seqlens_k = flash_attn_padding_info['cu_seqlens_k']
     max_seqlen_q = flash_attn_padding_info['max_seqlen_q']
     max_seqlen_k = flash_attn_padding_info['max_seqlen_k']
 
     query_unpad = bert_padding.index_first_axis(
-        rearrange(query, 'b s ... -> (b s) ...'), indices_q)
+        rearrange(query, 'b s ... -> (b s) ...'),
+        indices_q,
+    )
     query_unpad = rearrange(query_unpad, 'nnz (h d) -> nnz h d', h=n_heads)
 
     key_unpad = bert_padding.index_first_axis(
-        rearrange(key, 'b s ... -> (b s) ...'), indices_k)
+        rearrange(key, 'b s ... -> (b s) ...'),
+        indices_k,
+    )
     key_unpad = rearrange(key_unpad, 'nnz (h d) -> nnz h d', h=kv_n_heads)
 
     value_unpad = bert_padding.index_first_axis(
-        rearrange(value, 'b s ... -> (b s) ...'), indices_v)
+        rearrange(value, 'b s ... -> (b s) ...'),
+        indices_v,
+    )
     value_unpad = rearrange(value_unpad, 'nnz (h d) -> nnz h d', h=kv_n_heads)
 
-    if (kv_n_heads < n_heads) and (not is_flash_v2_installed()) and (
-            not should_repeat_kv_for_gqa):
+    if (kv_n_heads < n_heads) and (not is_flash_v2_installed()
+                                  ) and (not should_repeat_kv_for_gqa):
         raise ValueError(
-            'For Grouped Query Attention or Multi Query Attention, should_repeat_kv_for_gqa should be set to True if not using Flash Attention v2.'
+            'For Grouped Query Attention or Multi Query Attention, should_repeat_kv_for_gqa should be set to True if not using Flash Attention v2.',
         )
 
     if should_repeat_kv_for_gqa:
         # multi-query case
         if kv_n_heads == 1:
             # Expanding a tensor does not allocate new memory, but only creates a new
             # view on the existing tensor where a dimension of size one is expanded
             # to a larger size by setting the stride to 0.
             # - pytorch docs
             #
             # hopefully the kernels can utilize this and we're jot just wasting BW here
-            key_unpad = key_unpad.expand(key_unpad.size(0), n_heads,
-                                         key_unpad.size(-1))
-            value_unpad = value_unpad.expand(value_unpad.size(0), n_heads,
-                                             value_unpad.size(-1))
+            key_unpad = key_unpad.expand(
+                key_unpad.size(0),
+                n_heads,
+                key_unpad.size(-1),
+            )
+            value_unpad = value_unpad.expand(
+                value_unpad.size(0),
+                n_heads,
+                value_unpad.size(-1),
+            )
         # grouped query case
         elif kv_n_heads < n_heads:
             # Each query belong to a group of kv heads of group size n_heads // kv_n_heads
             # We repeat each kv head by the group size number to use the underlying MHA kernels
 
             # since repeat_kv_for_gqa expects input dims of (b, s, kv_n_heads, d)
             # we use .view to modify {key, value}_unpad appropriately
 
             key_unpad = repeat_kv_for_gqa(
                 key_unpad.view(1, key_unpad.size(0), kv_n_heads, -1),
-                n_heads // kv_n_heads).view(key_unpad.size(0), n_heads, -1)
+                n_heads // kv_n_heads,
+            ).view(key_unpad.size(0), n_heads, -1)
             value_unpad = repeat_kv_for_gqa(
                 value_unpad.view(1, value_unpad.size(0), kv_n_heads, -1),
-                n_heads // kv_n_heads).view(value_unpad.size(0), n_heads, -1)
+                n_heads // kv_n_heads,
+            ).view(value_unpad.size(0), n_heads, -1)
 
     dropout_p = dropout_p if training else 0.0
 
     reset_is_causal = _reset_is_causal(query.size(1), key.size(1), is_causal)
 
     if is_flash_v1_installed():
         output_unpad = flash_attn_interface.flash_attn_unpadded_func(
@@ -305,46 +346,54 @@
             cu_seqlens_q=cu_seqlens_q,
             cu_seqlens_k=cu_seqlens_k,
             max_seqlen_q=max_seqlen_q,
             max_seqlen_k=max_seqlen_k,
             dropout_p=dropout_p,
             softmax_scale=softmax_scale,
             causal=reset_is_causal,
-            return_attn_probs=needs_weights)
+            return_attn_probs=needs_weights,
+        )
     elif is_flash_v2_installed():
         alibi_kwargs = {}
         if check_alibi_support('flash'):
             alibi_kwargs = {'alibi_slopes': alibi_slopes}
         elif alibi_slopes is not None:
             raise ValueError(
-                'alibi_slopes is only supported for flash-attn>=2.4.2')
+                'alibi_slopes is only supported for flash-attn>=2.4.2',
+            )
         output_unpad = flash_attn_interface.flash_attn_varlen_func(
             q=query_unpad,
             k=key_unpad,
             v=value_unpad,
             cu_seqlens_q=cu_seqlens_q,
             cu_seqlens_k=cu_seqlens_k,
             max_seqlen_q=max_seqlen_q,
             max_seqlen_k=max_seqlen_k,
             dropout_p=dropout_p,
             softmax_scale=softmax_scale,
             causal=reset_is_causal,
             return_attn_probs=needs_weights,
             window_size=(sliding_window_size, sliding_window_size),
-            **alibi_kwargs)
+            **alibi_kwargs,
+        )
     else:
         raise RuntimeError(
-            'flash-attn==1.0.9 or flash-attn==2.4.2 is required.')
+            'flash-attn==1.0.9 or flash-attn==2.4.2 is required.',
+        )
 
     output = bert_padding.pad_input(
-        rearrange(output_unpad, 'nnz h d -> nnz (h d)'), indices_q, batch_size,
-        seqlen)
+        rearrange(output_unpad, 'nnz h d -> nnz (h d)'),
+        indices_q,
+        batch_size,
+        seqlen,
+    )
     return output, None, past_key_value
 
 
+@attention_classes.register_class('grouped_query_attention')
 class GroupedQueryAttention(nn.Module):
     """Grouped Query Attention (GQA) is a generalization of Multi-head (MHA).
 
     and Multi-query attention (MQA).
 
     This allows the user to set a variable of number of kv_n_heads, rather than
     just n_heads or 1, as in MHA and MQA. Using torch attention
@@ -383,64 +432,68 @@
         self.head_dim = d_model // n_heads
 
         if self.kv_n_heads <= 0:
             raise ValueError('kv_n_heads should be greater than zero.')
 
         if self.kv_n_heads > self.n_heads:
             raise ValueError(
-                'The number of KV heads should be less than or equal to Q heads.'
+                'The number of KV heads should be less than or equal to Q heads.',
             )
 
         if self.n_heads % self.kv_n_heads != 0:
             raise ValueError(
-                'Each Q head should get the same number of KV heads, so n_heads must be divisible by kv_n_heads.'
+                'Each Q head should get the same number of KV heads, so n_heads must be divisible by kv_n_heads.',
             )
         if qk_ln and qk_gn:
             raise ValueError('Only one of qk_ln and qk_gn can be set to True.')
 
         self.softmax_scale = softmax_scale
         if self.softmax_scale is None:
             self.softmax_scale = 1 / math.sqrt(self.d_model / self.n_heads)
         self.attn_dropout_p = attn_pdrop
 
         fc_kwargs: dict[str, Any] = {
             'bias': bias,
         }
         fc_kwargs['device'] = device
-        self.Wqkv = FC_CLASS_REGISTRY[fc_type](
-            self.d_model,
-            self.d_model + 2 * self.kv_n_heads * self.head_dim,
-            **fc_kwargs,
+        self.Wqkv = build_fc(
+            name=fc_type,
+            in_features=self.d_model,
+            out_features=self.d_model + 2 * self.kv_n_heads * self.head_dim,
+            fc_kwargs=fc_kwargs,
         )
         # for param init fn; enables shape based init of fused layers
         fuse_splits = [
             i * self.head_dim
             for i in range(1, self.n_heads + 2 * self.kv_n_heads)
         ]
         self.Wqkv._fused = (0, fuse_splits)
 
         if self.qk_ln or self.qk_gn:
-            norm_class = NORM_CLASS_REGISTRY[norm_type.lower()]
             norm_size = self.head_dim if qk_gn else d_model
-            self.q_ln = norm_class(norm_size, device=device)
+            self.q_ln = build_norm(
+                name=norm_type.lower(),
+                normalized_shape=norm_size,
+                device=device,
+            )
             if qk_ln:
                 norm_size = self.head_dim * kv_n_heads
-            self.k_ln = norm_class(norm_size, device=device)
+            self.k_ln = build_norm(
+                name=norm_type.lower(),
+                normalized_shape=norm_size,
+                device=device,
+            )
 
-        if self.attn_impl == 'flash':
-            self.attn_fn = flash_attn_fn
-        elif self.attn_impl == 'torch':
-            self.attn_fn = scaled_multihead_dot_product_attention
-        else:
-            raise ValueError(f'{attn_impl=} is an invalid setting.')
+        self.attn_fn = attention_implementations.get(self.attn_impl)
 
-        self.out_proj = FC_CLASS_REGISTRY[fc_type](
-            self.d_model,
-            self.d_model,
-            **fc_kwargs,
+        self.out_proj = build_fc(
+            name=fc_type,
+            in_features=self.d_model,
+            out_features=self.d_model,
+            fc_kwargs=fc_kwargs,
         )
         self.out_proj._is_residual = True
 
     def forward(
         self,
         x: torch.Tensor,
         past_key_value: Optional[tuple[torch.Tensor, torch.Tensor]] = None,
@@ -448,15 +501,15 @@
         attention_mask: Optional[torch.Tensor] = None,
         rotary_emb_w_meta_info: Optional[dict] = None,
         is_causal: bool = True,
         needs_weights: bool = False,
         alibi_slopes: Optional[torch.Tensor] = None,
         flash_attn_padding_info: Optional[dict[str, torch.Tensor]] = None,
     ) -> tuple[torch.Tensor, Optional[torch.Tensor], Optional[tuple[
-            torch.Tensor, torch.Tensor]]]:
+        torch.Tensor, torch.Tensor]]]:
         qkv = self.Wqkv(x)
 
         if self.clip_qkv:
             qkv = qkv.clamp(min=-self.clip_qkv, max=self.clip_qkv)
 
         query, key, value = qkv.split(
             [
@@ -488,50 +541,59 @@
             query = query.view(bsz, seqlen, -1, self.head_dim)
             key = key.view(bsz, seqlen, -1, self.head_dim)
 
             if rotary_emb_w_meta_info['impl'] == 'dail':
                 value = value.view(bsz, seqlen, -1, self.head_dim)
 
                 kv = torch.stack([key, value], dim=2)
-                query, kv = rotary_emb(query,
-                                       kv,
-                                       seqlen_offset=offset_info,
-                                       max_seqlen=seq_len)
+                query, kv = rotary_emb(
+                    query,
+                    kv,
+                    seqlen_offset=offset_info,
+                    max_seqlen=seq_len,
+                )
                 [key, value] = torch.unbind(kv, dim=2)
 
                 value = value.view(bsz, seqlen, self.kv_n_heads * self.head_dim)
             elif rotary_emb_w_meta_info['impl'] == 'hf':
                 if is_transformers_version_gte('4.38'):
-                    (cos, sin) = rotary_emb(x=value,
-                                            position_ids=offset_info,
-                                            seq_len=None)
+                    (cos, sin) = rotary_emb(
+                        x=value,
+                        position_ids=offset_info,
+                    )
                 else:
                     (cos, sin) = rotary_emb(x=value, seq_len=seq_len)
                 if is_transformers_version_gte('4.38'):
-                    query, key = apply_rotary_pos_emb(q=query,
-                                                      k=key,
-                                                      cos=cos,
-                                                      sin=sin,
-                                                      position_ids=None,
-                                                      unsqueeze_dim=2)
+                    query, key = apply_rotary_pos_emb(
+                        q=query,
+                        k=key,
+                        cos=cos,
+                        sin=sin,
+                        position_ids=None,
+                        unsqueeze_dim=2,
+                    )
                 elif is_transformers_version_gte('4.36'):
-                    query, key = apply_rotary_pos_emb(q=query,
-                                                      k=key,
-                                                      cos=cos,
-                                                      sin=sin,
-                                                      position_ids=offset_info,
-                                                      unsqueeze_dim=2)
+                    query, key = apply_rotary_pos_emb(
+                        q=query,
+                        k=key,
+                        cos=cos,
+                        sin=sin,
+                        position_ids=offset_info,
+                        unsqueeze_dim=2,
+                    )
                 else:
                     query = query.transpose(1, 2)
                     key = key.transpose(1, 2)
-                    query, key = apply_rotary_pos_emb(q=query,
-                                                      k=key,
-                                                      cos=cos,
-                                                      sin=sin,
-                                                      position_ids=offset_info)
+                    query, key = apply_rotary_pos_emb(
+                        q=query,
+                        k=key,
+                        cos=cos,
+                        sin=sin,
+                        position_ids=offset_info,
+                    )
                     query = query.transpose(1, 2)
                     key = key.transpose(1, 2)
 
             query = query.view(bsz, seqlen, self.d_model)
             key = key.view(bsz, seqlen, self.kv_n_heads * self.head_dim)
 
         extra_attn_kwargs = {}
@@ -560,14 +622,15 @@
             needs_weights=needs_weights,
             **extra_attn_kwargs,
         )
 
         return self.out_proj(context), attn_weights, past_key_value
 
 
+@attention_classes.register_class('multihead_attention')
 class MultiheadAttention(GroupedQueryAttention):
     """Multi-head self attention.
 
     Using torch attention implementation enables user to also use additive bias.
     """
 
     def __init__(
@@ -600,14 +663,15 @@
             fc_type=fc_type,
             device=device,
             bias=bias,
             sliding_window_size=sliding_window_size,
         )
 
 
+@attention_classes.register_class('multiquery_attention')
 class MultiQueryAttention(GroupedQueryAttention):
     """Multi-Query self attention.
 
     Using torch attention implementation enables user to also use additive bias.
     """
 
     def __init__(
@@ -641,16 +705,21 @@
             device=device,
             bias=bias,
             sliding_window_size=sliding_window_size,
         )
 
 
 def attn_bias_shape(
-        attn_impl: str, n_heads: int, seq_len: int, alibi: bool, causal: bool,
-        use_sequence_id: bool) -> Optional[tuple[int, int, int, int]]:
+    attn_impl: str,
+    n_heads: int,
+    seq_len: int,
+    alibi: bool,
+    causal: bool,
+    use_sequence_id: bool,
+) -> Optional[tuple[int, int, int, int]]:
     if attn_impl == 'flash':
         return None
     elif attn_impl == 'torch':
         if alibi:
             if (not causal) or use_sequence_id:
                 return (1, n_heads, seq_len, seq_len)
             return (1, n_heads, 1, seq_len)
@@ -680,24 +749,27 @@
                 build_alibi_bias(
                     n_heads,
                     seq_len,
                     full=not causal,
                     alibi_bias_max=alibi_bias_max,
                     device=device,
                     dtype=dtype,
-                ))
+                ),
+            )
         return attn_bias
     else:
         raise ValueError(f'{attn_impl=} is an invalid setting.')
 
 
-def gen_slopes(n_heads: int,
-               alibi_bias_max: int = 8,
-               device: Optional[torch.device] = None,
-               return_1d: bool = False) -> torch.Tensor:
+def gen_slopes(
+    n_heads: int,
+    alibi_bias_max: int = 8,
+    device: Optional[torch.device] = None,
+    return_1d: bool = False,
+) -> torch.Tensor:
     _n_heads = 2**math.ceil(math.log2(n_heads))
     m = torch.arange(1, _n_heads + 1, dtype=torch.float32, device=device)
     m = m.mul(alibi_bias_max / _n_heads)
     slopes = (1. / torch.pow(2, m))
 
     if _n_heads != n_heads:
         # if n_heads is not a power of two,
@@ -719,21 +791,24 @@
 ) -> torch.Tensor:
     alibi_bias = torch.arange(1 - seq_len, 1, dtype=torch.int32,
                               device=device).view(1, 1, 1, seq_len)
     if full:
         # generate 1 x Heads x SeqLen x SeqLen alibi bias mask
         # otherwise the mask is 1 x Heads x 1 x SeqLen (which is broadcast to the appropriate size)
         alibi_bias = alibi_bias - torch.arange(
-            1 - seq_len, 1, dtype=torch.int32, device=device).view(
-                1, 1, seq_len, 1)
+            1 - seq_len,
+            1,
+            dtype=torch.int32,
+            device=device,
+        ).view(1, 1, seq_len, 1)
         alibi_bias = alibi_bias.abs().mul(-1)
 
     slopes = gen_slopes(n_heads, alibi_bias_max, device=device)
     alibi_bias = alibi_bias * slopes
     return alibi_bias.to(dtype=dtype)
 
 
-ATTN_CLASS_REGISTRY = {
-    'multihead_attention': MultiheadAttention,
-    'multiquery_attention': MultiQueryAttention,
-    'grouped_query_attention': GroupedQueryAttention
-}
+attention_implementations.register('flash', func=flash_attn_fn)
+attention_implementations.register(
+    'torch',
+    func=scaled_multihead_dot_product_attention,
+)
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/layers/norm.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/layers/norm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
-from typing import Dict, List, Optional, Type, Union
+from typing import List, Optional, Union
 
 import torch
 
+from llmfoundry.layers_registry import norms
+
+__all__ = [
+    'LPLayerNorm',
+    'LPRMSNorm',
+    'RMSNorm',
+    'TritonRMSNorm',
+    'rms_norm',
+]
+
+norms.register(name='layernorm', func=torch.nn.LayerNorm)
+
 
 def _cast_if_autocast_enabled(tensor: torch.Tensor) -> torch.Tensor:
     if torch.is_autocast_enabled():
         if tensor.device.type == 'cuda':
             dtype = torch.get_autocast_gpu_dtype()
         elif tensor.device.type == 'cpu':
             dtype = torch.get_autocast_cpu_dtype()
         else:
             raise NotImplementedError()
         return tensor.to(dtype=dtype)
     return tensor
 
 
+@norms.register_class('low_precision_layernorm')
 class LPLayerNorm(torch.nn.LayerNorm):
 
     def __init__(
         self,
         normalized_shape: Union[int, List[int], torch.Size],
         eps: float = 1e-05,
         elementwise_affine: bool = True,
@@ -36,58 +49,65 @@
             dtype=dtype,
         )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         module_device = x.device
         downcast_x = _cast_if_autocast_enabled(x)
         downcast_weight = _cast_if_autocast_enabled(
-            self.weight) if self.weight is not None else self.weight
+            self.weight,
+        ) if self.weight is not None else self.weight
         downcast_bias = _cast_if_autocast_enabled(
-            self.bias) if self.bias is not None else self.bias
+            self.bias,
+        ) if self.bias is not None else self.bias
         with torch.autocast(enabled=False, device_type=module_device.type):
             return torch.nn.functional.layer_norm(
                 downcast_x,
                 self.normalized_shape,
                 downcast_weight,
                 downcast_bias,
                 self.eps,
             )
 
 
-def rms_norm(x: torch.Tensor,
-             weight: Optional[torch.Tensor] = None,
-             eps: float = 1e-5) -> torch.Tensor:
+def rms_norm(
+    x: torch.Tensor,
+    weight: Optional[torch.Tensor] = None,
+    eps: float = 1e-5,
+) -> torch.Tensor:
     output = x * torch.rsqrt(x.pow(2).mean(-1, keepdim=True) + eps)
     if weight is not None:
         return output * weight
     return output
 
 
+@norms.register_class('rmsnorm')
 class RMSNorm(torch.nn.Module):
 
     def __init__(
         self,
         normalized_shape: Union[int, List[int], torch.Size],
         eps: float = 1e-5,
         weight: bool = True,
         dtype: Optional[torch.dtype] = None,
         device: Optional[torch.device] = None,
     ):
         super().__init__()
         self.eps = eps
         if weight:
             self.weight = torch.nn.Parameter(
-                torch.ones(normalized_shape, dtype=dtype, device=device))
+                torch.ones(normalized_shape, dtype=dtype, device=device),
+            )
         else:
             self.register_parameter('weight', None)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         return rms_norm(x.float(), self.weight, self.eps).to(dtype=x.dtype)
 
 
+@norms.register_class('low_precision_rmsnorm')
 class LPRMSNorm(RMSNorm):
 
     def __init__(
         self,
         normalized_shape: Union[int, List[int], torch.Size],
         eps: float = 1e-5,
         weight: bool = True,
@@ -101,19 +121,56 @@
             dtype=dtype,
             device=device,
         )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         downcast_x = _cast_if_autocast_enabled(x)
         downcast_weight = _cast_if_autocast_enabled(
-            self.weight) if self.weight is not None else self.weight
+            self.weight,
+        ) if self.weight is not None else self.weight
         with torch.autocast(enabled=False, device_type=x.device.type):
             return rms_norm(downcast_x, downcast_weight,
                             self.eps).to(dtype=x.dtype)
 
 
-NORM_CLASS_REGISTRY: Dict[str, Type[torch.nn.Module]] = {
-    'layernorm': torch.nn.LayerNorm,
-    'low_precision_layernorm': LPLayerNorm,
-    'rmsnorm': RMSNorm,
-    'low_precision_rmsnorm': LPRMSNorm,
-}
+@norms.register_class('triton_rmsnorm')
+class TritonRMSNorm(torch.nn.Module):
+
+    def __init__(
+        self,
+        normalized_shape: Union[int, List[int], torch.Size],
+        eps: float = 1e-5,
+        device: Optional[torch.device] = None,
+        dtype: Optional[torch.dtype] = None,
+    ):
+        super().__init__()
+        self.eps = eps
+
+        try:
+            from flash_attn.ops.triton.layer_norm import rms_norm_fn
+        except ImportError:
+            raise ImportError(
+                'triton_rms_norm requires Flash Attention to be installed. ' +
+                'Please pip install flash-attn.',
+            )
+
+        if not isinstance(normalized_shape, int):
+            raise ValueError('TritonRMSNorm only supports 1D tensors')
+
+        self.rms_norm_fn = rms_norm_fn
+
+        self.weight = torch.nn.Parameter(
+            torch.ones(normalized_shape, device=device, dtype=dtype),
+        )
+
+    def forward(self, x: torch.Tensor):
+        # Flash Attention expect a flat tensor
+        return self.rms_norm_fn(
+            x,
+            self.weight,
+            None,  # no bias
+            residual=None,
+            eps=self.eps,
+            dropout_p=0.0,  # no dropout by default
+            prenorm=False,
+            residual_in_fp32=False,
+        )
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/mpt/configuration_mpt.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/mpt/configuration_mpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,30 @@
 """A HuggingFace-style model configuration."""
 
 import warnings
 from typing import Any, Dict, Optional, Union
 
 from transformers import PretrainedConfig
 
-from llmfoundry.models.layers.attention import (check_alibi_support,
-                                                is_flash_v2_installed)
+from llmfoundry.layers_registry import ffns_with_megablocks
+from llmfoundry.models.layers.attention import (
+    check_alibi_support,
+    is_flash_v2_installed,
+)
 from llmfoundry.models.layers.blocks import attn_config_defaults
 
 # NOTE: All utils are imported directly even if unused so that
 # HuggingFace can detect all the needed files to copy into its modules folder.
 # Otherwise, certain modules are missing.
 # isort: off
-from llmfoundry.models.layers.fc import FC_CLASS_REGISTRY  # type: ignore (see note)
 from llmfoundry.models.layers.norm import LPLayerNorm  # type: ignore (see note)
-from llmfoundry.models.layers.ffn import FFN_CLASS_REGISTRY  # type: ignore (see note)
+from llmfoundry.models.layers.layer_builders import build_norm, build_fc, build_ffn  # type: ignore (see note)
+from llmfoundry.models.layers.dmoe import dMoE  # type: ignore (see note)
+from llmfoundry.layers_registry import norms  # type: ignore (see note)
+from llmfoundry.utils.registry_utils import construct_from_registry  # type: ignore (see note)
 
 ffn_config_defaults: Dict = {
     'ffn_type': 'mptmlp',
 }
 
 init_config_defaults: Dict = {
     'name': 'kaiming_normal_',
@@ -152,38 +157,43 @@
         self.fc_type = fc_type
         self.use_pad_tok_in_ffn = use_pad_tok_in_ffn
 
         if 'name' in kwargs:
             del kwargs['name']
         if 'loss_fn' in kwargs:
             del kwargs['loss_fn']
-        if self.attn_config.get('alibi', False) or self.attn_config.get(
-                'rope', False):
+        if self.attn_config.get('alibi',
+                                False) or self.attn_config.get('rope', False):
             self.learned_pos_emb = False
             warnings.warn(
-                f'alibi or rope is turned on, setting `learned_pos_emb` to `False.`'
+                f'alibi or rope is turned on, setting `learned_pos_emb` to `False.`',
             )
         # tie_word_embeddings is set in Huggingface's PretrainedConfig __init__
         super().__init__(
             tie_word_embeddings=tie_word_embeddings,
             **kwargs,
         )
 
         self._validate_config()
 
-    def _set_config_defaults(self, config: Dict[str, Any],
-                             config_defaults: Dict[str, Any]) -> Dict[str, Any]:
+    def _set_config_defaults(
+        self,
+        config: Dict[str, Any],
+        config_defaults: Dict[str, Any],
+    ) -> Dict[str, Any]:
         # set config defaults
         for k, v in config_defaults.items():
             if k not in config:
                 config[k] = v
             elif isinstance(v, dict):
                 # recursively set default values for any sub-dicts
                 config[k] = self._set_config_defaults(
-                    config[k] if (config[k] is not None) else {}, v)
+                    config[k] if (config[k] is not None) else {},
+                    v,
+                )
         return config
 
     def _validate_config(self) -> None:
         # set config defaults
         self.attn_config = self._set_config_defaults(
             self.attn_config,
             attn_config_defaults,
@@ -196,107 +206,124 @@
             self.init_config,
             init_config_defaults,
         )
 
         if self.d_model % self.n_heads != 0:
             raise ValueError('d_model must be divisible by n_heads')
         if any(
-                prob < 0 or prob > 1 for prob in
-            [self.attn_config['attn_pdrop'], self.resid_pdrop, self.emb_pdrop]):
+            prob < 0 or prob > 1 for prob in
+            [self.attn_config['attn_pdrop'], self.resid_pdrop, self.emb_pdrop]
+        ):
             raise ValueError(
-                "self.attn_config['attn_pdrop'], resid_pdrop, emb_pdrop are probabilities and must be between 0 and 1"
+                "self.attn_config['attn_pdrop'], resid_pdrop, emb_pdrop are probabilities and must be between 0 and 1",
             )
         if self.attn_config['attn_impl'] not in ['torch', 'flash']:
             raise ValueError(
-                f"Unknown attn_impl={self.attn_config['attn_impl']}")
+                f"Unknown attn_impl={self.attn_config['attn_impl']}",
+            )
         if self.attn_config['alibi'] and not check_alibi_support(
-                self.attn_config['attn_impl']):
+            self.attn_config['attn_impl'],
+        ):
             raise NotImplementedError(
-                'alibi only implemented with torch and flash (v2.4.2 or higher) attention.'
+                'alibi only implemented with torch and flash (v2.4.2 or higher) attention.',
             )
         if self.attn_config['attn_uses_sequence_id'] and not (
-                self.attn_config['attn_impl'] == 'torch' or
-            (self.attn_config['attn_impl'] == 'flash' and
-             is_flash_v2_installed(v2_version='v2.1.2'))):
+            self.attn_config['attn_impl'] == 'torch' or (
+                self.attn_config['attn_impl'] == 'flash' and
+                is_flash_v2_installed(v2_version='v2.1.2')
+            )
+        ):
             raise NotImplementedError(
-                'attn_uses_sequence_id only implemented with torch and flash (v2.1.2 or higher) attention.'
+                'attn_uses_sequence_id only implemented with torch and flash (v2.1.2 or higher) attention.',
             )
-        if self.attn_config['rope'] and (self.attn_config['rope_impl']
-                                         not in ['dail', 'hf']):
+        if self.attn_config['rope'] and (
+            self.attn_config['rope_impl'] not in ['dail', 'hf']
+        ):
             raise ValueError(
-                'If rope is being used then rope_impl should be either "dail", or "hf".'
+                'If rope is being used then rope_impl should be either "dail", or "hf".',
             )
         if self.attn_config['rope'] and (
-                self.attn_config['rope_impl']
-                == 'hf') and self.attn_config['rope_hf_config']['type'] not in [
-                    'no_scaling', 'linear', 'dynamic'
-                ]:
+            self.attn_config['rope_impl'] == 'hf'
+        ) and self.attn_config['rope_hf_config']['type'] not in [
+            'no_scaling',
+            'linear',
+            'dynamic',
+        ]:
             raise ValueError(
-                'If using hf implementation of rope, the type should be one of "no_scaling", "linear" or "dynamic".'
+                'If using hf implementation of rope, the type should be one of "no_scaling", "linear" or "dynamic".',
             )
-        if self.attn_config['rope'] and (self.attn_config['rope_impl']
-                                         == 'dail'):
+        if self.attn_config['rope'] and (
+            self.attn_config['rope_impl'] == 'dail'
+        ):
             if self.attn_config['rope_dail_config']['type'] not in [
-                    'original', 'xpos'
+                'original',
+                'xpos',
             ]:
                 raise ValueError(
-                    'If using the dail implementation of rope, the type should be one of "original" or "xpos".'
+                    'If using the dail implementation of rope, the type should be one of "original" or "xpos".',
                 )
             if not is_flash_v2_installed(v2_version='2.0.1'):
                 raise ImportError(
-                    'If using the dail implementation of rope, the flash_attn library v2.0.1 or higher must be installed. Please check the instructions at https://github.com/mosaicml/llm-foundry/blob/main/TUTORIAL.md#what-kinds-of-positional-embeddings-does-llm-foundry-support'
+                    'If using the dail implementation of rope, the flash_attn library v2.0.1 or higher must be installed. Please check the instructions at https://github.com/mosaicml/llm-foundry/blob/main/TUTORIAL.md#what-kinds-of-positional-embeddings-does-llm-foundry-support',
                 )
         if self.attn_config['sliding_window_size'] != -1 and not (
-                self.attn_config['attn_impl'] == 'flash' and
-                is_flash_v2_installed(v2_version='v2.3.0')):
+            self.attn_config['attn_impl'] == 'flash' and
+            is_flash_v2_installed(v2_version='v2.3.0')
+        ):
             raise NotImplementedError(
-                'sliding window only implemented with flash attention v2.3.0 or higher.'
+                'sliding window only implemented with flash attention v2.3.0 or higher.',
             )
         if self.embedding_fraction > 1 or self.embedding_fraction <= 0:
             raise ValueError(
-                'model.embedding_fraction must be between 0 (exclusive) and 1 (inclusive)!'
+                'model.embedding_fraction must be between 0 (exclusive) and 1 (inclusive)!',
             )
-        if isinstance(self.logit_scale,
-                      str) and self.logit_scale != 'inv_sqrt_d_model':
+        if isinstance(
+            self.logit_scale,
+            str,
+        ) and self.logit_scale != 'inv_sqrt_d_model':
             raise ValueError(
-                f"{self.logit_scale=} is not recognized as an option; use numeric value or 'inv_sqrt_d_model'."
+                f"{self.logit_scale=} is not recognized as an option; use numeric value or 'inv_sqrt_d_model'.",
             )
         if self.init_config.get('name', None) is None:
             raise ValueError(f"{self.init_config=} 'name' needs to be set.")
-        if not (self.learned_pos_emb or self.attn_config['alibi'] or
-                self.attn_config['rope']):
+        if not (
+            self.learned_pos_emb or self.attn_config['alibi'] or
+            self.attn_config['rope']
+        ):
             warnings.warn(
-                f'Positional information not being provided to the model using either learned_pos_emb or alibi or rope.'
+                f'Positional information not being provided to the model using either learned_pos_emb or alibi or rope.',
             )
         if self.fc_type == 'te' or self.ffn_config['ffn_type'] == 'te_ln_mlp':
             try:
                 import transformer_engine.pytorch as te
                 del te  # unused
             except:
                 raise ImportError(
                     'TransformerEngine import fail. `fc_type: te` requires TransformerEngine be installed. '
                     +
                     'The required version of transformer_engine also requires FlashAttention v1.0.6 is installed:\n'
                     + 'pip install flash-attn==1.0.6 --no-build-isolation \n' +
-                    'pip install git+https://github.com/NVIDIA/TransformerEngine.git@144e4888b2cdd60bd52e706d5b7a79cb9c1a7156'
+                    'pip install git+https://github.com/NVIDIA/TransformerEngine.git@144e4888b2cdd60bd52e706d5b7a79cb9c1a7156',
                 )
         if self.ffn_config['ffn_type'] == 'mptgeglu':
             raise ValueError(
                 'API CHANGE: `ffn_type=="mptgeglu"` changed to `ffn_type=="mptglu"`. '
                 +
-                'See [#829](https://github.com/mosaicml/llm-foundry/pull/829) for details.'
+                'See [#829](https://github.com/mosaicml/llm-foundry/pull/829) for details.',
             )
         elif self.ffn_config['ffn_type'] in ['mptmlp', 'mptglu']:
             self.ffn_config['fc_type'] = self.fc_type
+        elif self.ffn_config['ffn_type'] in ffns_with_megablocks:
+            self.ffn_config['return_bias'] = False
         elif self.ffn_config['ffn_type'] == 'te_ln_mlp':
             self.ffn_config['bias'] = not self.no_bias
             if 'ffn_act_fn' in self.ffn_config.keys():
                 raise ValueError(
-                    f'Transformer Engine block does not support custom activation functions.'
+                    f'Transformer Engine block does not support custom activation functions.',
                 )
         if not self.use_pad_tok_in_ffn:
             try:
                 from flash_attn.bert_padding import unpad_input, pad_input  # type: ignore # yapf: disable # isort: skip
             except:
                 raise ImportError(
-                    'In order to set `use_pad_tok_in_ffn=False`, please install flash-attn==1.0.9 or flash-attn==2.3.6'
+                    'In order to set `use_pad_tok_in_ffn=False`, please install flash-attn==1.0.9 or flash-attn==2.3.6',
                 )
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/mpt/modeling_mpt.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/mpt/modeling_mpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,76 +6,103 @@
 Inspired by https://github.com/karpathy/minGPT/blob/master/mingpt/model.py
 """
 
 from __future__ import annotations
 
 import math
 import warnings
-from typing import (Any, Dict, List, Mapping, MutableMapping, Optional, Tuple,
-                    Union)
+from functools import cached_property
+from typing import (
+    Any,
+    Dict,
+    List,
+    Mapping,
+    MutableMapping,
+    Optional,
+    Tuple,
+    Union,
+)
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from composer.models import HuggingFaceModel
 from composer.utils import dist
 
+from llmfoundry.layers_registry import ffns_with_megablocks
 from llmfoundry.models.layers.attention import is_flash_v2_installed
-from llmfoundry.models.layers.norm import NORM_CLASS_REGISTRY
 
 if is_flash_v2_installed():
     try:  # This try...except is needed because transformers requires it despite the 'if' statement above
         from flash_attn import bert_padding
         from flash_attn.layers.rotary import \
             RotaryEmbedding as DAILRotaryEmbedding
     except Exception as e:
         raise e
 
 from omegaconf import DictConfig
 from omegaconf import OmegaConf as om
 from transformers import PreTrainedModel, PreTrainedTokenizerBase
-from transformers.modeling_outputs import (BaseModelOutputWithPast,
-                                           CausalLMOutputWithPast)
+from transformers.modeling_outputs import (
+    BaseModelOutputWithPast,
+    CausalLMOutputWithPast,
+)
 from transformers.models.llama.modeling_llama import \
     LlamaDynamicNTKScalingRotaryEmbedding as HFDynamicNTKScalingRotaryEmbedding
 from transformers.models.llama.modeling_llama import \
     LlamaLinearScalingRotaryEmbedding as HFLinearScalingRotaryEmbedding
 from transformers.models.llama.modeling_llama import \
     LlamaRotaryEmbedding as HFRotaryEmbedding
 
-from llmfoundry.models.layers.attention import (attn_bias_shape,
-                                                build_attn_bias, gen_slopes)
+from llmfoundry.layers_registry import norms, param_init_fns
+from llmfoundry.models.layers.attention import (
+    attn_bias_shape,
+    build_attn_bias,
+    gen_slopes,
+)
 from llmfoundry.models.layers.blocks import MPTBlock
 from llmfoundry.models.layers.custom_embedding import SharedEmbedding
-from llmfoundry.models.layers.ffn import build_ffn as build_ffn
+from llmfoundry.models.layers.layer_builders import build_norm
 from llmfoundry.models.mpt.configuration_mpt import MPTConfig
+from llmfoundry.models.utils.config_moe_args import config_moe_args
+from llmfoundry.models.utils.mpt_param_count import (
+    mpt_get_active_params,
+    mpt_get_total_params,
+)
 
 # NOTE: All utils are imported directly even if unused so that
 # HuggingFace can detect all the needed files to copy into its modules folder.
 # Otherwise, certain modules are missing.
 # isort: off
 from llmfoundry.models.utils.meta_init_context import \
     init_empty_weights  # type: ignore (see note)
 from llmfoundry.models.utils.param_init_fns import (
     generic_param_init_fn_,  # type: ignore (see note)
-    MODEL_INIT_REGISTRY,
 )
+from llmfoundry.models.layers.ffn import resolve_ffn_act_fn  # type: ignore (see note)
 
-from llmfoundry.models.utils.act_ckpt import (pass_on_block_idx,
-                                              build_act_ckpt_mod_to_blocks,
-                                              check_mapping_blocks_overlap)
+from llmfoundry.models.utils.act_ckpt import (
+    pass_on_block_idx,
+    build_act_ckpt_mod_to_blocks,
+    check_mapping_blocks_overlap,
+)
 
 import logging
 
 log = logging.getLogger(__name__)
 
 
-def gen_rotary_embedding(rope_head_dim: int, rope_impl: str, rope_theta: int,
-                         rope_dail_config: dict, rope_hf_config: dict,
-                         max_seq_len: int):
+def gen_rotary_embedding(
+    rope_head_dim: int,
+    rope_impl: str,
+    rope_theta: int,
+    rope_dail_config: dict,
+    rope_hf_config: dict,
+    max_seq_len: int,
+):
     if rope_impl == 'dail':
         return DAILRotaryEmbedding(
             dim=rope_head_dim,
             base=rope_theta,
             interleaved=False,
             scale_base=rope_dail_config['xpos_scale_base'] if
             (rope_dail_config['type'] == 'xpos') else None,
@@ -86,40 +113,44 @@
     elif rope_impl == 'hf':
         if rope_hf_config['type'] == 'no_scaling':
             return HFRotaryEmbedding(
                 rope_head_dim,
                 max_position_embeddings=max_seq_len,
                 base=rope_theta,
                 device=
-                'cpu'  # FSDP does not materialize modules with meta buffers, hence device is set to cpu
+                'cpu',  # FSDP does not materialize modules with meta buffers, hence device is set to cpu
             )
         elif rope_hf_config['type'] == 'linear':
             return HFLinearScalingRotaryEmbedding(
                 rope_head_dim,
                 max_position_embeddings=max_seq_len,
                 base=rope_theta,
                 scaling_factor=rope_hf_config['factor'],
                 device=
-                'cpu'  # FSDP does not materialize modules with meta buffers, hence device is set to cpu
+                'cpu',  # FSDP does not materialize modules with meta buffers, hence device is set to cpu
             )
         elif rope_hf_config['type'] == 'dynamic':
             return HFDynamicNTKScalingRotaryEmbedding(
                 rope_head_dim,
                 max_position_embeddings=max_seq_len,
                 base=rope_theta,
                 scaling_factor=rope_hf_config['factor'],
                 device=
-                'cpu'  # FSDP does not materialize modules with meta buffers, hence device is set to cpu
+                'cpu',  # FSDP does not materialize modules with meta buffers, hence device is set to cpu
             )
     raise ValueError('rope_impl needs to be either dail or hf')
 
 
-def gen_attention_mask_in_length(sequence_id: Union[None, torch.Tensor], S: int,
-                                 attn_uses_sequence_id: bool, attn_impl: str,
-                                 attention_mask: Union[torch.Tensor, None]):
+def gen_attention_mask_in_length(
+    sequence_id: Union[None, torch.Tensor],
+    S: int,
+    attn_uses_sequence_id: bool,
+    attn_impl: str,
+    attention_mask: Union[torch.Tensor, None],
+):
     """Generates the attention mask used for sequence masking in FA v2.
 
     Only supports sequence id based sparse attention for no attention masking or attention masking with right padding.
     In case of left padding:
         1. Training with left padding is not supported in MPT (see https://github.com/mosaicml/llm-foundry/blob/1eecd4cb8e734499f77f6a35f657b8b20c0adfcb/llmfoundry/models/mpt/modeling_mpt.py#L407).
         2. For generation with left padding, we only have a single sequence id per sample, so we don't need sequence id based sparse attention.
 
@@ -167,52 +198,56 @@
                 [1, 1, 1, 1, 1, 1]
             ]
             ]
             ```.
             (The description above is taken verbatim from https://github.com/Dao-AILab/flash-attention/blob/9356a1c0389660d7e231ff3163c1ac17d9e3824a/flash_attn/bert_padding.py#L125 .)
     """
     attention_mask_in_length = None
-    if (sequence_id is not None) and attn_uses_sequence_id and (attn_impl
-                                                                == 'flash'):
+    if (sequence_id
+        is not None) and attn_uses_sequence_id and (attn_impl == 'flash'):
         # Check if sequence has left padding. If yes, raise an error.
-        if (attention_mask is not None) and (attention_mask[:, 0].sum() !=
-                                             attention_mask.shape[0]):
+        if (attention_mask is not None
+           ) and (attention_mask[:, 0].sum() != attention_mask.shape[0]):
             raise NotImplementedError(
-                'Left padding is not supported with flash attention when attn_uses_sequence_id is set to True.'
+                'Left padding is not supported with flash attention when attn_uses_sequence_id is set to True.',
             )
         if S != sequence_id.shape[-1]:
             raise ValueError(
-                f'Sequence length ({S}) does not match length of sequences in sequence_id ({sequence_id.shape[-1]}).'
+                f'Sequence length ({S}) does not match length of sequences in sequence_id ({sequence_id.shape[-1]}).',
             )
         if attention_mask is not None:
             # -1 is used to pad the sequence_id where attention mask is False (https://github.com/mosaicml/llm-foundry/blob/706ea7dd40ba60a98dea5f37695d143d91c98b6c/llmfoundry/data/packing.py#L249).
             # We replace those -1 with 0 to prevent `torch.nn.functional.one_hot(sequence_id)` in the next line from failing.
             # We apply the attention mask again after the one_hot operation.
             sequence_id = sequence_id.masked_fill(~attention_mask, 0)
         attention_mask_in_length = torch.nn.functional.one_hot(sequence_id)
         if attention_mask is not None:
             attention_mask_in_length = attention_mask_in_length.masked_fill(
-                ~attention_mask.unsqueeze(-1), 0)
+                ~attention_mask.unsqueeze(-1),
+                0,
+            )
         attention_mask_in_length = attention_mask_in_length.sum(dim=1)
         attention_mask_in_length = torch.nn.functional.pad(
             attention_mask_in_length,
             (0, S - attention_mask_in_length.shape[-1]),
             mode='constant',
-            value=0)
+            value=0,
+        )
 
     return attention_mask_in_length
 
 
 def gen_flash_attn_padding_info(
-        bsz: int,
-        S: int,
-        past_key_len: int,
-        device: torch.device,
-        attention_mask_in_length: Optional[torch.Tensor] = None,
-        attention_mask: Optional[torch.Tensor] = None):
+    bsz: int,
+    S: int,
+    past_key_len: int,
+    device: torch.device,
+    attention_mask_in_length: Optional[torch.Tensor] = None,
+    attention_mask: Optional[torch.Tensor] = None,
+):
     flash_attn_padding_info = {}
     if attention_mask_in_length is None:
         key_padding_mask = attention_mask
         if key_padding_mask is None:
             key_padding_mask = torch.ones((bsz, past_key_len + S),
                                           dtype=torch.bool,
                                           device=device)
@@ -220,48 +255,58 @@
         unpadding_function = bert_padding.unpad_input
     else:
         key_padding_mask = attention_mask_in_length
         query_padding_mask = attention_mask_in_length
         unpadding_function = bert_padding.unpad_input_for_concatenated_sequences
 
     _, indices_q, cu_seqlens_q, max_seqlen_q = unpadding_function(
-        torch.empty(bsz, S, 1, device=device), query_padding_mask)
+        torch.empty(bsz, S, 1, device=device),
+        query_padding_mask,
+    )
     _, indices_k, cu_seqlens_k, max_seqlen_k = unpadding_function(
-        torch.empty(bsz, past_key_len + S, 1, device=device), key_padding_mask)
+        torch.empty(bsz, past_key_len + S, 1, device=device),
+        key_padding_mask,
+    )
     _, indices_v, _, _ = unpadding_function(
-        torch.empty(bsz, past_key_len + S, 1, device=device), key_padding_mask)
+        torch.empty(bsz, past_key_len + S, 1, device=device),
+        key_padding_mask,
+    )
 
     flash_attn_padding_info['indices_q'] = indices_q
     flash_attn_padding_info['indices_k'] = indices_k
     flash_attn_padding_info['indices_v'] = indices_v
     flash_attn_padding_info['cu_seqlens_q'] = cu_seqlens_q
     flash_attn_padding_info['cu_seqlens_k'] = cu_seqlens_k
     flash_attn_padding_info['max_seqlen_q'] = max_seqlen_q
     flash_attn_padding_info['max_seqlen_k'] = max_seqlen_k
     return flash_attn_padding_info
 
 
-def apply_sequence_id(attn_bias: torch.Tensor, sequence_id: torch.LongTensor,
-                      max_seq_len: int) -> torch.Tensor:
+def apply_sequence_id(
+    attn_bias: torch.Tensor,
+    sequence_id: torch.LongTensor,
+    max_seq_len: int,
+) -> torch.Tensor:
     seq_len = sequence_id.shape[-1]
     if seq_len > max_seq_len:
         raise ValueError(
-            f'sequence_id sequence length cannot exceed max_seq_len={max_seq_len}'
+            f'sequence_id sequence length cannot exceed max_seq_len={max_seq_len}',
         )
 
     # select seq_len subset of attn mask
     attn_bias = attn_bias[..., :seq_len, :seq_len]
 
     # Restrict attention to tokens that share the same value
     # in sequence_id
     cannot_attend = torch.logical_not(
         torch.eq(
             sequence_id.view(-1, seq_len, 1),
             sequence_id.view(-1, 1, seq_len),
-        )).unsqueeze(1)
+        ),
+    ).unsqueeze(1)
     min_val = torch.finfo(attn_bias.dtype).min
     attn_bias = attn_bias.masked_fill(cannot_attend, min_val)
 
     return attn_bias
 
 
 class MPTPreTrainedModel(PreTrainedModel):
@@ -271,14 +316,16 @@
 
 
 def _fsdp_wrap_fn(
     self: Union[MPTModel, MPTForCausalLM],
     module: nn.Module,
 ) -> bool:
     # FSDP Wrap function for MPT Models
+    if hasattr(module, '_fsdp_kwargs_dict'):
+        return module._fsdp_kwargs_dict
     return isinstance(module, MPTBlock)
 
 
 class MPTModel(MPTPreTrainedModel):
 
     def __init__(self, config: MPTConfig):
         config._validate_config()
@@ -293,63 +340,82 @@
 
         if config.init_device == 'mixed':
             if dist.get_local_rank() == 0:
                 config.init_device = 'cpu'
             else:
                 config.init_device = 'meta'
 
-        if config.norm_type.lower() not in NORM_CLASS_REGISTRY.keys():
-            norm_options = ' | '.join(NORM_CLASS_REGISTRY.keys())
+        if config.norm_type.lower() not in norms.get_all():
+            norm_options = ' | '.join(norms.get_all())
             raise NotImplementedError(
-                f'Requested norm type ({config.norm_type}) is not implemented within this repo (Options: {norm_options}).'
+                f'Requested norm type ({config.norm_type}) is not implemented within this repo (Options: {norm_options}).',
             )
-        norm_class = NORM_CLASS_REGISTRY[config.norm_type.lower()]
 
         # CogView (https://arxiv.org/abs/2105.13290) and GLM-130B (https://arxiv.org/abs/2210.02414)
         # both report this helping with stabilizing training
         self.embedding_fraction = config.embedding_fraction
 
-        self.wte = SharedEmbedding(config.vocab_size,
-                                   config.d_model,
-                                   device=config.init_device)
+        self.wte = SharedEmbedding(
+            config.vocab_size,
+            config.d_model,
+            device=config.init_device,
+        )
         if self.learned_pos_emb:
-            self.wpe = torch.nn.Embedding(config.max_seq_len,
-                                          config.d_model,
-                                          device=config.init_device)
+            self.wpe = torch.nn.Embedding(
+                config.max_seq_len,
+                config.d_model,
+                device=config.init_device,
+            )
         self.emb_drop = nn.Dropout(config.emb_pdrop)
+        self.mb_args = None
+        block_args = config.to_dict()
+        if block_args['ffn_config']['ffn_type'] in ffns_with_megablocks:
+            block_args['ffn_config'] = config_moe_args(
+                block_args['ffn_config'],
+                config.d_model,
+                config.expansion_ratio,
+                config.n_layers,
+            )
+            self.mb_args = block_args['ffn_config'].get('args')
+
         self.blocks = nn.ModuleList([
             MPTBlock(
                 device=config.init_device,
-                **config.to_dict(),
+                **block_args,
             ) for _ in range(config.n_layers)
         ])
 
         # Tag all modules in the transformer blocks with the corresponding block_idx and max_block_idx
         for i, block in enumerate(self.blocks):
             block.block_idx = i
             block.max_block_idx = config.n_layers - 1
             pass_on_block_idx(block)
 
-        self.norm_f = norm_class(config.d_model, device=config.init_device)
+        self.norm_f = build_norm(
+            name=config.norm_type.lower(),
+            normalized_shape=config.d_model,
+            device=config.init_device,
+        )
 
         self.rope = config.attn_config['rope']
         self.rope_impl = None
         if self.rope:
             self.rope_impl = config.attn_config['rope_impl']
             self.rotary_embedding = gen_rotary_embedding(
                 rope_head_dim=config.d_model // config.n_heads,
                 rope_impl=self.rope_impl,
                 rope_theta=config.attn_config['rope_theta'],
                 rope_dail_config=config.attn_config['rope_dail_config'],
                 rope_hf_config=config.attn_config['rope_hf_config'],
-                max_seq_len=self.config.max_seq_len)
+                max_seq_len=self.config.max_seq_len,
+            )
 
         if config.init_device != 'meta':
             log.info(
-                f'We recommend using config.init_device="meta" with Composer + FSDP for faster initialization.'
+                f'We recommend using config.init_device="meta" with Composer + FSDP for faster initialization.',
             )
             self.apply(self.param_init_fn)
 
         self.is_causal = True
 
         # define attn mask
         self._attn_bias_initialized = False
@@ -361,47 +427,51 @@
             self.alibi,
             causal=self.is_causal,
             use_sequence_id=self.attn_uses_sequence_id,
         )
 
         if config.no_bias:
             for module in self.modules():
-                if hasattr(module, 'bias') and isinstance(
-                        module.bias, nn.Parameter):
-                    log.info(f'Removing bias from {module=}.')
+                if hasattr(module,
+                           'bias') and isinstance(module.bias, nn.Parameter):
+                    log.debug(f'Removing bias from {module=}.')
                     module.register_parameter('bias', None)
 
                 # For transformer engine
-                if hasattr(module, 'use_bias'):
-                    log.info(f'Setting use_bias=False for {module=}.')
+                if hasattr(module, 'use_bias') and module.use_bias is True:
+                    log.debug(f'Setting use_bias=False for {module=}.')
                     module.use_bias = False
 
         log.debug(self)
         log.debug(f'Using {self.config.init_config["name"]} initialization.')
 
     def get_input_embeddings(self) -> Union[SharedEmbedding, nn.Embedding]:
         return self.wte
 
     def set_input_embeddings(
-            self, value: Union[SharedEmbedding, nn.Embedding]) -> None:
+        self,
+        value: Union[SharedEmbedding, nn.Embedding],
+    ) -> None:
         self.wte = value
 
     @torch.no_grad()
     def _attn_bias(
         self,
         device: torch.device,
         dtype: torch.dtype,
         attention_mask: Optional[torch.ByteTensor] = None,
         sequence_id: Optional[torch.LongTensor] = None,
     ) -> Tuple[Optional[torch.Tensor], Optional[torch.ByteTensor]]:
         if not self._attn_bias_initialized:
             if self.attn_bias_shape:
-                self.attn_bias = torch.zeros(self.attn_bias_shape,
-                                             device=device,
-                                             dtype=dtype)
+                self.attn_bias = torch.zeros(
+                    self.attn_bias_shape,
+                    device=device,
+                    dtype=dtype,
+                )
                 self.attn_bias = build_attn_bias(
                     self.attn_impl,
                     self.attn_bias,
                     self.config.n_heads,
                     self.config.max_seq_len,
                     causal=self.is_causal,
                     alibi=self.alibi,
@@ -419,16 +489,19 @@
             self.attn_bias = self.attn_bias.to(dtype=dtype, device=device)
 
         attn_bias = self.attn_bias
 
         # If using torch, we incorporate sequence_id (if appropriate)
         if self.attn_uses_sequence_id and sequence_id is not None:
             assert isinstance(attn_bias, torch.Tensor)  # pyright
-            attn_bias = apply_sequence_id(attn_bias, sequence_id,
-                                          self.config.max_seq_len)
+            attn_bias = apply_sequence_id(
+                attn_bias,
+                sequence_id,
+                self.config.max_seq_len,
+            )
 
         # If using torch, we incorporate attention_mask. This will output
         # None in place of attention_mask since it will not be further needed in the
         # attention modules.
         if attention_mask is not None:
             s_k = attention_mask.shape[-1]
             if attn_bias is None:
@@ -437,15 +510,17 @@
                                         dtype=dtype)
             else:
                 # clamp to 0 necessary for torch 2.0 compile()
                 _s_k = max(0, attn_bias.size(-1) - s_k)
                 attn_bias = attn_bias[:, :, :, _s_k:]
             min_val = torch.finfo(attn_bias.dtype).min
             attn_bias = attn_bias.masked_fill(
-                ~attention_mask.view(-1, 1, 1, s_k), min_val)
+                ~attention_mask.view(-1, 1, 1, s_k),
+                min_val,
+            )
 
         return attn_bias, attention_mask
 
     def forward(
         self,
         input_ids: Optional[torch.LongTensor] = None,
         past_key_values: Optional[List[Tuple[torch.FloatTensor]]] = None,
@@ -453,55 +528,63 @@
         sequence_id: Optional[torch.LongTensor] = None,
         return_dict: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         use_cache: Optional[bool] = None,
         inputs_embeds: Optional[torch.Tensor] = None,
     ) -> BaseModelOutputWithPast:
-        return_dict = (return_dict
-                       if return_dict is not None else self.config.return_dict)
-        use_cache = (use_cache
-                     if use_cache is not None else self.config.use_cache)
+        return_dict = (
+            return_dict if return_dict is not None else self.config.return_dict
+        )
+        use_cache = (
+            use_cache if use_cache is not None else self.config.use_cache
+        )
 
         if attention_mask is not None:
             attention_mask = attention_mask.bool()  # type: ignore
 
         # These args are passed in by keyword in huggingface's generate function
         # https://github.com/huggingface/transformers/blob/68287689f2f0d8b7063c400230b3766987abf18d/src/transformers/generation/utils.py#L2201-L2206
         # but have not yet been fully implemented in MPTModel
         if not return_dict:
             raise NotImplementedError(
-                'return_dict False is not implemented yet for MPT')
+                'return_dict False is not implemented yet for MPT',
+            )
         if output_attentions:
             if self.attn_impl != 'torch':
                 raise NotImplementedError(
-                    'output_attentions is not implemented for MPT when using attn_impl `flash`.'
+                    'output_attentions is not implemented for MPT when using attn_impl `flash`.',
                 )
 
-        if (self.training and attention_mask is not None and
-                attention_mask[:, 0].sum() != attention_mask.shape[0]):
+        if (
+            self.training and attention_mask is not None and
+            attention_mask[:, 0].sum() != attention_mask.shape[0]
+        ):
             raise NotImplementedError(
-                'MPT does not support training with left padding.')
+                'MPT does not support training with left padding.',
+            )
 
         if self.training:
             if self.attn_uses_sequence_id and sequence_id is None:
                 raise ValueError(
                     'sequence_id is a required argument when MPT is configured with attn_uses_sequence_id=True '
-                    + 'and the model is in train mode.')
-            elif (self.attn_uses_sequence_id is False) and (sequence_id
-                                                            is not None):
+                    + 'and the model is in train mode.',
+                )
+            elif (self.attn_uses_sequence_id is
+                  False) and (sequence_id is not None):
                 warnings.warn(
                     'MPT received non-None input for `sequence_id` but is configured with attn_uses_sequence_id=False. '
                     +
-                    'This input will be ignored. If you want the model to use `sequence_id`, set attn_uses_sequence_id to True.'
+                    'This input will be ignored. If you want the model to use `sequence_id`, set attn_uses_sequence_id to True.',
                 )
 
         if input_ids is not None and inputs_embeds is not None:
             raise ValueError(
-                'You cannot specify both input_ids and inputs_embeds.')
+                'You cannot specify both input_ids and inputs_embeds.',
+            )
         elif input_ids is not None:
             bsz = input_ids.size(0)
             S = input_ids.size(1)
             x = self.wte(input_ids)
             input_device = input_ids.device
         elif inputs_embeds is not None:
             bsz = inputs_embeds.size(0)
@@ -519,30 +602,31 @@
 
         past_position = 0
         if past_key_values is not None:
             if len(past_key_values) != self.config.n_layers:
                 raise ValueError(
                     f'past_key_values must provide a past_key_value for each attention '
                     +
-                    f'layer in the network ({len(past_key_values)=}; {self.config.n_layers=}).'
+                    f'layer in the network ({len(past_key_values)=}; {self.config.n_layers=}).',
                 )
             # For attn_impl: flash, the past key tensor spec is (batch, seq, dim).
             # For attn_impl: torch, the past key tensor spec is (batch, heads, head_dim, seq).
             # Here we shift position embedding using the `seq` dim of the past key
             past_position = past_key_values[0][0].size(1)
             if self.attn_impl == 'torch':
                 past_position = past_key_values[0][0].size(3)
 
         if self.learned_pos_emb or self.rope:
-            if self.learned_pos_emb and (S + past_position >
-                                         self.config.max_seq_len):
+            if self.learned_pos_emb and (
+                S + past_position > self.config.max_seq_len
+            ):
                 raise ValueError(
                     f'Cannot forward input with past sequence length {past_position} and current sequence length '
                     +
-                    f'{S + 1}, this model only supports total sequence length <= {self.config.max_seq_len}.'
+                    f'{S + 1}, this model only supports total sequence length <= {self.config.max_seq_len}.',
                 )
 
             if self.learned_pos_emb or (self.rope and self.rope_impl == 'hf'):
                 pos = torch.arange(
                     past_position,
                     S + past_position,
                     dtype=torch.long,
@@ -572,59 +656,68 @@
                     'seq_len': S + past_position,
                 }
 
         if self.embedding_fraction == 1:
             x = self.emb_drop(x)
         else:
             # this implementation is proposed on page 7 of the GLM-130B paper https://arxiv.org/abs/2210.02414
-            x_shrunk = (x * self.embedding_fraction) + (
-                x.detach() * (1 - self.embedding_fraction))
+            x_shrunk = (x * self.embedding_fraction
+                       ) + (x.detach() * (1 - self.embedding_fraction))
             assert isinstance(self.emb_drop, nn.Module)  # pyright
             x = self.emb_drop(x_shrunk)
 
         attn_bias, attention_mask = self._attn_bias(
             device=x.device,
             dtype=torch.float32,
             attention_mask=attention_mask,
             sequence_id=sequence_id,
         )
         attention_mask_in_length = gen_attention_mask_in_length(
             sequence_id=sequence_id,
             S=S,
             attn_uses_sequence_id=self.attn_uses_sequence_id,
             attn_impl=self.attn_impl,
-            attention_mask=attention_mask)
+            attention_mask=attention_mask,
+        )
 
         alibi_slopes = None  # alibi_slopes will only be used by flash attention for ALiBi
         if self.alibi and self.attn_impl == 'flash':
-            alibi_slopes = gen_slopes(n_heads=self.config.n_heads,
-                                      alibi_bias_max=self.alibi_bias_max,
-                                      device=x.device,
-                                      return_1d=True)
+            alibi_slopes = gen_slopes(
+                n_heads=self.config.n_heads,
+                alibi_bias_max=self.alibi_bias_max,
+                device=x.device,
+                return_1d=True,
+            )
 
         # initialize the past key values cache if it should be used
         presents = () if use_cache else None
         if use_cache and past_key_values is None:
             past_key_values = [() for _ in range(self.config.n_layers)
                               ]  # type: ignore
 
         all_hidden_states = () if output_hidden_states else None
         all_self_attns = () if output_attentions else None
         flash_attn_padding_info = {}
         if self.attn_impl == 'flash':
             flash_attn_padding_info = gen_flash_attn_padding_info(
-                bsz, S, past_position, x.device, attention_mask_in_length,
-                attention_mask)
+                bsz,
+                S,
+                past_position,
+                x.device,
+                attention_mask_in_length,
+                attention_mask,
+            )
 
         for b_idx, block in enumerate(self.blocks):
             if output_hidden_states:
                 assert all_hidden_states is not None  # pyright
                 all_hidden_states = all_hidden_states + (x,)
-            past_key_value = (past_key_values[b_idx]
-                              if past_key_values is not None else None)
+            past_key_value = (
+                past_key_values[b_idx] if past_key_values is not None else None
+            )
             x, attn_weights, present = block(
                 x,
                 past_key_value=past_key_value,
                 attn_bias=attn_bias,
                 rotary_emb_w_meta_info=rotary_emb_w_meta_info,
                 attention_mask=attention_mask,
                 is_causal=self.is_causal,
@@ -652,15 +745,15 @@
             hidden_states=all_hidden_states,
             attentions=all_self_attns,
         )
 
     # Param Initialization, needed for device='meta' fast initialization
     def param_init_fn(self, module: nn.Module) -> None:
         init_fn_name = self.config.init_config['name']
-        MODEL_INIT_REGISTRY[init_fn_name](
+        param_init_fns.get(init_fn_name)(
             module=module,
             n_layers=self.config.n_layers,
             d_model=self.config.d_model,
             **self.config.init_config,
         )
 
     # FSDP Wrap function
@@ -702,46 +795,52 @@
         if config.logit_scale is not None:
             logit_scale = config.logit_scale
             if isinstance(logit_scale, str):
                 if logit_scale == 'inv_sqrt_d_model':
                     logit_scale = 1 / math.sqrt(config.d_model)
                 else:
                     raise ValueError(
-                        f"{logit_scale=} is not recognized as an option; use numeric value or 'inv_sqrt_d_model'."
+                        f"{logit_scale=} is not recognized as an option; use numeric value or 'inv_sqrt_d_model'.",
                     )
             self.logit_scale = logit_scale
 
     def get_input_embeddings(self) -> Union[SharedEmbedding, nn.Embedding]:
         return self.transformer.get_input_embeddings()
 
     def set_input_embeddings(
-            self, value: Union[SharedEmbedding, nn.Embedding]) -> None:
+        self,
+        value: Union[SharedEmbedding, nn.Embedding],
+    ) -> None:
         self.transformer.set_input_embeddings(value)
 
     def get_output_embeddings(
-            self) -> Union[SharedEmbedding, nn.Embedding, nn.Linear]:
+        self,
+    ) -> Union[SharedEmbedding, nn.Embedding, nn.Linear]:
         if self.lm_head is not None:
             return self.lm_head
         return self.transformer.get_input_embeddings()
 
     def set_output_embeddings(
-        self, new_embeddings: Union[SharedEmbedding, nn.Embedding,
-                                    nn.Linear]) -> None:
+        self,
+        new_embeddings: Union[SharedEmbedding, nn.Embedding, nn.Linear],
+    ) -> None:
         if self.lm_head is not None:
             self.lm_head = new_embeddings
         else:
             if not isinstance(new_embeddings, (SharedEmbedding, nn.Embedding)):
                 raise ValueError(
                     'new_embeddings must be an instance of SharedEmbedding ' +
-                    f'or nn.Embedding, but got {type(new_embeddings)}.')
+                    f'or nn.Embedding, but got {type(new_embeddings)}.',
+                )
             warnings.warn(
                 'Using `set_output_embeddings` to set the embedding layer of ' +
                 'MPTForCausalLM with tied weights. Given weights are tied, ' +
                 'using `set_input_embeddings` is recommended over using ' +
-                '`set_output_embeddings`.')
+                '`set_output_embeddings`.',
+            )
             self.transformer.set_input_embeddings(new_embeddings)
 
     def tie_weights(self) -> None:
         if getattr(self.config, 'tie_word_embeddings', True):
             self.lm_head = None
 
     def set_decoder(self, decoder: MPTModel) -> None:
@@ -759,18 +858,20 @@
         labels: Optional[torch.LongTensor] = None,
         return_dict: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         use_cache: Optional[bool] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
     ) -> CausalLMOutputWithPast:
-        return_dict = (return_dict
-                       if return_dict is not None else self.config.return_dict)
-        use_cache = (use_cache
-                     if use_cache is not None else self.config.use_cache)
+        return_dict = (
+            return_dict if return_dict is not None else self.config.return_dict
+        )
+        use_cache = (
+            use_cache if use_cache is not None else self.config.use_cache
+        )
 
         outputs = self.transformer(
             input_ids=input_ids,
             past_key_values=past_key_values,
             attention_mask=attention_mask,
             sequence_id=sequence_id,
             return_dict=return_dict,
@@ -788,15 +889,15 @@
             out = outputs.last_hidden_state
             out = out.to(self.transformer.wte.weight.device)
             logits = self.transformer.wte(out, True)
 
         if self.logit_scale is not None:
             if self.logit_scale == 0:
                 warnings.warn(
-                    f'Multiplying logits by {self.logit_scale=}. This will produce uniform (uninformative) outputs.'
+                    f'Multiplying logits by {self.logit_scale=}. This will produce uniform (uninformative) outputs.',
                 )
             logits *= self.logit_scale
 
         loss = None
         if labels is not None:
             _labels = torch.roll(labels, shifts=-1)
             _labels[:, -1] = -100
@@ -812,15 +913,15 @@
             hidden_states=outputs.hidden_states,
             attentions=outputs.attentions,
         )
 
     # Param Initialization, needed for device='meta' fast initialization
     def param_init_fn(self, module: nn.Module) -> None:
         init_fn_name = self.config.init_config['name']
-        MODEL_INIT_REGISTRY[init_fn_name](
+        param_init_fns.get(init_fn_name)(
             module=module,
             n_layers=self.config.n_layers,
             d_model=self.config.d_model,
             **self.config.init_config,
         )
 
     # FSDP Wrap function
@@ -858,25 +959,33 @@
                         {
                             "mptblock": 'first-5',
                             "grouped_query_attention": 'last-35'
                         }
         """
         if not hasattr(module, 'block_idx'):
             log.debug(
-                f'{module.__class__.__name__} cannot be activation checkpointed. Only transformer block or its submodules are eligible for activation checkpointing.'
+                f'{module.__class__.__name__} cannot be activation checkpointed. Only transformer block or its submodules are eligible for activation checkpointing.',
             )
             return False
 
-        act_ckpt_target = getattr(self.config,
-                                  'activation_checkpointing_target', None)
+        act_ckpt_target = getattr(
+            self.config,
+            'activation_checkpointing_target',
+            None,
+        )
         act_ckpt_mod_to_blocks = build_act_ckpt_mod_to_blocks(
-            act_ckpt_target, MPTBlock, module.max_block_idx)
+            act_ckpt_target,
+            MPTBlock,
+            module.max_block_idx,
+        )
 
-        check_mapping_blocks_overlap(act_ckpt_mod_to_blocks,
-                                     module.max_block_idx)
+        check_mapping_blocks_overlap(
+            act_ckpt_mod_to_blocks,
+            module.max_block_idx,
+        )
 
         for k in act_ckpt_mod_to_blocks.keys():
             if isinstance(module, k):
                 blocks = act_ckpt_mod_to_blocks[k]
                 return True if blocks == -1 else module.block_idx in blocks
 
         return False
@@ -888,15 +997,16 @@
                                              torch.Tensor]]] = None,
         inputs_embeds: Optional[torch.Tensor] = None,
         **kwargs: Any,
     ) -> Dict[str, Any]:
         attention_mask = kwargs['attention_mask'].bool()
         if attention_mask[:, -1].sum() != attention_mask.shape[0]:
             raise NotImplementedError(
-                'MPT does not support generation with right padding.')
+                'MPT does not support generation with right padding.',
+            )
 
         if self.transformer.attn_uses_sequence_id and self.training:
             sequence_id = torch.zeros_like(input_ids[:1])
         else:
             sequence_id = None
 
         # only last token for inputs_ids if past is defined in kwargs
@@ -915,123 +1025,179 @@
             'past_key_values': past_key_values,
             'use_cache': kwargs.get('use_cache', True),
         })
         return model_inputs
 
     @staticmethod
     def _reorder_cache(
-            past_key_values: List[Tuple[torch.Tensor, torch.Tensor]],
-            beam_idx: torch.LongTensor) -> List[Tuple[torch.Tensor, ...]]:
+        past_key_values: List[Tuple[torch.Tensor, torch.Tensor]],
+        beam_idx: torch.LongTensor,
+    ) -> List[Tuple[torch.Tensor, ...]]:
         """Used by HuggingFace generate when using beam search with kv-caching.
 
         See https://github.com/huggingface/transformers/blob/3ec7a47664ebe40c40f4b722f6bb1cd30c3821ec/src/transformers/models/gpt2/modeling_gpt2.py#L1122-L1133
         for an example in transformers.
         """
         reordered_past = []
         for layer_past in past_key_values:
             reordered_past += [
                 tuple(
                     past_state.index_select(0, beam_idx)
-                    for past_state in layer_past)
+                    for past_state in layer_past
+                ),
             ]
         return reordered_past
 
 
 class ComposerMPTCausalLM(HuggingFaceModel):
 
     def __init__(
         self,
         om_model_config: DictConfig,
         tokenizer: Optional[PreTrainedTokenizerBase] = None,
     ):
-        from llmfoundry.metrics import (DEFAULT_CAUSAL_LM_EVAL_METRICS,
-                                        DEFAULT_CAUSAL_LM_TRAIN_METRICS)
+        from llmfoundry.metrics import (
+            DEFAULT_CAUSAL_LM_EVAL_METRICS,
+            DEFAULT_CAUSAL_LM_TRAIN_METRICS,
+        )
         from llmfoundry.utils.builders import build_metric
 
-        resolved_om_model_config = om.to_container(om_model_config,
-                                                   resolve=True)
+        resolved_om_model_config = om.to_container(
+            om_model_config,
+            resolve=True,
+        )
         assert isinstance(resolved_om_model_config, dict)
 
         hf_config = MPTConfig.from_dict(resolved_om_model_config)
         model = MPTForCausalLM(hf_config)
 
         use_train_metrics = om_model_config.get('use_train_metrics', True)
         train_metric_names = DEFAULT_CAUSAL_LM_TRAIN_METRICS + resolved_om_model_config.get(
-            'additional_train_metrics', [])
+            'additional_train_metrics',
+            [],
+        )
         train_metrics = [
             build_metric(metric, {}) for metric in train_metric_names
         ] if use_train_metrics else []
         eval_metric_names = DEFAULT_CAUSAL_LM_EVAL_METRICS + resolved_om_model_config.get(
-            'additional_eval_metrics', [])
+            'additional_eval_metrics',
+            [],
+        )
         eval_metrics = [
             build_metric(metric, {}) for metric in eval_metric_names
         ]
 
         super().__init__(
             model=model,
             tokenizer=tokenizer,
             use_logits=True,
             metrics=train_metrics,
             eval_metrics=eval_metrics,
             shift_labels=True,
             allow_embedding_resizing=True,
         )
 
-        self.n_active_params = sum(p.numel() for p in self.parameters())
-
         loss_fn_config = om_model_config.get('loss_fn', 'fused_crossentropy')
         if loss_fn_config == 'fused_crossentropy':
             try:
                 from flash_attn.losses.cross_entropy import \
                     CrossEntropyLoss as FusedCrossEntropyLoss
 
-                self.loss_fn = FusedCrossEntropyLoss(ignore_index=-100)
+                self.loss_fn = FusedCrossEntropyLoss(
+                    ignore_index=-100,
+                    reduction='none',
+                )
             except:
                 raise ValueError(
                     'Fused Cross Entropy is not installed. Either (1) have a CUDA-compatible GPU '
                     +
                     'and `pip install .[gpu]` if installing from source or `pip install xentropy-cuda-lib@git+https://github.com/HazyResearch/flash-attention.git@v1.0.3#subdirectory=csrc/xentropy` '
                     +
-                    'if installing from pypi, or (2) set your config model.loss_fn=torch_crossentropy.'
+                    'if installing from pypi, or (2) set your config model.loss_fn=torch_crossentropy.',
                 )
         elif loss_fn_config == 'torch_crossentropy':
-            self.loss_fn = nn.CrossEntropyLoss(ignore_index=-100)
+            self.loss_fn = nn.CrossEntropyLoss(
+                ignore_index=-100,
+                reduction='none',
+            )
         else:
             raise ValueError(
-                f'Specified loss_fn={self.loss_fn} not recognized. `loss_fn` must be one of [`fused_crossentropy`, `torch_crossentropy`].'
+                f'Specified loss_fn={self.loss_fn} not recognized. `loss_fn` must be one of [`fused_crossentropy`, `torch_crossentropy`].',
             )
 
     def get_targets(self, batch: Mapping) -> torch.Tensor:
         targets = torch.roll(batch['labels'], shifts=-1)
         targets[:, -1] = -100
         return targets
 
     def forward(self, batch: MutableMapping) -> CausalLMOutputWithPast:
+        if self.config.ffn_config['ffn_type'] in ffns_with_megablocks:
+            # Clear MegaBlocks MoE load balancing loss cache
+            try:  # Add try/catch to avoid transformers complaining and raising errors
+                from megablocks.layers.moe import clear_load_balancing_loss
+            except:
+                raise RuntimeError(
+                    'Requirements for MegaBlocks not installed; see install instructions in `README.md`.',
+                )
+            clear_load_balancing_loss()
         return self.model(
             input_ids=batch.get('input_ids', None),
             attention_mask=batch.get('attention_mask', None),
             sequence_id=batch.get('sequence_id', None),
             inputs_embeds=batch.get('inputs_embeds', None),
         )
 
     def loss(self, outputs: CausalLMOutputWithPast,
-             batch: Mapping) -> torch.Tensor:
+             batch: Mapping) -> Union[dict, torch.Tensor]:
         targets = self.get_targets(batch)
-        return self.loss_fn(outputs.logits.view(-1, outputs.logits.size(-1)),
-                            targets.view(-1))
+        losses = self.loss_fn(
+            outputs.logits.view(-1, outputs.logits.size(-1)),
+            targets.view(-1),
+        )
+
+        if torch.all(targets == self.loss_fn.ignore_index):
+            loss = losses.sum()
+        else:
+            loss = losses.sum() / (targets != self.loss_fn.ignore_index).sum()
 
-    def flops_per_batch(self, batch: Mapping) -> int:
+        if self.config.ffn_config['ffn_type'] in ffns_with_megablocks:
+            # MegaBlocks MoE load balancing loss
+            try:  # Add try/catch to avoid transformers complaining and raising errors
+                from megablocks.layers.moe import batched_load_balancing_loss
+            except:
+                raise RuntimeError(
+                    'Requirements for MegaBlocks not installed; see install instructions in `README.md`.',
+                )
+            lbl = batched_load_balancing_loss(self.model.transformer.mb_args)
+            return {
+                'total': loss + lbl,
+                'loss': loss,
+                'lbl': lbl,
+            }
+
+        return loss
+
+    @cached_property
+    def n_total_params(self):
+        """Gets the total number of parameters in the model."""
+        return mpt_get_total_params(self)
+
+    @cached_property
+    def n_active_params(self):
+        """Gets the total number of active parameters in the model."""
+        return mpt_get_active_params(self)
+
+    def flops_per_batch(self, batch: Mapping):
         # Note: this computation does not take into account padding, and assumes
         # that the dataset has been constructed without padding. Additionally, we
         # assume the backward pass is approximately 2x the forward pass
 
         bs, msl = batch['input_ids'].shape[0:2]
         params = self.n_active_params
-        if not self.model.transformer.config.tie_word_embeddings:
-            # embedding layers are lookup tables, therefore are not counted in the FLOP computation
-            params -= self.model.transformer.wte.weight.numel()
         params_flops_per_token = 2 * params
         params_flops_per_seq = params_flops_per_token * msl
-        attn_flops_per_seq = (self.model.config.n_layers * 2 * 2 *
-                              (self.model.config.d_model * (msl**2)))
+        attn_flops_per_seq = (
+            self.model.config.n_layers * 2 * 2 *
+            (self.model.config.d_model * (msl**2))
+        )
 
         return (params_flops_per_seq + attn_flops_per_seq) * 3 * bs
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/utils/act_ckpt.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/utils/act_ckpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 # Copyright 2024 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 from typing import Any
 
 import torch
 
-from llmfoundry.models.layers.attention import ATTN_CLASS_REGISTRY
-from llmfoundry.models.layers.blocks import MPTBlock
-from llmfoundry.models.layers.ffn import FFN_CLASS_REGISTRY
-from llmfoundry.models.layers.norm import NORM_CLASS_REGISTRY
+from llmfoundry.layers_registry import (
+    attention_classes,
+    ffns,
+    ffns_with_megablocks,
+    ffns_with_norm,
+    norms,
+)
+from llmfoundry.models.layers.blocks import FusedNormAttentionNorm, MPTBlock
+
+__all__ = [
+    'build_act_ckpt_mod_to_blocks',
+    'pass_on_block_idx',
+    'check_mapping_blocks_overlap',
+]
 
 
 def pass_on_block_idx(parent: torch.nn.Module):
     if not hasattr(parent, 'block_idx') or not hasattr(parent, 'max_block_idx'):
         return
     for child in parent.children():
         child.block_idx = parent.block_idx
@@ -21,26 +31,35 @@
             pass_on_block_idx(child)
 
 
 def get_act_ckpt_module(mod_name: str) -> Any:
     """Get the module type from the module name."""
     if mod_name.lower() == 'mptblock':
         mod_type = MPTBlock
-    elif mod_name in ATTN_CLASS_REGISTRY:
-        mod_type = ATTN_CLASS_REGISTRY[mod_name]
-    elif mod_name in FFN_CLASS_REGISTRY:
-        mod_type = FFN_CLASS_REGISTRY[mod_name]
-    elif mod_name in NORM_CLASS_REGISTRY:
-        mod_type = NORM_CLASS_REGISTRY[mod_name]
+    elif mod_name in attention_classes:
+        mod_type = attention_classes.get(mod_name)
+    elif mod_name.lower() == 'norm_attn_norm':
+        mod_type = FusedNormAttentionNorm
+    elif mod_name in ffns:
+        mod_type = ffns.get(mod_name)
+    elif mod_name in ffns_with_norm:
+        mod_type = ffns_with_norm.get(mod_name)
+    elif mod_name in ffns_with_megablocks:
+        mod_type = ffns_with_megablocks.get(mod_name)
+    elif mod_name in norms:
+        mod_type = norms.get(mod_name)
     else:
         msg = ', '.join(
-            list(ATTN_CLASS_REGISTRY.keys()) + list(FFN_CLASS_REGISTRY.keys()) +
-            list(NORM_CLASS_REGISTRY.keys()) + ['MPTBlock'])
+            list(attention_classes.keys()) + list(ffns.get_all()) +
+            list(ffns_with_norm.get_all()) +
+            list(ffns_with_megablocks.get_all()) + list(norms.get_all()) +
+            ['MPTBlock'],
+        )
         raise ValueError(
-            f'{mod_name} (specified in activation_checkpointing_target) is not a recognized option out of available options {msg}.'
+            f'{mod_name} (specified in activation_checkpointing_target) is not a recognized option out of available options {msg}.',
         )
     return mod_type
 
 
 def parse_ele_str(ele: str, max_block_idx: int) -> list:
     """Parse a string in target_blocks and return a list of block ids to add.
 
@@ -50,15 +69,16 @@
     to_add = None
     if ele.startswith('first-'):
         assert ele[6:].isdigit(), f'Invalid target_blocks element {ele}'
         to_add = list(range(min(int(ele[6:]), max_block_idx + 1)))
     elif ele.startswith('last-'):
         assert ele[5:].isdigit(), f'Invalid target_blocks element {ele}'
         to_add = list(
-            range(max(max_block_idx - int(ele[5:]) + 1, 0), max_block_idx + 1))
+            range(max(max_block_idx - int(ele[5:]) + 1, 0), max_block_idx + 1),
+        )
     elif ele.startswith('middle-'):
         assert ele[7:].isdigit(), f'Invalid target_blocks element {ele}'
         num = int(ele[7:])
         start = max(max_block_idx // 2 - num // 2, 0)
         end = min(start + num, max_block_idx + 1)
         to_add = list(range(start, end))
     elif ele.startswith('range-'):
@@ -83,24 +103,24 @@
             if isinstance(ele, int):
                 candidate_block_ids.append(ele)
             elif isinstance(ele, str):
                 to_add = parse_ele_str(ele, max_block_idx)
                 candidate_block_ids.extend(to_add)
             else:
                 raise ValueError(
-                    f'target_blocks must be a list of integers or "first-n", "middle-m", "last-k", or "range-i-j" where n, m, k, i, j are integers, but got {target_blocks}'
+                    f'target_blocks must be a list of integers or "first-n", "middle-m", "last-k", or "range-i-j" where n, m, k, i, j are integers, but got {target_blocks}',
                 )
     elif isinstance(target_blocks, str):
         target_blocks = target_blocks.replace(' ', '')
         for ele in target_blocks.split(','):
             to_add = parse_ele_str(ele, max_block_idx)
             candidate_block_ids.extend(to_add)
     else:
         raise ValueError(
-            f'target_blocks must be either a single intege, or a list of integers, or a comma separated string made of "first-n", "last-m", "middle-k", "range-i-j", or a list of mixed integers and before-mentioned strings, but got {type(target_blocks)}'
+            f'target_blocks must be either a single integer, or a list of integers, or a comma separated string made of "first-n", "last-m", "middle-k", "range-i-j", or a list of mixed integers and before-mentioned strings, but got {type(target_blocks)}',
         )
 
     candidate_block_ids = list(set(candidate_block_ids))
     return candidate_block_ids
 
 
 def check_mapping_blocks_overlap(mapping: dict, max_block_idx: int) -> None:
@@ -111,22 +131,25 @@
             v = list(range(max_block_idx + 1))
         for vv in v:
             if vv < 0 or vv > max_block_idx:
                 continue
             else:
                 if all_blocks[vv] is not None:
                     raise ValueError(
-                        f'Block {vv} is assigned to both {k} and {all_blocks[vv]}. Each block can only have one granularity of activation checkpointing. Make sure the target_blocks in activation_checkpointing_target do not overlap. For more details, refer to the docs of activation_checkpointing_fn.'
+                        f'Block {vv} is assigned to both {k} and {all_blocks[vv]}. Each block can only have one granularity of activation checkpointing. Make sure the target_blocks in activation_checkpointing_target do not overlap. For more details, refer to the docs of activation_checkpointing_fn.',
                     )
                 else:
                     all_blocks[vv] = k
 
 
-def build_act_ckpt_mod_to_blocks(act_ckpt_target: Any, top_module: Any,
-                                 max_block_idx: int) -> dict:
+def build_act_ckpt_mod_to_blocks(
+    act_ckpt_target: Any,
+    top_module: Any,
+    max_block_idx: int,
+) -> dict:
     act_ckpt_mod_to_blocks = {}
     if act_ckpt_target is None or act_ckpt_target == []:
         mod = top_module
         act_ckpt_mod_to_blocks[mod] = -1
     elif isinstance(act_ckpt_target, str):
         mod = get_act_ckpt_module(act_ckpt_target)
         act_ckpt_mod_to_blocks[mod] = -1
@@ -137,11 +160,11 @@
     elif isinstance(act_ckpt_target, dict):
         for k, v in act_ckpt_target.items():
             mod = get_act_ckpt_module(k)
             block_ids = get_target_block_list(v, max_block_idx)
             act_ckpt_mod_to_blocks[mod] = block_ids
     else:
         raise ValueError(
-            f'activation_checkpointing_target must be either a single string or a list or a dict, but got {type(act_ckpt_target)}'
+            f'activation_checkpointing_target must be either a single string or a list or a dict, but got {type(act_ckpt_target)}',
         )
 
     return act_ckpt_mod_to_blocks
```

### Comparing `llm-foundry-0.7.0/llmfoundry/models/utils/meta_init_context.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/utils/meta_init_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 
 from contextlib import contextmanager
 # Modified from https://github.com/huggingface/accelerate/blob/main/src/accelerate/big_modeling.py
 from typing import Any, Callable, Optional
 
 import torch
 import torch.nn as nn
+from torch.distributed._tensor import DTensor
+
+__all__ = [
+    'init_empty_weights',
+    'init_on_device',
+]
 
 
 @contextmanager
 def init_empty_weights(include_buffers: bool = False):
     """Meta initialization context manager.
 
     A context manager under which models are initialized with all parameters
@@ -47,16 +53,18 @@
     <Tip warning={true}>
 
     Any model created under this context manager has no weights. As such you can't do something like
     `model.to(some_device)` with it. To load weights inside your empty model, see [`load_checkpoint_and_dispatch`].
 
     </Tip>
     """
-    with init_on_device(torch.device('meta'),
-                        include_buffers=include_buffers) as f:
+    with init_on_device(
+        torch.device('meta'),
+        include_buffers=include_buffers,
+    ) as f:
         yield f
 
 
 @contextmanager
 def init_on_device(device: torch.device, include_buffers: bool = False):
     """Device initialization context manager.
 
@@ -76,30 +84,39 @@
         tst = nn.Liner(100, 100)  # on `cuda` device
     ```
     """
     old_register_parameter = nn.Module.register_parameter
     if include_buffers:
         old_register_buffer = nn.Module.register_buffer
 
-    def register_empty_parameter(self: torch.nn.Module, name: str,
-                                 param: Optional[torch.nn.Parameter]):
+    def register_empty_parameter(
+        self: torch.nn.Module,
+        name: str,
+        param: Optional[torch.nn.Parameter],
+    ):
         old_register_parameter(self, name, param)
         if param is not None:
             parameter = self._parameters[name]
             assert parameter is not None
-
-            param_cls = type(parameter)
-            kwargs = parameter.__dict__
-
-            self._parameters[name] = param_cls(parameter.to(device), **kwargs)
-
-    def register_empty_buffer(self: torch.nn.Module,
-                              name: str,
-                              tensor: Optional[torch.Tensor],
-                              persistent: bool = True):
+            if isinstance(parameter, DTensor):
+                self._parameters[name] = parameter.to(device)  # type: ignore
+            else:
+                param_cls = type(parameter)
+                kwargs = parameter.__dict__
+                self._parameters[name] = param_cls(
+                    parameter.to(device),
+                    **kwargs,
+                )
+
+    def register_empty_buffer(
+        self: torch.nn.Module,
+        name: str,
+        tensor: Optional[torch.Tensor],
+        persistent: bool = True,
+    ):
         old_register_buffer(self, name, tensor, persistent=persistent)
         if tensor is not None:
             named_buffer = self._buffers[name]
             assert named_buffer is not None
             self._buffers[name] = named_buffer.to(device)
 
     # Patch tensor creation
@@ -121,16 +138,18 @@
 
     try:
         nn.Module.register_parameter = register_empty_parameter
         if include_buffers:
             nn.Module.register_buffer = register_empty_buffer
         for torch_function_name in tensor_constructors_to_patch.keys():
             setattr(
-                torch, torch_function_name,
-                patch_tensor_constructor(getattr(torch, torch_function_name)))
+                torch,
+                torch_function_name,
+                patch_tensor_constructor(getattr(torch, torch_function_name)),
+            )
         yield
     finally:
         nn.Module.register_parameter = old_register_parameter
         if include_buffers:
             nn.Module.register_buffer = old_register_buffer
         for torch_function_name, old_torch_function in tensor_constructors_to_patch.items(
         ):
```

### Comparing `llm-foundry-0.7.0/llmfoundry/optim/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/optim/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
-from composer.optim import (ConstantWithWarmupScheduler,
-                            CosineAnnealingWithWarmupScheduler, DecoupledAdamW,
-                            LinearWithWarmupScheduler)
+from composer.optim import (
+    ConstantWithWarmupScheduler,
+    CosineAnnealingWithWarmupScheduler,
+    DecoupledAdamW,
+    LinearWithWarmupScheduler,
+)
 
 from llmfoundry.optim.adaptive_lion import DecoupledAdaLRLion, DecoupledClipLion
 from llmfoundry.optim.lion import DecoupledLionW
 from llmfoundry.optim.scheduler import InverseSquareRootWithWarmupScheduler
 from llmfoundry.registry import optimizers, schedulers
 
 optimizers.register('adalr_lion', func=DecoupledAdaLRLion)
 optimizers.register('clip_lion', func=DecoupledClipLion)
 optimizers.register('decoupled_lionw', func=DecoupledLionW)
 optimizers.register('decoupled_adamw', func=DecoupledAdamW)
 
 schedulers.register('constant_with_warmup', func=ConstantWithWarmupScheduler)
-schedulers.register('cosine_with_warmup',
-                    func=CosineAnnealingWithWarmupScheduler)
+schedulers.register(
+    'cosine_with_warmup',
+    func=CosineAnnealingWithWarmupScheduler,
+)
 schedulers.register('linear_decay_with_warmup', func=LinearWithWarmupScheduler)
-schedulers.register('inv_sqrt_with_warmup',
-                    func=InverseSquareRootWithWarmupScheduler)
+schedulers.register(
+    'inv_sqrt_with_warmup',
+    func=InverseSquareRootWithWarmupScheduler,
+)
 
 __all__ = [
     'DecoupledLionW',
     'DecoupledClipLion',
     'DecoupledAdaLRLion',
+    'InverseSquareRootWithWarmupScheduler',
 ]
```

### Comparing `llm-foundry-0.7.0/llmfoundry/optim/adaptive_lion.py` & `llm-foundry-0.9.0.dev0/llmfoundry/optim/adaptive_lion.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 from composer.utils import dist
 from torch.optim.optimizer import Optimizer
 
 from llmfoundry.optim.outlier_detection import OutlierDetector
 
 log = logging.getLogger(__name__)
 
+__all__ = [
+    'DecoupledAdaLRLion',
+    'DecoupledClipLion',
+]
+
 
 class DecoupledAdaLRLion(Optimizer):
     """DecoupledAdaLRLion.
 
     This class implements a variant of Lion which lowers the layerwise
     learning rate when the layer's moment becomes an outlier. A moment is an
     outlier if it is some multiple `outlier_threshold` times larger than the
@@ -33,79 +38,92 @@
         outlier_threshold (float): Multiplicative factor determining what constitutes an "outlier" relative to the MVA of gradient norms.
         timeout (int): Number of steps to lower the learning for after seeing an outlier.
         lr_penalty (float): Multiplicative scale by which to lower the LR for each outlier.
         min_scale (float): Minimum allowed scaling of the LR .
     """
     metric_functions = {
         'l2_norm/moment':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                optim_state['exp_avg']),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(optim_state['exp_avg']),
         'l2_norm/param':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                param.data),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(param.data),
         'l2_norm/update':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                step_tensor),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(step_tensor),
         'l2_norm/grad':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                param.grad),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(param.grad),
     }
 
-    def __init__(self,
-                 params: Union[Iterable[torch.Tensor], Iterable[dict]],
-                 lr: float = 1e-4,
-                 betas: Tuple[float, float] = (0.9, 0.99),
-                 weight_decay: float = 0.0,
-                 outlier_threshold: float = 10.0,
-                 timeout: int = 100,
-                 lr_penalty: float = .707,
-                 min_scale: float = 1e-4):
+    def __init__(
+        self,
+        params: Union[Iterable[torch.Tensor], Iterable[dict]],
+        lr: float = 1e-4,
+        betas: Tuple[float, float] = (0.9, 0.99),
+        weight_decay: float = 0.0,
+        outlier_threshold: float = 10.0,
+        timeout: int = 100,
+        lr_penalty: float = .707,
+        min_scale: float = 1e-4,
+    ):
         if lr <= 0.:
             raise Exception(f'Invalid LR: {lr}. LR must be > 0')
-        if not all([0. <= beta <= 1. for beta in betas]):
+        if not all(0. <= beta <= 1. for beta in betas):
             raise Exception(
-                f'Invalid beta values: {betas} All betas must be between 0 and 1.'
+                f'Invalid beta values: {betas} All betas must be between 0 and 1.',
             )
         if weight_decay >= 1e-3:
             log.warning(
                 f'You are using a high value of `weight_decay={weight_decay}` for the `DecoupledLionW` optimizer. Are you sure you want to do this? '
                 +
-                f'Your model\'s weights will be multiplied by {1.0 - weight_decay} on every step!'
+                f'Your model\'s weights will be multiplied by {1.0 - weight_decay} on every step!',
             )
 
         defaults = {'lr': lr, 'betas': betas, 'weight_decay': weight_decay}
 
         super().__init__(params, defaults)
 
         for group in self.param_groups:
             group['initial_lr'] = group['lr']
         self.outlier_threshold = outlier_threshold
         self.timeout = timeout
         self.lr_penalty = lr_penalty
         self.min_scale = min_scale
 
     @staticmethod
-    def lionw(p: torch.Tensor, grad: torch.Tensor, exp_avg: torch.Tensor,
-              lr: float, initial_lr: float, wd: float, beta1: float,
-              beta2: float) -> None:
+    def lionw(
+        p: torch.Tensor,
+        grad: torch.Tensor,
+        exp_avg: torch.Tensor,
+        lr: float,
+        initial_lr: float,
+        wd: float,
+        beta1: float,
+        beta2: float,
+    ) -> None:
         # stepweight decay
         if wd != 0:
             decay_factor = (lr / initial_lr) if initial_lr else 1.0
             p.data.mul_(1 - decay_factor * wd)
 
         # update is interpolation between gradient and momentum
         update = exp_avg.lerp(grad, 1 - beta1).sign_()
         p.add_(update, alpha=-lr)
 
         # momentum is interp b/w gradient and itself
         exp_avg.lerp_(grad, 1 - beta2)
 
     @staticmethod
-    def adjust_lr(lr: float, lr_penalty: float, num_times: int,
-                  min_scale: float) -> float:
+    def adjust_lr(
+        lr: float,
+        lr_penalty: float,
+        num_times: int,
+        min_scale: float,
+    ) -> float:
         """Adjusts LR.
 
         Multiplicatively scales down the LR by lr_penalty for each outlier
         that has occurred in the last `timeout` number of steps, capping the
         scaling to be no smaller than `min_scale`.
 
         Args:
@@ -124,54 +142,61 @@
 
         loss = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
-            for p in filter(lambda p: p.grad is not None and p.requires_grad,
-                            group['params']):
+            for p in filter(
+                lambda p: p.grad is not None and p.requires_grad,
+                group['params'],
+            ):
 
                 grad, lr, initial_lr, wd, beta1, beta2, state = p.grad, group[
                     'lr'], group['initial_lr'], group[
                         'weight_decay'], *group['betas'], self.state[p]
 
                 # init state - exponential moving average of gradient values
 
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
                     state['moment_tracker'] = OutlierDetector(
-                        self.outlier_threshold)
+                        self.outlier_threshold,
+                    )
                     state['outlier_timestamp'] = []
                     state['step'] = 0
 
                 exp_avg = state['exp_avg']
 
                 # determine if the new moment resulting from this grad would be an outlier
                 moment_norm = torch.linalg.vector_norm(
-                    exp_avg.lerp(grad, 1 - beta2))**2
+                    exp_avg.lerp(grad, 1 - beta2),
+                )**2
 
                 if dist.get_world_size() > 1:
                     dist.all_reduce(moment_norm, reduce_operation='SUM')
                 moment_norm = math.sqrt(moment_norm)
 
                 if state['moment_tracker'].insert_observation(moment_norm):
                     state['outlier_timestamp'].append(state['step'])
 
-                removed = []
-                for ts in state['outlier_timestamp']:
-                    if state['step'] - ts > self.timeout:
-                        removed.append(ts)
+                removed = [
+                    ts for ts in state['outlier_timestamp']
+                    if state['step'] - ts > self.timeout
+                ]
 
                 for ts in removed:
                     state['outlier_timestamp'].remove(ts)
 
-                lr = self.adjust_lr(lr, self.lr_penalty,
-                                    len(state['outlier_timestamp']),
-                                    self.min_scale)
+                lr = self.adjust_lr(
+                    lr,
+                    self.lr_penalty,
+                    len(state['outlier_timestamp']),
+                    self.min_scale,
+                )
                 self.lionw(p, grad, exp_avg, lr, initial_lr, wd, beta1, beta2)
                 state['step'] += 1
 
         return loss
 
     def dist_reduce_metrics(self, optimizer_metrics: Dict[str, torch.Tensor]):
         for metric in optimizer_metrics:
@@ -188,16 +213,16 @@
 
                 _, vectors, layer = tuple(metric.split('/'))
 
                 A, B = tuple(vectors.split('_'))
 
                 A_reduced_norm = optimizer_metrics[f'l2_norm/{A}/{layer}']
                 B_reduced_norm = optimizer_metrics[f'l2_norm/{B}/{layer}']
-                optimizer_metrics[metric] = reduced / (A_reduced_norm *
-                                                       B_reduced_norm)
+                optimizer_metrics[
+                    metric] = reduced / (A_reduced_norm * B_reduced_norm)
             elif metric.startswith('layerwise_lr'):
                 continue
             else:
                 reduced = optimizer_metrics[metric]
                 if dist.get_world_size() > 1:
                     dist.all_reduce(reduced, reduce_operation='SUM')
                 optimizer_metrics[metric] = reduced / dist.get_world_size()
@@ -208,37 +233,47 @@
         """Preprocess metrics to reduce across ranks correctly."""
         # Only L2 norm metric keys are present, can skip sorting at this stage
         for metric in optimizer_metrics:
             # L2 norms need to be squared, before they are reduced via summation
             optimizer_metrics[metric] = optimizer_metrics[metric]**2
         return optimizer_metrics
 
-    def report_per_parameter_metrics(self, param: torch.Tensor, name: str,
-                                     optimizer_metrics: dict):
+    def report_per_parameter_metrics(
+        self,
+        param: torch.Tensor,
+        name: str,
+        optimizer_metrics: dict,
+    ):
         lr = self.param_groups[0]['lr']
         weight_decay = self.param_groups[0]['weight_decay']
         initial_lr = self.param_groups[0]['initial_lr']
 
         beta1, _ = self.param_groups[0]['betas']
         if param in self.state:
             param_optim_state = self.state[param]
             layerwise_lr = self.adjust_lr(
-                lr, self.lr_penalty,
-                len(param_optim_state['outlier_timestamp']), self.min_scale)
+                lr,
+                self.lr_penalty,
+                len(param_optim_state['outlier_timestamp']),
+                self.min_scale,
+            )
 
             step_tensor = param_optim_state['exp_avg'].clone().lerp_(
-                param.grad, 1 - beta1).sign_().mul_(lr)
+                param.grad,
+                1 - beta1,
+            ).sign_().mul_(lr)
             decay_factor = (lr / initial_lr) if initial_lr else 1.0
             step_tensor.add_(param, alpha=-weight_decay * decay_factor)
             for metric in self.metric_functions:
                 optimizer_metrics[f'{metric}/{name}'] = self.metric_functions[
                     metric](param, param_optim_state, step_tensor)
 
             optimizer_metrics[f'layerwise_lr/{name}'] = torch.tensor(
-                layerwise_lr)
+                layerwise_lr,
+            )
 
         return optimizer_metrics
 
 
 class DecoupledClipLion(Optimizer):
     """DecoupledClipLION.
 
@@ -254,58 +289,67 @@
         lr (float): Learning rate for updates
         betas (Tuple[float]): Momentum factors
         weight_decay (float): Weight decay
         outlier_threshold (float): Multiplicative factor determining what constitutes an "outlier" relative to the MVA of gradient norms.
     """
     metric_functions = {
         'l2_norm/moment':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                optim_state['exp_avg']),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(optim_state['exp_avg']),
         'l2_norm/param':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                param.data),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(param.data),
         'l2_norm/update':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                step_tensor),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(step_tensor),
         'l2_norm/grad':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                param.grad),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(param.grad),
     }
 
-    def __init__(self,
-                 params: Union[Iterable[torch.Tensor], Iterable[dict]],
-                 lr: float = 1e-4,
-                 betas: Tuple[float, float] = (0.9, 0.99),
-                 weight_decay: float = 0.0,
-                 outlier_threshold: float = 5.0):
+    def __init__(
+        self,
+        params: Union[Iterable[torch.Tensor], Iterable[dict]],
+        lr: float = 1e-4,
+        betas: Tuple[float, float] = (0.9, 0.99),
+        weight_decay: float = 0.0,
+        outlier_threshold: float = 5.0,
+    ):
         if lr <= 0.:
             raise Exception(f'Invalid LR: {lr}. LR must be > 0')
-        if not all([0. <= beta <= 1. for beta in betas]):
+        if not all(0. <= beta <= 1. for beta in betas):
             raise Exception(
-                f'Invalid beta values: {betas} All betas must be between 0 and 1.'
+                f'Invalid beta values: {betas} All betas must be between 0 and 1.',
             )
         if weight_decay >= 1e-3:
             log.warning(
                 f'You are using a high value of `weight_decay={weight_decay}` for the `DecoupledLionW` optimizer. Are you sure you want to do this? '
                 +
-                f'Your model\'s weights will be multiplied by {1.0 - weight_decay} on every step!'
+                f'Your model\'s weights will be multiplied by {1.0 - weight_decay} on every step!',
             )
 
         defaults = {'lr': lr, 'betas': betas, 'weight_decay': weight_decay}
 
         super().__init__(params, defaults)
 
         for group in self.param_groups:
             group['initial_lr'] = group['lr']
         self.outlier_threshold = outlier_threshold
 
     @staticmethod
-    def lionw(p: torch.Tensor, grad: torch.Tensor, exp_avg: torch.Tensor,
-              lr: float, initial_lr: float, wd: float, beta1: float,
-              beta2: float) -> None:
+    def lionw(
+        p: torch.Tensor,
+        grad: torch.Tensor,
+        exp_avg: torch.Tensor,
+        lr: float,
+        initial_lr: float,
+        wd: float,
+        beta1: float,
+        beta2: float,
+    ) -> None:
         # stepweight decay
         if wd != 0:
             decay_factor = (lr / initial_lr) if initial_lr else 1.0
             p.data.mul_(1 - decay_factor * wd)
 
         # update is interpolation between gradient and momentum
         update = exp_avg.lerp(grad, 1 - beta1).sign_()
@@ -319,27 +363,30 @@
 
         loss = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
-            for p in filter(lambda p: p.grad is not None and p.requires_grad,
-                            group['params']):
+            for p in filter(
+                lambda p: p.grad is not None and p.requires_grad,
+                group['params'],
+            ):
 
                 grad, lr, initial_lr, wd, beta1, beta2, state = p.grad, group[
                     'lr'], group['initial_lr'], group[
                         'weight_decay'], *group['betas'], self.state[p]
 
                 # init state - exponential moving average of gradient values
 
                 if len(state) == 0:
                     state['exp_avg'] = torch.zeros_like(p)
                     state['grad_tracker'] = OutlierDetector(
-                        self.outlier_threshold)
+                        self.outlier_threshold,
+                    )
                     state['clipped_batches'] = torch.tensor(0.0)
 
                 exp_avg = state['exp_avg']
 
                 # determine if the new moment resulting from this grad would be an outlier
                 grad_norm = torch.linalg.vector_norm(grad)**2
 
@@ -384,47 +431,57 @@
 
         return optimizer_metrics
 
     def pre_reduce_metrics(self, optimizer_metrics: Dict[str, torch.Tensor]):
         """Preprocess metrics to reduce across ranks correctly."""
         # Sort L2 norms first so they are squared before other metrics, which depend on squared values
         metrics = optimizer_metrics.keys()
-        metrics = sorted(metrics,
-                         key=lambda metric: 0 if 'l2_norm' in metric else 1)
+        metrics = sorted(
+            metrics,
+            key=lambda metric: 0 if 'l2_norm' in metric else 1,
+        )
         for metric in metrics:
             if metric.startswith('l2_norm'):
                 # L2 norms need to be squared, before they are reduced via summation
                 optimizer_metrics[metric] = optimizer_metrics[metric]**2
             elif metric.startswith('cosine'):
                 _, vectors, layer = tuple(metric.split('/'))
 
                 A, B = tuple(vectors.split('_'))
 
                 # L2 norm would've been squared in previous branch
                 A_rank_subset_norm = math.sqrt(
-                    optimizer_metrics[f'l2_norm/{A}/{layer}'])
+                    optimizer_metrics[f'l2_norm/{A}/{layer}'],
+                )
                 B_rank_subset_norm = math.sqrt(
-                    optimizer_metrics[f'l2_norm/{B}/{layer}'])
+                    optimizer_metrics[f'l2_norm/{B}/{layer}'],
+                )
 
-                optimizer_metrics[
-                    metric] *= A_rank_subset_norm * B_rank_subset_norm
+                optimizer_metrics[metric
+                                 ] *= A_rank_subset_norm * B_rank_subset_norm
 
         return optimizer_metrics
 
-    def report_per_parameter_metrics(self, param: torch.Tensor, name: str,
-                                     optimizer_metrics: dict):
+    def report_per_parameter_metrics(
+        self,
+        param: torch.Tensor,
+        name: str,
+        optimizer_metrics: dict,
+    ):
         lr = self.param_groups[0]['lr']
         weight_decay = self.param_groups[0]['weight_decay']
         initial_lr = self.param_groups[0]['initial_lr']
 
         beta1, _ = self.param_groups[0]['betas']
         if param in self.state:
             param_optim_state = self.state[param]
             step_tensor = param_optim_state['exp_avg'].clone().lerp_(
-                param.grad, 1 - beta1).sign_().mul_(lr)
+                param.grad,
+                1 - beta1,
+            ).sign_().mul_(lr)
             decay_factor = (lr / initial_lr) if initial_lr else 1.0
             step_tensor.add_(param, alpha=-weight_decay * decay_factor)
             for metric in self.metric_functions:
                 optimizer_metrics[f'{metric}/{name}'] = self.metric_functions[
                     metric](param, param_optim_state, step_tensor)
 
             optimizer_metrics[f'clipped_batches/{name}'] = param_optim_state[
```

### Comparing `llm-foundry-0.7.0/llmfoundry/optim/lion.py` & `llm-foundry-0.9.0.dev0/llmfoundry/optim/lion.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,62 +7,73 @@
 
 import torch
 from composer.utils import dist
 from torch.optim.optimizer import Optimizer
 
 log = logging.getLogger(__name__)
 
+__all__ = [
+    'DecoupledLionW',
+]
+
 
 class DecoupledLionW(Optimizer):
     metric_functions = {
         'l2_norm/moment':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                optim_state['exp_avg']),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(optim_state['exp_avg']),
         'l2_norm/param':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                param.data),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(param.data),
         'l2_norm/update':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                step_tensor),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(step_tensor),
         'l2_norm/grad':
-            lambda param, optim_state, step_tensor: torch.linalg.vector_norm(
-                param.grad),
+            lambda param, optim_state, step_tensor: torch.linalg.
+            vector_norm(param.grad),
     }
 
     def __init__(
-            self,
-            params: Union[Iterable[torch.Tensor], Iterable[dict]],
-            lr: float = 1e-4,
-            betas: Tuple[float, float] = (0.9, 0.99),
-            weight_decay: float = 0.0,
+        self,
+        params: Union[Iterable[torch.Tensor], Iterable[dict]],
+        lr: float = 1e-4,
+        betas: Tuple[float, float] = (0.9, 0.99),
+        weight_decay: float = 0.0,
     ):
         if lr <= 0.:
             raise Exception(f'Invalid LR: {lr}. LR must be > 0')
-        if not all([0. <= beta <= 1. for beta in betas]):
+        if not all(0. <= beta <= 1. for beta in betas):
             raise Exception(
-                f'Invalid beta values: {betas} All betas must be between 0 and 1.'
+                f'Invalid beta values: {betas} All betas must be between 0 and 1.',
             )
         if weight_decay >= 1e-3:
             log.warning(
                 f'You are using a high value of `weight_decay={weight_decay}` for the `DecoupledLionW` optimizer. Are you sure you want to do this? '
                 +
-                f'Your model\'s weights will be multiplied by {1.0 - weight_decay} on every step!'
+                f'Your model\'s weights will be multiplied by {1.0 - weight_decay} on every step!',
             )
 
         defaults = {'lr': lr, 'betas': betas, 'weight_decay': weight_decay}
 
         super().__init__(params, defaults)
 
         for group in self.param_groups:
             group['initial_lr'] = group['lr']
 
     @staticmethod
-    def lionw(p: torch.Tensor, grad: torch.Tensor, exp_avg: torch.Tensor,
-              lr: float, initial_lr: float, wd: float, beta1: float,
-              beta2: float) -> None:
+    def lionw(
+        p: torch.Tensor,
+        grad: torch.Tensor,
+        exp_avg: torch.Tensor,
+        lr: float,
+        initial_lr: float,
+        wd: float,
+        beta1: float,
+        beta2: float,
+    ) -> None:
         # stepweight decay
         if wd != 0:
             decay_factor = (lr / initial_lr) if initial_lr else 1.0
             p.data.mul_(1 - decay_factor * wd)
 
         # update is interpolation between gradient and momentum
         update = exp_avg.lerp(grad, 1 - beta1).sign_()
@@ -76,16 +87,18 @@
 
         loss = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
-            for p in filter(lambda p: p.grad is not None and p.requires_grad,
-                            group['params']):
+            for p in filter(
+                lambda p: p.grad is not None and p.requires_grad,
+                group['params'],
+            ):
 
                 grad, lr, initial_lr, wd, beta1, beta2, state = p.grad, group[
                     'lr'], group['initial_lr'], group[
                         'weight_decay'], *group['betas'], self.state[p]
 
                 # init state - exponential moving average of gradient values
 
@@ -127,25 +140,31 @@
         """Preprocess metrics to reduce across ranks correctly."""
         # Only L2 norm metric keys are present, can skip sorting at this stage
         for metric in optimizer_metrics:
             # L2 norms need to be squared, before they are reduced via summation
             optimizer_metrics[metric] = optimizer_metrics[metric]**2
         return optimizer_metrics
 
-    def report_per_parameter_metrics(self, param: torch.Tensor, name: str,
-                                     optimizer_metrics: dict):
+    def report_per_parameter_metrics(
+        self,
+        param: torch.Tensor,
+        name: str,
+        optimizer_metrics: dict,
+    ):
         lr = self.param_groups[0]['lr']
         weight_decay = self.param_groups[0]['weight_decay']
         initial_lr = self.param_groups[0]['initial_lr']
 
         beta1, _ = self.param_groups[0]['betas']
         if param in self.state:
             param_optim_state = self.state[param]
             step_tensor = param_optim_state['exp_avg'].clone().lerp_(
-                param.grad, 1 - beta1).sign_().mul_(lr)
+                param.grad,
+                1 - beta1,
+            ).sign_().mul_(lr)
             decay_factor = (lr / initial_lr) if initial_lr else 1.0
             step_tensor.add_(param, alpha=-weight_decay * decay_factor)
             for metric in self.metric_functions:
                 optimizer_metrics[f'{metric}/{name}'] = self.metric_functions[
                     metric](param, param_optim_state, step_tensor)
 
         return optimizer_metrics
```

### Comparing `llm-foundry-0.7.0/llmfoundry/optim/outlier_detection.py` & `llm-foundry-0.9.0.dev0/llmfoundry/optim/outlier_detection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 import collections
 from typing import Optional
 
+__all__ = ['OutlierDetector']
+
 
 class OutlierDetector:
     """OutlierDetector.
 
     This class implements an algorithm to detect outliers in sequential
     numeric data (e.g. for gradient/moment norms in optimizers). It relies on a
     delayed moving average which is the moving average of observations from time
@@ -40,23 +42,25 @@
             obs (float): Numeric observation for the current timestep.
 
         Returns:
             bool: Indicator of whether the most recent observation was an outlier.
         """
         assert self.intermediate_data_queue.maxlen is not None, 'expected maxlen defined'
 
-        if len(self.intermediate_data_queue
-              ) >= self.intermediate_data_queue.maxlen:
+        if len(
+            self.intermediate_data_queue,
+        ) >= self.intermediate_data_queue.maxlen:
             # move data from intermediate queue to slow moving average queue
             intermediate_obs = self.intermediate_data_queue.popleft()
             self.delayed_moving_average.append(intermediate_obs)
 
         self.intermediate_data_queue.append(obs)
         delayed_mva = self.get_delayed_mva()
         return delayed_mva is not None and obs > self.threshold * delayed_mva
 
     def get_delayed_mva(self) -> Optional[float]:
         if len(self.delayed_moving_average) > 0:
-            return sum(self.delayed_moving_average) / len(
-                self.delayed_moving_average)
+            return sum(
+                self.delayed_moving_average,
+            ) / len(self.delayed_moving_average)
         else:
             return None
```

### Comparing `llm-foundry-0.7.0/llmfoundry/optim/scheduler.py` & `llm-foundry-0.9.0.dev0/llmfoundry/optim/scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 from composer.optim.scheduler import _convert_time
 
 from llmfoundry.utils.warnings import experimental_class
 
 __all__ = ['InverseSquareRootWithWarmupScheduler']
 
 
-def _raise_if_units_dont_match(time: Union[str, Time], t_max: Union[str, Time],
-                               name: str) -> None:
+def _raise_if_units_dont_match(
+    time: Union[str, Time],
+    t_max: Union[str, Time],
+    name: str,
+) -> None:
     new_time = Time.from_input(time)
     new_t_max = Time.from_input(t_max)
 
     if new_time.unit != new_t_max.unit:
         raise ValueError(
-            f'{name} (unit {new_time.unit=}) must match max_duration unit ({new_t_max.unit=}).'
+            f'{name} (unit {new_time.unit=}) must match max_duration unit ({new_t_max.unit=}).',
         )
 
 
 def _raise_if_units_dur(time: Union[str, Time], name: str) -> None:
     new_time = Time.from_input(time)
 
     if new_time.unit == TimeUnit('dur'):
@@ -73,53 +76,68 @@
         t_scale (str | Time): The time scale.
         t_cooldown (str | Time): The cooldown time.
         t_max (str | Time): The duration of this scheduler. Default = ``"1dur"``.
         alpha_f_decay (float): The learning rate multiplier to decay inverse square root decay to. Default = ``0.0``.
         alpha_f_cooldown (float): The learning rate multiplier to decay linear cooldown to. Default = ``0.0``.
     """
 
-    def __init__(self,
-                 t_warmup: Union[str, Time],
-                 t_scale: Union[str, Time],
-                 t_cooldown: Union[str, Time],
-                 t_max: Union[str, Time] = '1dur',
-                 alpha_f_decay: float = 0.0,
-                 alpha_f_cooldown: float = 0.0) -> None:
+    def __init__(
+        self,
+        t_warmup: Union[str, Time],
+        t_scale: Union[str, Time],
+        t_cooldown: Union[str, Time],
+        t_max: Union[str, Time] = '1dur',
+        alpha_f_decay: float = 0.0,
+        alpha_f_cooldown: float = 0.0,
+    ) -> None:
         if alpha_f_decay < alpha_f_cooldown:
-            raise ValueError(('Required: alpha_f_decay >= alpha_f_cooldown. '
-                              f'Current: alpha_f_decay={alpha_f_decay}, '
-                              f'alpha_f_cooldown={alpha_f_cooldown}.'))
+            raise ValueError((
+                'Required: alpha_f_decay >= alpha_f_cooldown. '
+                f'Current: alpha_f_decay={alpha_f_decay}, '
+                f'alpha_f_cooldown={alpha_f_cooldown}.'
+            ))
         _raise_if_units_dur(t_warmup, 't_warmup')
         _raise_if_units_dur(t_scale, 't_scale')
         _raise_if_units_dur(t_cooldown, 't_cooldown')
         self.t_warmup = t_warmup
         self.t_scale = t_scale
         self.t_cooldown = t_cooldown
         self.t_max = t_max
         self.alpha_f_decay = alpha_f_decay
         self.alpha_f_cooldown = alpha_f_cooldown
-        self.warmup_scheduler = LinearScheduler(alpha_i=0.0,
-                                                alpha_f=1.0,
-                                                t_max=t_warmup)
+        self.warmup_scheduler = LinearScheduler(
+            alpha_i=0.0,
+            alpha_f=1.0,
+            t_max=t_warmup,
+        )
 
     def __call__(self, state: State, ssr: float = 1.0) -> float:
         assert state.max_duration is not None, 'max_duration should be set whenever schedulers are invoked'
-        _raise_if_units_dont_match(self.t_warmup, state.max_duration,
-                                   't_warmup')
+        _raise_if_units_dont_match(
+            self.t_warmup,
+            state.max_duration,
+            't_warmup',
+        )
         _raise_if_units_dont_match(self.t_scale, state.max_duration, 't_scale')
-        _raise_if_units_dont_match(self.t_cooldown, state.max_duration,
-                                   't_cooldown')
+        _raise_if_units_dont_match(
+            self.t_cooldown,
+            state.max_duration,
+            't_cooldown',
+        )
 
         t_warmup = _convert_time(self.t_warmup, state)
         if t_warmup.value == 0:
             warnings.warn(
-                textwrap.dedent("""\
+                textwrap.dedent(
+                    """\
                 The warmup duration is 0. If warmup was specified as a fraction of the total
                 training duration, the warmup duration is calculated in the
-                same unit as the trainer's max_duration parameter."""))
+                same unit as the trainer's max_duration parameter.""",
+                ),
+            )
 
         if state.timestamp < t_warmup:
             return self.warmup_scheduler(state)
 
         t_scale = _convert_time(self.t_scale, state, ssr=ssr)
         t_cooldown = _convert_time(self.t_cooldown, state, ssr=ssr)
         t_max = _convert_time(self.t_max, state, ssr=ssr)
@@ -132,26 +150,28 @@
             t_cooldown_start = t_warmup
 
         if state.timestamp < t_cooldown_start:
             # Rescale LR by a coefficient equal to the inverse square root of the time
             # elapsed after warmup, rescaled by the time scale, such that, at
             # infinite time, the LR decays to alpha_f_decay.
             coeff = 1 / ((current_time + t_shift) / t_scale).value**0.5
-            current_factor = (self.alpha_f_decay + coeff *
-                              (1.0 - self.alpha_f_decay))
+            current_factor = (
+                self.alpha_f_decay + coeff * (1.0 - self.alpha_f_decay)
+            )
             return current_factor
 
         else:
             coeff = 1 / ((t_cooldown_start + t_shift) / t_scale).value**0.5
             alpha_i = self.alpha_f_decay + coeff * (1.0 - self.alpha_f_decay)
 
             if t_cooldown.value == 0:
                 return alpha_i
 
             # Linearly decay the LR from its value at the step at which cooldown
             # started to alpha_f_cooldown over t_cooldown time.
             frac_of_cooldown = ((current_time - t_cooldown_start) /
                                 t_cooldown).value
             frac_of_cooldown = min(1.0, frac_of_cooldown)
-            current_factor = (alpha_i + frac_of_cooldown *
-                              (self.alpha_f_cooldown - alpha_i))
+            current_factor = (
+                alpha_i + frac_of_cooldown * (self.alpha_f_cooldown - alpha_i)
+            )
             return current_factor
```

### Comparing `llm-foundry-0.7.0/llmfoundry/tokenizers/tiktoken.py` & `llm-foundry-0.9.0.dev0/llmfoundry/tokenizers/tiktoken.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-# Copyright 2022 MosaicML LLM Foundry authors
+# Copyright 2024 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
+
 from functools import lru_cache
 from typing import Any, Dict, List, Optional, Tuple
 
 from transformers import PreTrainedTokenizer
 
+__all__ = [
+    'TiktokenTokenizerWrapper',
+]
+
 DEFAULT_SYSTEM_PROMPT = """You are a helpful, respectful and honest assistant. Always answer as helpfully as possible."""
 
 
 # Taken from
 # https://github.com/huggingface/transformers/blob/8aca43bdb3cb9a5020f6d57589d85679dc873b1c/src/transformers/models/gpt2/tokenization_gpt2.py#L62-L84
 @lru_cache()
 def bytes_to_unicode():
@@ -20,19 +25,21 @@
     The reversible bpe codes work on unicode strings. This means you need a
     large # of unicode characters in your vocab if you want to avoid UNKs. When
     you're at something like a 10B token dataset you end up needing around 5K
     for decent coverage. This is a significant percentage of your normal, say,
     32K bpe vocab. To avoid that, we want lookup tables between utf-8 bytes and
     unicode strings.
     """
-    bs = (list(range(ord('!'),
-                     ord('~') + 1)) + list(range(ord('¡'),
-                                                 ord('¬') + 1)) +
-          list(range(ord('®'),
-                     ord('ÿ') + 1)))
+    bs = (
+        list(range(ord('!'),
+                   ord('~') + 1)) + list(range(ord('¡'),
+                                               ord('¬') + 1)) +
+        list(range(ord('®'),
+                   ord('ÿ') + 1))
+    )
     cs = bs[:]
     n = 0
     for b in range(2**8):
         if b not in bs:
             bs.append(b)
             cs.append(2**8 + n)
             n += 1
@@ -46,26 +53,28 @@
     tokenizers.
 
     See HuggingFace for further documentation on general tokenizer methods.
     """
 
     model_input_names = ['input_ids', 'attention_mask']
 
-    def __init__(self,
-                 model_name: Optional[str] = None,
-                 encoding_name: Optional[str] = None,
-                 add_bos_token: bool = False,
-                 add_eos_token: bool = False,
-                 use_default_system_prompt: bool = False,
-                 unk_token: Optional[str] = '<|endoftext|>',
-                 eos_token: Optional[str] = '<|endoftext|>',
-                 bos_token: Optional[str] = '<|endoftext|>',
-                 pad_token: Optional[str] = None,
-                 errors: str = 'replace',
-                 **kwargs: Any):
+    def __init__(
+        self,
+        model_name: Optional[str] = None,
+        encoding_name: Optional[str] = None,
+        add_bos_token: bool = False,
+        add_eos_token: bool = False,
+        use_default_system_prompt: bool = False,
+        unk_token: Optional[str] = '<|endoftext|>',
+        eos_token: Optional[str] = '<|endoftext|>',
+        bos_token: Optional[str] = '<|endoftext|>',
+        pad_token: Optional[str] = None,
+        errors: str = 'replace',
+        **kwargs: Any,
+    ):
         """Constructor creates a tiktoken tokenizer to use as the underlying.
 
         tokenizer.
 
         Args:
             model_name (Optional[str], optional): The name of the model to load from tiktoken. Defaults to None.
                 Either model_name or encoding_name must be set, but not both.
@@ -82,50 +91,57 @@
                 [bytes.decode](https://docs.python.org/3/library/stdtypes.html#bytes.decode) for more information.
                 Defaults to `"replace"`.
         """
         try:
             import tiktoken
         except:
             raise ImportError(
-                'You need to install tiktoken to use TiktokenTokenizerWrapper.')
+                'You need to install tiktoken to use TiktokenTokenizerWrapper.',
+            )
 
         # Workaround to make tiktokenizer picklable.
         # https://github.com/huggingface/datasets/issues/5536#issuecomment-1682309347
         # There is an open PR from HF to add this to tiktoken: https://github.com/openai/tiktoken/pull/181
         import copyreg
         import functools
 
         from tiktoken import Encoding  # type: ignore (thirdParty)
 
         def pickle_Encoding(enc: Encoding):
-            return (functools.partial(Encoding,
-                                      enc.name,
-                                      pat_str=enc._pat_str,
-                                      mergeable_ranks=enc._mergeable_ranks,
-                                      special_tokens=enc._special_tokens), ())
+            return (
+                functools.partial(
+                    Encoding,
+                    enc.name,
+                    pat_str=enc._pat_str,
+                    mergeable_ranks=enc._mergeable_ranks,
+                    special_tokens=enc._special_tokens,
+                ),
+                (),
+            )
 
         copyreg.pickle(Encoding, pickle_Encoding)
 
         if model_name is not None and encoding_name is not None:
             raise ValueError(
-                'You need to specify either model_name or encoding_name, not both.'
+                'You need to specify either model_name or encoding_name, not both.',
             )
 
         self.model_name = model_name
         self.encoding_name = encoding_name
 
         if self.model_name is not None:
             self.encoding = tiktoken.encoding_for_model(  # type: ignore (thirdParty)
                 self.model_name)
         elif self.encoding_name is not None:
             self.encoding = tiktoken.get_encoding(  # type: ignore (thirdParty)
                 self.encoding_name)
         else:
             raise ValueError(
-                'You need to specify either model_name or encoding_name.')
+                'You need to specify either model_name or encoding_name.',
+            )
 
         self.add_bos_token = add_bos_token
         self.add_eos_token = add_eos_token
         self.use_default_system_prompt = use_default_system_prompt
 
         self.byte_encoder = bytes_to_unicode()
         self.byte_decoder = {v: k for k, v in self.byte_encoder.items()}
@@ -146,25 +162,27 @@
             self.decoder[i] = decoding
 
         self.encoder: Dict[str, int] = {}
         for i in range(self.encoding.n_vocab):
             if i in self.decoder:
                 self.encoder[self.decoder[i]] = i
 
-        super().__init__(model_name=model_name,
-                         encoding_name=encoding_name,
-                         add_bos_token=add_bos_token,
-                         add_eos_token=add_eos_token,
-                         use_default_system_prompt=use_default_system_prompt,
-                         unk_token=unk_token,
-                         eos_token=eos_token,
-                         bos_token=bos_token,
-                         pad_token=pad_token,
-                         errors=errors,
-                         **kwargs)
+        super().__init__(
+            model_name=model_name,
+            encoding_name=encoding_name,
+            add_bos_token=add_bos_token,
+            add_eos_token=add_eos_token,
+            use_default_system_prompt=use_default_system_prompt,
+            unk_token=unk_token,
+            eos_token=eos_token,
+            bos_token=bos_token,
+            pad_token=pad_token,
+            errors=errors,
+            **kwargs,
+        )
 
     @property
     def vocab_size(self) -> int:
         """Returns vocab size."""
         return self.encoding.n_vocab
 
     @property
@@ -196,50 +214,56 @@
             "{{ '<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' }}"
             '{% else %}'
             "{{ '\n' + '<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' }}"
             '{% endif %}'
             '{% if (add_generation_prompt == true and loop.last) %}'
             "{{ '\n' + '<|im_start|>' + 'assistant' + '\n' }}"
             '{% endif %}'
-            '{% endfor %}')
+            '{% endfor %}'
+        )
         template = template.replace(
             'USE_DEFAULT_PROMPT',
-            'true' if self.use_default_system_prompt else 'false')
-        template = template.replace('DEFAULT_SYSTEM_PROMPT',
-                                    DEFAULT_SYSTEM_PROMPT)
+            'true' if self.use_default_system_prompt else 'false',
+        )
+        template = template.replace(
+            'DEFAULT_SYSTEM_PROMPT',
+            DEFAULT_SYSTEM_PROMPT,
+        )
         return template
 
     def get_vocab(self) -> Dict[str, int]:
         """Returns vocab as a dict."""
         # As far as I can tell, we don't require get_vocab to completely work,
         # but when using additional_special_tokens, Hugging Face determines the next
         # token index to add with len(self.get_vocab()) so we need the _size_ of this dictionary to be correct.
         vocab_clone = self.encoder.copy()
         extra_id_index = 0
         candidate_extra_id = f'<extra_id_{extra_id_index}>'
-        indices_to_fill_in = {i for i in range(self.vocab_size)} - set(
-            vocab_clone.values())
+        indices_to_fill_in = (
+            set(range(self.vocab_size)) - set(vocab_clone.values())
+        )
 
         # Add enough indices to make get_vocab() the right length
         for index_to_add in indices_to_fill_in:
             # Make sure we don't overwrite a token that already exists
             while candidate_extra_id in vocab_clone:
                 extra_id_index += 1
                 candidate_extra_id = f'<extra_id_{extra_id_index}>'
 
             # Get an index to add and add the item
             vocab_clone[candidate_extra_id] = index_to_add
 
-        return vocab_clone
+        return dict(vocab_clone, **self.added_tokens_encoder)
 
     def _tokenize(self, text: str) -> List[str]:
         """Returns a tokenized string."""
         if not isinstance(text, str):
             raise ValueError(
-                f'Expected a string input to _tokenize but got {type(text)}.')
+                f'Expected a string input to _tokenize but got {type(text)}.',
+            )
 
         tokens = [
             self.decoder[t]
             for t in self.encoding.encode(text, allowed_special='all')
         ]
 
         return tokens
@@ -255,36 +279,38 @@
         # but not slow tokenizers.
         return self.decoder.get(index, '')
 
     def convert_tokens_to_string(self, tokens: List[str]) -> str:
         """Converts a sequence of tokens (string) in a single string."""
         text = ''.join(tokens)
         text = bytearray([self.byte_decoder[c] for c in text
-                         ]).decode('utf-8', errors=self.errors)
+                         ],).decode('utf-8', errors=self.errors)
         return text
 
     def build_inputs_with_special_tokens(
-            self,
-            token_ids_0: List[int],
-            token_ids_1: Optional[List[int]] = None) -> List[int]:
+        self,
+        token_ids_0: List[int],
+        token_ids_1: Optional[List[int]] = None,
+    ) -> List[int]:
         bos_token_id = [self.bos_token_id] if self.add_bos_token else []
         eos_token_id = [self.eos_token_id] if self.add_eos_token else []
 
         output = bos_token_id + token_ids_0 + eos_token_id
 
         if token_ids_1 is not None:
             output = output + bos_token_id + token_ids_1 + eos_token_id
 
         return output
 
     def get_special_tokens_mask(
-            self,
-            token_ids_0: List[int],
-            token_ids_1: Optional[List[int]] = None,
-            already_has_special_tokens: bool = False) -> List[int]:
+        self,
+        token_ids_0: List[int],
+        token_ids_1: Optional[List[int]] = None,
+        already_has_special_tokens: bool = False,
+    ) -> List[int]:
         """Retrieves sequence ids from a token list that has no special tokens.
 
         Function copied from
         https://github.com/huggingface/transformers/blob/e3a4bd2bee212a2d0fd9f03b27fe7bfc1debe42d/src/transformers/models/gpt2/tokenization_gpt2.py#L265-L295
 
         added. This method is called when adding special tokens using the
         tokenizer `prepare_for_model` or `encode_plus` methods.
@@ -300,37 +326,43 @@
         Returns:
             `List[int]`: A list of integers in the range [0, 1]: 1 for a special token, 0 for a sequence token.
         """
         if already_has_special_tokens:
             return super().get_special_tokens_mask(
                 token_ids_0=token_ids_0,
                 token_ids_1=token_ids_1,
-                already_has_special_tokens=True)
+                already_has_special_tokens=True,
+            )
 
         bos_token_id = [1] if self.add_bos_token else []
         eos_token_id = [1] if self.add_eos_token else []
 
         if token_ids_1 is None:
             return bos_token_id + ([0] * len(token_ids_0)) + eos_token_id
-        return (bos_token_id + ([0] * len(token_ids_0)) + eos_token_id +
-                bos_token_id + ([0] * len(token_ids_1)) + eos_token_id)
+        return (
+            bos_token_id + ([0] * len(token_ids_0)) + eos_token_id +
+            bos_token_id + ([0] * len(token_ids_1)) + eos_token_id
+        )
 
     def create_token_type_ids_from_sequences(
-            self,
-            token_ids_0: List[int],
-            token_ids_1: Optional[List[int]] = None) -> List[int]:
+        self,
+        token_ids_0: List[int],
+        token_ids_1: Optional[List[int]] = None,
+    ) -> List[int]:
         sep = [self.sep_token_id]
 
         if token_ids_1 is None:
             return len(token_ids_0 + sep) * [0]
         return len(token_ids_0 + sep) * [0] + len(token_ids_1 + sep) * [1]
 
-    def save_vocabulary(self,
-                        save_directory: str,
-                        filename_prefix: Optional[str] = None) -> Tuple[str]:
+    def save_vocabulary(
+        self,
+        save_directory: str,
+        filename_prefix: Optional[str] = None,
+    ) -> Tuple[str]:
 
         # ignore the below type to keep the original signature
         # we are knowingly breaking the signature here, although not 100% certain
         # it doesn't have side effects
         # There is some code in huggingface that calls this function to get the vocab files,
         # but it doesn't seem to access them (or at least checks for their existence
         # before accessing them)
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,104 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
-from llmfoundry.utils.builders import (build_algorithm, build_callback,
-                                       build_logger, build_optimizer,
-                                       build_scheduler, build_tokenizer)
+from llmfoundry.utils.builders import (
+    build_algorithm,
+    build_callback,
+    build_composer_model,
+    build_evaluators,
+    build_icl_data_and_gauntlet,
+    build_icl_evaluators,
+    build_logger,
+    build_metric,
+    build_optimizer,
+    build_scheduler,
+    build_tokenizer,
+)
 from llmfoundry.utils.checkpoint_conversion_helpers import (
-    convert_and_save_ft_weights, get_hf_tokenizer_from_composer_state_dict,
-    load_tokenizer)
-from llmfoundry.utils.config_utils import (calculate_batch_size_info,
-                                           log_config, pop_config,
-                                           process_init_device,
-                                           update_batch_size_info)
-from llmfoundry.utils.data_prep_utils import (DownloadingIterable,
-                                              merge_shard_groups, with_id)
+    convert_and_save_ft_weights,
+    get_hf_tokenizer_from_composer_state_dict,
+    load_tokenizer,
+)
+from llmfoundry.utils.config_utils import (
+    calculate_batch_size_info,
+    log_config,
+    pop_config,
+    process_init_device,
+    update_batch_size_info,
+)
+from llmfoundry.utils.data_prep_utils import (
+    DownloadingIterable,
+    merge_shard_groups,
+)
 from llmfoundry.utils.huggingface_hub_utils import \
     edit_files_for_hf_compatibility
 from llmfoundry.utils.logging_utils import SpecificWarningFilter
 from llmfoundry.utils.model_download_utils import (
-    download_from_hf_hub, download_from_http_fileserver, download_from_oras)
-
-# isort: off
+    download_from_hf_hub,
+    download_from_http_fileserver,
+    download_from_oras,
+)
 from llmfoundry.utils.mosaicml_logger_utils import (
     find_mosaicml_logger,
     log_eval_analytics,
     log_train_analytics,
     maybe_create_mosaicml_logger,
 )
-# isort: on
 from llmfoundry.utils.prompt_files import load_prompts, load_prompts_from_file
-from llmfoundry.utils.registry_utils import (TypedRegistry,
-                                             construct_from_registry,
-                                             create_registry)
-from llmfoundry.utils.warnings import VersionedDeprecationWarning
+from llmfoundry.utils.registry_utils import (
+    TypedRegistry,
+    construct_from_registry,
+    create_registry,
+    import_file,
+    save_registry,
+)
+from llmfoundry.utils.warnings import (
+    ExperimentalWarning,
+    VersionedDeprecationWarning,
+    experimental_class,
+    experimental_function,
+)
 
 __all__ = [
     'build_algorithm',
     'build_callback',
+    'build_evaluators',
+    'build_icl_data_and_gauntlet',
+    'build_icl_evaluators',
     'build_logger',
     'build_optimizer',
     'build_scheduler',
     'build_tokenizer',
-    'convert_and_save_ft_weights',
+    'build_composer_model',
+    'build_metric',
     'get_hf_tokenizer_from_composer_state_dict',
     'load_tokenizer',
-    'calculate_batch_size_info',
-    'log_config',
+    'convert_and_save_ft_weights',
     'pop_config',
+    'calculate_batch_size_info',
     'update_batch_size_info',
     'process_init_device',
+    'log_config',
     'DownloadingIterable',
     'merge_shard_groups',
-    'with_id',
     'edit_files_for_hf_compatibility',
     'SpecificWarningFilter',
     'download_from_http_fileserver',
     'download_from_hf_hub',
     'download_from_oras',
+    'maybe_create_mosaicml_logger',
+    'find_mosaicml_logger',
+    'log_eval_analytics',
+    'log_train_analytics',
     'load_prompts',
     'load_prompts_from_file',
-    'VersionedDeprecationWarning',
+    'TypedRegistry',
     'create_registry',
     'construct_from_registry',
-    'TypedRegistry',
-    'find_mosaicml_logger',
-    'log_eval_analytics',
-    'log_train_analytics',
-    'maybe_create_mosaicml_logger',
+    'import_file',
+    'save_registry',
+    'VersionedDeprecationWarning',
+    'ExperimentalWarning',
+    'experimental_function',
+    'experimental_class',
 ]
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/builders.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/builders.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,34 +3,42 @@
 
 import contextlib
 import functools
 import logging
 import os
 import re
 from collections import OrderedDict
-from typing import (Any, ContextManager, Dict, Iterable, List, Optional, Tuple,
-                    Union)
+from typing import (
+    Any,
+    ContextManager,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
 
 import torch
 from composer.core import Algorithm, Callback, Evaluator
-from composer.datasets.in_context_learning_evaluation import \
-    get_icl_task_dataloader
 from composer.loggers import LoggerDestination
 from composer.models import ComposerModel
 from composer.optim.scheduler import ComposerScheduler
 from composer.utils import dist
 from omegaconf import DictConfig, ListConfig
 from omegaconf import OmegaConf as om
 from torch.optim.optimizer import Optimizer
 from torchmetrics import Metric
 from transformers import AutoTokenizer, PreTrainedTokenizerBase
 
 from llmfoundry import registry
 from llmfoundry.callbacks import EvalGauntlet
 from llmfoundry.data.dataloader import build_dataloader
+from llmfoundry.eval.datasets.in_context_learning_evaluation import \
+    get_icl_task_dataloader
 from llmfoundry.tokenizers.tiktoken import TiktokenTokenizerWrapper
 from llmfoundry.utils.registry_utils import construct_from_registry
 
 log = logging.getLogger(__name__)
 
 __all__ = [
     'build_algorithm',
@@ -92,22 +100,26 @@
         eval_configs: ListConfig = eval_loader_config
         is_multi_eval = True
     else:
         eval_configs = ListConfig([eval_loader_config])
         is_multi_eval = False
 
     for eval_config in eval_configs:
-        eval_dataloader = build_dataloader(eval_config, tokenizer,
-                                           device_eval_batch_size)
+        eval_dataloader = build_dataloader(
+            eval_config,
+            tokenizer,
+            device_eval_batch_size,
+        )
         eval_loader: Evaluator = Evaluator(
             label=f'eval/{eval_config.label}' if is_multi_eval else 'eval',
             dataloader=eval_dataloader,
             # Load the eval data to fail fast. metrics will get added
             # later in add_metrics_to_eval_loaders, after the model is loaded
             metric_names=[],
+            device_eval_microbatch_size=device_eval_batch_size,
         )
         evaluators.append(eval_loader)
     return evaluators
 
 
 def add_metrics_to_eval_loaders(
     evaluators: List[Evaluator],
@@ -127,33 +139,34 @@
 
 def build_icl_data_and_gauntlet(
     icl_tasks_config: Union[str, ListConfig],
     eval_gauntlet_config: Optional[Union[str, DictConfig]],
     tokenizer: PreTrainedTokenizerBase,
     device_eval_batch_size: int,
     icl_seq_len: int,
-    icl_subset_num_batches: Optional[int] = None
+    icl_subset_num_batches: Optional[int] = None,
 ) -> Tuple[List[Evaluator], List[str], Optional[EvalGauntlet]]:
     icl_evaluators, logger_keys = build_icl_evaluators(
         icl_tasks_config,
         tokenizer,
         icl_seq_len,
         device_eval_batch_size,
-        icl_subset_num_batches=icl_subset_num_batches)
+        icl_subset_num_batches=icl_subset_num_batches,
+    )
     eval_gauntlet_cb = None
     if eval_gauntlet_config is not None:
         if isinstance(eval_gauntlet_config, str):
             with open(eval_gauntlet_config, 'r') as icl_f:
                 eval_gauntlet_cfg = om.load(icl_f)
             eval_gauntlet = eval_gauntlet_cfg.eval_gauntlet
         elif isinstance(eval_gauntlet_config, DictConfig):  # pyright: ignore
             eval_gauntlet = eval_gauntlet_config
         else:
             raise ValueError(
-                f'Got invalid type for eval_gauntlet_config: {type(eval_gauntlet_config)}'
+                f'Got invalid type for eval_gauntlet_config: {type(eval_gauntlet_config)}',
             )
         eval_gauntlet.logger_keys = logger_keys
         eval_gauntlet.benchmark_sizes = {
             e.label: e.dataloader.num_samples for e in icl_evaluators
         }
         eval_gauntlet_cb = EvalGauntlet(**eval_gauntlet)
     return icl_evaluators, logger_keys, eval_gauntlet_cb
@@ -185,91 +198,104 @@
         model = construct_from_registry(
             name=name,
             registry=registry.models,
             pre_validation_function=ComposerModel,
             post_validation_function=None,
             kwargs={
                 'om_model_config': cfg,
-                'tokenizer': tokenizer
+                'tokenizer': tokenizer,
             },
         )
 
     str_dtype_to_torch_dtype = {
         'f16': torch.float16,
         'float16': torch.float16,
         'bf16': torch.bfloat16,
         'bfloat16': torch.bfloat16,
     }
 
     if master_weights_dtype is not None:
         if master_weights_dtype not in str_dtype_to_torch_dtype:
             raise ValueError(
                 f'Invalid master_weights_dtype: {master_weights_dtype}. ' +
-                f'Valid options are: {list(str_dtype_to_torch_dtype.keys())}.')
+                f'Valid options are: {list(str_dtype_to_torch_dtype.keys())}.',
+            )
         dtype = str_dtype_to_torch_dtype[master_weights_dtype]
         model = model.to(dtype=dtype)
 
     return model
 
 
 def build_callback(
     name: str,
     kwargs: Optional[Dict[str, Any]] = None,
-    config: Any = None,
+    train_config: Any = None,
 ) -> Callback:
     """Builds a callback from the registry."""
     registry_to_use = registry.callbacks
     if name in registry.callbacks_with_config:
         if kwargs is None:
             kwargs = {}
-        if 'config' in kwargs:
+        if 'train_config' in kwargs:
             raise ValueError(
-                f'`config` is a reserved keyword for callbacks with config. Please remove it from the kwargs.'
+                f'`train_config` is a reserved keyword for callbacks with config. Please remove it from the kwargs.',
             )
-        kwargs['config'] = config
+        kwargs['train_config'] = train_config
         registry_to_use = registry.callbacks_with_config
 
-    return construct_from_registry(name=name,
-                                   registry=registry_to_use,
-                                   partial_function=True,
-                                   pre_validation_function=Callback,
-                                   post_validation_function=None,
-                                   kwargs=kwargs)
+    return construct_from_registry(
+        name=name,
+        registry=registry_to_use,
+        partial_function=True,
+        pre_validation_function=Callback,
+        post_validation_function=None,
+        kwargs=kwargs,
+    )
 
 
-def build_logger(name: str,
-                 kwargs: Optional[Dict[str, Any]] = None) -> LoggerDestination:
+def build_logger(
+    name: str,
+    kwargs: Optional[Dict[str, Any]] = None,
+) -> LoggerDestination:
     """Builds a logger from the registry."""
-    return construct_from_registry(name=name,
-                                   registry=registry.loggers,
-                                   partial_function=True,
-                                   pre_validation_function=LoggerDestination,
-                                   post_validation_function=None,
-                                   kwargs=kwargs)
+    return construct_from_registry(
+        name=name,
+        registry=registry.loggers,
+        partial_function=True,
+        pre_validation_function=LoggerDestination,
+        post_validation_function=None,
+        kwargs=kwargs,
+    )
 
 
-def build_algorithm(name: str,
-                    kwargs: Optional[Dict[str, Any]] = None) -> Algorithm:
+def build_algorithm(
+    name: str,
+    kwargs: Optional[Dict[str, Any]] = None,
+) -> Algorithm:
     """Builds an algorithm from the registry."""
-    return construct_from_registry(name=name,
-                                   registry=registry.algorithms,
-                                   partial_function=True,
-                                   pre_validation_function=Algorithm,
-                                   post_validation_function=None,
-                                   kwargs=kwargs)
+    return construct_from_registry(
+        name=name,
+        registry=registry.algorithms,
+        partial_function=True,
+        pre_validation_function=Algorithm,
+        post_validation_function=None,
+        kwargs=kwargs,
+    )
 
 
 def build_metric(name: str, kwargs: Optional[Dict[str, Any]] = None) -> Metric:
     """Builds a metric from the registry."""
-    return construct_from_registry(name=name,
-                                   registry=registry.metrics,
-                                   partial_function=True,
-                                   pre_validation_function=Metric,
-                                   post_validation_function=None,
-                                   kwargs=kwargs)
+    return construct_from_registry(
+        name=name,
+        registry=registry.metrics,
+        partial_function=True,
+        pre_validation_function=Metric,
+        post_validation_function=None,
+        kwargs=kwargs,
+    )
 
 
 def _extract_param_groups(
     model: torch.nn.Module,
     optimizer_config: Optional[Dict[str, Any]] = None,
 ) -> Union[Iterable[torch.Tensor], Iterable[Dict[str, Any]]]:
     """Extracts parameter groups defined in the optimizer config.
@@ -368,82 +394,90 @@
         params.insert(0, {'params': param_dict.values()})
         return params
 
     return model.parameters()
 
 
 def build_optimizer(
-        model: torch.nn.Module,
-        name: str,
-        optimizer_config: Optional[Dict[str, Any]] = None) -> Optimizer:
+    model: torch.nn.Module,
+    name: str,
+    optimizer_config: Optional[Dict[str, Any]] = None,
+) -> Optimizer:
 
     params = _extract_param_groups(model, optimizer_config)
     kwargs = optimizer_config
 
     if kwargs is None:
         kwargs = {}
     if 'params' in kwargs:
         raise ValueError(
             'The `params` will be automatically extracted from the model and ' +
-            'optimizer config. Please remove it from the optimizer config kwargs.'
+            'optimizer config. Please remove it from the optimizer config kwargs.',
         )
 
     kwargs['params'] = params
-    return construct_from_registry(name=name,
-                                   registry=registry.optimizers,
-                                   partial_function=True,
-                                   pre_validation_function=Optimizer,
-                                   post_validation_function=None,
-                                   kwargs=kwargs)
+    return construct_from_registry(
+        name=name,
+        registry=registry.optimizers,
+        partial_function=True,
+        pre_validation_function=Optimizer,
+        post_validation_function=None,
+        kwargs=kwargs,
+    )
 
 
 def build_scheduler(
-        name: str,
-        scheduler_config: Optional[Dict[str, Any]] = None) -> ComposerScheduler:
+    name: str,
+    scheduler_config: Optional[Dict[str, Any]] = None,
+) -> ComposerScheduler:
     return construct_from_registry(
         name=name,
         registry=registry.schedulers,
         partial_function=True,
         pre_validation_function=ComposerScheduler,
         post_validation_function=None,
         kwargs=scheduler_config,
     )
 
 
 def build_tokenizer(
-        tokenizer_name: str,
-        tokenizer_kwargs: Dict[str, Any]) -> PreTrainedTokenizerBase:
+    tokenizer_name: str,
+    tokenizer_kwargs: Dict[str, Any],
+) -> PreTrainedTokenizerBase:
     os.environ['TRANSFORMERS_NO_ADVISORY_WARNINGS'] = '1'
     os.environ['TOKENIZERS_PARALLELISM'] = 'false'
 
     signal_file_path = f'.node_{dist.get_node_rank()}_local_rank0_completed_tokenizer_setup'
 
     if dist.is_available() and dist.is_initialized(
     ) and dist.get_world_size() > 1:
         # Make sure the tokenizer files are downloaded and cached first by local rank 0
         with dist.local_rank_zero_download_and_wait(signal_file_path):
             pass
 
     if tokenizer_name.startswith('tiktoken'):
         tokenizer = TiktokenTokenizerWrapper(**tokenizer_kwargs)
     else:
-        tokenizer = AutoTokenizer.from_pretrained(tokenizer_name,
-                                                  **tokenizer_kwargs)
+        tokenizer = AutoTokenizer.from_pretrained(
+            tokenizer_name,
+            **tokenizer_kwargs,
+        )
 
         # HuggingFace does not respect the model_max_length kwarg, and overrides it with
         # min(kwargs['model_max_length'], original_config['model_max_length']), so we
         # explicitly set it here
         tokenizer.model_max_length = tokenizer_kwargs.get(
             'model_max_length',
             int(1e30),
         )
 
     if not hasattr(tokenizer, 'eos_token') or tokenizer.eos_token is None:
         raise ValueError(
-            f'The tokenizer {tokenizer_name} must have an eos_token.')
+            f'The tokenizer {tokenizer_name} must have an eos_token.',
+        )
 
     if dist.is_available() and dist.is_initialized(
     ) and dist.get_world_size() > 1:
         if dist.get_local_rank() == 0:
             with open(signal_file_path, 'wb') as f:
                 f.write(b'local_rank0_completed_tokenizer_setup')
 
@@ -485,27 +519,27 @@
         assert 'num_fewshot' in icl_cfg
 
         if 'metric_names' not in icl_cfg:
             if icl_cfg.icl_task_type == 'language_modeling':
                 icl_cfg.metric_names = ['InContextLearningLMAccuracy']
             elif icl_cfg.icl_task_type == 'multiple_choice':
                 icl_cfg.metric_names = [
-                    'InContextLearningMultipleChoiceAccuracy'
+                    'InContextLearningMultipleChoiceAccuracy',
                 ]
             elif icl_cfg.icl_task_type == 'schema':
                 icl_cfg.metric_names = [
-                    'InContextLearningMultipleChoiceAccuracy'
+                    'InContextLearningMultipleChoiceAccuracy',
+                ]
+            elif icl_cfg.icl_task_type == 'generation_task_with_answers':
+                icl_cfg.metric_names = [
+                    'InContextLearningGenerationExactMatchAccuracy',
                 ]
-            elif icl_cfg.icl_task_type == 'question_answering':
-                icl_cfg.metric_names = ['InContextLearningQAAccuracy']
-            elif icl_cfg.icl_task_type == 'code_evaluation':
-                icl_cfg.metric_names = ['InContextLearningCodeEvalAccuracy']
             else:
                 raise ValueError(
-                    f'No metric_names defined, unable to build default metrics for icl_task_type={icl_cfg.icl_task_type}.'
+                    f'No metric_names defined, unable to build default metrics for icl_task_type={icl_cfg.icl_task_type}.',
                 )
 
         if 'prompt_string' not in icl_cfg:
             icl_cfg.prompt_string = ''
         if 'example_delimiter' not in icl_cfg:
             icl_cfg.example_delimiter = '\n'
         if 'continuation_delimiter' not in icl_cfg:
@@ -542,21 +576,26 @@
             if dist.get_local_rank() == 0 and os.path.exists(destination_path):
                 os.remove(destination_path)
             dist.barrier()
 
             hf_parsing_map = icl_cfg.get('hf_parsing_map', {})
             hf_loading_vars = icl_cfg.get('hf_loading_vars', {})
 
-            early_stopping_criteria = icl_cfg.get('early_stopping_criteria',
-                                                  None)
+            early_stopping_criteria = icl_cfg.get(
+                'early_stopping_criteria',
+                None,
+            )
             if isinstance(early_stopping_criteria, ListConfig):
                 early_stopping_criteria = om.to_container(
-                    early_stopping_criteria)
+                    early_stopping_criteria,
+                )
             assert early_stopping_criteria is None or isinstance(
-                early_stopping_criteria, list)
+                early_stopping_criteria,
+                list,
+            )
             dataloaders = get_icl_task_dataloader(
                 icl_cfg.icl_task_type,
                 icl_cfg.dataset_uri,
                 tokenizer,
                 batch_size=icl_cfg.batch_size,
                 max_seq_len=icl_cfg.max_seq_len,
                 pad_tok_id=pad_tok_id,
@@ -571,30 +610,38 @@
                 fewshot_random_seed=icl_cfg.fewshot_random_seed,
                 pass_at_k=icl_cfg.pass_at_k,
                 generations_per_sample=icl_cfg.generations_per_sample,
                 has_categories=icl_cfg.get('has_categories', False),
                 cot_delimiter=icl_cfg.get('cot_delimiter', ''),
                 generation_kwargs=icl_cfg.get('generation_kwargs', {}),
                 early_stopping_criteria=early_stopping_criteria,
-                do_normalization=icl_cfg.get('do_normalization', True))
+                do_normalization=icl_cfg.get('do_normalization', True),
+            )
             if hasattr(
-                    icl_cfg,
-                    'has_categories') and icl_cfg.has_categories and isinstance(
-                        dataloaders, dict):
+                icl_cfg,
+                'has_categories',
+            ) and icl_cfg.has_categories and isinstance(dataloaders, dict):
                 for category in dataloaders.keys():
                     logger_keys.extend([
                         f'metrics/{label}/{category}/{m}' for m in metric_names
                     ])
                     evaluators.append(
-                        Evaluator(label=f'{label}/{category}',
-                                  dataloader=dataloaders[category],
-                                  metric_names=metric_names),)
+                        Evaluator(
+                            label=f'{label}/{category}',
+                            dataloader=dataloaders[category],
+                            metric_names=metric_names,
+                        ),
+                    )
             else:
-                logger_keys.extend(
-                    [f'metrics/{label}/{m}' for m in metric_names])
+                logger_keys.extend([
+                    f'metrics/{label}/{m}' for m in metric_names
+                ])
                 evaluators.append(
-                    Evaluator(label=label,
-                              dataloader=dataloaders,
-                              metric_names=metric_names,
-                              subset_num_batches=icl_subset_num_batches))
+                    Evaluator(
+                        label=label,
+                        dataloader=dataloaders,
+                        metric_names=metric_names,
+                        subset_num_batches=icl_subset_num_batches,
+                    ),
+                )
 
     return evaluators, logger_keys
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/checkpoint_conversion_helpers.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/checkpoint_conversion_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 import os
 import random
 import string
 from pathlib import Path
 from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np
-import sentencepiece as spm
-from transformers import (AutoTokenizer, PreTrainedTokenizer,
-                          PreTrainedTokenizerFast)
+from transformers import (
+    AutoTokenizer,
+    PreTrainedTokenizer,
+    PreTrainedTokenizerFast,
+)
 
 log = logging.getLogger(__name__)
 
 __all__ = [
     'get_hf_tokenizer_from_composer_state_dict',
     'load_tokenizer',
     'convert_and_save_ft_weights',
@@ -44,30 +46,33 @@
 def get_hf_tokenizer_from_composer_state_dict(
     state_dict: Dict[str, Any],
     trust_remote_code: bool,
     tokenizer_save_dir: Optional[str] = None,
 ) -> Optional[PreTrainedTokenizer]:
     if 'state' not in state_dict:
         raise RuntimeError(
-            'Unexpected composer state dictionary. Did you pass in a full composer checkpoint?'
+            'Unexpected composer state dictionary. Did you pass in a full composer checkpoint?',
         )
     if 'integrations' not in state_dict[
-            'state'] or 'huggingface' not in state_dict['state']['integrations']:
+        'state'] or 'huggingface' not in state_dict['state']['integrations']:
         raise RuntimeError(
-            'Did not find HuggingFace related state (e.g., tokenizer) in the provided composer checkpoint!'
+            'Did not find HuggingFace related state (e.g., tokenizer) in the provided composer checkpoint!',
         )
     hf_tokenizer_state = state_dict['state']['integrations']['huggingface'][
         'tokenizer']
     hf_tokenizer = None
     if hf_tokenizer_state != {}:
         if tokenizer_save_dir is None:
             unique_suffix = ''.join(
-                random.choices(string.ascii_letters + string.digits, k=6))
+                random.choices(string.ascii_letters + string.digits, k=6),
+            )
             tokenizer_save_dir = os.path.join(
-                os.getcwd(), f'tokenizer-save-dir-{unique_suffix}')
+                os.getcwd(),
+                f'tokenizer-save-dir-{unique_suffix}',
+            )
         os.makedirs(tokenizer_save_dir, exist_ok=True)
 
         for filename, saved_content in hf_tokenizer_state.items():
             # For backwards compatibility, check if the filename already has the file extension
             if filename.endswith(saved_content['file_extension']):
                 tokenizer_file_name = filename
             else:
@@ -84,70 +89,90 @@
                     for line in saved_content['content']:
                         _tmp_file.write(line)
                         _tmp_file.write('\n')
             elif saved_content['file_extension'] == '.py':
                 with open(tokenizer_file_path, 'w') as _tmp_file:
                     _tmp_file.write(saved_content['content'])
             elif saved_content['file_extension'] == '.model':
+                try:
+                    import sentencepiece as spm
+                except ImportError as e:
+                    raise ImportError(
+                        'Your tokenizer uses `sentencepiece`. Please install `sentencepiece` to load it.',
+                    ) from e
+
                 s = spm.SentencePieceProcessor()
                 s.load_from_serialized_proto(saved_content['content'])
                 with open(tokenizer_file_path, 'wb') as _tmp_file:
                     _tmp_file.write(s.serialized_model_proto())
 
-        hf_tokenizer = load_tokenizer(tokenizer_save_dir,
-                                      trust_remote_code=trust_remote_code)
+        hf_tokenizer = load_tokenizer(
+            tokenizer_save_dir,
+            trust_remote_code=trust_remote_code,
+        )
 
         # remove 'name_or_path'
         hf_tokenizer.name_or_path = ''
         hf_tokenizer.init_kwargs['name_or_path'] = ''
 
     return hf_tokenizer
 
 
 def load_tokenizer(
-    tokenizer_save_dir: str, trust_remote_code: bool
+    tokenizer_save_dir: str,
+    trust_remote_code: bool,
 ) -> Union[PreTrainedTokenizer, PreTrainedTokenizerFast]:
     try:
         return AutoTokenizer.from_pretrained(
-            tokenizer_save_dir, trust_remote_code=trust_remote_code)
+            tokenizer_save_dir,
+            trust_remote_code=trust_remote_code,
+        )
     except ValueError as e:
         raise ValueError(
             f'Got error while loading tokenizer with trust_remote_code={trust_remote_code}: {e}. '
             +
             'If accessing a tokenizer defined outside of the transformers module,'
-            + ' please use --trust_remote_code.')
+            + ' please use --trust_remote_code.',
+        )
 
 
-def _write_zero_bias(weight_name: str, weight_file_path: str,
-                     bias_shape: Union[Tuple[int, ...],
-                                       int], np_data_type: np.dtype) -> None:
+def _write_zero_bias(
+    weight_name: str,
+    weight_file_path: str,
+    bias_shape: Union[Tuple[int, ...], int],
+    np_data_type: np.dtype,
+) -> None:
     """Write zeros for bias when converting MPT to FasterTransformer weights.
 
     MPT model might not have bias while FT expects bias.
 
     Args:
         weight_name (str): Name of the weight tensor.
         weight_file_path (str): Output path for storing the weight (NOT zero bias).
         bias_shape (Union[Tuple[int, ...], int]): Shape of the bias array.
         np_data_type (np.dtype): The data type for bias.
     """
     if 'weight' not in weight_file_path:
         raise RuntimeError(
-            f'Cannot write zero bias for {weight_name}. Input is not a weight tensor'
+            f'Cannot write zero bias for {weight_name}. Input is not a weight tensor',
         )
     log.debug(f'zero bias for weight: {weight_name}')
     bias_file_path = weight_file_path.replace('.weight', '.bias')
     bias = np.zeros(bias_shape, dtype=np_data_type)
     bias.tofile(bias_file_path)
 
 
-def _convert_weight_to_ft_each(save_dir: str, infer_gpu_num: int,
-                               tensor_name: str, config: Dict[str, Any],
-                               data: np.ndarray,
-                               np_weight_data_type: np.dtype) -> None:
+def _convert_weight_to_ft_each(
+    save_dir: str,
+    infer_gpu_num: int,
+    tensor_name: str,
+    config: Dict[str, Any],
+    data: np.ndarray,
+    np_weight_data_type: np.dtype,
+) -> None:
     """Convert each MPT weight to a FasterTransformer compatible format.
 
     Args:
         save_dir (str): Path of the directory to save the weight in FT format. The directory must already exist.
         infer_gpu_num (int): The number of gpus you are planning to use for inference.
         tensor_name (str): Name of the weight tensor. Used in naming the output file.
         config (Dict[str, Any]): Configuration for the model. This is used in getting model specific parameters.
@@ -160,117 +185,142 @@
         tensor_name.find('attention.dense.bias') != -1 or tensor_name.find('post_attention_layernorm.weight') != -1 or \
         tensor_name.find('post_attention_layernorm.bias') != -1 or tensor_name.find('mlp.dense_4h_to_h.bias') != -1 or \
         tensor_name.find('final_layernorm.weight') != -1 or tensor_name.find('final_layernorm.bias') != -1:
 
         save_path = os.path.join(save_dir, f'model.{tensor_name}.bin')
         data.tofile(save_path)
         if 'weight' in tensor_name and config['no_bias']:
-            _write_zero_bias(tensor_name, save_path, data.shape[-1],
-                             np_weight_data_type
-                            )  # pyright: ignore [reportGeneralTypeIssues]
+            _write_zero_bias(
+                tensor_name,
+                save_path,
+                data.shape[-1],
+                np_weight_data_type,
+            )  # pyright: ignore [reportGeneralTypeIssues]
 
     elif tensor_name.find('attention.dense.weight') != -1:
         assert data.shape == (
             config['d_model'],
-            config['d_model']), f'unexpected dim for {tensor_name}'
+            config['d_model'],
+        ), f'unexpected dim for {tensor_name}'
         # nn.Linear weights are transposed
         data = data.T
         split_vals = np.split(data, infer_gpu_num, axis=0)
         for j in range(infer_gpu_num):
             save_path = os.path.join(save_dir, f'model.{tensor_name}.{j}.bin')
             split_vals[j].tofile(save_path)
         if config['no_bias']:
-            fake_weight_path = os.path.join(save_dir,
-                                            f'model.{tensor_name}.bin')
-            _write_zero_bias(tensor_name, fake_weight_path, data.shape[-1],
-                             np_weight_data_type
-                            )  # pyright: ignore [reportGeneralTypeIssues]
+            fake_weight_path = os.path.join(
+                save_dir,
+                f'model.{tensor_name}.bin',
+            )
+            _write_zero_bias(
+                tensor_name,
+                fake_weight_path,
+                data.shape[-1],
+                np_weight_data_type,
+            )  # pyright: ignore [reportGeneralTypeIssues]
 
     elif tensor_name.find('mlp.dense_4h_to_h.weight') != -1:
         assert data.shape == (
-            config['d_model'], config['expansion_ratio'] *
-            config['d_model']), f'unexpected dim for {tensor_name}'
+            config['d_model'],
+            config['expansion_ratio'] * config['d_model'],
+        ), f'unexpected dim for {tensor_name}'
         # nn.Linear weights are transposed
         data = data.T
         split_vals = np.split(data, infer_gpu_num, axis=0)
         for j in range(infer_gpu_num):
             save_path = os.path.join(save_dir, f'model.{tensor_name}.{j}.bin')
             split_vals[j].tofile(save_path)
         if config['no_bias']:
-            fake_weight_path = os.path.join(save_dir,
-                                            f'model.{tensor_name}.bin')
-            _write_zero_bias(tensor_name, fake_weight_path, data.shape[-1],
-                             np_weight_data_type
-                            )  # pyright: ignore [reportGeneralTypeIssues]
+            fake_weight_path = os.path.join(
+                save_dir,
+                f'model.{tensor_name}.bin',
+            )
+            _write_zero_bias(
+                tensor_name,
+                fake_weight_path,
+                data.shape[-1],
+                np_weight_data_type,
+            )  # pyright: ignore [reportGeneralTypeIssues]
 
     elif tensor_name.find('mlp.dense_h_to_4h.weight') != -1:
         assert data.shape == (
             config['expansion_ratio'] * config['d_model'],
-            config['d_model']), f'unexpected dim for {tensor_name}'
+            config['d_model'],
+        ), f'unexpected dim for {tensor_name}'
         # nn.Linear weights are transposed
         data = data.T
 
         split_vals = np.split(data, infer_gpu_num, axis=-1)
         for j in range(infer_gpu_num):
             save_path = os.path.join(save_dir, f'model.{tensor_name}.{j}.bin')
             split_vals[j].tofile(save_path)
             if config['no_bias']:
-                _write_zero_bias(tensor_name, save_path,
-                                 split_vals[j].shape[-1], np_weight_data_type
-                                )  # pyright: ignore [reportGeneralTypeIssues]
+                _write_zero_bias(
+                    tensor_name,
+                    save_path,
+                    split_vals[j].shape[-1],
+                    np_weight_data_type,
+                )  # pyright: ignore [reportGeneralTypeIssues]
 
     elif tensor_name.find('mlp.dense_h_to_4h.bias') != -1:
         assert data.shape == (
-            config['expansion_ratio'] *
-            config['d_model'],), f'unexpected dim for {tensor_name}'
+            config['expansion_ratio'] * config['d_model'],
+        ), f'unexpected dim for {tensor_name}'
         split_vals = np.split(data, infer_gpu_num, axis=-1)
         for j in range(infer_gpu_num):
             save_path = os.path.join(save_dir + f'model.{tensor_name}.{j}.bin')
             split_vals[j].tofile(save_path)
 
     elif tensor_name.find('attention.query_key_value.bias') != -1:
         assert data.shape == (
-            3 * config['d_model'],), f'unexpected dim for {tensor_name}'
+            3 * config['d_model'],
+        ), f'unexpected dim for {tensor_name}'
 
         data = data.reshape(3, config['d_model'])
 
         split_vals = np.split(data, infer_gpu_num, axis=-1)
 
         for j in range(infer_gpu_num):
             save_path = os.path.join(save_dir, f'model.{tensor_name}.{j}.bin')
             split_vals[j].tofile(save_path)
 
     elif tensor_name.find('attention.query_key_value.weight') != -1:
         assert data.shape == (
             3 * config['d_model'],
-            config['d_model']), f'unexpected dim for {tensor_name}'
+            config['d_model'],
+        ), f'unexpected dim for {tensor_name}'
         # nn.Linear weights are transposed
         data = data.T
 
         data = data.reshape(config['d_model'], 3, config['d_model'])
         split_vals = np.split(data, infer_gpu_num, axis=-1)
 
         for j in range(infer_gpu_num):
             save_path = os.path.join(save_dir, f'model.{tensor_name}.{j}.bin')
             split_vals[j].tofile(save_path)
             if config['no_bias']:
-                _write_zero_bias(tensor_name, save_path,
-                                 (3, split_vals[j].shape[-1]),
-                                 np_weight_data_type
-                                )  # pyright: ignore [reportGeneralTypeIssues]
+                _write_zero_bias(
+                    tensor_name,
+                    save_path,
+                    (3, split_vals[j].shape[-1]),
+                    np_weight_data_type,
+                )  # pyright: ignore [reportGeneralTypeIssues]
 
     else:
         raise RuntimeError(f'Tensor with name {tensor_name} is not handled')
 
 
-def convert_and_save_ft_weights(named_params: dict,
-                                config: dict,
-                                infer_gpu_num: int = 1,
-                                weight_data_type: str = 'fp32',
-                                save_dir: str = '') -> None:
+def convert_and_save_ft_weights(
+    named_params: dict,
+    config: dict,
+    infer_gpu_num: int = 1,
+    weight_data_type: str = 'fp32',
+    save_dir: str = '',
+) -> None:
     """Convert a Composer MPT checkpoint to a FasterTransformer format.
 
     Args:
         named_params (Dict[str, Parameter]): A dictionary containing the Composer MPT model's parameter names and data.
         config (Dict[str, Any]): Configuration for the model. This is used in getting model specific parameters.
         infer_gpu_num (int): The number of gpus you are planning to use for inference.
         weight_data_type (str): The dtype of the converted FasterTransformer model.
@@ -301,48 +351,56 @@
         data = param.detach().cpu().numpy().astype(np_weight_data_type)
         if name.find('weight') == -1 and name.find('bias') == -1:
             log.debug(f'found a parameter name that is not handled: {name}')
             continue
         if name == 'transformer.wpe.weight':
             assert data.shape == (
                 config['max_seq_len'],
-                config['d_model']), f'unexpected dim for {name}'
+                config['d_model'],
+            ), f'unexpected dim for {name}'
             data.tofile(os.path.join(save_dir, 'model.wpe.bin'))
         elif name == 'transformer.wte.weight':
             assert data.shape == (
                 config['vocab_size'],
-                config['d_model']), f'unexpected dim for {name}'
+                config['d_model'],
+            ), f'unexpected dim for {name}'
             data.tofile(os.path.join(save_dir, 'model.wte.bin'))
         elif name == 'transformer.norm_f.bias':
             assert data.shape == (
-                config['d_model'],), f'unexpected dim for {name}'
-            data.tofile(os.path.join(save_dir,
-                                     'model.final_layernorm.bias.bin'))
+                config['d_model'],
+            ), f'unexpected dim for {name}'
+            data.tofile(
+                os.path.join(save_dir, 'model.final_layernorm.bias.bin'),
+            )
         elif name == 'transformer.norm_f.weight':
             assert data.shape == (
-                config['d_model'],), f'unexpected dim for {name}'
-            save_path = os.path.join(save_dir,
-                                     'model.final_layernorm.weight.bin')
+                config['d_model'],
+            ), f'unexpected dim for {name}'
+            save_path = os.path.join(
+                save_dir,
+                'model.final_layernorm.weight.bin',
+            )
             data.tofile(save_path)
             if config['no_bias']:
                 _write_zero_bias(
                     name,
                     save_path,
                     data.shape[-1],
-                    np_weight_data_type  # pyright: ignore [reportGeneralTypeIssues]
+                    np_weight_data_type,  # pyright: ignore [reportGeneralTypeIssues]
                 )
         elif name == 'transformer.lm_head.weight':
             data.tofile(os.path.join(save_dir, 'model.lm_head.weight.bin'))
         else:
             for mpt_pattern, ft_pattern in param_remapping.items():
                 if name.find(mpt_pattern) != -1:
-                    new_name = name.replace('transformer.blocks.',
-                                            'layers.').replace(
-                                                mpt_pattern, ft_pattern)
+                    new_name = name.replace(
+                        'transformer.blocks.',
+                        'layers.',
+                    ).replace(mpt_pattern, ft_pattern)
                     _convert_weight_to_ft_each(
                         save_dir,
                         infer_gpu_num,
                         new_name,
                         config,
                         data,
-                        np_weight_data_type  # pyright: ignore [reportGeneralTypeIssues]
+                        np_weight_data_type,  # pyright: ignore [reportGeneralTypeIssues]
                     )
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/data_prep_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/data_prep_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 from glob import glob
 from typing import List, Optional
 
 from composer.utils import ObjectStore
 
 __all__ = [
-    'with_id',
     'merge_shard_groups',
     'DownloadingIterable',
 ]
 
 
 def with_id(basename: str, shard_id: int) -> str:
     """Get a new basename with the given shard_id.
@@ -90,29 +89,33 @@
         """Iterable that downloads files from an object store before yielding.
 
         If object_store is None, input_folder_prefix is treated as a local path.
 
         Args:
             object_names (List[str]): Names of objects to download
             output_folder (str): Local folder to write downloaded files to
-            object_store (Optiona[ObjectStore]): Object store to download from
+            object_store (Optional[ObjectStore]): Object store to download from
         """
         self.object_names = object_names
         self.object_store = object_store
         self.output_folder = output_folder
 
     def __iter__(self):
         for object_name in self.object_names:
             # Default output_filename, used for local paths.
             output_filename = object_name
 
             # Download objects if remote path.
             if self.object_store is not None:
-                output_filename = os.path.join(self.output_folder,
-                                               object_name.strip('/'))
-                self.object_store.download_object(object_name=object_name,
-                                                  filename=output_filename,
-                                                  overwrite=True)
+                output_filename = os.path.join(
+                    self.output_folder,
+                    object_name.strip('/'),
+                )
+                self.object_store.download_object(
+                    object_name=object_name,
+                    filename=output_filename,
+                    overwrite=True,
+                )
 
             with open(output_filename) as _txt_file:
                 txt = _txt_file.read()
             yield {'text': txt}
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/exceptions.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,95 @@
 # Copyright 2024 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Custom exceptions for the LLMFoundry."""
 from collections.abc import Mapping
 from typing import Any, Dict, List
 
+__all__ = [
+    'ALLOWED_RESPONSE_KEYS',
+    'ALLOWED_PROMPT_KEYS',
+    'ALLOWED_MESSAGES_KEYS',
+    'MissingHuggingFaceURLSplitError',
+    'NotEnoughDatasetSamplesError',
+    'UnknownExampleTypeError',
+    'NotEnoughChatDataError',
+    'ConsecutiveRepeatedChatRolesError',
+    'InvalidLastChatMessageRoleError',
+    'IncorrectMessageKeyQuantityError',
+    'InvalidRoleError',
+    'InvalidContentTypeError',
+    'InvalidPromptTypeError',
+    'InvalidResponseTypeError',
+    'InvalidPromptResponseKeysError',
+    'InvalidFileExtensionError',
+    'UnableToProcessPromptResponseError',
+    'ClusterDoesNotExistError',
+    'FailedToCreateSQLConnectionError',
+    'FailedToConnectToDatabricksError',
+    'InputFolderMissingDataError',
+    'OutputFolderNotEmptyError',
+    'MisconfiguredHfDatasetError',
+]
+
+ALLOWED_RESPONSE_KEYS = {'response', 'completion'}
+ALLOWED_PROMPT_KEYS = {'prompt'}
+ALLOWED_MESSAGES_KEYS = {'messages'}
+
 
 # Finetuning dataloader exceptions
 class MissingHuggingFaceURLSplitError(ValueError):
     """Error thrown when there's no split used in HF dataset config."""
 
     def __init__(self) -> None:
         message = 'When using a HuggingFace dataset from a URL, you must set the ' + \
                     '`split` key in the dataset config.'
         super().__init__(message)
 
 
 class NotEnoughDatasetSamplesError(ValueError):
     """Error thrown when there is not enough data to train a model."""
 
-    def __init__(self, dataset_name: str, split: str,
-                 dataloader_batch_size: int, world_size: int,
-                 full_dataset_size: int, minimum_dataset_size: int) -> None:
+    def __init__(
+        self,
+        dataset_name: str,
+        split: str,
+        dataloader_batch_size: int,
+        world_size: int,
+        full_dataset_size: int,
+        minimum_dataset_size: int,
+    ) -> None:
         self.dataset_name = dataset_name
         self.split = split
         self.dataloader_batch_size = dataloader_batch_size
         self.world_size = world_size
         self.full_dataset_size = full_dataset_size
         self.minimum_dataset_size = minimum_dataset_size
         message = (
             f'Your dataset (name={dataset_name}, split={split}) ' +
             f'has {full_dataset_size} samples, but your minimum batch size ' +
             f'is {minimum_dataset_size} because you are running on {world_size} gpus and '
             +
             f'your per device batch size is {dataloader_batch_size}. Please increase the number '
-            + f'of samples in your dataset to at least {minimum_dataset_size}.')
+            + f'of samples in your dataset to at least {minimum_dataset_size}.'
+        )
         super().__init__(message)
 
 
 ## Tasks exceptions
 class UnknownExampleTypeError(KeyError):
     """Error thrown when an unknown example type is used in a task."""
 
     def __init__(self, example: Mapping) -> None:
-        message = f'Unknown example type {example=}'
-        super().__init__(message)
-
-
-class TooManyKeysInExampleError(ValueError):
-    """Error thrown when a data sample has too many keys."""
-
-    def __init__(self, desired_keys: set[str], keys: set[str]) -> None:
-        message = f'Data sample has {len(keys)} keys in `allowed_keys`: {desired_keys} Please specify exactly one. Provided keys: {keys}'
+        self.example = example
+        message = (
+            f'Found keys {example.keys()} in dataset. Unknown example type. For prompt and response '
+            f'finetuning, the valid prompt keys are {ALLOWED_PROMPT_KEYS} and the valid response keys are '
+            f'{ALLOWED_RESPONSE_KEYS}. For chat finetuning, the allowed keys are {ALLOWED_MESSAGES_KEYS}'
+        )
         super().__init__(message)
 
 
 class NotEnoughChatDataError(ValueError):
     """Error thrown when there is not enough chat data to train a model."""
 
     def __init__(self) -> None:
@@ -72,14 +106,16 @@
         super().__init__(message)
 
 
 class InvalidLastChatMessageRoleError(ValueError):
     """Error thrown when the last message role in a chat example is invalid."""
 
     def __init__(self, last_role: str, expected_roles: set[str]) -> None:
+        self.last_role = last_role
+        self.expected_roles = expected_roles
         message = f'Invalid last message role: {last_role}. Expected one of: {expected_roles}'
         super().__init__(message)
 
 
 class IncorrectMessageKeyQuantityError(ValueError):
     """Error thrown when a message has an incorrect number of keys."""
 
@@ -139,22 +175,24 @@
     """Error thrown when a file extension is not a safe extension."""
 
     def __init__(self, dataset_name: str, valid_extensions: List[str]) -> None:
         self.dataset_name = dataset_name
         self.valid_extensions = valid_extensions
         message = (
             f'safe_load is set to True. No data files with safe extensions {valid_extensions} '
-            + f'found for dataset at local path {dataset_name}.')
+            + f'found for dataset at local path {dataset_name}.'
+        )
         super().__init__(message)
 
 
 class UnableToProcessPromptResponseError(ValueError):
     """Error thrown when a prompt and response cannot be processed."""
 
     def __init__(self, input: Dict) -> None:
+        self.input = input
         message = f'Unable to extract prompt/response from {input}'
         super().__init__(message)
 
 
 ## Convert Delta to JSON exceptions
 class ClusterDoesNotExistError(ValueError):
     """Error thrown when the cluster does not exist."""
@@ -194,7 +232,17 @@
 class OutputFolderNotEmptyError(FileExistsError):
     """Error thrown when the output folder is not empty."""
 
     def __init__(self, output_folder: str) -> None:
         self.output_folder = output_folder
         message = f'{output_folder} is not empty. Please remove or empty it and retry.'
         super().__init__(message)
+
+
+class MisconfiguredHfDatasetError(ValueError):
+    """Error thrown when a HuggingFace dataset is misconfigured."""
+
+    def __init__(self, dataset_name: str, split: str) -> None:
+        self.dataset_name = dataset_name
+        self.split = split
+        message = f'Your dataset (name={dataset_name}, split={split}) is misconfigured. Please check your dataset format and make sure you can load your dataset locally.'
+        super().__init__(message)
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/huggingface_hub_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/huggingface_hub_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,17 @@
         if node in self.nodes_to_remove:
             return None
 
         return super().visit(node)
 
 
 def convert_to_relative_import(
-        module_name: str, original_parent_module_name: Optional[str]) -> str:
+    module_name: str,
+    original_parent_module_name: Optional[str],
+) -> str:
     parts = module_name.split('.')
     if parts[-1] == original_parent_module_name:
         return '.'
     return '.' + parts[-1]
 
 
 def find_module_file(module_name: str) -> str:
@@ -84,36 +86,46 @@
 
     tree = ast.parse(source)
     new_files_to_process = []
     nodes_to_remove = []
     for node in ast.walk(tree):
         # Remove any imports matching the remove_imports_prefix
         if isinstance(
-                node,
-                ast.ImportFrom) and node.module is not None and _remove_import(
-                    node, remove_imports_prefix):
+            node,
+            ast.ImportFrom,
+        ) and node.module is not None and _remove_import(
+            node,
+            remove_imports_prefix,
+        ):
             nodes_to_remove.append(node)
         # Convert any (remaining) imports matching the flatten_imports_prefix
         # to relative imports
-        elif (isinstance(node, ast.ImportFrom) and node.module is not None and
-              _flatten_import(node, flatten_imports_prefix)):
+        elif (
+            isinstance(node, ast.ImportFrom) and node.module is not None and
+            _flatten_import(node, flatten_imports_prefix)
+        ):
             module_path = find_module_file(node.module)
-            node.module = convert_to_relative_import(node.module,
-                                                     parent_module_name)
+            node.module = convert_to_relative_import(
+                node.module,
+                parent_module_name,
+            )
             # Recursively process any llmfoundry files
             new_files_to_process.append(module_path)
         # Remove the Composer* class
-        elif (isinstance(node, ast.ClassDef) and
-              node.name.startswith('Composer')):
+        elif (
+            isinstance(node, ast.ClassDef) and node.name.startswith('Composer')
+        ):
             nodes_to_remove.append(node)
         # Remove the __all__ declaration in any __init__.py files, whose
         # enclosing module will be converted to a single file of the same name
-        elif (isinstance(node, ast.Assign) and len(node.targets) == 1 and
-              isinstance(node.targets[0], ast.Name) and
-              node.targets[0].id == '__all__'):
+        elif (
+            isinstance(node, ast.Assign) and len(node.targets) == 1 and
+            isinstance(node.targets[0], ast.Name) and
+            node.targets[0].id == '__all__'
+        ):
             nodes_to_remove.append(node)
 
     transformer = DeleteSpecificNodes(nodes_to_remove)
     new_tree = transformer.visit(tree)
 
     new_filename = os.path.basename(file_path)
     # Special case for __init__.py to mimic the original submodule
@@ -126,17 +138,21 @@
 
     return new_files_to_process
 
 
 def edit_files_for_hf_compatibility(
     folder: str,
     flatten_imports_prefix: Sequence[str] = ('llmfoundry',),
-    remove_imports_prefix: Sequence[str] = ('composer', 'omegaconf',
-                                            'llmfoundry.metrics',
-                                            'llmfoundry.utils.builders'),
+    remove_imports_prefix: Sequence[str] = (
+        'composer',
+        'omegaconf',
+        'llmfoundry.metrics',
+        'llmfoundry.eval',
+        'llmfoundry.utils.builders',
+    ),
 ) -> None:
     """Edit files to be compatible with Hugging Face Hub.
 
     Args:
         folder (str): The folder to process.
         flatten_imports_prefix (Sequence[str], optional): Sequence of prefixes to flatten. Defaults to ('llmfoundry',).
         remove_imports_prefix (Sequence[str], optional): Sequence of prefixes to remove. Takes precedence over flattening.
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/logging_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/logging_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Copyright 2022 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 import logging
 import os
 
 from composer.loggers import MosaicMLLogger
-from composer.loggers.mosaicml_logger import (MOSAICML_ACCESS_TOKEN_ENV_VAR,
-                                              MOSAICML_PLATFORM_ENV_VAR)
+from composer.loggers.mosaicml_logger import (
+    MOSAICML_ACCESS_TOKEN_ENV_VAR,
+    MOSAICML_PLATFORM_ENV_VAR,
+)
 
 __all__ = [
     'SpecificWarningFilter',
 ]
 
 
 class SpecificWarningFilter(logging.Filter):
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/model_download_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/model_download_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,18 +45,21 @@
 __all__ = [
     'download_from_hf_hub',
     'download_from_http_fileserver',
     'download_from_oras',
 ]
 
 
-@tenacity.retry(retry=tenacity.retry_if_not_exception_type(
-    (ValueError, hf_hub.utils.RepositoryNotFoundError)),
-                stop=tenacity.stop_after_attempt(3),
-                wait=tenacity.wait_exponential(min=1, max=10))
+@tenacity.retry(
+    retry=tenacity.retry_if_not_exception_type(
+        (ValueError, hf_hub.utils.RepositoryNotFoundError),
+    ),
+    stop=tenacity.stop_after_attempt(3),
+    wait=tenacity.wait_exponential(min=1, max=10),
+)
 def download_from_hf_hub(
     model: str,
     save_dir: str,
     prefer_safetensors: bool = True,
     tokenizer_only: bool = False,
     token: Optional[str] = None,
 ):
@@ -79,52 +82,57 @@
         ValueError: If the model repo doesn't contain any supported model weights.
     """
     repo_files = set(hf_hub.list_repo_files(model))
 
     # Ignore TensorFlow, TensorFlow 2, and Flax weights as they are not supported by Composer.
     ignore_patterns = copy.deepcopy(DEFAULT_IGNORE_PATTERNS)
 
-    safetensors_available = (SAFE_WEIGHTS_NAME in repo_files or
-                             SAFE_WEIGHTS_INDEX_NAME in repo_files)
-    pytorch_available = (PYTORCH_WEIGHTS_NAME in repo_files or
-                         PYTORCH_WEIGHTS_INDEX_NAME in repo_files)
+    safetensors_available = (
+        SAFE_WEIGHTS_NAME in repo_files or SAFE_WEIGHTS_INDEX_NAME in repo_files
+    )
+    pytorch_available = (
+        PYTORCH_WEIGHTS_NAME in repo_files or
+        PYTORCH_WEIGHTS_INDEX_NAME in repo_files
+    )
 
     if safetensors_available and pytorch_available:
         if prefer_safetensors:
             log.info(
-                'Safetensors available and preferred. Excluding pytorch weights.'
+                'Safetensors available and preferred. Excluding pytorch weights.',
             )
             ignore_patterns.append(PYTORCH_WEIGHTS_PATTERN)
         else:
             log.info(
-                'Pytorch available and preferred. Excluding safetensors weights.'
+                'Pytorch available and preferred. Excluding safetensors weights.',
             )
             ignore_patterns.append(SAFE_WEIGHTS_PATTERN)
     elif safetensors_available:
         log.info('Only safetensors available. Ignoring weights preference.')
     elif pytorch_available:
         log.info('Only pytorch available. Ignoring weights preference.')
     else:
         raise ValueError(
             f'No supported model weights found in repo {model}.' +
-            ' Please make sure the repo contains either safetensors or pytorch weights.'
+            ' Please make sure the repo contains either safetensors or pytorch weights.',
         )
 
     allow_patterns = TOKENIZER_FILES if tokenizer_only else None
 
     download_start = time.time()
-    hf_hub.snapshot_download(model,
-                             local_dir=save_dir,
-                             local_dir_use_symlinks=False,
-                             ignore_patterns=ignore_patterns,
-                             allow_patterns=allow_patterns,
-                             token=token)
+    hf_hub.snapshot_download(
+        model,
+        local_dir=save_dir,
+        local_dir_use_symlinks=False,
+        ignore_patterns=ignore_patterns,
+        allow_patterns=allow_patterns,
+        token=token,
+    )
     download_duration = time.time() - download_start
     log.info(
-        f'Downloaded model {model} from Hugging Face Hub in {download_duration} seconds'
+        f'Downloaded model {model} from Hugging Face Hub in {download_duration} seconds',
     )
 
 
 def _extract_links_from_html(html: str):
     """Extracts links from HTML content.
 
     Args:
@@ -164,23 +172,23 @@
     """
     url = urljoin(base_url, path)
     print(url)
     response = session.get(url, verify=(not ignore_cert))
 
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         raise PermissionError(
-            f'Not authorized to download file from {url}. Received status code {response.status_code}. '
+            f'Not authorized to download file from {url}. Received status code {response.status_code}. ',
         )
     elif response.status_code == HTTPStatus.NOT_FOUND:
         raise ValueError(
-            f'Could not find file at {url}. Received status code {response.status_code}'
+            f'Could not find file at {url}. Received status code {response.status_code}',
         )
     elif response.status_code != HTTPStatus.OK:
         raise RuntimeError(
-            f'Could not download file from {url}. Received unexpected status code {response.status_code}'
+            f'Could not download file from {url}. Received unexpected status code {response.status_code}',
         )
 
     # Assume that the URL points to a file if it does not end with a slash.
     if not url.endswith('/'):
         save_path = os.path.join(save_dir, path)
         parent_dir = os.path.dirname(save_path)
         if not os.path.exists(parent_dir):
@@ -193,25 +201,28 @@
             return
 
     # If the URL is a directory, the response should be an HTML directory listing that we can parse for additional links
     # to download.
     child_links = _extract_links_from_html(response.content.decode())
     print(child_links)
     for child_link in child_links:
-        _recursive_download(session,
-                            base_url,
-                            urljoin(path, child_link),
-                            save_dir,
-                            ignore_cert=ignore_cert)
+        _recursive_download(
+            session,
+            base_url,
+            urljoin(path, child_link),
+            save_dir,
+            ignore_cert=ignore_cert,
+        )
 
 
-@tenacity.retry(retry=tenacity.retry_if_not_exception_type(
-    (PermissionError, ValueError)),
-                stop=tenacity.stop_after_attempt(3),
-                wait=tenacity.wait_exponential(min=1, max=10))
+@tenacity.retry(
+    retry=tenacity.retry_if_not_exception_type((PermissionError, ValueError)),
+    stop=tenacity.stop_after_attempt(3),
+    wait=tenacity.wait_exponential(min=1, max=10),
+)
 def download_from_http_fileserver(
     url: str,
     save_dir: str,
     ignore_cert: bool = False,
 ):
     """Downloads files from a remote HTTP file server.
 
@@ -224,65 +235,73 @@
     """
     with requests.Session() as session:
         # Temporarily suppress noisy SSL certificate verification warnings if ignore_cert is set to True
         with warnings.catch_warnings():
             if ignore_cert:
                 warnings.simplefilter('ignore', category=InsecureRequestWarning)
 
-            _recursive_download(session,
-                                url,
-                                '',
-                                save_dir,
-                                ignore_cert=ignore_cert)
+            _recursive_download(
+                session,
+                url,
+                '',
+                save_dir,
+                ignore_cert=ignore_cert,
+            )
 
 
-def download_from_oras(model: str,
-                       config_file: str,
-                       credentials_dir: str,
-                       save_dir: str,
-                       tokenizer_only: bool = False,
-                       concurrency: int = 10):
+def download_from_oras(
+    model: str,
+    config_file: str,
+    credentials_dir: str,
+    save_dir: str,
+    tokenizer_only: bool = False,
+    concurrency: int = 10,
+):
     """Download from an OCI-compliant registry using oras.
 
     Args:
         model (str): The name of the model to download.
         config_file (str): Path to a YAML config file that maps model and tokenizer names to registry paths.
         credentials_dir (str): Path to a directory containing credentials for the registry. It is expected to contain three
             files: `username`, `password`, and `registry`, each of which contains the corresponding credential.
         save_dir (str): Path to the directory where files will be downloaded.
-        tokenizer_only (bool): If true, only download the tokenzier files.
+        tokenizer_only (bool): If true, only download the tokenizer files.
         concurrency (int): The number of concurrent downloads to run.
     """
     if shutil.which(ORAS_CLI) is None:
         raise Exception(
-            f'oras cli command `{ORAS_CLI}` is not found. Please install oras: https://oras.land/docs/installation '
+            f'oras cli command `{ORAS_CLI}` is not found. Please install oras: https://oras.land/docs/installation ',
         )
 
     def _read_secrets_file(secret_file_path: str,):
         try:
             with open(secret_file_path, encoding='utf-8') as f:
                 return f.read().strip()
         except Exception as error:
             raise ValueError(
-                f'secrets file {secret_file_path} failed to be read') from error
+                f'secrets file {secret_file_path} failed to be read',
+            ) from error
 
     secrets = {}
     for secret in ['username', 'password', 'registry']:
         secrets[secret] = _read_secrets_file(
-            os.path.join(credentials_dir, secret))
+            os.path.join(credentials_dir, secret),
+        )
 
     with open(config_file, 'r', encoding='utf-8') as f:
         configs = yaml.safe_load(f.read())
 
     config_type = 'tokenizers' if tokenizer_only else 'models'
     path = configs[config_type][model]
     registry = secrets['registry']
 
-    def get_oras_cmd(username: Optional[str] = None,
-                     password: Optional[str] = None):
+    def get_oras_cmd(
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+    ):
         cmd = [
             ORAS_CLI,
             'pull',
             f'{registry}/{path}',
             '-o',
             save_dir,
             '--verbose',
@@ -294,15 +313,21 @@
         if password is not None:
             cmd.extend(['--password', password])
 
         return cmd
 
     cmd_without_creds = get_oras_cmd()
     log.info(f'CMD for oras cli to run: {" ".join(cmd_without_creds)}')
-    cmd_to_run = get_oras_cmd(username=secrets['username'],
-                              password=secrets['password'])
+    cmd_to_run = get_oras_cmd(
+        username=secrets['username'],
+        password=secrets['password'],
+    )
     try:
         subprocess.run(cmd_to_run, check=True)
     except subprocess.CalledProcessError as e:
         # Intercept the error and replace the cmd, which may have sensitive info.
-        raise subprocess.CalledProcessError(e.returncode, cmd_without_creds,
-                                            e.output, e.stderr)
+        raise subprocess.CalledProcessError(
+            e.returncode,
+            cmd_without_creds,
+            e.output,
+            e.stderr,
+        )
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/mosaicml_logger_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/mosaicml_logger_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 # SPDX-License-Identifier: Apache-2.0
 import json
 import os
 from typing import Any, Dict, List, Optional, Union
 
 from composer.loggers import MosaicMLLogger
 from composer.loggers.logger_destination import LoggerDestination
-from composer.loggers.mosaicml_logger import (MOSAICML_ACCESS_TOKEN_ENV_VAR,
-                                              MOSAICML_PLATFORM_ENV_VAR)
+from composer.loggers.mosaicml_logger import (
+    MOSAICML_ACCESS_TOKEN_ENV_VAR,
+    MOSAICML_PLATFORM_ENV_VAR,
+)
 from omegaconf import DictConfig, ListConfig
 
+__all__ = [
+    'maybe_create_mosaicml_logger',
+    'find_mosaicml_logger',
+    'log_eval_analytics',
+    'log_train_analytics',
+]
+
 _MODEL_KEYS_TO_LOG = [
     'pretrained_model_name_or_path',
     'pretrained',
     'vocab_size',
     'd_model',
     'n_heads',
     'n_layers',
@@ -26,79 +35,92 @@
     """Creates a MosaicMLLogger if the run was sent from the Mosaic platform."""
     if os.environ.get(MOSAICML_PLATFORM_ENV_VAR, 'false').lower(
     ) == 'true' and os.environ.get(MOSAICML_ACCESS_TOKEN_ENV_VAR):
         return MosaicMLLogger()
 
 
 def find_mosaicml_logger(
-        loggers: List[LoggerDestination]) -> Optional[MosaicMLLogger]:
+    loggers: List[LoggerDestination],
+) -> Optional[MosaicMLLogger]:
     """Returns the first MosaicMLLogger from a list, and None otherwise."""
     return next(
         (logger for logger in loggers if isinstance(logger, MosaicMLLogger)),
-        None)
+        None,
+    )
 
 
-def log_eval_analytics(mosaicml_logger: MosaicMLLogger,
-                       model_configs: ListConfig, icl_tasks: Union[str,
-                                                                   ListConfig],
-                       eval_gauntlet_config: Optional[Union[str, DictConfig]]):
+def log_eval_analytics(
+    mosaicml_logger: MosaicMLLogger,
+    model_configs: ListConfig,
+    icl_tasks: Union[str, ListConfig],
+    eval_gauntlet_config: Optional[Union[str, DictConfig]],
+):
     """Logs analytics for runs using the `eval.py` script."""
     metrics: Dict[str, Any] = {
         'llmfoundry/script': 'eval',
     }
 
     metrics['llmfoundry/gauntlet_configured'] = eval_gauntlet_config is not None
-    metrics['llmfoundry/icl_configured'] = isinstance(icl_tasks,
-                                                      str) or len(icl_tasks) > 0
+    metrics['llmfoundry/icl_configured'] = isinstance(
+        icl_tasks,
+        str,
+    ) or len(icl_tasks) > 0
 
     metrics['llmfoundry/model_configs'] = []
     for model_config in model_configs:
         nested_model_config = model_config.get('model', {})
         model_config_data = {}
         for key in _MODEL_KEYS_TO_LOG:
             if nested_model_config.get(key, None) is not None:
                 model_config_data[key] = nested_model_config.get(key)
 
         if len(model_config_data) > 0:
             metrics['llmfoundry/model_configs'].append(
-                json.dumps(model_config_data, sort_keys=True))
+                json.dumps(model_config_data, sort_keys=True),
+            )
 
     mosaicml_logger.log_metrics(metrics)
     mosaicml_logger._flush_metadata(force_flush=True)
 
 
-def log_train_analytics(mosaicml_logger: MosaicMLLogger,
-                        model_config: DictConfig,
-                        train_loader_config: DictConfig,
-                        eval_loader_config: Optional[Union[DictConfig,
-                                                           ListConfig]],
-                        callback_configs: Optional[DictConfig],
-                        tokenizer_name: str, load_path: Optional[str],
-                        icl_tasks_config: Optional[Union[ListConfig, str]],
-                        eval_gauntlet: Optional[Union[DictConfig, str]]):
+def log_train_analytics(
+    mosaicml_logger: MosaicMLLogger,
+    model_config: DictConfig,
+    train_loader_config: DictConfig,
+    eval_loader_config: Optional[Union[DictConfig, ListConfig]],
+    callback_configs: Optional[DictConfig],
+    tokenizer_name: str,
+    load_path: Optional[str],
+    icl_tasks_config: Optional[Union[ListConfig, str]],
+    eval_gauntlet: Optional[Union[DictConfig, str]],
+):
     """Logs analytics for runs using the `train.py` script."""
     train_loader_dataset = train_loader_config.get('dataset', {})
     metrics: Dict[str, Any] = {
         'llmfoundry/tokenizer_name': tokenizer_name,
         'llmfoundry/script': 'train',
         'llmfoundry/train_loader_name': train_loader_config.get('name'),
     }
 
     if callback_configs is not None:
         metrics['llmfoundry/callbacks'] = [
             name for name, _ in callback_configs.items()
         ]
 
     metrics['llmfoundry/gauntlet_configured'] = eval_gauntlet is not None
-    metrics['llmfoundry/icl_configured'] = (icl_tasks_config is not None and (
-        (isinstance(icl_tasks_config, str) or len(icl_tasks_config) > 0)))
+    metrics['llmfoundry/icl_configured'] = (
+        icl_tasks_config is not None and
+        ((isinstance(icl_tasks_config, str) or len(icl_tasks_config) > 0))
+    )
 
     if train_loader_dataset.get('hf_name', None) is not None:
         metrics['llmfoundry/train_dataset_hf_name'] = train_loader_dataset.get(
-            'hf_name', None)
+            'hf_name',
+            None,
+        )
     if train_loader_config.get('name') == 'finetuning':
         metrics['llmfoundry/train_task_type'] = 'INSTRUCTION_FINETUNE'
     elif train_loader_config.get('name') == 'text':
         if load_path is not None or model_config.get('pretrained') == True:
             metrics['llmfoundry/train_task_type'] = 'CONTINUED_PRETRAIN'
         else:
             metrics['llmfoundry/train_task_type'] = 'PRETRAIN'
@@ -113,19 +135,21 @@
 
         for loader_config in eval_loader_configs:
             eval_loader_info = {}
             eval_loader_dataset = loader_config.get('dataset', {})
             eval_loader_info['name'] = loader_config.get('name')
             if eval_loader_dataset.get('hf_name', None) is not None:
                 eval_loader_info['dataset_hf_name'] = eval_loader_dataset.get(
-                    'hf_name')
+                    'hf_name',
+                )
 
             # Log as a key-sorted JSON string, so that we can easily parse it in Spark / SQL
             metrics['llmfoundry/eval_loaders'].append(
-                json.dumps(eval_loader_info, sort_keys=True))
+                json.dumps(eval_loader_info, sort_keys=True),
+            )
 
     model_config_data = {}
     for key in _MODEL_KEYS_TO_LOG:
         if model_config.get(key, None) is not None:
             model_config_data[f'llmfoundry/{key}'] = model_config.get(key)
 
     if len(model_config_data) > 0:
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/prompt_files.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/prompt_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,18 @@
             prompts = load_prompts_from_file(prompt, prompt_delimiter)
             prompt_strings.extend(prompts)
         else:
             prompt_strings.append(prompt)
     return prompt_strings
 
 
-def load_prompts_from_file(prompt_path: str,
-                           prompt_delimiter: Optional[str] = None) -> List[str]:
+def load_prompts_from_file(
+    prompt_path: str,
+    prompt_delimiter: Optional[str] = None,
+) -> List[str]:
     """Load a set of prompts from a text fie.
 
     Args:
         prompt_path (str): Path for text file
         prompt_delimiter (Optional str): Delimiter for text file
             If not provided, assumes the prompt file is a single prompt (non-delimited)
 
@@ -49,15 +51,16 @@
     if not prompt_path.startswith(PROMPTFILE_PREFIX):
         raise ValueError(f'prompt_path_str must start with {PROMPTFILE_PREFIX}')
 
     _, prompt_file_path = prompt_path.split(PROMPTFILE_PREFIX, maxsplit=1)
     prompt_file_path = os.path.expanduser(prompt_file_path)
     if not os.path.isfile(prompt_file_path):
         raise FileNotFoundError(
-            f'{prompt_file_path=} does not match any existing files.')
+            f'{prompt_file_path=} does not match any existing files.',
+        )
 
     with open(prompt_file_path, 'r') as f:
         prompt_string = f.read()
 
     if prompt_delimiter is None:
         return [prompt_string]
     return [i for i in prompt_string.split(prompt_delimiter) if i]
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/registry_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/registry_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,74 @@
 # Copyright 2024 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
+import copy
 import functools
 import importlib.util
 import os
+from contextlib import contextmanager
 from pathlib import Path
 from types import ModuleType
-from typing import (Any, Callable, Dict, Generic, Optional, Sequence, Type,
-                    TypeVar, Union)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Optional,
+    Sequence,
+    Type,
+    TypeVar,
+    Union,
+)
 
 import catalogue
 
-__all__ = ['TypedRegistry', 'create_registry', 'construct_from_registry']
+__all__ = [
+    'TypedRegistry',
+    'create_registry',
+    'construct_from_registry',
+    'import_file',
+    'save_registry',
+]
 
 T = TypeVar('T')
+TypeBoundT = TypeVar('TypeBoundT', bound=Type)
+CallableBoundT = TypeVar('CallableBoundT', bound=Callable[..., Any])
 
 
 class TypedRegistry(catalogue.Registry, Generic[T]):
     """A thin wrapper around catalogue.Registry to add static typing and.
 
     descriptions.
     """
 
-    def __init__(self,
-                 namespace: Sequence[str],
-                 entry_points: bool = False,
-                 description: str = '') -> None:
+    def __init__(
+        self,
+        namespace: Sequence[str],
+        entry_points: bool = False,
+        description: str = '',
+    ) -> None:
         super().__init__(namespace, entry_points=entry_points)
 
         self.description = description
 
     def __call__(self, name: str, func: Optional[T] = None) -> Callable[[T], T]:
         return super().__call__(name, func)
 
     def register(self, name: str, *, func: Optional[T] = None) -> T:
         return super().register(name, func=func)
 
+    def register_class(
+        self,
+        name: str,
+        *,
+        func: Optional[TypeBoundT] = None,
+    ) -> TypeBoundT:
+        return super().register(name, func=func)
+
     def get(self, name: str) -> T:
         return super().get(name)
 
     def get_all(self) -> Dict[str, T]:
         return super().get_all()
 
     def get_entry_point(self, name: str, default: Optional[T] = None) -> T:
@@ -68,17 +97,19 @@
 
     Returns:
         The TypedRegistry object.
     """
     if catalogue.check_exists(*namespace):
         raise catalogue.RegistryError(f'Namespace already exists: {namespace}')
 
-    return TypedRegistry[generic_type](namespace,
-                                       entry_points=entry_points,
-                                       description=description)
+    return TypedRegistry[generic_type](
+        namespace,
+        entry_points=entry_points,
+        description=description,
+    )
 
 
 def construct_from_registry(
     name: str,
     registry: TypedRegistry,
     partial_function: bool = True,
     pre_validation_function: Optional[Union[Callable[[Any], None],
@@ -108,38 +139,39 @@
 
     registered_constructor = registry.get(name)
 
     if pre_validation_function is not None:
         if isinstance(pre_validation_function, type):
             if not issubclass(registered_constructor, pre_validation_function):
                 raise ValueError(
-                    f'Expected {name} to be of type {pre_validation_function}, but got {type(registered_constructor)}'
+                    f'Expected {name} to be of type {pre_validation_function}, but got {type(registered_constructor)}',
                 )
         elif isinstance(pre_validation_function, Callable):
             pre_validation_function(registered_constructor)
         else:
             raise ValueError(
-                f'Expected pre_validation_function to be a callable or a type, but got {type(pre_validation_function)}'
+                f'Expected pre_validation_function to be a callable or a type, but got {type(pre_validation_function)}',
             )
 
     # If it is a class, or a builder function, construct the class with kwargs
     # If it is a function, create a partial with kwargs
     if isinstance(
-            registered_constructor,
-            type) or callable(registered_constructor) and not partial_function:
+        registered_constructor,
+        type,
+    ) or callable(registered_constructor) and not partial_function:
         constructed_item = registered_constructor(**kwargs)
     elif callable(registered_constructor):
         constructed_item = functools.partial(registered_constructor, **kwargs)
     else:
         raise ValueError(
-            f'Expected {name} to be a class or function, but got {type(registered_constructor)}'
+            f'Expected {name} to be a class or function, but got {type(registered_constructor)}',
         )
 
     if post_validation_function is not None:
-        post_validation_function(registered_constructor)
+        post_validation_function(constructed_item)
 
     return constructed_item
 
 
 def import_file(loc: Union[str, Path]) -> ModuleType:
     """Import module from a file.
 
@@ -162,7 +194,17 @@
     module = importlib.util.module_from_spec(spec)
 
     try:
         spec.loader.exec_module(module)
     except Exception as e:
         raise RuntimeError(f'Error executing {loc}') from e
     return module
+
+
+@contextmanager
+def save_registry():
+    """Save the registry state and restore after the context manager exits."""
+    saved_registry_state = copy.deepcopy(catalogue.REGISTRY)
+
+    yield
+
+    catalogue.REGISTRY = saved_registry_state
```

### Comparing `llm-foundry-0.7.0/llmfoundry/utils/warnings.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/warnings.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 # SPDX-License-Identifier: Apache-2.0
 import functools
 import warnings
 from typing import Any, Callable, Type, TypeVar, cast
 
 __all__ = [
     'VersionedDeprecationWarning',
+    'ExperimentalWarning',
+    'experimental_function',
+    'experimental_class',
 ]
 
 
 class VersionedDeprecationWarning(UserWarning):
     """A custom deprecation warning class that includes version information.
 
     Attributes:
@@ -26,28 +29,29 @@
         ...     )
         ...
         >>> deprecated_function()
         DeprecationWarning: Function XYZ is deprecated. It will be removed in version 2.0.0.
     """
 
     def __init__(self, message: str, remove_version: str) -> None:
-        super().__init__(message +
-                         f' It will be removed in version {remove_version}.')
+        super().__init__(
+            message + f' It will be removed in version {remove_version}.',
+        )
 
 
 class ExperimentalWarning(Warning):
     """A warning for experimental features.
 
     Attributes:
         feature_name (str): The name of the experimental feature.
     """
 
     def __init__(self, feature_name: str) -> None:
         super().__init__(
-            f'{feature_name} is experimental and may change with future versions.'
+            f'{feature_name} is experimental and may change with future versions.',
         )
 
 
 F = TypeVar('F', bound=Callable[..., Any])
 
 
 # Decorator version of experimental warning
```

### Comparing `llm-foundry-0.7.0/pyproject.toml` & `llm-foundry-0.9.0.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,33 @@
 build-backend = "setuptools.build_meta"
 
 # iSort
 [tool.isort]
 multi_line_output = 0
 line_length = 80
 skip = [ "env", "wandb", "runs", "build", "node_modules" ]
+include_trailing_comma = true
+split_on_trailing_comma = true
+
+[tool.ruff.lint]
+select = [
+    "C4",
+    # TODO port pydocstyle
+    # "D", # pydocstyle
+    "LOG",
+    "PERF",
+    "PLE",
+    "COM812",
+]
+[tool.ruff]
+exclude = [
+    "build/**",
+    "docs/**",
+    "node_modules/**",
+]
 
 # Coverage
 [tool.coverage.run]
 parallel = true
 branch = true
 relative_files = true
 concurrency = ["thread"]
@@ -159,15 +178,15 @@
 #
 # would reformat to:
 #
 #    call_func_that_takes_a_dict({
 #        'key1': 'value1',
 #        'key2': 'value2',
 #    })
-coalesce_brackets = false
+coalesce_brackets = true
 
 # The column limit.
 column_limit = 80
 
 # The style for continuation alignment. Possible values are:
 #
 # - SPACE: Use spaces for continuation alignment. This is default behavior.
@@ -194,15 +213,15 @@
 #   time_series = self.remote_client.query_entity_counters(
 #       entity='dev3246.region1',
 #       key='dns.query_latency_tcp',
 #       transform=Transformation.AVERAGE(window=timedelta(seconds=60)),
 #       start_ts=now()-timedelta(days=3),
 #       end_ts=now(),
 #   )        # <--- this bracket is dedented and on a separate line
-dedent_closing_brackets = false
+dedent_closing_brackets = true
 
 # Disable the heuristic which places each list element on a separate line
 # if the list is comma-terminated.
 disable_ending_comma_heuristic = false
 
 # Place each dictionary entry onto its own line.
 each_dict_entry_on_separate_line = true
@@ -365,15 +384,15 @@
 
 # Split before arguments, but do not split all subexpressions recursively
 # (unless needed).
 split_all_top_level_comma_separated_values = false
 
 # Split before arguments if the argument list is terminated by a
 # comma.
-split_arguments_when_comma_terminated = false
+split_arguments_when_comma_terminated = true
 
 # Set to True to prefer splitting before '+', '-', '*', '/', '//', or '@'
 # rather than after.
 split_before_arithmetic_operator = false
 
 # Set to True to prefer splitting before '&', '|' or '^' rather than
 # after.
```

### Comparing `llm-foundry-0.7.0/setup.py` & `llm-foundry-0.9.0.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 
 # Read the repo version
 # We can't use `.__version__` from the library since it's not installed yet
 with open(os.path.join(_PACKAGE_REAL_PATH, '__init__.py')) as f:
     content = f.read()
 # regex: '__version__', whitespace?, '=', whitespace, quote, version, quote
 # we put parens around the version so that it becomes elem 1 of the match
-expr = re.compile(r"""^__version__\W+=\W+['"]([0-9\.]*)['"]""", re.MULTILINE)
+expr = re.compile(
+    r"""^__version__\s*=\s*['"]([0-9]+\.[0-9]+\.[0-9]+(?:\.\w+)?)['"]""",
+    re.MULTILINE,
+)
 repo_version = expr.findall(content)[0]
 
 # Use repo README for PyPi description
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # Hide the content between <!-- SETUPTOOLS_LONG_DESCRIPTION_HIDE_BEGIN --> and
@@ -47,102 +50,111 @@
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
 ]
 
 install_requires = [
-    'mosaicml[libcloud,wandb,oci,gcs]>=0.21.1,<0.22',
-    'mlflow>=2.10,<3',
+    'mosaicml[libcloud,wandb,oci,gcs]>=0.22.0,<0.23',
+    'mlflow>=2.12.1,<2.13',
     'accelerate>=0.25,<0.26',  # for HF inference `device_map`
-    'transformers>=4.38.2,<4.39',
-    'mosaicml-streaming>=0.7.4,<0.8',
-    'torch>=2.2.1,<2.3',
-    'datasets>=2.16,<2.17',
+    'transformers>=4.40,<4.41',
+    'mosaicml-streaming>=0.7.5,<0.8',
+    'torch>=2.3.0,<2.4',
+    'datasets>=2.19,<2.20',
     'fsspec==2023.6.0',  # newer version results in a bug in datasets that duplicates data
     'sentencepiece==0.1.97',
     'einops==0.7.0',
     'omegaconf>=2.2.3,<3',
     'slack-sdk<4',
     'mosaicml-cli>=0.6.10,<1',
     'onnx==1.14.0',
     'onnxruntime==1.15.1',
     'boto3>=1.21.45,<2',
-    'huggingface-hub>=0.17.0,<1.0',
+    'huggingface-hub>=0.19.0,<0.23',
     'beautifulsoup4>=4.12.2,<5',  # required for model download utils
     'tenacity>=8.2.3,<9',
     'catalogue>=2,<3',
     'typer[all]<1',
 ]
 
 extra_deps = {}
 
 extra_deps['dev'] = [
+    'coverage[toml]==7.4.4',
     'pre-commit>=3.4.0,<4',
     'pytest>=7.2.1,<8',
     'pytest_codeblocks>=0.16.1,<0.17',
     'pytest-cov>=4,<5',
     'pyright==1.1.256',
     'toml>=0.10.2,<0.11',
     'packaging>=21,<23',
     'hf_transfer==0.1.3',
 ]
 
 extra_deps['databricks'] = [
-    'mosaicml[databricks]>=0.21.1,<0.22',
+    'mosaicml[databricks]>=0.22.0,<0.23',
     'databricks-sql-connector>=3,<4',
     'databricks-connect==14.1.0',
     'lz4>=4,<5',
 ]
 
 extra_deps['tensorboard'] = [
-    'mosaicml[tensorboard]>=0.21.1,<0.22',
+    'mosaicml[tensorboard]>=0.22.0,<0.23',
 ]
 
 # Flash 2 group kept for backwards compatibility
 extra_deps['gpu-flash2'] = [
-    'flash-attn==2.5.0',
+    'flash-attn==2.5.8',
 ]
 
 extra_deps['gpu'] = copy.deepcopy(extra_deps['gpu-flash2'])
 
 extra_deps['peft'] = [
-    'mosaicml[peft]>=0.21.1,<0.22',
-]
-
-extra_deps['olmo'] = [
-    'ai2-olmo>0.2.4',
+    'mosaicml[peft]>=0.22.0,<0.23',
 ]
 
 extra_deps['openai'] = [
     'openai==1.3.8',
     'tiktoken==0.4.0',
 ]
-extra_deps['all-cpu'] = set(
-    dep for key, deps in extra_deps.items() for dep in deps if 'gpu' not in key)
-extra_deps['all'] = set(dep for key, deps in extra_deps.items() for dep in deps
-                        if key not in {'gpu-flash2', 'all-cpu'})
-extra_deps['all-flash2'] = set(dep for key, deps in extra_deps.items()
-                               for dep in deps
-                               if key not in {'gpu', 'all', 'all-cpu'})
+
+extra_deps['megablocks'] = [
+    'megablocks==0.5.1',
+    'grouped-gemm==0.1.4',
+]
+
+extra_deps['all-cpu'] = {
+    dep for key, deps in extra_deps.items() for dep in deps
+    if 'gpu' not in key and 'megablocks' not in key
+}
+extra_deps['all'] = {
+    dep for key, deps in extra_deps.items() for dep in deps
+    if key not in {'gpu-flash2', 'all-cpu'}
+}
+extra_deps['all-flash2'] = {
+    dep for key, deps in extra_deps.items() for dep in deps
+    if key not in {'gpu', 'all', 'all-cpu'}
+}
 
 setup(
     name=_PACKAGE_NAME,
     version=repo_version,
     author='MosaicML',
     author_email='team@mosaicml.com',
     description='LLM Foundry',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mosaicml/llm-foundry/',
     package_data={
         'llmfoundry': ['py.typed'],
     },
     packages=setuptools.find_packages(
-        exclude=['.github*', 'mcli*', 'scripts*', 'tests*']),
+        exclude=['.github*', 'mcli*', 'scripts*', 'tests*'],
+    ),
     classifiers=classifiers,
     install_requires=install_requires,
     extras_require=extra_deps,
     python_requires='>=3.9',
     entry_points={
         'console_scripts': ['llmfoundry = llmfoundry.cli.cli:app'],
     },
```

### Comparing `llm-foundry-0.7.0/tests/test_registry.py` & `llm-foundry-0.9.0.dev0/tests/test_registry.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,64 +24,84 @@
         'loggers',
         'optimizers',
         'schedulers',
         'callbacks',
         'algorithms',
         'callbacks_with_config',
         'dataloaders',
+        'dataset_replication_validators',
+        'collators',
+        'data_specs',
         'metrics',
         'models',
+        'norms',
+        'param_init_fns',
+        'module_init_fns',
+        'ffns',
+        'ffns_with_norm',
+        'ffns_with_megablocks',
+        'attention_classes',
+        'attention_implementations',
+        'fcs',
     }
 
     assert existing_registries == expected_registry_names
 
 
 def test_registry_create(monkeypatch: pytest.MonkeyPatch):
     monkeypatch.setattr(catalogue, 'Registry', {})
 
-    new_registry = registry_utils.create_registry('llmfoundry',
-                                                  'test_registry',
-                                                  generic_type=str,
-                                                  entry_points=False)
+    new_registry = registry_utils.create_registry(
+        'llmfoundry',
+        'test_registry',
+        generic_type=str,
+        entry_points=False,
+    )
 
     assert new_registry.namespace == ('llmfoundry', 'test_registry')
     assert isinstance(new_registry, registry_utils.TypedRegistry)
 
 
 def test_registry_typing(monkeypatch: pytest.MonkeyPatch):
     monkeypatch.setattr(catalogue, 'Registry', {})
-    new_registry = registry_utils.create_registry('llmfoundry',
-                                                  'test_registry',
-                                                  generic_type=str,
-                                                  entry_points=False)
+    new_registry = registry_utils.create_registry(
+        'llmfoundry',
+        'test_registry',
+        generic_type=str,
+        entry_points=False,
+    )
     new_registry.register('test_name', func='test')
 
     # This would fail type checking without the type ignore
     # It is here to show that the TypedRegistry is working (gives a type error without the ignore),
     # although this would not catch a regression in this regard
     new_registry.register('test_name', func=1)  # type: ignore
 
 
 def test_registry_add(monkeypatch: pytest.MonkeyPatch):
     monkeypatch.setattr(catalogue, 'Registry', {})
-    new_registry = registry_utils.create_registry('llmfoundry',
-                                                  'test_registry',
-                                                  generic_type=str,
-                                                  entry_points=False)
+    new_registry = registry_utils.create_registry(
+        'llmfoundry',
+        'test_registry',
+        generic_type=str,
+        entry_points=False,
+    )
     new_registry.register('test_name', func='test')
 
     assert new_registry.get('test_name') == 'test'
 
 
 def test_registry_overwrite(monkeypatch: pytest.MonkeyPatch):
     monkeypatch.setattr(catalogue, 'Registry', {})
-    new_registry = registry_utils.create_registry('llmfoundry',
-                                                  'test_registry',
-                                                  generic_type=str,
-                                                  entry_points=False)
+    new_registry = registry_utils.create_registry(
+        'llmfoundry',
+        'test_registry',
+        generic_type=str,
+        entry_points=False,
+    )
     new_registry.register('test_name', func='test')
     new_registry.register('test_name', func='test2')
 
     assert new_registry.get('test_name') == 'test2'
 
 
 def test_registry_init_code(tmp_path: pathlib.Path):
@@ -108,102 +128,129 @@
     assert 'test_logger' not in registry.loggers
 
 
 def test_registry_entrypoint(monkeypatch: pytest.MonkeyPatch):
     monkeypatch.setattr(catalogue, 'Registry', {})
 
     monkeypatch.setattr(
-        importlib.metadata, 'entry_points', lambda: {
+        importlib.metadata,
+        'entry_points',
+        lambda: {
             'llmfoundry_test_registry': [
-                EntryPoint(name='test_entry',
-                           value='composer.loggers:InMemoryLogger',
-                           group='llmfoundry_test_registry')
-            ]
-        })
-
-    monkeypatch.setattr(catalogue, 'AVAILABLE_ENTRY_POINTS',
-                        importlib.metadata.entry_points())
-    new_registry = registry_utils.create_registry('llmfoundry',
-                                                  'test_registry',
-                                                  generic_type=str,
-                                                  entry_points=True)
+                EntryPoint(
+                    name='test_entry',
+                    value='composer.loggers:InMemoryLogger',
+                    group='llmfoundry_test_registry',
+                ),
+            ],
+        },
+    )
+
+    monkeypatch.setattr(
+        catalogue,
+        'AVAILABLE_ENTRY_POINTS',
+        importlib.metadata.entry_points(),
+    )
+    new_registry = registry_utils.create_registry(
+        'llmfoundry',
+        'test_registry',
+        generic_type=str,
+        entry_points=True,
+    )
     assert new_registry.get('test_entry') == InMemoryLogger
 
 
 def test_registry_builder(monkeypatch: pytest.MonkeyPatch):
     monkeypatch.setattr(catalogue, 'Registry', {})
 
     new_registry = registry_utils.create_registry(
         'llmfoundry',
         'test_registry',
         entry_points=False,
         generic_type=Union[Type[LoggerDestination],
-                           Callable[..., LoggerDestination]])
+                           Callable[..., LoggerDestination]],
+    )
 
     class TestLoggerDestination(LoggerDestination):
         pass
 
     new_registry.register('test_destination', func=TestLoggerDestination)
 
     # Valid, no validation
     valid_class = registry_utils.construct_from_registry(
         'test_destination',
         new_registry,
-        pre_validation_function=TestLoggerDestination)
+        pre_validation_function=TestLoggerDestination,
+    )
     assert isinstance(valid_class, TestLoggerDestination)
 
     # Invalid, class validation
-    with pytest.raises(ValueError,
-                       match='Expected test_destination to be of type'):
+    with pytest.raises(
+        ValueError,
+        match='Expected test_destination to be of type',
+    ):
         registry_utils.construct_from_registry(
             'test_destination',
             new_registry,
-            pre_validation_function=InMemoryLogger)
+            pre_validation_function=InMemoryLogger,
+        )
 
     # Invalid, function pre-validation
     with pytest.raises(ValueError, match='Invalid'):
 
         def pre_validation_function(x: Any):
             raise ValueError('Invalid')
 
         registry_utils.construct_from_registry(
             'test_destination',
             new_registry,
-            pre_validation_function=pre_validation_function)
+            pre_validation_function=pre_validation_function,
+        )
 
     # Invalid, function post-validation
     with pytest.raises(ValueError, match='Invalid'):
 
         def post_validation_function(x: Any):
             raise ValueError('Invalid')
 
         registry_utils.construct_from_registry(
             'test_destination',
             new_registry,
-            post_validation_function=post_validation_function)
+            post_validation_function=post_validation_function,
+        )
 
     # Invalid, not a class or function
     new_registry.register('non_callable', func=1)  # type: ignore
-    with pytest.raises(ValueError,
-                       match='Expected non_callable to be a class or function'):
+    with pytest.raises(
+        ValueError,
+        match='Expected non_callable to be a class or function',
+    ):
         registry_utils.construct_from_registry('non_callable', new_registry)
 
     # Valid, partial function
-    new_registry.register('partial_func',
-                          func=lambda x, y: x * y)  # type: ignore
-    partial_func = registry_utils.construct_from_registry('partial_func',
-                                                          new_registry,
-                                                          partial_function=True,
-                                                          kwargs={'x': 2})
+    new_registry.register(
+        'partial_func',
+        func=lambda x,
+        y: x * y,
+    )  # type: ignore
+    partial_func = registry_utils.construct_from_registry(
+        'partial_func',
+        new_registry,
+        partial_function=True,
+        kwargs={'x': 2},
+    )
     assert partial_func(y=3) == 6
 
     # Valid, builder function
     new_registry.register('builder_func', func=lambda: TestLoggerDestination())
     valid_built_class = registry_utils.construct_from_registry(
-        'builder_func', new_registry, partial_function=False)
+        'builder_func',
+        new_registry,
+        partial_function=False,
+    )
     assert isinstance(valid_built_class, TestLoggerDestination)
     assert os.environ['TEST_ENVIRON_REGISTRY_KEY'] == 'test'
 
     del os.environ['TEST_ENVIRON_REGISTRY_KEY']
 
 
 def test_registry_init_code_fails(tmp_path: pathlib.Path):
```

### Comparing `llm-foundry-0.7.0/tests/test_smoketest.py` & `llm-foundry-0.9.0.dev0/tests/test_smoketest.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.7.0/tests/test_utils.py` & `llm-foundry-0.9.0.dev0/tests/test_utils.py`

 * *Files identical despite different names*

