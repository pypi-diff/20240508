# Comparing `tmp/llm-foundry-0.8.0.tar.gz` & `tmp/llm-foundry-0.9.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-foundry-0.8.0.tar", last modified: Wed May  8 02:22:29 2024, max compression
+gzip compressed data, was "llm-foundry-0.9.0.dev0.tar", last modified: Wed May  8 01:43:25 2024, max compression
```

## Comparing `llm-foundry-0.8.0.tar` & `llm-foundry-0.9.0.dev0.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.761501 llm-foundry-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19628 2024-05-08 02:22:29.761501 llm-foundry-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19181 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.745501 llm-foundry-0.8.0/llm_foundry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19628 2024-05-08 02:22:29.000000 llm-foundry-0.8.0/llm_foundry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-08 02:22:29.000000 llm-foundry-0.8.0/llm_foundry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:22:29.000000 llm-foundry-0.8.0/llm_foundry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 02:22:29.000000 llm-foundry-0.8.0/llm_foundry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 02:22:29.000000 llm-foundry-0.8.0/llm_foundry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 02:22:29.000000 llm-foundry-0.8.0/llm_foundry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.749501 llm-foundry-0.8.0/llmfoundry/
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.749501 llm-foundry-0.8.0/llmfoundry/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.749501 llm-foundry-0.8.0/llmfoundry/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22934 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/callbacks/async_eval_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/callbacks/curriculum_learning_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/callbacks/eval_gauntlet_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/callbacks/eval_output_logging_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/callbacks/fdiff_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    25723 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/callbacks/hf_checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/callbacks/log_mbmoe_tok_per_expert_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/callbacks/monolithic_ckpt_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/callbacks/resumption_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/callbacks/scheduled_gc_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.749501 llm-foundry-0.8.0/llmfoundry/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/cli/registry_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.749501 llm-foundry-0.8.0/llmfoundry/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/data/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/data/dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.753501 llm-foundry-0.8.0/llmfoundry/data/finetuning/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/data/finetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19557 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/data/finetuning/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)    30847 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/data/finetuning/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    40793 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/data/finetuning/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/data/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17293 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/data/text_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.753501 llm-foundry-0.8.0/llmfoundry/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/eval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.753501 llm-foundry-0.8.0/llmfoundry/eval/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/eval/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    81670 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/eval/datasets/in_context_learning_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/eval/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.753501 llm-foundry-0.8.0/llmfoundry/eval/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/eval/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31388 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/eval/metrics/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.753501 llm-foundry-0.8.0/llmfoundry/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/interfaces/callback_with_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/layers_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.753501 llm-foundry-0.8.0/llmfoundry/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/loggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.753501 llm-foundry-0.8.0/llmfoundry/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/metrics/token_acc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.753501 llm-foundry-0.8.0/llmfoundry/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.753501 llm-foundry-0.8.0/llmfoundry/models/hf/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/hf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15971 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/hf/hf_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/hf/hf_fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/hf/hf_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/hf/model_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.753501 llm-foundry-0.8.0/llmfoundry/models/inference_api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/inference_api_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/inference_api_wrapper/fmapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/inference_api_wrapper/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/inference_api_wrapper/openai_causal_lm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.757501 llm-foundry-0.8.0/llmfoundry/models/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27930 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/layers/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/layers/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/layers/custom_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/layers/dmoe.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/layers/fc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/layers/ffn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/layers/layer_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/layers/norm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.757501 llm-foundry-0.8.0/llmfoundry/models/mpt/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/mpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17835 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/mpt/configuration_mpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    47730 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/mpt/modeling_mpt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.757501 llm-foundry-0.8.0/llmfoundry/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/utils/act_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/utils/config_moe_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/utils/meta_init_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/utils/mpt_param_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    31016 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/models/utils/param_init_fns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.757501 llm-foundry-0.8.0/llmfoundry/optim/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18558 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/optim/adaptive_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/optim/outlier_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/optim/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.761501 llm-foundry-0.8.0/llmfoundry/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/tokenizers/tiktoken.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.761501 llm-foundry-0.8.0/llmfoundry/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23395 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    16245 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/checkpoint_conversion_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13944 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/data_prep_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/huggingface_hub_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/model_download_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/mosaicml_logger_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/prompt_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/llmfoundry/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15403 2024-05-08 02:22:19.000000 llm-foundry-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 02:22:29.761501 llm-foundry-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-08 02:22:20.000000 llm-foundry-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:22:29.761501 llm-foundry-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-05-08 02:22:20.000000 llm-foundry-0.8.0/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-08 02:22:20.000000 llm-foundry-0.8.0/tests/test_smoketest.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 02:22:20.000000 llm-foundry-0.8.0/tests/test_utils.py
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

### Comparing `llm-foundry-0.8.0/LICENSE` & `llm-foundry-0.9.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/PKG-INFO` & `llm-foundry-0.9.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-foundry
-Version: 0.8.0
+Version: 0.9.0.dev0
 Summary: LLM Foundry
 Home-page: https://github.com/mosaicml/llm-foundry/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: llm-foundry Version: 0.8.0 Summary: LLM Foundry
-Home-page: https://github.com/mosaicml/llm-foundry/ Author: MosaicML Author-
-email: team@mosaicml.com Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1 Name: llm-foundry Version: 0.9.0.dev0 Summary: LLM
+Foundry Home-page: https://github.com/mosaicml/llm-foundry/ Author: MosaicML
+Author-email: team@mosaicml.com Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
 dev Provides-Extra: databricks Provides-Extra: tensorboard Provides-Extra: gpu-
 flash2 Provides-Extra: gpu Provides-Extra: peft Provides-Extra: openai
 Provides-Extra: megablocks Provides-Extra: all-cpu Provides-Extra: all
 Provides-Extra: all-flash2 License-File: LICENSE
```

### Comparing `llm-foundry-0.8.0/README.md` & `llm-foundry-0.9.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llm_foundry.egg-info/PKG-INFO` & `llm-foundry-0.9.0.dev0/llm_foundry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-foundry
-Version: 0.8.0
+Version: 0.9.0.dev0
 Summary: LLM Foundry
 Home-page: https://github.com/mosaicml/llm-foundry/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: llm-foundry Version: 0.8.0 Summary: LLM Foundry
-Home-page: https://github.com/mosaicml/llm-foundry/ Author: MosaicML Author-
-email: team@mosaicml.com Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1 Name: llm-foundry Version: 0.9.0.dev0 Summary: LLM
+Foundry Home-page: https://github.com/mosaicml/llm-foundry/ Author: MosaicML
+Author-email: team@mosaicml.com Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
 dev Provides-Extra: databricks Provides-Extra: tensorboard Provides-Extra: gpu-
 flash2 Provides-Extra: gpu Provides-Extra: peft Provides-Extra: openai
 Provides-Extra: megablocks Provides-Extra: all-cpu Provides-Extra: all
 Provides-Extra: all-flash2 License-File: LICENSE
```

### Comparing `llm-foundry-0.8.0/llm_foundry.egg-info/SOURCES.txt` & `llm-foundry-0.9.0.dev0/llm_foundry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llm_foundry.egg-info/requires.txt` & `llm-foundry-0.9.0.dev0/llm_foundry.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -17,75 +17,75 @@
 huggingface-hub<0.23,>=0.19.0
 beautifulsoup4<5,>=4.12.2
 tenacity<9,>=8.2.3
 catalogue<3,>=2
 typer[all]<1
 
 [all]
-mosaicml[peft]<0.23,>=0.22.0
-flash-attn==2.5.8
-databricks-connect==14.1.0
 pytest_codeblocks<0.17,>=0.16.1
-megablocks==0.5.1
+lz4<5,>=4
 pytest<8,>=7.2.1
-pre-commit<4,>=3.4.0
-packaging<23,>=21
+pyright==1.1.256
+mosaicml[tensorboard]<0.23,>=0.22.0
+flash-attn==2.5.8
+pytest-cov<5,>=4
 grouped-gemm==0.1.4
-toml<0.11,>=0.10.2
+databricks-connect==14.1.0
+coverage[toml]==7.4.4
 tiktoken==0.4.0
-pytest-cov<5,>=4
-databricks-sql-connector<4,>=3
-mosaicml[tensorboard]<0.23,>=0.22.0
-openai==1.3.8
-pyright==1.1.256
 hf_transfer==0.1.3
 mosaicml[databricks]<0.23,>=0.22.0
-lz4<5,>=4
-coverage[toml]==7.4.4
-
-[all-cpu]
-databricks-sql-connector<4,>=3
-mosaicml[tensorboard]<0.23,>=0.22.0
+megablocks==0.5.1
+pre-commit<4,>=3.4.0
 openai==1.3.8
-mosaicml[databricks]<0.23,>=0.22.0
+toml<0.11,>=0.10.2
+databricks-sql-connector<4,>=3
 mosaicml[peft]<0.23,>=0.22.0
-pytest<8,>=7.2.1
-databricks-connect==14.1.0
-pyright==1.1.256
+packaging<23,>=21
+
+[all-cpu]
 pytest_codeblocks<0.17,>=0.16.1
 pre-commit<4,>=3.4.0
-packaging<23,>=21
+openai==1.3.8
 lz4<5,>=4
-hf_transfer==0.1.3
-coverage[toml]==7.4.4
-toml<0.11,>=0.10.2
+pytest<8,>=7.2.1
+pyright==1.1.256
+mosaicml[tensorboard]<0.23,>=0.22.0
 tiktoken==0.4.0
+toml<0.11,>=0.10.2
 pytest-cov<5,>=4
+hf_transfer==0.1.3
+databricks-connect==14.1.0
+coverage[toml]==7.4.4
+mosaicml[databricks]<0.23,>=0.22.0
+mosaicml[peft]<0.23,>=0.22.0
+databricks-sql-connector<4,>=3
+packaging<23,>=21
 
 [all-flash2]
-mosaicml[peft]<0.23,>=0.22.0
-flash-attn==2.5.8
-databricks-connect==14.1.0
 pytest_codeblocks<0.17,>=0.16.1
-megablocks==0.5.1
+lz4<5,>=4
 pytest<8,>=7.2.1
-pre-commit<4,>=3.4.0
-packaging<23,>=21
+pyright==1.1.256
+mosaicml[tensorboard]<0.23,>=0.22.0
+flash-attn==2.5.8
+pytest-cov<5,>=4
 grouped-gemm==0.1.4
-toml<0.11,>=0.10.2
+databricks-connect==14.1.0
+coverage[toml]==7.4.4
 tiktoken==0.4.0
-pytest-cov<5,>=4
-databricks-sql-connector<4,>=3
-mosaicml[tensorboard]<0.23,>=0.22.0
-openai==1.3.8
-pyright==1.1.256
 hf_transfer==0.1.3
 mosaicml[databricks]<0.23,>=0.22.0
-lz4<5,>=4
-coverage[toml]==7.4.4
+megablocks==0.5.1
+pre-commit<4,>=3.4.0
+openai==1.3.8
+toml<0.11,>=0.10.2
+databricks-sql-connector<4,>=3
+mosaicml[peft]<0.23,>=0.22.0
+packaging<23,>=21
 
 [databricks]
 mosaicml[databricks]<0.23,>=0.22.0
 databricks-sql-connector<4,>=3
 databricks-connect==14.1.0
 lz4<5,>=4
```

### Comparing `llm-foundry-0.8.0/llmfoundry/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,8 +67,8 @@
     'metrics',
     'models',
     'optim',
     'tokenizers',
     'utils',
 ]
 
-__version__ = '0.8.0'
+__version__ = '0.9.0.dev0'
```

### Comparing `llm-foundry-0.8.0/llmfoundry/callbacks/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/callbacks/async_eval_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/async_eval_callback.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/callbacks/curriculum_learning_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/curriculum_learning_callback.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/callbacks/eval_gauntlet_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/eval_gauntlet_callback.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/callbacks/eval_output_logging_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/eval_output_logging_callback.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/callbacks/fdiff_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/fdiff_callback.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/callbacks/hf_checkpointer.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/hf_checkpointer.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/callbacks/log_mbmoe_tok_per_expert_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/log_mbmoe_tok_per_expert_callback.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/callbacks/monolithic_ckpt_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/monolithic_ckpt_callback.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/callbacks/resumption_callbacks.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/resumption_callbacks.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/callbacks/scheduled_gc_callback.py` & `llm-foundry-0.9.0.dev0/llmfoundry/callbacks/scheduled_gc_callback.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/cli/registry_cli.py` & `llm-foundry-0.9.0.dev0/llmfoundry/cli/registry_cli.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/data/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/data/data.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/data.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/data/dataloader.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/data/finetuning/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/data/finetuning/collator.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/collator.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/data/finetuning/dataloader.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/dataloader.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/data/finetuning/tasks.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/finetuning/tasks.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/data/packing.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/packing.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/data/text_data.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/text_data.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/data/utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/data/utils.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/eval/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/eval/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 # Copyright 2024 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 from llmfoundry.eval.datasets.in_context_learning_evaluation import (
-    InContextLearningCodeEvalDataset,
     InContextLearningDataset,
     InContextLearningGenerationTaskWithAnswersDataset,
     InContextLearningLMTaskDataset,
     InContextLearningMultipleChoiceTaskDataset,
     InContextLearningSchemaTaskDataset,
     get_icl_task_dataloader,
 )
 from llmfoundry.eval.metrics.nlp import (
-    InContextLearningCodeEvalAccuracy,
     InContextLearningGenerationExactMatchAccuracy,
     InContextLearningLMAccuracy,
     InContextLearningLMExpectedCalibrationError,
     InContextLearningMCExpectedCalibrationError,
     InContextLearningMetric,
     InContextLearningMultipleChoiceAccuracy,
 )
 
 __all__ = [
     'InContextLearningDataset',
     'InContextLearningLMTaskDataset',
     'InContextLearningMultipleChoiceTaskDataset',
     'InContextLearningSchemaTaskDataset',
-    'InContextLearningCodeEvalDataset',
     'InContextLearningGenerationTaskWithAnswersDataset',
     'get_icl_task_dataloader',
     'InContextLearningMetric',
     'InContextLearningLMAccuracy',
     'InContextLearningMultipleChoiceAccuracy',
     'InContextLearningGenerationExactMatchAccuracy',
-    'InContextLearningCodeEvalAccuracy',
     'InContextLearningLMExpectedCalibrationError',
     'InContextLearningMCExpectedCalibrationError',
 ]
```

### Comparing `llm-foundry-0.8.0/llmfoundry/eval/datasets/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/eval/datasets/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright 2024 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Natively supported in-context learning evaluation datasets."""
 
 from llmfoundry.eval.datasets.in_context_learning_evaluation import (
-    InContextLearningCodeEvalDataset,
     InContextLearningDataset,
     InContextLearningGenerationTaskWithAnswersDataset,
     InContextLearningLMTaskDataset,
     InContextLearningMultipleChoiceTaskDataset,
     InContextLearningSchemaTaskDataset,
     get_icl_task_dataloader,
 )
@@ -24,15 +23,14 @@
     trim_context,
 )
 
 __all__ = [
     'InContextLearningDataset',
     'InContextLearningGenerationTaskWithAnswersDataset',
     'InContextLearningLMTaskDataset',
-    'InContextLearningCodeEvalDataset',
     'InContextLearningMultipleChoiceTaskDataset',
     'InContextLearningSchemaTaskDataset',
     'get_icl_task_dataloader',
     'MultiTokenEOSCriteria',
     'strip_data',
     'tokenizer_needs_prefix_space',
     'trim_context',
```

### Comparing `llm-foundry-0.8.0/llmfoundry/eval/datasets/in_context_learning_evaluation.py` & `llm-foundry-0.9.0.dev0/llmfoundry/eval/datasets/in_context_learning_evaluation.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from __future__ import annotations
 
 import copy
 import json
 import logging
 import os
 import random
-import warnings
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Union
 
 import torch
 import transformers
 from composer.core import DataSpec
 from composer.core.data_spec import _default_split_batch, _split_list
 from composer.utils import MissingConditionalImportError, dist, get_file
@@ -26,27 +25,25 @@
     get_fewshot_sample_idxs,
     make_padded_input,
     stop_sequences_criteria,
     strip_data,
     tokenizer_needs_prefix_space,
     trim_context,
 )
-from llmfoundry.utils.warnings import VersionedDeprecationWarning
 
 log = logging.getLogger(__name__)
 
 # Allow models to have slightly more tokens than were used in the most verbose CoT in the dataset
 _MAX_ANSWER_BUFFER_LENGTH = 10
 
 __all__ = [
     'InContextLearningDataset',
     'InContextLearningLMTaskDataset',
     'InContextLearningMultipleChoiceTaskDataset',
     'InContextLearningSchemaTaskDataset',
-    'InContextLearningCodeEvalDataset',
     'InContextLearningGenerationTaskWithAnswersDataset',
     'get_icl_task_dataloader',
 ]
 
 
 class InContextLearningDataset(Dataset):
     r"""A base dataset that constructs batches for in-context learning task.
@@ -1288,253 +1285,14 @@
             )
             tokenized_example[self.answer_key].append(tokenized_continuation)
 
         tokenized_example['gold'] = example['gold']
         return tokenized_example
 
 
-class InContextLearningCodeEvalDataset(InContextLearningDataset):
-    """A dataset that constructs batches for in-context learning code.
-
-    evaluation.
-
-    The input format is expected to be a jsonl file with the following fields:
-
-    - task_id: Label of given task
-    - prompt: The code snippet that must be completed
-    - entry_point: The entry to the function/code snippet to generate
-    - canonical_solution: Working solution
-    - test: The checker code that will run to completion if the code generation is valid and otherwise throw assertion
-    - test_inputs: List of test inputs
-    - test_outputs: List of test outputs
-    - language: The language of the code snippet
-
-    Each batch then consists of the following the structure
-
-    - input_ids: Input tensor batch x seqlen x num tokens
-    - mode: Indicates to the model that this is an ICL task and may rely on a custom code path to properly update metrics
-    - mode: Always set to 'generate'
-    - labels: Exact solution for the coding problem
-    - prompts: Prompt for the task
-    - entry_points: List of entry points
-    - test_inputs: List of test inputs
-    - test_outputs: List of test outputs
-    - languages:  List of languages
-    - pass_at_k: Passed value for pass_at_k
-    - generation_kwargs: Dictionary of kwargs needed for generation. Includes the following, which will be individually overwritten
-      by keys in generation_kwargs if set (see https://huggingface.co/docs/transformers/main_classes/text_generation#transformers.GenerationConfig
-      for more details):
-
-        - pad_token_id: ID for padding token, derived automatically
-        - num_beams: How many beams to search for generations, default set to 1
-        - do_sample: Determines whether model is sampling or greedily decoding. Always set to True
-        - use_cache: Whether or not to use past key values to speed up sampling. Always set to True
-
-    Additional Args:
-        generations_per_sample (int) (defaults to 1): The number of independently computed returned sequences for each element in the batch
-        pass_at_k (int) (defaults to 1): k for how many chances the model gets to write passing code
-    """
-
-    def __init__(
-        self,
-        generations_per_sample: int,
-        pass_at_k: Union[int, list[int]] = 1,
-        *args: Any,
-        **kwargs: Any,
-    ):
-        if isinstance(pass_at_k, int):
-            pass_at_k = [pass_at_k]
-        if generations_per_sample < max(pass_at_k):
-            raise ValueError(
-                f'generations_per_sample ({generations_per_sample}) must be greater than or equal to pass_at_k ({pass_at_k}) for code evaluation.',
-            )
-        batch_mapping = {
-            'input_ids': 'prompt',
-            'prompts': 'prompt_text',
-            'tests': 'test',
-            'labels': 'canonical_solution',
-            'entry_points': 'entry_point',
-            'test_inputs': 'test_inputs',
-            'test_outputs': 'test_outputs',
-            'languages': 'language',
-            'sample_id': 'sample_id',
-        }
-        # Linting complains if these are not set in init
-        self.max_prompt_length = 0
-        self.max_answer_length = 0
-        static_keys = [
-            'mode',
-            'pass_at_k',
-            'generation_kwargs',
-            'generations_per_sample',
-            'dataset_size',
-        ]
-        list_keys = [
-            'prompts',
-            'tests',
-            'entry_points',
-            'test_inputs',
-            'test_outputs',
-            'languages',
-            'labels',
-            'sample_id',
-        ]
-        tensor_keys = ['input_ids', 'attention_mask']
-        super().__init__(
-            context_key='prompt',
-            answer_key='canonical_solution',
-            strip_dataset=False,
-            static_keys=static_keys,
-            list_keys=list_keys,
-            tensor_keys=tensor_keys,
-            tokenize_labels=False,
-            padding_side='left',
-            batch_mapping=batch_mapping,
-            *args,
-            **kwargs,
-        )
-        self._set_max_prompt_and_answer_lengths()
-        if self.max_seq_len < self.max_prompt_length:
-            log.warning(f'`max_seq_len` {self.max_seq_len} was less than `max_prompt_len`: {self.max_prompt_length}' \
-                        + ' setting  `max_seq_len`=`max_prompt_len`')
-            self.max_seq_len = self.max_prompt_length
-        dataset_size = len(self.dataset)
-        self.dataset = self.dataset.map(self._trim_padding)
-        self.dataset = self.repeat_dataset(self.dataset, generations_per_sample)
-
-        if self.max_answer_length < self.max_seq_len - self.max_prompt_length:
-            max_new_tokens = self.max_answer_length
-        else:
-            max_new_tokens = self.max_seq_len - self.max_prompt_length
-
-        self.base_batch = {
-            'input_ids': [],
-            'mode': 'generate',
-            'labels': [],
-            'prompts': [],
-            'tests': [],
-            'entry_points': [],
-            'test_inputs': [],
-            'test_outputs': [],
-            'languages': [],
-            'pass_at_k': pass_at_k,
-            'generation_kwargs': {
-                'pad_token_id': self.pad_tok_id,
-                'num_beams': 1,  # single beam
-                'do_sample': True,
-                'temperature': 0.2,  # good default for code
-                'use_cache': True,
-                'eos_token_id': self.tokenizer.eos_token_id,
-                'max_new_tokens': max(max_new_tokens, 1),
-            },
-            'sample_id': [],
-            'pass_at_k': list(pass_at_k),
-            'generations_per_sample': generations_per_sample,
-            'dataset_size': dataset_size,
-        }
-        if 'generation_kwargs' in kwargs:
-            self.update_generation_kwargs(kwargs['generation_kwargs'])
-
-    def repeat_dataset(self, dataset: HFDataset, repetitions: int) -> HFDataset:
-
-        def _repeat_dataset():
-            for i, sample in enumerate(dataset):
-                for _ in range(repetitions):
-                    assert isinstance(sample, dict)
-                    yield {'sample_id': i, **sample}
-
-        from datasets import \
-            Dataset as HFDataset  # pyright: ignore[reportGeneralTypeIssues]
-
-        repeated_dataset = HFDataset.from_generator(_repeat_dataset)
-        assert isinstance(repeated_dataset, HFDataset)
-        return repeated_dataset
-
-    def _set_max_prompt_and_answer_lengths(self):
-        """Iterates through the dataset and finds the maximum prompt length and.
-
-        sequence lengths.
-
-        Returns:
-            None
-        """
-        max_prompt_length = 0
-        max_answer_length = 0
-        for example in self.dataset:
-            assert isinstance(example, Dict)
-            unpadded_example = [
-                token for token in example[self.context_key]
-                if token != self.pad_tok_id
-            ]
-            max_prompt_length = max(max_prompt_length, len(unpadded_example))
-
-            tokenized_answer = self.tokenizer(
-                example['canonical_solution'],
-                add_special_tokens=False,
-            )['input_ids']
-            assert isinstance(tokenized_answer, list)
-            len_tokenized_answer = len(tokenized_answer)
-            max_answer_length = max(max_answer_length, len_tokenized_answer)
-
-        self.max_prompt_length = max_prompt_length
-        self.max_answer_length = max_answer_length + _MAX_ANSWER_BUFFER_LENGTH
-
-    def _trim_padding(self, example: Dict):
-        """Adjusts padding to the maximum prompt length rather than max_seq_len.
-
-        Needs to be done after the dataset has been processed because we don't
-        know the maximum prompt length until after we've tokenized it.
-
-        Returns:
-            dataset: A HuggingFace Dataset with different padding lengths for example[self.context_key]
-        """
-        # Remove padding tokens applied during tokenization
-        unpadded_prompt = [
-            token for token in example[self.context_key]
-            if token != self.pad_tok_id
-        ]
-        # Reapply padding only to max_prompt_length
-        full_prompt = trim_context(unpadded_prompt, [], self.max_prompt_length)
-        padded_context = make_padded_input(
-            full_prompt,
-            [],
-            self.max_prompt_length,
-            self.pad_tok_id,
-            self.padding_side,
-        )
-
-        example[self.context_key] = padded_context
-        return example
-
-    def tokenize_example(
-        self,
-        prompt_and_fewshot: str,
-        ctxt: str,
-        example: Dict,
-    ) -> Dict[str, Any]:
-        """Adds extra code task details to the example dictionary.
-
-        See InContextLearningDataset for more details
-        """
-        tokenized_example = super().tokenize_example(
-            prompt_and_fewshot,
-            ctxt,
-            example,
-        )
-        tokenized_example['prompt_text'] = example['prompt']
-        tokenized_example['task_id'] = example['task_id']
-        tokenized_example['canonical_solution'] = example['canonical_solution']
-        tokenized_example['test'] = example['test']
-        tokenized_example['entry_point'] = example['entry_point']
-        tokenized_example['test_inputs'] = example['test_inputs']
-        tokenized_example['test_outputs'] = example['test_outputs']
-        tokenized_example['language'] = example['language']
-        return tokenized_example
-
-
 def build_icl_dataloader(
     icl_task_type: str,
     dataset_uri: str,
     tokenizer: transformers.PreTrainedTokenizerBase,
     batch_size: int,
     max_seq_len: int,
     pad_tok_id: int,
@@ -1617,22 +1375,15 @@
             prelimiter=prelimiter,
             fewshot_random_seed=fewshot_random_seed,
             hf_loading_vars=hf_loading_vars,
             hf_parsing_map=hf_parsing_map,
             generation_kwargs=generation_kwargs,
         )
         effective_batchsize = batch_size
-    elif icl_task_type == 'generation_task_with_answers' or icl_task_type == 'question_answering':
-        if icl_task_type == 'question_answering':
-            warnings.warn(
-                VersionedDeprecationWarning(
-                    "ICL task type 'question_answering' is now deprecated. Use identifier 'generation_task_with_answers'",
-                    'v0.9.0',
-                ),
-            )
+    elif icl_task_type == 'generation_task_with_answers':
         dataset = InContextLearningGenerationTaskWithAnswersDataset(
             dataset_uri=dataset_uri,
             tokenizer=tokenizer,
             max_seq_len=max_seq_len,
             pad_tok_id=pad_tok_id,
             num_fewshot=num_fewshot,
             prompt_string=prompt_string,
@@ -1645,52 +1396,25 @@
             hf_parsing_map=hf_parsing_map,
             cot_delimiter=cot_delimiter,
             early_stopping_criteria=early_stopping_criteria,
             do_normalization=do_normalization,
             generation_kwargs=generation_kwargs,
         )
         effective_batchsize = batch_size
-    elif icl_task_type == 'code_evaluation':
-        warnings.warn(
-            VersionedDeprecationWarning(
-                "ICL task type 'code_evaluation' is deprecated and will no longer be supported. ",
-                'v0.9.0',
-            ),
-        )
-        dataset = InContextLearningCodeEvalDataset(
-            dataset_uri=dataset_uri,
-            tokenizer=tokenizer,
-            max_seq_len=max_seq_len,
-            pad_tok_id=pad_tok_id,
-            num_fewshot=num_fewshot,
-            prompt_string=prompt_string,
-            example_delimiter=example_delimiter,
-            continuation_delimiter=continuation_delimiter,
-            destination_path=destination_path,
-            prelimiter=prelimiter,
-            fewshot_random_seed=fewshot_random_seed,
-            hf_loading_vars=hf_loading_vars,
-            hf_parsing_map=hf_parsing_map,
-            pass_at_k=pass_at_k,
-            generations_per_sample=generations_per_sample,
-            generation_kwargs=generation_kwargs,
-        )
-        effective_batchsize = batch_size
     else:
         raise Exception(f'Unrecognized ICL task type: {icl_task_type}')
 
     sampler = dist.get_sampler(dataset, drop_last=False, shuffle=False)
 
     split_batch = None
     if isinstance(
         dataset,
         (
             InContextLearningMultipleChoiceTaskDataset,
             InContextLearningGenerationTaskWithAnswersDataset,
-            InContextLearningCodeEvalDataset,
         ),
     ):
         split_batch = dataset.split_batch
 
     return DataSpec(
         DataLoader(
             dataset,
```

### Comparing `llm-foundry-0.8.0/llmfoundry/eval/datasets/utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/eval/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/eval/metrics/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/eval/metrics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # Copyright 2024 MosaicML LLM Foundry authors
 # SPDX-License-Identifier: Apache-2.0
 
 """A collection of common torchmetrics."""
 
 from llmfoundry.eval.metrics.nlp import (
-    InContextLearningCodeEvalAccuracy,
     InContextLearningGenerationExactMatchAccuracy,
     InContextLearningLMAccuracy,
     InContextLearningLMExpectedCalibrationError,
     InContextLearningMCExpectedCalibrationError,
     InContextLearningMetric,
     InContextLearningMultipleChoiceAccuracy,
 )
 
 __all__ = [
     'InContextLearningMetric',
     'InContextLearningLMAccuracy',
     'InContextLearningMultipleChoiceAccuracy',
     'InContextLearningGenerationExactMatchAccuracy',
-    'InContextLearningCodeEvalAccuracy',
     'InContextLearningLMExpectedCalibrationError',
     'InContextLearningMCExpectedCalibrationError',
 ]
```

### Comparing `llm-foundry-0.8.0/llmfoundry/eval/metrics/nlp.py` & `llm-foundry-0.9.0.dev0/llmfoundry/eval/metrics/nlp.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,41 +2,30 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """A collection of common torchmetrics for NLP tasks."""
 
 import copy
 import functools
 import logging
-import os
 import re
 import string
-import warnings
 from typing import Any, Callable, Dict, List
 
-import numpy as np
 import torch
-from composer.utils import dist
-from composer.utils.eval_client import (
-    EvalClient,
-    LambdaEvalClient,
-    LocalEvalClient,
-    MosaicMLLambdaEvalClient,
-)
 from torch import Tensor
 from torch.nn import functional as F
 from torchmetrics import Metric
 
 log = logging.getLogger(__name__)
 
 __all__ = [
     'InContextLearningMetric',
     'InContextLearningLMAccuracy',
     'InContextLearningMultipleChoiceAccuracy',
     'InContextLearningGenerationExactMatchAccuracy',
-    'InContextLearningCodeEvalAccuracy',
     'InContextLearningLMExpectedCalibrationError',
     'InContextLearningMCExpectedCalibrationError',
 ]
 
 
 class InContextLearningMetric(Metric):
 
@@ -404,231 +393,14 @@
 
     def compute(self):
         assert isinstance(self.correct, Tensor)
         assert isinstance(self.total, Tensor)
         return self.correct.float() / self.total
 
 
-class InContextLearningCodeEvalAccuracy(InContextLearningMetric):
-    r"""Computes accuracy for In-context learning (ICL) code evaluation tasks.
-
-    ICL code eval tasks consist of some number of example code eval tasks (referred to as the 'context'), followed by a test task where the model must
-    complete the code, where we term the code completion a 'continuation'.
-
-    In each case, the model constructs a given number of continuations (termed pass@K for K continuations), and each continuation is run against a set of test cases. The model is considered
-    correct if at least one of the proposed continuations passes all the test cases.
-
-    Runs on AWS Lambdas by default.
-
-    Adds metric state variables:
-        correct (float): The number of instances where the predictions passed all the test cases.
-        total (float): The number of total instances that were predicted.
-
-    Args:
-        dist_sync_on_step (bool, optional): Synchronize metric state across processes at
-            each forward() before returning the value at the step. Default: ``False``.
-    """
-
-    # Make torchmetrics call update only once
-    full_state_update = False
-
-    def __init__(self, dist_sync_on_step: bool = False):
-        # state from multiple processes
-        super().__init__(dist_sync_on_step=dist_sync_on_step)
-
-        self._initialized = False
-        self.dataset_size = 0
-        self.pass_at_k = []
-        self.num_generations = 0
-        self.eval_device = os.environ.get('CODE_EVAL_DEVICE', None)
-        if self.eval_device is not None:
-            self.eval_device = self.eval_device.upper()
-        self.metric_result_dict = {
-            'context': [],
-            'output': [],
-            'result': [],
-            'sample_id': [],
-        }
-
-    def get_client(self) -> EvalClient:
-        """Returns a client for the appropriate remote platform."""
-        client = None
-        if self.eval_device == 'LOCAL':
-            warnings.warn(
-                'Running code eval locally may be insecure. Please set environment variable CODE_EVAL_DEVICE '
-                +
-                'to LAMBDA to run on remote. To use Lambdas, spin up your instance that checks code, set the URL as '
-                + 'CODE_EVAL_URL and the API key as CODE_EVAL_APIKEY.',
-            )
-            log.debug('Running code eval locally.')
-            client = LocalEvalClient()
-        elif self.eval_device == 'LAMBDA':
-            client = LambdaEvalClient()
-        elif self.eval_device == 'MOSAICML':
-            client = MosaicMLLambdaEvalClient()
-        elif self.eval_device is None:
-            raise ValueError(
-                'Attempting to use InContextLearningCodeEvalAccuracy but environment '
-                +
-                'variable `CODE_EVAL_DEVICE` is not set. Please set it to `CODE_EVAL_DEVICE` '
-                +
-                'to one of `LOCAL` (for unsafe local eval), `LAMBDA` (for AWS lambda '
-                + 'evaluation), or `MOSAICML` (for lambda eval through MAPI).',
-            )
-        else:
-            raise ValueError(
-                'Environment variable `CODE_EVAL_DEVICE` must be one of `LOCAL`, '
-                + f'`LAMBDA`, or `MOSAICML` but got {self.eval_device}.',
-            )
-
-        return client
-
-    def estimator(self, n: int, c: int, k: int) -> float:
-        """Computes the pass@k metric.
-
-        Given the number of generated samples, n, the number of correct samples, c, and the k of interest,
-        this function calculates pass@k as 1 - comb(n - c, k) / comb(n, k) as per the definition of
-        pass@k in the HumanEval paper (https://arxiv.org/abs/2107.03374) and it's associated implementation:
-        https://github.com/openai/human-eval.
-        """
-        if n - c < k:
-            return 1.0
-        return 1.0 - float(np.prod(1.0 - k / np.arange(n - c + 1, n + 1)))
-
-    def _initialize_state(self, batch: dict[str, Any]):
-        device = batch['input_ids'].device
-        self.dataset_size = batch['dataset_size']
-        self.pass_at_k = batch['pass_at_k']
-        self.num_generations = batch['generations_per_sample']
-
-        # We need to defer the accumulator initialization because it depends on dataset size
-        self.add_state(
-            'correct',
-            default=torch.zeros(self.dataset_size, device=device),
-            dist_reduce_fx='sum',
-        )
-        self.add_state(
-            'total',
-            default=torch.zeros(self.dataset_size, device=device),
-            dist_reduce_fx='sum',
-        )
-        dist.barrier()
-        self._initialized = True
-
-    def update(
-        self,
-        batch: Dict[str, Any],
-        outputs: List[str],
-        labels: List[str],
-    ):
-        """Updates the pass@k accuracy of code generation.
-
-        Given a batch of prompts, test cases, and code generations, evaluates the code generations
-        against the test cases and augments the pass@k accuracy of the batch to the values so far.
-
-        Args:
-            batch (Dict[str, Any]): A batch of data produced by the InContextLearningCodeEvalDataset, with
-            the prompt, test cases, and entry points. This will be a dictionary that must have the following
-            arguments:
-            {
-                'prompts': List[str],
-                'test_inputs': List[List[str]],
-                'test_outputs': List[List[str]],
-                'entry_points': List[str],
-                'languages': List[str],
-                'generation_kwargs': Dict[str, Any]
-            }
-            outputs (List[str]): A list of code generations in the format of HF generate with beam search,
-            which is the a list of strings in groups of beam_size e.g. for beam size 2 and batch size 2, the list
-            will be of the format [prompt 1 gen 1, prompt 1 gen 2, prompt 2 gen 1, prompt 2 gen 2]
-            labels (List[str]): A list of the correct code generations, for compatibility with existing HF generate
-            functionalities. This is not used.
-        """
-        if not self._initialized:
-            self._initialize_state(batch)
-
-        del labels  # never used
-        client = self.get_client()
-
-        metric_result_dict = copy.deepcopy(self.metric_result_dict)
-        for sample_id, code_gen, sample_prompt, test_inputs, test_outputs, entry_point, language in zip(
-            batch['sample_id'],
-            outputs,
-            batch['prompts'],
-            batch['test_inputs'],
-            batch['test_outputs'],
-            batch['entry_points'],
-            batch['languages'],
-        ):
-
-            idx = sample_id
-            self.total[idx] += 1.0
-            metric_result_dict['sample_id'].append(sample_id)
-
-            code_gen = re.split(r'\n[A-Za-z0-9#`]', code_gen)[
-                0]  # remove everything after function ends
-            final_code = sample_prompt + code_gen  # combine prompt with the code generation
-            metric_result_dict['context'].append(sample_prompt)
-            metric_result_dict['output'].append(code_gen)
-
-            test_results = []
-            for test_input, test_output in zip(test_inputs, test_outputs):
-                payload = {
-                    'code': final_code,
-                    'input': test_input,
-                    'output': test_output,
-                    'entry_point': entry_point,
-                    'language': language,
-                }
-
-                result = client.invoke([[[payload]]])[0][0][0]
-                test_results.append(result)
-
-            if all(test_results):
-                self.correct[idx] += 1.0
-                metric_result_dict['result'].append(1)
-            else:
-                metric_result_dict['result'].append(0)
-
-        client.close()  # pyright: ignore [reportOptionalMemberAccess]
-        return metric_result_dict
-
-    def compute(self):
-        assert isinstance(self.correct, Tensor)
-        assert isinstance(self.total, Tensor)
-        complete = self.total == self.num_generations  # so that eval subset batches can be used
-
-        if complete.sum() < (self.total != 0).sum():
-            warnings.warn(
-                'Some samples in the dataset have less than the expected number of generations. '
-                +
-                'This is expected if you are using a subset of the dataset for evaluation.',
-            )
-
-        if (self.correct > self.total).any().item():
-            raise ValueError(
-                'Internal error some samples have more correct than  total generations. This should not happen.',
-            )
-
-        results = {}
-        n = self.num_generations
-
-        for k in self.pass_at_k:
-            pass_at_k = sum([
-                self.estimator(n, int(c.item()), k)
-                for c in self.correct[complete]
-            ]) / complete.sum().item()
-            results[f'pass@{k}'] = torch.tensor(pass_at_k)
-
-        if len(results) == 1:  # backwards compatibility
-            return list(results.values())[0]
-
-        return results
-
-
 class InContextLearningExpectedCalibrationError(InContextLearningMetric):
     """Generic class for Expected Calibration Error (ECE).
 
     Citation: https://arxiv.org/pdf/1706.04599.pdf
 
     Expected calibration error is calculated by dividing predictions into buckets based on the model's confidence (a probability value between 0 and 1).
     We then calculate the accuracy within each bucket and calculate the average gap between confidence and accuracy
```

### Comparing `llm-foundry-0.8.0/llmfoundry/interfaces/callback_with_config.py` & `llm-foundry-0.9.0.dev0/llmfoundry/interfaces/callback_with_config.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/layers_registry.py` & `llm-foundry-0.9.0.dev0/llmfoundry/layers_registry.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/loggers/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/metrics/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/metrics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from composer.metrics import (
     LanguageCrossEntropy,
     LanguagePerplexity,
     MaskedAccuracy,
 )
 
 from llmfoundry.eval.metrics import (
-    InContextLearningCodeEvalAccuracy,
     InContextLearningGenerationExactMatchAccuracy,
     InContextLearningLMAccuracy,
     InContextLearningLMExpectedCalibrationError,
     InContextLearningMCExpectedCalibrationError,
     InContextLearningMultipleChoiceAccuracy,
 )
 from llmfoundry.metrics.token_acc import TokenAccuracy
@@ -29,15 +28,14 @@
     func=InContextLearningMCExpectedCalibrationError,
 )
 metrics.register('mc_accuracy', func=InContextLearningMultipleChoiceAccuracy)
 metrics.register(
     'qa_accuracy',
     func=InContextLearningGenerationExactMatchAccuracy,
 )
-metrics.register('code_eval_accuracy', func=InContextLearningCodeEvalAccuracy)
 metrics.register('language_cross_entropy', func=LanguageCrossEntropy)
 metrics.register('language_perplexity', func=LanguagePerplexity)
 metrics.register('masked_accuracy', func=MaskedAccuracy)
 
 DEFAULT_CAUSAL_LM_TRAIN_METRICS = [
     'language_cross_entropy',
     'language_perplexity',
@@ -49,27 +47,25 @@
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
     'InContextLearningGenerationExactMatchAccuracy',
-    'InContextLearningCodeEvalAccuracy',
     'DEFAULT_CAUSAL_LM_TRAIN_METRICS',
     'DEFAULT_CAUSAL_LM_EVAL_METRICS',
     'DEFAULT_ENC_DEC_METRICS',
 ]
```

### Comparing `llm-foundry-0.8.0/llmfoundry/metrics/token_acc.py` & `llm-foundry-0.9.0.dev0/llmfoundry/metrics/token_acc.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/hf/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/hf/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/hf/hf_causal_lm.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/hf/hf_causal_lm.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/hf/hf_fsdp.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/hf/hf_fsdp.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/hf/hf_t5.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/hf/hf_t5.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/hf/model_wrapper.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/hf/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/inference_api_wrapper/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/inference_api_wrapper/fmapi.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/fmapi.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/inference_api_wrapper/interface.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/interface.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/inference_api_wrapper/openai_causal_lm.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/inference_api_wrapper/openai_causal_lm.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/layers/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/layers/attention.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/layers/attention.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/layers/blocks.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/layers/dmoe.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/layers/dmoe.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/layers/ffn.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/layers/ffn.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/layers/layer_builders.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/layers/layer_builders.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/layers/norm.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/layers/norm.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/mpt/configuration_mpt.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/mpt/configuration_mpt.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/mpt/modeling_mpt.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/mpt/modeling_mpt.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/utils/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/utils/act_ckpt.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/utils/act_ckpt.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/utils/config_moe_args.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/utils/config_moe_args.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/utils/meta_init_context.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/utils/meta_init_context.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/utils/mpt_param_count.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/utils/mpt_param_count.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/models/utils/param_init_fns.py` & `llm-foundry-0.9.0.dev0/llmfoundry/models/utils/param_init_fns.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/optim/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/optim/adaptive_lion.py` & `llm-foundry-0.9.0.dev0/llmfoundry/optim/adaptive_lion.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/optim/lion.py` & `llm-foundry-0.9.0.dev0/llmfoundry/optim/lion.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/optim/outlier_detection.py` & `llm-foundry-0.9.0.dev0/llmfoundry/optim/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/optim/scheduler.py` & `llm-foundry-0.9.0.dev0/llmfoundry/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/registry.py` & `llm-foundry-0.9.0.dev0/llmfoundry/registry.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/tokenizers/tiktoken.py` & `llm-foundry-0.9.0.dev0/llmfoundry/tokenizers/tiktoken.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/__init__.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/builders.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import contextlib
 import functools
 import logging
 import os
 import re
-import warnings
 from collections import OrderedDict
 from typing import (
     Any,
     ContextManager,
     Dict,
     Iterable,
     List,
@@ -34,15 +33,14 @@
 from llmfoundry import registry
 from llmfoundry.callbacks import EvalGauntlet
 from llmfoundry.data.dataloader import build_dataloader
 from llmfoundry.eval.datasets.in_context_learning_evaluation import \
     get_icl_task_dataloader
 from llmfoundry.tokenizers.tiktoken import TiktokenTokenizerWrapper
 from llmfoundry.utils.registry_utils import construct_from_registry
-from llmfoundry.utils.warnings import VersionedDeprecationWarning
 
 log = logging.getLogger(__name__)
 
 __all__ = [
     'build_algorithm',
     'build_callback',
     'build_evaluators',
@@ -527,27 +525,18 @@
                 icl_cfg.metric_names = [
                     'InContextLearningMultipleChoiceAccuracy',
                 ]
             elif icl_cfg.icl_task_type == 'schema':
                 icl_cfg.metric_names = [
                     'InContextLearningMultipleChoiceAccuracy',
                 ]
-            elif icl_cfg.icl_task_type == 'generation_task_with_answers' or icl_cfg.icl_task_type == 'question_answering':
-                if icl_cfg.icl_task_type == 'question_answering':
-                    warnings.warn(
-                        VersionedDeprecationWarning(
-                            "ICL task type 'question_answering' is now deprecated. Use identifier 'generation_task_with_answers'",
-                            'v0.9.0',
-                        ),
-                    )
+            elif icl_cfg.icl_task_type == 'generation_task_with_answers':
                 icl_cfg.metric_names = [
                     'InContextLearningGenerationExactMatchAccuracy',
                 ]
-            elif icl_cfg.icl_task_type == 'code_evaluation':
-                icl_cfg.metric_names = ['InContextLearningCodeEvalAccuracy']
             else:
                 raise ValueError(
                     f'No metric_names defined, unable to build default metrics for icl_task_type={icl_cfg.icl_task_type}.',
                 )
 
         if 'prompt_string' not in icl_cfg:
             icl_cfg.prompt_string = ''
```

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/checkpoint_conversion_helpers.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/checkpoint_conversion_helpers.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/config_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/data_prep_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/data_prep_utils.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/exceptions.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/huggingface_hub_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/huggingface_hub_utils.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/logging_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/model_download_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/model_download_utils.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/mosaicml_logger_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/mosaicml_logger_utils.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/prompt_files.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/prompt_files.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/registry_utils.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/llmfoundry/utils/warnings.py` & `llm-foundry-0.9.0.dev0/llmfoundry/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/pyproject.toml` & `llm-foundry-0.9.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/setup.py` & `llm-foundry-0.9.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/tests/test_registry.py` & `llm-foundry-0.9.0.dev0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/tests/test_smoketest.py` & `llm-foundry-0.9.0.dev0/tests/test_smoketest.py`

 * *Files identical despite different names*

### Comparing `llm-foundry-0.8.0/tests/test_utils.py` & `llm-foundry-0.9.0.dev0/tests/test_utils.py`

 * *Files identical despite different names*

