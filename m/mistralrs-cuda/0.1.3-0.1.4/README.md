# Comparing `tmp/mistralrs_cuda-0.1.3.tar.gz` & `tmp/mistralrs_cuda-0.1.4.tar.gz`

## Comparing `mistralrs_cuda-0.1.3.tar` & `mistralrs_cuda-0.1.4.tar`

### file list

```diff
@@ -1,75 +1,78 @@
--rw-r--r--   0     1001      127     1974 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/Cargo.toml
--rw-r--r--   0     1001      127        0 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/README.md
--rw-r--r--   0     1001      127      133 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/aici/README.md
--rw-r--r--   0     1001      127     6567 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/aici/bintokens.rs
--rw-r--r--   0     1001      127      320 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/aici/bytes.rs
--rw-r--r--   0     1001      127    15114 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/aici/cfg.rs
--rw-r--r--   0     1001      127     9819 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/aici/lex.rs
--rw-r--r--   0     1001      127      179 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/aici/mod.rs
--rw-r--r--   0     1001      127     2447 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/aici/recognizer.rs
--rw-r--r--   0     1001      127     1696 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/aici/rx.rs
--rw-r--r--   0     1001      127     3094 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/aici/svob.rs
--rw-r--r--   0     1001      127    17311 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/aici/toktree.rs
--rw-r--r--   0     1001      127     4667 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/device_map.rs
--rw-r--r--   0     1001      127    36507 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/engine/mod.rs
--rw-r--r--   0     1001      127     7663 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/layers.rs
--rw-r--r--   0     1001      127     7868 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/lib.rs
--rw-r--r--   0     1001      127     8310 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/model_loader.rs
--rw-r--r--   0     1001      127    10703 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/model_selected.rs
--rw-r--r--   0     1001      127    16512 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/models/gemma.rs
--rw-r--r--   0     1001      127    15309 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/models/llama.rs
--rw-r--r--   0     1001      127    17943 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/models/mistral.rs
--rw-r--r--   0     1001      127    22512 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/models/mixtral.rs
--rw-r--r--   0     1001      127     2620 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/models/mod.rs
--rw-r--r--   0     1001      127    15629 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/models/phi2.rs
--rw-r--r--   0     1001      127    17509 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/models/phi3.rs
--rw-r--r--   0     1001      127    19605 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/models/quantized_llama.rs
--rw-r--r--   0     1001      127    10138 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/models/quantized_phi2.rs
--rw-r--r--   0     1001      127    16101 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/models/qwen2.rs
--rw-r--r--   0     1001      127     5912 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/chat_template.rs
--rw-r--r--   0     1001      127    13809 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/ggml.rs
--rw-r--r--   0     1001      127    15835 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/gguf.rs
--rw-r--r--   0     1001      127    20832 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/loaders.rs
--rw-r--r--   0     1001      127    10912 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/macros.rs
--rw-r--r--   0     1001      127    33649 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/mod.rs
--rw-r--r--   0     1001      127    12269 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/normal.rs
--rw-r--r--   0     1001      127     6358 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/prefix_cacher.rs
--rw-r--r--   0     1001      127     1250 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/request.rs
--rw-r--r--   0     1001      127     3848 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/response.rs
--rw-r--r--   0     1001      127    11276 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/sampler.rs
--rw-r--r--   0     1001      127     7286 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/scheduler.rs
--rw-r--r--   0     1001      127    15979 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/sequence.rs
--rw-r--r--   0     1001      127     7395 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/utils/mod.rs
--rw-r--r--   0     1001      127     1716 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/utils/tokens.rs
--rw-r--r--   0     1001      127     4799 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/utils/varbuilder_utils.rs
--rw-r--r--   0     1001      127    11049 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/classifier.rs
--rw-r--r--   0     1001      127     1544 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/config.rs
--rw-r--r--   0     1001      127    26714 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/gemma.rs
--rw-r--r--   0     1001      127    25200 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/llama.rs
--rw-r--r--   0     1001      127    27603 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/mistral.rs
--rw-r--r--   0     1001      127    32915 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/mixtral.rs
--rw-r--r--   0     1001      127     4305 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/mod.rs
--rw-r--r--   0     1001      127    24492 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/phi2.rs
--rw-r--r--   0     1001      127    25455 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/phi3.rs
--rw-r--r--   0     1001      127    34219 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/quantized_llama.rs
--rw-r--r--   0     1001      127      794 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-lora/Cargo.toml
--rw-r--r--   0     1001      127        0 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-lora/README.md
--rw-r--r--   0     1001      127     2395 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-lora/src/layer.rs
--rw-r--r--   0     1001      127     5818 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-lora/src/lib.rs
--rw-r--r--   0     1001      127     9472 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-lora/src/loralinear.rs
--rw-r--r--   0     1001      127     9961 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-lora/src/qloralinear.rs
--rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 mistralrs_cuda-0.1.3/mistralrs-pyo3/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-pyo3/.gitignore
--rw-r--r--   0     1001      127     3508 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-pyo3/API.md
--rw-r--r--   0     1001      127      855 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-pyo3/Cargo_template.toml
--rw-r--r--   0     1001      127     3755 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-pyo3/README.md
--rw-r--r--   0     1001      127     7962 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-pyo3/mistralrs.pyi
--rw-r--r--   0     1001      127      530 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-pyo3/pyproject_template.toml
--rw-r--r--   0     1001      127    28898 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-pyo3/src/lib.rs
--rw-r--r--   0     1001      127     1672 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-pyo3/src/stream.rs
--rw-r--r--   0     1001      127     3114 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-pyo3/src/which.rs
--rwxr-xr-x   0     1001      127     2203 2024-05-02 01:30:24.000000 mistralrs_cuda-0.1.3/mistralrs-pyo3/upload.py
--rw-r--r--   0     1001      127    99209 2024-05-02 01:30:41.000000 mistralrs_cuda-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 mistralrs_cuda-0.1.3/Cargo.toml
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 mistralrs_cuda-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 mistralrs_cuda-0.1.3/PKG-INFO
+-rw-r--r--   0     1001      127      794 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-lora/Cargo.toml
+-rw-r--r--   0     1001      127        0 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-lora/README.md
+-rw-r--r--   0     1001      127     2395 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-lora/src/layer.rs
+-rw-r--r--   0     1001      127     5818 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-lora/src/lib.rs
+-rw-r--r--   0     1001      127     9472 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-lora/src/loralinear.rs
+-rw-r--r--   0     1001      127     9961 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-lora/src/qloralinear.rs
+-rw-r--r--   0     1001      127     1997 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/Cargo.toml
+-rw-r--r--   0     1001      127        0 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/README.md
+-rw-r--r--   0     1001      127      133 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/aici/README.md
+-rw-r--r--   0     1001      127     6567 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/aici/bintokens.rs
+-rw-r--r--   0     1001      127      320 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/aici/bytes.rs
+-rw-r--r--   0     1001      127    15100 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/aici/cfg.rs
+-rw-r--r--   0     1001      127     9819 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/aici/lex.rs
+-rw-r--r--   0     1001      127      179 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/aici/mod.rs
+-rw-r--r--   0     1001      127     2447 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/aici/recognizer.rs
+-rw-r--r--   0     1001      127     1696 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/aici/rx.rs
+-rw-r--r--   0     1001      127     3094 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/aici/svob.rs
+-rw-r--r--   0     1001      127    17311 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/aici/toktree.rs
+-rw-r--r--   0     1001      127     4674 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/device_map.rs
+-rw-r--r--   0     1001      127    19350 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/engine/mod.rs
+-rw-r--r--   0     1001      127     7768 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/layers.rs
+-rw-r--r--   0     1001      127     7898 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/lib.rs
+-rw-r--r--   0     1001      127     8310 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/model_loader.rs
+-rw-r--r--   0     1001      127    10703 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/model_selected.rs
+-rw-r--r--   0     1001      127    16539 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/models/gemma.rs
+-rw-r--r--   0     1001      127    15336 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/models/llama.rs
+-rw-r--r--   0     1001      127    17970 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/models/mistral.rs
+-rw-r--r--   0     1001      127    22539 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/models/mixtral.rs
+-rw-r--r--   0     1001      127     2620 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/models/mod.rs
+-rw-r--r--   0     1001      127    15656 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/models/phi2.rs
+-rw-r--r--   0     1001      127    17536 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/models/phi3.rs
+-rw-r--r--   0     1001      127    19614 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/models/quantized_llama.rs
+-rw-r--r--   0     1001      127    10147 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/models/quantized_phi2.rs
+-rw-r--r--   0     1001      127    16128 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/models/qwen2.rs
+-rw-r--r--   0     1001      127     5363 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/cache_manager.rs
+-rw-r--r--   0     1001      127     5911 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/chat_template.rs
+-rw-r--r--   0     1001      127    14988 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/ggml.rs
+-rw-r--r--   0     1001      127    18077 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/gguf.rs
+-rw-r--r--   0     1001      127    22337 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/loaders.rs
+-rw-r--r--   0     1001      127    10912 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/macros.rs
+-rw-r--r--   0     1001      127    36836 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/mod.rs
+-rw-r--r--   0     1001      127    13466 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/normal.rs
+-rw-r--r--   0     1001      127     2677 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/sampling.rs
+-rw-r--r--   0     1001      127     9680 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/sampling_pipeline.rs
+-rw-r--r--   0     1001      127     6693 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/prefix_cacher.rs
+-rw-r--r--   0     1001      127     1250 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/request.rs
+-rw-r--r--   0     1001      127     3848 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/response.rs
+-rw-r--r--   0     1001      127    11276 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/sampler.rs
+-rw-r--r--   0     1001      127     6993 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/scheduler.rs
+-rw-r--r--   0     1001      127    16663 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/sequence.rs
+-rw-r--r--   0     1001      127     7534 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/utils/mod.rs
+-rw-r--r--   0     1001      127     1716 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/utils/tokens.rs
+-rw-r--r--   0     1001      127     4799 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/utils/varbuilder_utils.rs
+-rw-r--r--   0     1001      127    11049 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/classifier.rs
+-rw-r--r--   0     1001      127     1544 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/config.rs
+-rw-r--r--   0     1001      127    26767 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/gemma.rs
+-rw-r--r--   0     1001      127    25253 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/llama.rs
+-rw-r--r--   0     1001      127    27656 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/mistral.rs
+-rw-r--r--   0     1001      127    32968 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/mixtral.rs
+-rw-r--r--   0     1001      127     4322 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/mod.rs
+-rw-r--r--   0     1001      127    24545 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/phi2.rs
+-rw-r--r--   0     1001      127    25484 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/phi3.rs
+-rw-r--r--   0     1001      127    34254 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/quantized_llama.rs
+-rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 mistralrs_cuda-0.1.4/mistralrs-pyo3/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-pyo3/.gitignore
+-rw-r--r--   0     1001      127     3508 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-pyo3/API.md
+-rw-r--r--   0     1001      127      855 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-pyo3/Cargo_template.toml
+-rw-r--r--   0     1001      127     3755 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-pyo3/README.md
+-rw-r--r--   0     1001      127     7962 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-pyo3/mistralrs.pyi
+-rw-r--r--   0     1001      127      530 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-pyo3/pyproject_template.toml
+-rw-r--r--   0     1001      127    28898 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     1672 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-pyo3/src/stream.rs
+-rw-r--r--   0     1001      127     3114 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-pyo3/src/which.rs
+-rwxr-xr-x   0     1001      127     2203 2024-05-08 09:09:24.000000 mistralrs_cuda-0.1.4/mistralrs-pyo3/upload.py
+-rw-r--r--   0     1001      127   100986 2024-05-08 09:09:59.000000 mistralrs_cuda-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 mistralrs_cuda-0.1.4/Cargo.toml
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 mistralrs_cuda-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 mistralrs_cuda-0.1.4/PKG-INFO
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/Cargo.toml` & `mistralrs_cuda-0.1.4/mistralrs-core/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 dirs = "5.0.1"
 hf-hub = "0.3.2"
 thiserror = "1.0.57"
 tokenizers = "0.15.2"
 tqdm = "0.7.0"
 range-checked = { git = "https://github.com/EricLBuehler/range-checked.git", version = "0.1.0" }
 chrono = "0.4.34"
-mistralrs-lora = { version = "0.1.3", path = "../mistralrs-lora" }
+mistralrs-lora = { version = "0.1.4", path = "../mistralrs-lora" }
 minijinja = "1.0.12"
 either.workspace = true
 indexmap.workspace = true
 half = "2.4.0"
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 tracing.workspace = true
@@ -47,14 +47,15 @@
 pyo3.workspace = true
 rayon = "1.10.0"
 tokio.workspace = true
 tokio-rayon = "2.1.0"
 rand_isaac = "0.3.0"
 futures.workspace = true
 indicatif = { version = "0.17.8", features = ["rayon"] }
+async-trait = "0.1.80"
 
 [features]
 cuda = ["candle-core/cuda", "candle-nn/cuda", "candle-transformers/cuda"]
 cudnn = ["candle-core/cudnn"]
 metal = ["candle-core/metal", "candle-nn/metal", "candle-transformers/metal"]
 flash-attn = ["cuda", "candle-transformers/flash-attn", "dep:candle-flash-attn"]
 accelerate = ["candle-core/accelerate", "candle-nn/accelerate", "candle-transformers/accelerate"]
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/aici/bintokens.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/aici/bintokens.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/aici/cfg.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/aici/cfg.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 use anyhow::Result;
 use cfgrammar::{
     yacc::{YaccGrammar, YaccKind},
     Span, Spanned, Symbol, TIdx,
 };
 use lrtable::{from_yacc, Action, Minimiser, StIdx, StateTable};
 use rustc_hash::FxHashMap;
-use std::sync::Arc;
-use std::{cell::RefCell, vec};
+use std::sync::{Arc, RwLock};
+use std::vec;
 use tracing::debug;
 use vob::{vob, Vob};
 
 type StorageT = u32;
 type PStack<StorageT> = Vec<StIdx<StorageT>>; // Parse stack
 
 const LOG_PARSER: bool = false;
@@ -26,23 +26,22 @@
 
 #[derive(Clone)]
 struct CfgStats {
     yacc_actions: usize,
     states_pushed: usize,
 }
 
-#[derive(Clone)]
 pub struct CfgParser {
     grm: Arc<YaccGrammar<StorageT>>,
     stable: Arc<StateTable<StorageT>>,
     lexer: Lexer,
     byte_states: Vec<ByteState>,
     pat_idx_to_tidx: Vec<TIdx<u32>>,
     vobset: VobSet,
-    stats: RefCell<CfgStats>,
+    stats: RwLock<CfgStats>,
     tidx_to_pat_idx: FxHashMap<TIdx<u32>, usize>,
     parse_stacks: Vec<Vec<StIdx<u32>>>,
     skip_patterns: Vob,
     friendly_pattern_names: Vec<String>,
     viable_vobidx_by_state: Vec<VobIdx>,
 }
 
@@ -238,15 +237,15 @@
             pat_idx_to_tidx,
             tidx_to_pat_idx,
             viable_vobidx_by_state,
             skip_patterns,
             friendly_pattern_names,
             parse_stacks,
             vobset,
-            stats: RefCell::new(CfgStats {
+            stats: RwLock::new(CfgStats {
                 yacc_actions: 0,
                 states_pushed: 0,
             }),
         };
 
         cfg.vobset.pre_compute();
 
@@ -369,15 +368,15 @@
         }
         self.parse_stacks[new_idx.0] = pstack;
         new_idx
     }
 
     fn run_parser(&mut self, pat_idx: usize, top: &ByteState, ls: LexerState) -> Option<ByteState> {
         {
-            let mut s = self.stats.borrow_mut();
+            let mut s = self.stats.write().unwrap();
             s.yacc_actions += 1;
         }
 
         let pstack = self.pstack_for(top);
         if self.skip_patterns[pat_idx] {
             let stidx = *pstack.last().unwrap();
             let viable = self.viable_vobidx(stidx);
@@ -406,29 +405,29 @@
     #[allow(dead_code)]
     pub fn viable_now(&self) {
         let v = self.byte_states.last().unwrap().viable;
         self.print_viable("now", self.vobset.resolve(v))
     }
 
     pub fn get_stats(&self) -> String {
-        let mut s = self.stats.borrow_mut();
+        let mut s = self.stats.write().unwrap();
         let r = format!("yacc: {}/{}", s.yacc_actions, s.states_pushed);
         s.yacc_actions = 0;
         s.states_pushed = 0;
         r
     }
 
     fn mk_byte_state(
         &self,
         ls: LexerState,
         pstack: PStackIdx,
         viable: VobIdx,
     ) -> Option<ByteState> {
         {
-            let mut s = self.stats.borrow_mut();
+            let mut s = self.stats.write().unwrap();
             s.states_pushed += 1;
         }
         if self.vobset.and_is_zero(viable, ls.reachable) {
             None
         } else {
             // print!(
             //     " {:?} {:?} ",
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/aici/lex.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/aici/lex.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/aici/recognizer.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/aici/recognizer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/aici/rx.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/aici/rx.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/aici/svob.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/aici/svob.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/aici/toktree.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/aici/toktree.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/device_map.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/device_map.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::fmt::Debug;
 
 use candle_core::{Device, Result, Tensor};
 use candle_nn::VarBuilder;
 use serde::Deserialize;
 use tracing::info;
 
-#[derive(Debug, Default, Deserialize)]
+#[derive(Debug, Default, Deserialize, Clone)]
 pub struct DeviceMapMetadata {
     device_layers: Option<usize>,
     host_layers: Option<usize>,
 }
 
 impl DeviceMapMetadata {
     pub fn from_num_device_layers(device_layers: usize) -> Self {
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/layers.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/layers.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 use std::{ops::Mul, str::FromStr};
 
-use candle_core::{quantized::QTensor, DType, Device, Result, Tensor};
+use candle_core::{quantized::QTensor, DType, Device, IndexOp, Result, Tensor};
 use candle_nn::{
     layer_norm::{RmsNormNonQuantized, RmsNormQuantized},
     Module, VarBuilder,
 };
 
 use crate::models::phi3;
 
@@ -205,18 +205,20 @@
         seqlen_offsets: &[usize],
         position_ids: &[usize],
     ) -> Result<(Tensor, Tensor)> {
         let (_b_sz, _h, seq_len, _n_embd) = q.dims4()?;
         let mut q_embeds = Vec::new();
         let mut k_embeds = Vec::new();
         let (sin, cos) = self.get_long_or_short_sin_cos(position_ids);
-        for offset in seqlen_offsets {
+        for (i, offset) in seqlen_offsets.iter().enumerate() {
             let cos = cos.narrow(0, *offset, seq_len)?;
             let sin = sin.narrow(0, *offset, seq_len)?;
-            let q_embed = candle_nn::rotary_emb::rope(&q.contiguous()?, &cos, &sin)?;
-            let k_embed = candle_nn::rotary_emb::rope(&k.contiguous()?, &cos, &sin)?;
+            let q_embed =
+                candle_nn::rotary_emb::rope(&q.i(i)?.unsqueeze(0)?.contiguous()?, &cos, &sin)?;
+            let k_embed =
+                candle_nn::rotary_emb::rope(&k.i(i)?.unsqueeze(0)?.contiguous()?, &cos, &sin)?;
             q_embeds.push(q_embed);
             k_embeds.push(k_embed);
         }
         Ok((Tensor::cat(&q_embeds, 0)?, Tensor::cat(&k_embeds, 0)?))
     }
 }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/lib.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -64,26 +64,26 @@
     next_request_id: Mutex<RefCell<usize>>,
 }
 
 /// The MistralRsBuilder takes the pipeline and a scheduler method and constructs
 /// an Engine and a MistralRs instance. The Engine runs on a separate thread, and the MistralRs
 /// instance stays on the calling thread.
 pub struct MistralRsBuilder {
-    pipeline: Arc<Mutex<dyn Pipeline>>,
+    pipeline: Arc<tokio::sync::Mutex<dyn Pipeline>>,
     method: SchedulerMethod,
     log: Option<String>,
     truncate_sequence: Option<bool>,
     no_kv_cache: Option<bool>,
     no_prefix_cache: Option<bool>,
     prefix_cache_n: Option<usize>,
     disable_eos_stop: Option<bool>,
 }
 
 impl MistralRsBuilder {
-    pub fn new(pipeline: Arc<Mutex<dyn Pipeline>>, method: SchedulerMethod) -> Self {
+    pub fn new(pipeline: Arc<tokio::sync::Mutex<dyn Pipeline>>, method: SchedulerMethod) -> Self {
         Self {
             pipeline,
             method,
             log: None,
             truncate_sequence: None,
             no_kv_cache: None,
             no_prefix_cache: None,
@@ -148,15 +148,15 @@
         let (tx, rx) = channel(10_000);
         let (isq_tx, isq_rx) = channel(10_000);
 
         let this = Arc::new(Self {
             sender: tx,
             sender_isq: isq_tx,
             log,
-            id: pipeline.lock().unwrap().name(),
+            id: pipeline.try_lock().unwrap().name(),
             creation_time: SystemTime::now()
                 .duration_since(UNIX_EPOCH)
                 .expect("Time travel has occurred!")
                 .as_secs(),
             next_request_id: Mutex::new(RefCell::new(0)),
         });
         thread::spawn(move || {
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/model_loader.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/model_loader.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/model_selected.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/model_selected.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/models/gemma.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/models/gemma.rs`

 * *Files 2% similar despite different names*

```diff
@@ -409,15 +409,15 @@
     }
 
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         let (b_size, seq_len) = input_ids.dims2()?;
         let attention_mask = if seq_len <= 1 {
             None
         } else {
             let mask = self.prepare_decoder_attention_mask(b_size, seq_len, seqlen_offsets[0])?;
             Some(mask)
@@ -449,15 +449,15 @@
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
@@ -469,15 +469,15 @@
         _input_ids_full: &Tensor,
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/models/llama.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/models/llama.rs`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 
 impl Llama {
     pub fn forward(
         &mut self,
         x: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         let mut x = self.wte.forward(x)?;
         let mut cache = self.kv_cache.lock();
         for (block_idx, block) in self.blocks.iter().enumerate() {
             x = self.mapper.map(x, block_idx)?;
             x = block.forward(
                 &x,
@@ -408,15 +408,15 @@
 
 impl NormalModel for Llama {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
@@ -428,15 +428,15 @@
         _input_ids_full: &Tensor,
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &super::Cache {
         &self.kv_cache
     }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/models/mistral.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/models/mistral.rs`

 * *Files 1% similar despite different names*

```diff
@@ -420,15 +420,15 @@
     }
 
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         let (b_size, seq_len) = input_ids.dims2()?;
         if seqlen_offsets.len() > b_size {
             candle_core::bail!("Expected seqlen offsets have length equal to batch size.")
         }
 
         let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
@@ -465,15 +465,15 @@
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
@@ -485,15 +485,15 @@
         _input_ids_full: &Tensor,
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/models/mixtral.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/models/mixtral.rs`

 * *Files 1% similar despite different names*

```diff
@@ -522,15 +522,15 @@
     }
 
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         let (b_size, seq_len) = input_ids.dims2()?;
         let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
         let attention_mask = if seq_len <= 1 {
             None
         } else {
             let mask =
@@ -563,15 +563,15 @@
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
@@ -583,15 +583,15 @@
         _input_ids_full: &Tensor,
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/models/mod.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/models/phi2.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/models/phi2.rs`

 * *Files 2% similar despite different names*

```diff
@@ -383,15 +383,15 @@
     }
 
     pub fn forward(
         &mut self,
         xs: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         let (_b_size, seq_len) = xs.dims2()?;
         let mut xs = xs.apply(&self.embed_tokens)?;
         let mask = if seq_len <= 1 {
             None
         } else {
             Some(get_mask(seq_len, xs.device())?)
@@ -420,15 +420,15 @@
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
@@ -440,15 +440,15 @@
         _input_ids_full: &Tensor,
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/models/phi3.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/models/phi3.rs`

 * *Files 1% similar despite different names*

```diff
@@ -415,15 +415,15 @@
     }
 
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         position_ids: &[usize],
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         let (b_size, seq_len) = input_ids.dims2()?;
         let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
         let attention_mask = if seq_len <= 1 {
             None
         } else {
             let mask = self.prepare_decoder_attention_mask(
@@ -466,30 +466,30 @@
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(input_ids, seqlen_offsets, &position_ids, context_lens)
     }
     fn xlora_forward(
         &mut self,
         _input_ids: &Tensor,
         _input_ids_full: &Tensor,
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/models/quantized_llama.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/models/quantized_llama.rs`

 * *Files 0% similar despite different names*

```diff
@@ -420,15 +420,15 @@
     }
 
     pub fn forward(
         &mut self,
         x: &Tensor,
         start_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         let (_b_sz, seq_len) = x.dims2()?;
         let mask = if seq_len == 1 {
             None
         } else {
             Some(self.mask(seq_len, x.device())?)
         };
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/models/quantized_phi2.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/models/quantized_phi2.rs`

 * *Files 2% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         }
     }
 
     pub fn forward(
         &mut self,
         xs: &Tensor,
         seqlen_offsets: &[usize],
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         let (_b_sz, seq_len) = xs.dims2()?;
         let mask = if seq_len == 1 {
             None
         } else {
             Some(self.mask(seq_len, xs.device())?)
         };
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/models/qwen2.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/models/qwen2.rs`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,15 @@
     }
 
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         let (b_size, seq_len) = input_ids.dims2()?;
         let past_key_values_length = self.calculate_past_kv_len(seq_len)?;
         let attention_mask = if seq_len <= 1 {
             None
         } else {
             let mask =
@@ -431,15 +431,15 @@
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             seqlen_offsets,
             start_offsets_kernel,
             context_lens,
@@ -451,15 +451,15 @@
         _input_ids_full: &Tensor,
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
         _start_offsets_kernel: Tensor,
         _start_offsets_kernel_full: Tensor,
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
     fn cache(&self) -> &Cache {
         &self.cache
     }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/chat_template.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/chat_template.rs`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     gen_conf: Option<GenerationConfig>,
     tokenizer: &Tokenizer,
 ) -> Vec<u32> {
     let mut eos_tok_ids = vec![chat_template.eos_tok()];
     let mut bos_tok_ids = chat_template.bos_tok().map(|b| vec![b]).unwrap_or_default();
 
     for alternate in SUPPORTED_ALTERNATE_EOS {
-        if tokenizer.get_vocab(true).get(alternate).is_some() {
+        if tokenizer.get_vocab(true).contains_key(alternate) {
             eos_tok_ids.push(alternate.to_string())
         }
     }
 
     if let Some(gen_conf) = gen_conf {
         let ids = match gen_conf.eos_token_id {
             Either::Left(id) => vec![id],
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/ggml.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/ggml.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,56 @@
+use super::cache_manager::DefaultCacheManager;
 use super::{
-    calculate_inputs, get_model_paths, get_xlora_paths, Loader, ModelInputs, ModelKind, ModelPaths,
-    Pipeline, TokenSource, XLoraPaths,
+    get_model_paths, get_xlora_paths, CacheManager, GeneralMetadata, Loader, ModelInputs,
+    ModelKind, ModelPaths, Pipeline, TokenSource, XLoraPaths,
 };
 use crate::aici::bintokens::build_tok_trie;
 use crate::aici::toktree::TokTrie;
 use crate::models::Cache;
 use crate::pipeline::chat_template::calculate_eos_tokens;
 use crate::pipeline::{ChatTemplate, SimpleModelPaths};
+use crate::prefix_cacher::PrefixCacheManager;
+use crate::sequence::Sequence;
 use crate::utils::varbuilder_utils::from_mmaped_safetensors;
 use crate::xlora_models::NonGranularState;
-use crate::{deserialize_chat_template, get_paths, DeviceMapMetadata};
+use crate::{deserialize_chat_template, do_sample, get_mut_arcmutex, get_paths, DeviceMapMetadata};
 use crate::{
-    models::quantized_llama::ModelWeights as QLlama, sequence::Sequence, utils::tokens::get_token,
+    models::quantized_llama::ModelWeights as QLlama, utils::tokens::get_token,
     xlora_models::XLoraModelWeights as XLoraQLlama,
 };
 use anyhow::Result;
 use candle_core::quantized::{ggml_file, GgmlDType};
 use candle_core::{DType, Device, Tensor};
 use hf_hub::{api::sync::ApiBuilder, Repo, RepoType};
 use mistralrs_lora::Ordering;
+use rand_isaac::Isaac64Rng;
 use serde_json::Value;
 use std::collections::HashMap;
 use std::fs;
 use std::path::PathBuf;
 use std::str::FromStr;
 use std::sync::Arc;
-use std::sync::Mutex;
 use tokenizers::Tokenizer;
+use tokio::sync::Mutex;
 use tracing::info;
 
 enum Model {
     Llama(QLlama),
     XLoraLlama(XLoraQLlama),
 }
 
 pub struct GGMLPipeline {
     model: Model,
-    config: GGMLSpecificConfig,
     tokenizer: Arc<Tokenizer>,
     tok_trie: Arc<TokTrie>,
     no_kv_cache: bool,
-    chat_template: ChatTemplate,
+    chat_template: Arc<ChatTemplate>,
     model_id: String,
-    eos_tok: Vec<u32>,
     non_granular_state: Option<NonGranularState>,
-    is_lora: bool,
+    metadata: GeneralMetadata,
 }
 
 pub struct GGMLLoader {
     model_id: String,
     config: GGMLSpecificConfig,
     quantized_model_id: Option<String>,
     quantized_filename: Option<String>,
@@ -214,53 +216,51 @@
             kind,
             tgt_non_granular_index,
         }
     }
 }
 
 impl Loader for GGMLLoader {
-    fn download_model(
+    #[allow(clippy::type_complexity, clippy::too_many_arguments)]
+    fn load_model(
         &self,
         revision: Option<String>,
         token_source: TokenSource,
+        _dtype: Option<DType>,
+        device: &Device,
         silent: bool,
-    ) -> Result<Box<dyn ModelPaths>> {
-        get_paths!(
+        mapper: DeviceMapMetadata,
+        in_situ_quant: Option<GgmlDType>,
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
+        let paths: anyhow::Result<Box<dyn ModelPaths>> = get_paths!(
             SimpleModelPaths,
             &token_source,
             revision,
             self,
             self.quantized_model_id,
             self.quantized_filename,
             silent
-        )
-    }
+        );
+        let paths = paths?;
 
-    fn _setup_model(
-        &self,
-        paths: &dyn ModelPaths,
-        _dtype: Option<DType>,
-        device: &Device,
-        silent: bool,
-        mapper: DeviceMapMetadata,
-        in_situ_quant: Option<GgmlDType>,
-    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
         if in_situ_quant.is_some() {
             anyhow::bail!(
                 "You are trying to in-situ quantize a GGUF model. This will not do anything."
             );
         }
         if !mapper.is_dummy() {
             info!("⚠️ WARNING: GGML models do not support device mapping. Device mapping will not work. Please consider using a GGUF model.");
         }
 
         let mut file = std::fs::File::open(paths.get_weight_filenames().first().unwrap())?;
         let model = ggml_file::Content::read(&mut file, device)
             .map_err(|e| e.with_path(paths.get_weight_filenames().first().unwrap()))?;
 
+        info!("Model config: {:?}", model.hparams);
+
         let mut is_lora = false;
         let model = match self.kind {
             ModelKind::QuantizedGGML => Model::Llama(QLlama::from_ggml(model, self.config.gqa)?),
             ModelKind::XLoraGGML => {
                 let vb = from_mmaped_safetensors(
                     vec![paths.get_classifier_path().as_ref().unwrap().to_path_buf()],
                     paths
@@ -313,65 +313,80 @@
         };
 
         let tokenizer =
             Tokenizer::from_file(paths.get_tokenizer_filename()).map_err(anyhow::Error::msg)?;
 
         let (chat_template, gen_conf) = deserialize_chat_template!(paths, self);
 
+        let max_seq_len = match model {
+            Model::Llama(ref l) => l.max_seq_len,
+            Model::XLoraLlama(ref xl) => xl.max_seq_len,
+        };
+        let tok_trie: Arc<TokTrie> = build_tok_trie(tokenizer.clone()).into();
+        let is_xlora = match &model {
+            Model::Llama(_) => false,
+            Model::XLoraLlama(_) => !is_lora,
+        };
+        let num_hidden_layers = match model {
+            Model::Llama(ref model) => model.cache.lock().len(),
+            Model::XLoraLlama(ref model) => model.cache.lock().len(),
+        };
+        let eos = calculate_eos_tokens(&chat_template, gen_conf, &tokenizer);
         Ok(Arc::new(Mutex::new(GGMLPipeline {
             model,
-            config: self.config,
-            eos_tok: calculate_eos_tokens(&chat_template, gen_conf, &tokenizer),
-            tok_trie: build_tok_trie(tokenizer.clone()).into(),
+            tok_trie: tok_trie.clone(),
             tokenizer: tokenizer.into(),
             no_kv_cache: self.no_kv_cache,
-            chat_template,
+            chat_template: Arc::new(chat_template),
             model_id: self.model_id.clone(),
             non_granular_state: self.tgt_non_granular_index.map(|tgt_non_granular_index| {
                 NonGranularState {
                     non_granular_index: Arc::new(Mutex::new(0)),
                     tgt_non_granular_index,
                 }
             }),
-            is_lora,
+            metadata: GeneralMetadata {
+                max_seq_len,
+                repeat_last_n: self.config.repeat_last_n,
+                tok_trie,
+                has_no_kv_cache: self.no_kv_cache,
+                is_xlora,
+                num_hidden_layers,
+                eos_tok: eos,
+            },
         })))
     }
 
-    fn get_id(&self) -> &str {
-        self.xlora_model_id.as_deref().unwrap_or(&self.model_id)
+    fn get_id(&self) -> String {
+        self.xlora_model_id
+            .as_deref()
+            .unwrap_or(&self.model_id)
+            .to_string()
     }
 
     fn get_kind(&self) -> ModelKind {
-        self.kind
+        self.kind.clone()
     }
 }
 
+#[async_trait::async_trait]
 impl Pipeline for GGMLPipeline {
-    fn forward(
+    fn forward_inputs(
         &mut self,
-        input_toks: &[&mut Sequence],
-        is_prompt: bool,
-    ) -> Result<Tensor, candle_core::Error> {
-        let ModelInputs {
+        ModelInputs {
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             seqlen_offsets_kernel,
             seqlen_offsets_kernel_full,
             context_lens,
             position_ids: _, // NOTE(EricLBuehler): ignore, it is for phi3
-        } = calculate_inputs(
-            input_toks,
-            is_prompt,
-            self.is_xlora(),
-            self.device(),
-            self.no_kv_cache,
-        )
-        .unwrap();
+        }: ModelInputs,
+    ) -> Result<Tensor, candle_core::Error> {
         match self.model {
             Model::Llama(ref mut model) => model.forward(
                 &input_ids,
                 &seqlen_offsets,
                 seqlen_offsets_kernel,
                 context_lens,
             ),
@@ -384,64 +399,65 @@
                 seqlen_offsets_kernel_full.unwrap_or(seqlen_offsets_kernel),
                 self.no_kv_cache,
                 &self.non_granular_state,
                 context_lens,
             ),
         }
     }
-    fn device(&self) -> &Device {
-        match self.model {
-            Model::Llama(ref model) => &model.device,
-            Model::XLoraLlama(ref model) => &model.device,
-        }
-    }
-    fn num_hidden_layers(&self) -> usize {
-        self.cache().lock().len()
+    async fn sample(
+        &self,
+        seqs: &mut [&mut Sequence],
+        logits: Tensor,
+        prefix_cacher: &mut PrefixCacheManager,
+        disable_eos_stop: bool,
+        rng: Arc<std::sync::Mutex<Isaac64Rng>>,
+    ) -> Result<(), candle_core::Error> {
+        do_sample!(self, seqs, logits, prefix_cacher, disable_eos_stop, rng)
     }
-    fn cache(&self) -> &Cache {
+    fn device(&self) -> Device {
         match self.model {
-            Model::Llama(ref model) => &model.cache,
-            Model::XLoraLlama(ref model) => &model.cache,
+            Model::Llama(ref model) => model.device.clone(),
+            Model::XLoraLlama(ref model) => model.device.clone(),
         }
     }
-    fn get_repeat_last_n(&self) -> usize {
-        self.config.repeat_last_n
-    }
     fn tokenizer(&self) -> Arc<Tokenizer> {
         self.tokenizer.clone()
     }
-    fn eos_tok(&self) -> &[u32] {
-        &self.eos_tok
-    }
     fn name(&self) -> String {
         self.model_id.clone()
     }
-    fn get_max_seq_len(&self) -> usize {
-        match &self.model {
-            Model::Llama(model) => model.max_seq_len,
-            Model::XLoraLlama(model) => model.max_seq_len,
-        }
+    fn get_chat_template(&self) -> Arc<ChatTemplate> {
+        self.chat_template.clone()
     }
-    fn is_xlora(&self) -> bool {
-        match &self.model {
-            Model::Llama(_) => false,
-            Model::XLoraLlama(_) => !self.is_lora,
+    fn reset_non_granular_state(&self) {
+        if let Some(s) = self.non_granular_state.as_ref() {
+            *self.cache().get_scalings_cache() = None;
+            *get_mut_arcmutex!(s.non_granular_index) = 0;
         }
     }
-    fn has_no_kv_cache(&self) -> bool {
-        self.no_kv_cache
+    fn re_isq_model(&mut self, _dtype: GgmlDType) -> Result<()> {
+        anyhow::bail!(
+            "You are trying to in-situ requantize a GGML model. This will not do anything."
+        )
+    }
+    fn get_metadata(&self) -> &GeneralMetadata {
+        &self.metadata
     }
-    fn get_chat_template(&self) -> &ChatTemplate {
-        &self.chat_template
+    fn clone_in_cache(&mut self, seqs: &mut [&mut Sequence]) {
+        DefaultCacheManager.clone_in_cache(self, seqs)
     }
-    fn get_non_granular_state(&self) -> &Option<NonGranularState> {
-        &None
+    fn clone_out_cache(&mut self, seqs: &mut [&mut Sequence]) {
+        DefaultCacheManager.clone_out_cache(self, seqs)
     }
-    fn tok_trie(&self) -> Arc<TokTrie> {
-        self.tok_trie.clone()
+    fn set_none_cache(&mut self, reset_non_granular: bool) {
+        DefaultCacheManager.set_none_cache(self);
+        if reset_non_granular {
+            self.reset_non_granular_state()
+        }
     }
-    fn re_isq_model(&mut self, _dtype: GgmlDType) -> Result<()> {
-        anyhow::bail!(
-            "You are trying to in-situ requantize a GGUF model. This will not do anything."
-        )
+    fn cache(&self) -> &Cache {
+        match self.model {
+            Model::Llama(ref model) => &model.cache,
+            Model::XLoraLlama(ref model) => &model.cache,
+        }
     }
 }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/gguf.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/normal.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,104 @@
+use super::cache_manager::DefaultCacheManager;
+use super::loaders::{
+    GemmaLoader, LlamaLoader, MistralLoader, MixtralLoader, NormalLoaderType, Phi2Loader,
+    Phi3Loader, Qwen2Loader,
+};
 use super::{
-    calculate_inputs, get_model_paths, get_xlora_paths, Loader, ModelInputs, ModelKind, ModelPaths,
-    Pipeline, TokenSource, XLoraPaths,
+    get_model_paths, get_xlora_paths, CacheManager, GeneralMetadata, Loader, ModelInputs,
+    ModelKind, ModelPaths, NormalModel, NormalModelLoader, Pipeline, TokenSource, XLoraPaths,
 };
 use crate::aici::bintokens::build_tok_trie;
 use crate::aici::toktree::TokTrie;
 use crate::models::Cache;
 use crate::pipeline::chat_template::calculate_eos_tokens;
 use crate::pipeline::{ChatTemplate, SimpleModelPaths};
-use crate::utils::varbuilder_utils::from_mmaped_safetensors;
+use crate::prefix_cacher::PrefixCacheManager;
+use crate::sequence::Sequence;
+use crate::utils::{tokens::get_token, varbuilder_utils::from_mmaped_safetensors};
 use crate::xlora_models::NonGranularState;
-use crate::{deserialize_chat_template, get_paths, DeviceMapMetadata};
 use crate::{
-    models::quantized_llama::ModelWeights as QLlama, models::quantized_phi2::ModelWeights as QPhi,
-    sequence::Sequence, utils::tokens::get_token, xlora_models::XLoraModelWeights as XLoraQLlama,
+    deserialize_chat_template, do_sample, get_mut_arcmutex, get_paths, lora_model_loader,
+    normal_model_loader, xlora_model_loader, DeviceMapMetadata,
 };
-use anyhow::{bail, Result};
-use candle_core::quantized::{gguf_file, GgmlDType};
+use anyhow::Result;
+use candle_core::quantized::GgmlDType;
 use candle_core::{DType, Device, Tensor};
 use hf_hub::{api::sync::ApiBuilder, Repo, RepoType};
 use mistralrs_lora::Ordering;
+use rand_isaac::Isaac64Rng;
 use serde_json::Value;
 use std::collections::HashMap;
 use std::fs;
 use std::path::PathBuf;
 use std::str::FromStr;
 use std::sync::Arc;
-use std::sync::Mutex;
 use tokenizers::Tokenizer;
+use tokio::sync::Mutex;
 use tracing::info;
 
-enum Model {
-    Llama(QLlama),
-    Phi2(QPhi),
-    XLoraLlama(XLoraQLlama),
-}
-
-pub struct GGUFPipeline {
-    model: Model,
-    config: GGUFSpecificConfig,
+pub struct NormalPipeline {
+    model: Box<dyn NormalModel + Send + Sync>,
     tokenizer: Arc<Tokenizer>,
     tok_trie: Arc<TokTrie>,
     no_kv_cache: bool,
-    chat_template: ChatTemplate,
-    model_id: String,
-    eos_tok: Vec<u32>,
+    chat_template: Arc<ChatTemplate>,
     non_granular_state: Option<NonGranularState>,
-    is_lora: bool,
+    model_id: String,
+    metadata: GeneralMetadata,
 }
 
-pub struct GGUFLoader {
+/// A loader for a "normal" (non-quantized) model.
+pub struct NormalLoader {
+    inner: Box<dyn NormalModelLoader>,
     model_id: String,
-    config: GGUFSpecificConfig,
-    quantized_model_id: Option<String>,
-    quantized_filename: Option<String>,
+    config: NormalSpecificConfig,
     xlora_model_id: Option<String>,
+    kind: ModelKind,
     xlora_order: Option<Ordering>,
     no_kv_cache: bool,
     chat_template: Option<String>,
     tokenizer_json: Option<String>,
-    kind: ModelKind,
     tgt_non_granular_index: Option<usize>,
 }
 
-#[derive(Debug)]
-enum GGUFArchitecture {
-    Llama,
-    Mpt,
-    Gptneox,
-    Gptj,
-    Gpt2,
-    Bloom,
-    Falcon,
-    Mamba,
-    Rwkv,
-    Phi2,
-}
-
-impl FromStr for GGUFArchitecture {
-    type Err = String;
-
-    fn from_str(s: &str) -> Result<Self, Self::Err> {
-        match s {
-            "llama" => Ok(GGUFArchitecture::Llama),
-            "mpt" => Ok(GGUFArchitecture::Mpt),
-            "gptneox" => Ok(GGUFArchitecture::Gptneox),
-            "gptj" => Ok(GGUFArchitecture::Gptj),
-            "gpt2" => Ok(GGUFArchitecture::Gpt2),
-            "bloom" => Ok(GGUFArchitecture::Bloom),
-            "falcon" => Ok(GGUFArchitecture::Falcon),
-            "mamba" => Ok(GGUFArchitecture::Mamba),
-            "rwkv" => Ok(GGUFArchitecture::Rwkv),
-            "phi2" => Ok(GGUFArchitecture::Phi2),
-            a => Err(format!("Unknown GGUF architecture `{a}`")),
-        }
-    }
-}
-
-#[derive(Clone, Copy, Default)]
-/// A config for a GGUF loader.
-pub struct GGUFSpecificConfig {
-    pub repeat_last_n: usize,
-}
-
 #[derive(Default)]
-/// A builder for a GGUF loader.
-pub struct GGUFLoaderBuilder {
+/// A builder for a loader for a "normal" (non-quantized) model.
+pub struct NormalLoaderBuilder {
     model_id: Option<String>,
-    config: GGUFSpecificConfig,
-    quantized_model_id: String,
-    quantized_filename: String,
+    config: NormalSpecificConfig,
     xlora_model_id: Option<String>,
     kind: ModelKind,
     xlora_order: Option<Ordering>,
     no_kv_cache: bool,
     chat_template: Option<String>,
     tokenizer_json: Option<String>,
     tgt_non_granular_index: Option<usize>,
 }
 
-impl GGUFLoaderBuilder {
+#[derive(Clone, Copy, Default)]
+/// Config specific to loading a normal model.
+pub struct NormalSpecificConfig {
+    pub use_flash_attn: bool,
+    pub repeat_last_n: usize,
+}
+
+impl NormalLoaderBuilder {
     pub fn new(
-        config: GGUFSpecificConfig,
+        config: NormalSpecificConfig,
         chat_template: Option<String>,
         tokenizer_json: Option<String>,
         model_id: Option<String>,
-        quantized_model_id: String,
-        quantized_filename: String,
     ) -> Self {
         Self {
             config,
             chat_template,
             tokenizer_json,
             model_id,
-            kind: ModelKind::QuantizedGGUF,
-            quantized_filename,
-            quantized_model_id,
+            kind: ModelKind::Normal,
             ..Default::default()
         }
     }
 
     fn with_adapter(
         mut self,
         xlora_model_id: String,
@@ -165,15 +125,15 @@
     pub fn with_xlora(
         mut self,
         xlora_model_id: String,
         xlora_order: Ordering,
         no_kv_cache: bool,
         tgt_non_granular_index: Option<usize>,
     ) -> Self {
-        self.kind = ModelKind::XLoraGGUF;
+        self.kind = ModelKind::XLoraNormal;
         self.with_adapter(
             xlora_model_id,
             xlora_order,
             no_kv_cache,
             tgt_non_granular_index,
         )
     }
@@ -181,324 +141,282 @@
     pub fn with_lora(
         mut self,
         xlora_model_id: String,
         xlora_order: Ordering,
         no_kv_cache: bool,
         tgt_non_granular_index: Option<usize>,
     ) -> Self {
-        self.kind = ModelKind::LoraGGUF;
+        self.kind = ModelKind::LoraNormal;
         self.with_adapter(
             xlora_model_id,
             xlora_order,
             no_kv_cache,
             tgt_non_granular_index,
         )
     }
 
-    pub fn build(self) -> Box<dyn Loader> {
-        Box::new(GGUFLoader {
+    pub fn build(self, loader: NormalLoaderType) -> Box<dyn Loader> {
+        let loader: Box<dyn NormalModelLoader> = match loader {
+            NormalLoaderType::Mistral => Box::new(MistralLoader),
+            NormalLoaderType::Gemma => Box::new(GemmaLoader),
+            NormalLoaderType::Llama => Box::new(LlamaLoader),
+            NormalLoaderType::Mixtral => Box::new(MixtralLoader),
+            NormalLoaderType::Phi2 => Box::new(Phi2Loader),
+            NormalLoaderType::Phi3 => Box::new(Phi3Loader),
+            NormalLoaderType::Qwen2 => Box::new(Qwen2Loader),
+        };
+        Box::new(NormalLoader {
+            inner: loader,
             model_id: self.model_id.unwrap(),
             config: self.config,
             xlora_model_id: self.xlora_model_id,
             kind: self.kind,
             xlora_order: self.xlora_order,
             no_kv_cache: self.no_kv_cache,
             chat_template: self.chat_template,
             tokenizer_json: self.tokenizer_json,
             tgt_non_granular_index: self.tgt_non_granular_index,
-            quantized_filename: Some(self.quantized_filename),
-            quantized_model_id: Some(self.quantized_model_id),
         })
     }
 }
 
-impl GGUFLoader {
-    #[allow(clippy::too_many_arguments)]
-    pub fn new(
-        model_id: Option<String>,
-        config: GGUFSpecificConfig,
-        quantized_model_id: Option<String>,
-        quantized_filename: Option<String>,
-        xlora_model_id: Option<String>,
-        kind: ModelKind,
-        xlora_order: Option<Ordering>,
-        no_kv_cache: bool,
-        chat_template: Option<String>,
-        tokenizer_json: Option<String>,
-        tgt_non_granular_index: Option<usize>,
-    ) -> Self {
-        let model_id = if let Some(id) = model_id {
-            id
-        } else {
-            info!(
-                "Using adapter base model ID: `{}`",
-                xlora_order.as_ref().unwrap().base_model_id
-            );
-            xlora_order.as_ref().unwrap().base_model_id.clone()
-        };
-        Self {
-            model_id,
-            config,
-            quantized_model_id,
-            quantized_filename,
-            xlora_model_id,
-            xlora_order,
-            no_kv_cache,
-            chat_template,
-            tokenizer_json,
-            kind,
-            tgt_non_granular_index,
-        }
-    }
-}
-
-impl Loader for GGUFLoader {
-    fn download_model(
+impl Loader for NormalLoader {
+    #[allow(clippy::type_complexity, clippy::too_many_arguments)]
+    fn load_model(
         &self,
         revision: Option<String>,
         token_source: TokenSource,
+        dtype: Option<DType>,
+        device: &Device,
         silent: bool,
-    ) -> Result<Box<dyn ModelPaths>> {
-        get_paths!(
+        mapper: DeviceMapMetadata,
+        in_situ_quant: Option<GgmlDType>,
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
+        let paths: anyhow::Result<Box<dyn ModelPaths>> = get_paths!(
             SimpleModelPaths,
             &token_source,
             revision,
             self,
-            self.quantized_model_id,
-            self.quantized_filename,
+            None,
+            None,
             silent
-        )
-    }
+        );
+        let paths = paths?;
 
-    fn _setup_model(
-        &self,
-        paths: &dyn ModelPaths,
-        _dtype: Option<DType>,
-        device: &Device,
-        silent: bool,
-        mapper: DeviceMapMetadata,
-        in_situ_quant: Option<GgmlDType>,
-    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
-        if in_situ_quant.is_some() {
-            anyhow::bail!(
-                "You are trying to in-situ quantize a GGUF model. This will not do anything."
-            );
-        }
-        let mut file = std::fs::File::open(paths.get_weight_filenames().first().unwrap())?;
-        let model = gguf_file::Content::read(&mut file)
-            .map_err(|e| e.with_path(paths.get_weight_filenames().first().unwrap()))?;
-        let arch: GGUFArchitecture = model.metadata["general.architecture"]
-            .to_string()
-            .unwrap()
-            .parse()
-            .map_err(anyhow::Error::msg)?;
+        let config = std::fs::read_to_string(paths.get_config_filename())?;
+        let default_dtype = if device.is_cuda() && mapper.is_dummy() {
+            DType::BF16
+        } else if !mapper.is_dummy() {
+            DType::F16
+        } else {
+            DType::F32
+        };
 
-        let mut is_lora = false;
-        let model = match self.kind {
-            ModelKind::QuantizedGGUF => match arch {
-                GGUFArchitecture::Llama => {
-                    Model::Llama(QLlama::from_gguf(model, &mut file, device, mapper)?)
-                }
-                GGUFArchitecture::Phi2 => {
-                    Model::Phi2(QPhi::from_gguf(model, &mut file, device, mapper)?)
-                }
-                a => bail!("Unsupported architecture `{a:?}`"),
-            },
-            ModelKind::XLoraGGUF => {
-                let vb = from_mmaped_safetensors(
-                    vec![paths.get_classifier_path().as_ref().unwrap().to_path_buf()],
-                    paths
-                        .get_adapter_filenames()
-                        .as_ref()
-                        .unwrap()
-                        .iter()
-                        .map(|(_, x)| (*x).to_owned())
-                        .collect::<Vec<_>>(),
-                    DType::F32,
-                    device,
-                    silent,
-                )?;
+        info!(
+            "Model config: {:?}",
+            self.inner
+                .get_config_repr(&config, self.config.use_flash_attn)?
+        );
 
-                match arch {
-                    GGUFArchitecture::Llama => Model::XLoraLlama(XLoraQLlama::from_gguf(
-                        model,
-                        &mut file,
-                        device,
-                        paths.get_adapter_configs().as_ref().unwrap(),
-                        &vb,
-                        paths.get_ordering().as_ref().unwrap(),
-                        Some(paths.get_classifier_config().as_ref().unwrap().clone()),
-                        mapper,
-                    )?),
-                    a => bail!("Unsupported architecture for GGUF X-LoRA `{a:?}`"),
-                }
-            }
-            ModelKind::LoraGGUF => {
+        let load_device = if in_situ_quant.is_none() {
+            device.clone()
+        } else {
+            Device::Cpu
+        };
+
+        let mut is_lora = false;
+        let mut model = match self.kind {
+            ModelKind::QuantizedGGUF => unreachable!(),
+            ModelKind::QuantizedGGML => unreachable!(),
+            ModelKind::Normal => normal_model_loader!(
+                paths,
+                dtype,
+                default_dtype,
+                &load_device,
+                config,
+                self.inner,
+                self.config.use_flash_attn,
+                silent,
+                mapper,
+                in_situ_quant.is_some(),
+                device.clone()
+            ),
+            ModelKind::XLoraNormal => xlora_model_loader!(
+                paths,
+                dtype,
+                default_dtype,
+                &load_device,
+                config,
+                self.inner,
+                self.config.use_flash_attn,
+                silent,
+                mapper,
+                in_situ_quant.is_some(),
+                device.clone()
+            ),
+            ModelKind::LoraNormal => {
                 is_lora = true;
-                let vb = from_mmaped_safetensors(
-                    vec![],
-                    paths
-                        .get_adapter_filenames()
-                        .as_ref()
-                        .unwrap()
-                        .iter()
-                        .map(|(_, x)| (*x).to_owned())
-                        .collect::<Vec<_>>(),
-                    DType::F32,
-                    device,
+                lora_model_loader!(
+                    paths,
+                    dtype,
+                    default_dtype,
+                    &load_device,
+                    config,
+                    self.inner,
+                    self.config.use_flash_attn,
                     silent,
-                )?;
-
-                match arch {
-                    GGUFArchitecture::Llama => Model::XLoraLlama(XLoraQLlama::from_gguf(
-                        model,
-                        &mut file,
-                        device,
-                        paths.get_adapter_configs().as_ref().unwrap(),
-                        &vb,
-                        paths.get_ordering().as_ref().unwrap(),
-                        None,
-                        mapper,
-                    )?),
-                    a => bail!("Unsupported architecture for GGUF X-LoRA `{a:?}`"),
-                }
+                    mapper,
+                    in_situ_quant.is_some(),
+                    device.clone()
+                )
             }
-            _ => unreachable!(),
+            ModelKind::XLoraGGUF => unreachable!(),
+            ModelKind::XLoraGGML => unreachable!(),
+            ModelKind::LoraGGUF => unreachable!(),
+            ModelKind::LoraGGML => unreachable!(),
+            ModelKind::Speculative {
+                target: _,
+                draft: _,
+            } => unreachable!(),
         };
 
         let tokenizer =
             Tokenizer::from_file(paths.get_tokenizer_filename()).map_err(anyhow::Error::msg)?;
 
         let (chat_template, gen_conf) = deserialize_chat_template!(paths, self);
 
-        Ok(Arc::new(Mutex::new(GGUFPipeline {
+        if let Some(in_situ_quant) = in_situ_quant {
+            model.quantize(in_situ_quant, device.clone())?;
+        }
+
+        let max_seq_len = model.max_seq_len();
+        let tok_trie: Arc<TokTrie> = build_tok_trie(tokenizer.clone()).into();
+        let is_xlora = model.is_xlora() && !is_lora;
+        let num_hidden_layers = model.cache().lock().len();
+        let eos = calculate_eos_tokens(&chat_template, gen_conf, &tokenizer);
+        Ok(Arc::new(Mutex::new(NormalPipeline {
             model,
-            config: self.config,
-            eos_tok: calculate_eos_tokens(&chat_template, gen_conf, &tokenizer),
-            tok_trie: build_tok_trie(tokenizer.clone()).into(),
+            tok_trie: tok_trie.clone(),
             tokenizer: tokenizer.into(),
             no_kv_cache: self.no_kv_cache,
-            chat_template,
-            model_id: self.model_id.clone(),
+            chat_template: Arc::new(chat_template),
             non_granular_state: self.tgt_non_granular_index.map(|tgt_non_granular_index| {
                 NonGranularState {
                     non_granular_index: Arc::new(Mutex::new(0)),
                     tgt_non_granular_index,
                 }
             }),
-            is_lora,
+            model_id: self.model_id.clone(),
+            metadata: GeneralMetadata {
+                max_seq_len,
+                repeat_last_n: self.config.repeat_last_n,
+                tok_trie,
+                has_no_kv_cache: self.no_kv_cache,
+                is_xlora,
+                num_hidden_layers,
+                eos_tok: eos,
+            },
         })))
     }
 
-    fn get_id(&self) -> &str {
-        self.xlora_model_id.as_deref().unwrap_or(&self.model_id)
+    fn get_id(&self) -> String {
+        self.xlora_model_id
+            .as_deref()
+            .unwrap_or(&self.model_id)
+            .to_string()
     }
 
     fn get_kind(&self) -> ModelKind {
-        self.kind
+        self.kind.clone()
     }
 }
 
-impl Pipeline for GGUFPipeline {
-    fn forward(
+#[async_trait::async_trait]
+impl Pipeline for NormalPipeline {
+    fn forward_inputs(
         &mut self,
-        input_toks: &[&mut Sequence],
-        is_prompt: bool,
-    ) -> Result<Tensor, candle_core::Error> {
-        let ModelInputs {
+        ModelInputs {
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
             seqlen_offsets_kernel,
             seqlen_offsets_kernel_full,
             context_lens,
-            position_ids: _, // NOTE(EricLBuehler): ignore, it is for phi3
-        } = calculate_inputs(
-            input_toks,
-            is_prompt,
-            self.is_xlora(),
-            self.device(),
-            self.no_kv_cache,
-        )
-        .unwrap();
-        match self.model {
-            Model::Llama(ref mut model) => model.forward(
+            position_ids,
+        }: ModelInputs,
+    ) -> Result<Tensor, candle_core::Error> {
+        match self.model.is_xlora() {
+            false => self.model.forward(
                 &input_ids,
                 &seqlen_offsets,
                 seqlen_offsets_kernel,
                 context_lens,
+                position_ids,
             ),
-            Model::Phi2(ref mut model) => model.forward(&input_ids, &seqlen_offsets, context_lens),
-            Model::XLoraLlama(ref mut model) => model.forward(
+            true => self.model.xlora_forward(
                 &input_ids,
                 input_ids_full.as_ref().unwrap_or(&input_ids),
                 &seqlen_offsets,
                 seqlen_offsets_full.as_ref().unwrap_or(&seqlen_offsets),
                 seqlen_offsets_kernel.clone(),
                 seqlen_offsets_kernel_full.unwrap_or(seqlen_offsets_kernel),
                 self.no_kv_cache,
                 &self.non_granular_state,
                 context_lens,
+                position_ids,
             ),
         }
     }
-    fn device(&self) -> &Device {
-        match self.model {
-            Model::Llama(ref model) => &model.device,
-            Model::Phi2(ref model) => &model.device,
-            Model::XLoraLlama(ref model) => &model.device,
-        }
-    }
-    fn num_hidden_layers(&self) -> usize {
-        self.cache().lock().len()
-    }
-    fn cache(&self) -> &Cache {
-        match self.model {
-            Model::Llama(ref model) => &model.cache,
-            Model::Phi2(ref model) => &model.cache,
-            Model::XLoraLlama(ref model) => &model.cache,
-        }
+    async fn sample(
+        &self,
+        seqs: &mut [&mut Sequence],
+        logits: Tensor,
+        prefix_cacher: &mut PrefixCacheManager,
+        disable_eos_stop: bool,
+        rng: Arc<std::sync::Mutex<Isaac64Rng>>,
+    ) -> Result<(), candle_core::Error> {
+        do_sample!(self, seqs, logits, prefix_cacher, disable_eos_stop, rng)
     }
-    fn get_repeat_last_n(&self) -> usize {
-        self.config.repeat_last_n
+    fn device(&self) -> Device {
+        self.model.device().clone()
     }
     fn tokenizer(&self) -> Arc<Tokenizer> {
         self.tokenizer.clone()
     }
-    fn eos_tok(&self) -> &[u32] {
-        &self.eos_tok
-    }
     fn name(&self) -> String {
         self.model_id.clone()
     }
-    fn get_max_seq_len(&self) -> usize {
-        match &self.model {
-            Model::Llama(model) => model.max_seq_len,
-            Model::Phi2(model) => model.max_seq_len,
-            Model::XLoraLlama(model) => model.max_seq_len,
-        }
+    fn get_chat_template(&self) -> Arc<ChatTemplate> {
+        self.chat_template.clone()
     }
-    fn is_xlora(&self) -> bool {
-        match &self.model {
-            Model::Llama(_) | Model::Phi2(_) => false,
-            Model::XLoraLlama(_) => !self.is_lora,
+    fn reset_non_granular_state(&self) {
+        if let Some(s) = self.non_granular_state.as_ref() {
+            *self.cache().get_scalings_cache() = None;
+            *get_mut_arcmutex!(s.non_granular_index) = 0;
         }
     }
-    fn has_no_kv_cache(&self) -> bool {
-        self.no_kv_cache
-    }
-    fn get_chat_template(&self) -> &ChatTemplate {
-        &self.chat_template
-    }
-    fn get_non_granular_state(&self) -> &Option<NonGranularState> {
-        &None
-    }
-    fn tok_trie(&self) -> Arc<TokTrie> {
-        self.tok_trie.clone()
+    fn re_isq_model(&mut self, dtype: GgmlDType) -> Result<()> {
+        let device = self.device().clone();
+        self.model
+            .quantize(dtype, device)
+            .map_err(anyhow::Error::msg)
+    }
+    fn get_metadata(&self) -> &GeneralMetadata {
+        &self.metadata
+    }
+    fn clone_in_cache(&mut self, seqs: &mut [&mut Sequence]) {
+        DefaultCacheManager.clone_in_cache(self, seqs)
+    }
+    fn clone_out_cache(&mut self, seqs: &mut [&mut Sequence]) {
+        DefaultCacheManager.clone_out_cache(self, seqs)
+    }
+    fn set_none_cache(&mut self, reset_non_granular: bool) {
+        DefaultCacheManager.set_none_cache(self);
+        if reset_non_granular {
+            self.reset_non_granular_state()
+        }
     }
-    fn re_isq_model(&mut self, _dtype: GgmlDType) -> Result<()> {
-        anyhow::bail!(
-            "You are trying to in-situ requantize a GGML model. This will not do anything."
-        )
+    fn cache(&self) -> &Cache {
+        self.model.cache()
     }
 }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/loaders.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/loaders.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::{collections::HashMap, str::FromStr};
+use std::{collections::HashMap, fmt::Debug, str::FromStr};
 
 use anyhow::Result;
 use candle_core::Device;
 use candle_nn::{Activation, VarBuilder};
 use either::Either;
 use mistralrs_lora::{LoraConfig, Ordering};
 use pyo3::pyclass;
@@ -42,15 +42,15 @@
             a => Err(format!("Unknown architecture `{a}`")),
         }
     }
 }
 
 // ======================== Mistral loader
 
-#[derive(Deserialize)]
+#[derive(Deserialize, Debug)]
 struct MistralBasicConfig {
     vocab_size: usize,
     hidden_size: usize,
     intermediate_size: usize,
     num_hidden_layers: usize,
     num_attention_heads: usize,
     num_key_value_heads: usize,
@@ -125,14 +125,20 @@
             loading_isq,
             device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
+    fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
+        Ok(Box::new(MistralBasicConfig::deserialize(
+            config,
+            use_flash_attn,
+        )?))
+    }
 }
 
 // ======================== Gemma loader
 
 fn default_max_position_embeddings() -> usize {
     4096
 }
@@ -223,14 +229,20 @@
             loading_isq,
             device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
+    fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
+        Ok(Box::new(GemmaBasicConfig::deserialize(
+            config,
+            use_flash_attn,
+        )?))
+    }
 }
 
 // ======================== Llama loader
 
 #[derive(Deserialize)]
 struct LlamaBasicConfig {
     hidden_size: usize,
@@ -313,14 +325,20 @@
             loading_isq,
             device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
+    fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
+        Ok(Box::new(LlamaBasicConfig::deserialize(
+            config,
+            use_flash_attn,
+        )?))
+    }
 }
 
 // ======================== Mixtral loader
 
 #[derive(Deserialize)]
 struct MixtralBasicConfig {
     vocab_size: usize,
@@ -404,14 +422,20 @@
             loading_isq,
             device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
+    fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
+        Ok(Box::new(MixtralBasicConfig::deserialize(
+            config,
+            use_flash_attn,
+        )?))
+    }
 }
 
 // ======================== Phi2 loader
 
 #[derive(Deserialize)]
 struct Phi2BasicConfig {
     vocab_size: usize,
@@ -495,14 +519,20 @@
             loading_isq,
             device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
+    fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
+        Ok(Box::new(Phi2BasicConfig::deserialize(
+            config,
+            use_flash_attn,
+        )?))
+    }
 }
 
 // ======================== Phi3 loader
 
 #[derive(Deserialize)]
 struct RopeScaling(#[serde(with = "either::serde_untagged")] Either<Vec<f32>, String>);
 
@@ -597,14 +627,20 @@
             loading_isq,
             device,
         )?))
     }
     fn is_gptx(&self) -> bool {
         true
     }
+    fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
+        Ok(Box::new(Phi3BasicConfig::deserialize(
+            config,
+            use_flash_attn,
+        )?))
+    }
 }
 
 // ======================== Qwen2 loader
 
 #[derive(Deserialize)]
 struct Qwen2BasicConfig {
     vocab_size: usize,
@@ -680,8 +716,14 @@
         _device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>> {
         todo!()
     }
     fn is_gptx(&self) -> bool {
         true
     }
+    fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>> {
+        Ok(Box::new(Qwen2BasicConfig::deserialize(
+            config,
+            use_flash_attn,
+        )?))
+    }
 }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/macros.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/macros.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/pipeline/mod.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/pipeline/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+mod cache_manager;
 mod chat_template;
 mod ggml;
 mod gguf;
 mod loaders;
 mod macros;
 mod normal;
+mod sampling;
 use crate::aici::toktree::TokTrie;
 use crate::device_map::DeviceMapper;
+use crate::prefix_cacher::PrefixCacheManager;
+mod sampling_pipeline;
 use crate::{api_dir_list, api_get_file, DeviceMapMetadata};
 use candle_core::quantized::{GgmlDType, QMatMul, QTensor};
 use candle_nn::VarBuilder;
 use chat_template::{apply_chat_template_to, ChatTemplate};
 use core::fmt;
 use either::Either;
 pub use ggml::{GGMLLoader, GGMLLoaderBuilder, GGMLSpecificConfig};
@@ -22,27 +26,30 @@
 use indicatif::{ParallelProgressIterator, ProgressBar, ProgressStyle};
 pub use loaders::{
     GemmaLoader, LlamaLoader, MistralLoader, MixtralLoader, NormalLoaderType, Phi2Loader,
     Phi3Loader, Qwen2Loader,
 };
 use mistralrs_lora::{LoraConfig, Ordering};
 pub use normal::{NormalLoader, NormalLoaderBuilder, NormalSpecificConfig};
+use rand_isaac::Isaac64Rng;
 use rayon::iter::{IndexedParallelIterator, IntoParallelIterator, ParallelIterator};
+pub(crate) use sampling::sample_sequence;
+use std::fmt::{Debug, Display};
 use std::path::Path;
 use std::sync::atomic::AtomicUsize;
 use std::sync::Arc;
-use std::{collections::HashMap, fs, iter::repeat, path::PathBuf, str::FromStr, sync::Mutex};
+use std::{collections::HashMap, fs, iter::repeat, path::PathBuf, str::FromStr};
 use tokenizers::Tokenizer;
+use tokio::sync::Mutex;
 use tracing::info;
 
 use anyhow::Result;
 use candle_core::{DType, Device, Tensor};
 
 use crate::{
-    get_mut_arcmutex,
     models::Cache,
     sequence::Sequence,
     utils::tokens::get_token,
     xlora_models::{NonGranularState, XLoraConfig},
 };
 
 pub trait ModelPaths {
@@ -149,41 +156,48 @@
             TokenSource::Path(value) => write!(f, "path:{}", value),
             TokenSource::CacheToken => write!(f, "cache"),
             TokenSource::None => write!(f, "none"),
         }
     }
 }
 
-#[derive(Copy, Clone, Default)]
+#[derive(Clone, Default)]
 /// The kind of model to build.
 pub enum ModelKind {
     #[default]
     Normal,
     XLoraNormal,
     XLoraGGUF,
     XLoraGGML,
     QuantizedGGUF,
     QuantizedGGML,
     LoraGGUF,
     LoraGGML,
     LoraNormal,
+    Speculative {
+        target: Box<ModelKind>,
+        draft: Box<ModelKind>,
+    },
 }
 
-impl AsRef<str> for ModelKind {
-    fn as_ref(&self) -> &str {
+impl Display for ModelKind {
+    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         match self {
-            ModelKind::Normal => "normal (no quant, no adapters)",
-            ModelKind::QuantizedGGML => "quantized from ggml (no adapters)",
-            ModelKind::QuantizedGGUF => "quantized from gguf (no adapters)",
-            ModelKind::XLoraNormal => "x-lora (no quant)",
-            ModelKind::XLoraGGML => "x-lora, quantized from ggml",
-            ModelKind::XLoraGGUF => "x-lora, quantized from gguf",
-            ModelKind::LoraGGUF => "lora, quantized from gguf",
-            ModelKind::LoraGGML => "lora, quantized from ggml",
-            ModelKind::LoraNormal => "lora (no quant)",
+            ModelKind::Normal => write!(f, "normal (no quant, no adapters)"),
+            ModelKind::QuantizedGGML => write!(f, "quantized from ggml (no adapters)"),
+            ModelKind::QuantizedGGUF => write!(f, "quantized from gguf (no adapters)"),
+            ModelKind::XLoraNormal => write!(f, "x-lora (no quant)"),
+            ModelKind::XLoraGGML => write!(f, "x-lora, quantized from ggml"),
+            ModelKind::XLoraGGUF => write!(f, "x-lora, quantized from gguf"),
+            ModelKind::LoraGGUF => write!(f, "lora, quantized from gguf"),
+            ModelKind::LoraGGML => write!(f, "lora, quantized from ggml"),
+            ModelKind::LoraNormal => write!(f, "lora (no quant)"),
+            ModelKind::Speculative { target, draft } => {
+                write!(f, "speculative: target: `{target}`, draft: `{draft}`")
+            }
         }
     }
 }
 
 /// The `Loader` trait abstracts the loading process. The primary entrypoint is the
 /// `load_model` method.
 ///
@@ -200,91 +214,133 @@
 ///     &Device::cuda_if_available(0).unwrap(),
 ///     false,
 ///     DeviceMapMetadata::dummy(),
 ///     None,
 /// ).unwrap();
 /// ```
 pub trait Loader {
-    fn download_model(
-        &self,
-        revision: Option<String>,
-        token_source: TokenSource,
-        silent: bool,
-    ) -> Result<Box<dyn ModelPaths>>;
-
-    #[allow(clippy::type_complexity)]
-    fn _setup_model(
-        &self,
-        paths: &dyn ModelPaths,
-        dtype: Option<DType>,
-        device: &Device,
-        silent: bool,
-        mapper: DeviceMapMetadata,
-        in_situ_quant: Option<GgmlDType>,
-    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>>;
-
     /// If `revision` is None, then it defaults to `main`.
     /// If `dtype` is None, then it defaults to the model default (usually BF16).
     #[allow(clippy::type_complexity, clippy::too_many_arguments)]
     fn load_model(
         &self,
         revision: Option<String>,
         token_source: TokenSource,
         dtype: Option<DType>,
         device: &Device,
         silent: bool,
         mapper: DeviceMapMetadata,
         in_situ_quant: Option<GgmlDType>,
-    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
-        let paths = self.download_model(revision, token_source, silent)?;
-        self._setup_model(&*paths, dtype, device, silent, mapper, in_situ_quant)
-    }
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>>;
 
-    fn get_id(&self) -> &str;
+    fn get_id(&self) -> String;
     fn get_kind(&self) -> ModelKind;
 }
 
+#[derive(Clone)]
+pub struct GeneralMetadata {
+    pub max_seq_len: usize,
+    pub repeat_last_n: usize,
+    pub tok_trie: Arc<TokTrie>,
+    pub has_no_kv_cache: bool,
+    pub is_xlora: bool,
+    pub num_hidden_layers: usize,
+    pub eos_tok: Vec<u32>,
+}
+
+pub enum CacheInstruction {
+    In,
+    Out,
+    Reset { reset_non_granular: bool },
+    Nonthing,
+}
+
+#[async_trait::async_trait]
 pub trait Pipeline: Send + Sync {
-    fn forward(
+    fn forward_inputs(&mut self, inputs: ModelInputs) -> Result<Tensor, candle_core::Error>;
+    /// This does forward pass of model followed by run.
+    #[allow(clippy::too_many_arguments)]
+    async fn step(
         &mut self,
-        input_seqs: &[&mut Sequence],
+        input_seqs: &mut [&mut Sequence],
         is_prompt: bool,
-    ) -> Result<Tensor, candle_core::Error>;
+        prefix_cacher: &mut PrefixCacheManager,
+        disable_eos_stop: bool,
+        rng: Arc<std::sync::Mutex<Isaac64Rng>>,
+        pre_op: CacheInstruction,
+        post_op: CacheInstruction,
+    ) -> Result<(), candle_core::Error> {
+        let inputs = calculate_inputs(
+            input_seqs,
+            is_prompt,
+            self.get_metadata().is_xlora,
+            &self.device(),
+            self.get_metadata().has_no_kv_cache,
+            None,
+        )
+        .unwrap();
+
+        match pre_op {
+            CacheInstruction::In => self.clone_in_cache(input_seqs),
+            CacheInstruction::Nonthing => (),
+            CacheInstruction::Reset { reset_non_granular } => {
+                self.set_none_cache(reset_non_granular)
+            }
+            _ => unreachable!("Unreachable PRE cache op."),
+        }
+
+        let logits = self.forward_inputs(inputs)?;
+
+        match post_op {
+            CacheInstruction::Out => self.clone_out_cache(input_seqs),
+            CacheInstruction::Nonthing => (),
+            CacheInstruction::Reset { reset_non_granular } => {
+                self.set_none_cache(reset_non_granular)
+            }
+            _ => unreachable!("Unreachable POST cache op."),
+        }
+
+        self.sample(input_seqs, logits, prefix_cacher, disable_eos_stop, rng)
+            .await?;
+        Ok(())
+    }
+    async fn sample(
+        &self,
+        seqs: &mut [&mut Sequence],
+        logits: Tensor,
+        prefix_cacher: &mut PrefixCacheManager,
+        disable_eos_stop: bool,
+        rng: Arc<std::sync::Mutex<Isaac64Rng>>,
+    ) -> Result<(), candle_core::Error>;
     fn tokenize_prompt(&self, prompt: &str) -> Result<Vec<u32>> {
         let encoding = self
             .tokenizer()
             .encode(prompt, false)
             .map_err(|e| anyhow::Error::msg(e.to_string()))?;
         Ok(encoding.get_ids().to_vec())
     }
-    fn device(&self) -> &Device;
-    fn num_hidden_layers(&self) -> usize;
-    fn cache(&self) -> &Cache;
+    fn device(&self) -> Device;
     fn tokenizer(&self) -> Arc<Tokenizer>;
-    fn tok_trie(&self) -> Arc<TokTrie>;
-    fn eos_tok(&self) -> &[u32];
     fn name(&self) -> String;
-    fn get_max_seq_len(&self) -> usize;
-    fn is_xlora(&self) -> bool;
-    fn has_no_kv_cache(&self) -> bool;
     fn apply_chat_template(
         &self,
         messages: Vec<IndexMap<String, String>>,
         add_generation_prompt: bool,
     ) -> Result<String> {
-        let template = self.get_chat_template().chat_template.as_ref().unwrap();
+        let chat_template = self.get_chat_template();
+        let template = chat_template.chat_template.as_ref().unwrap();
         let bos_tok = if let Some(ref bos) = self.get_chat_template().bos_token {
             match bos.0 {
                 Either::Left(ref lit) => Some(lit.to_string()),
                 Either::Right(ref added) => Some(added.content.to_string()),
             }
         } else {
             None
         };
-        let eos_tok = match self.get_chat_template().eos_token {
+        let eos_tok = match chat_template.eos_token {
             Either::Left(ref lit) => lit,
             Either::Right(ref added) => &added.content,
         };
         let unk_tok = if let Some(ref unk) = self.get_chat_template().unk_token {
             match unk.0 {
                 Either::Left(ref lit) => Some(lit.to_string()),
                 Either::Right(ref added) => Some(added.content.to_string()),
@@ -297,28 +353,36 @@
             add_generation_prompt,
             template,
             bos_tok,
             eos_tok,
             unk_tok,
         )
     }
-    fn get_chat_template(&self) -> &ChatTemplate;
-    fn get_non_granular_state(&self) -> &Option<NonGranularState>;
-    fn reset_non_granular_state(&self) {
-        if let Some(s) = self.get_non_granular_state().as_ref() {
-            *self.cache().get_scalings_cache() = None;
-            *get_mut_arcmutex!(s.non_granular_index) = 0;
-        }
-    }
-    fn get_repeat_last_n(&self) -> usize;
-
+    fn get_chat_template(&self) -> Arc<ChatTemplate>;
+    fn reset_non_granular_state(&self);
+    fn get_metadata(&self) -> &GeneralMetadata;
     fn re_isq_model(&mut self, dtype: GgmlDType) -> Result<()>;
+    /// Clone the cache FROM the sequences' cache TO the model cache. Only called for completion seqs.
+    /// It is not a guarantee that this will be called for each completion step.
+    fn clone_in_cache(&mut self, seqs: &mut [&mut Sequence]);
+    /// Clone the cache FROM the model cache TO the sequences. Called for prompt and completion seqs.
+    /// It is not a guarantee that this will be called for each step.
+    fn clone_out_cache(&mut self, seqs: &mut [&mut Sequence]);
+    /// Set the model cache to all None. Only called for prompt seqs.
+    /// It is not a guarantee that this will be called for each prompt step.
+    /// This may also reset the non granular state if applicable.
+    fn set_none_cache(&mut self, reset_non_granular: bool);
+    fn cache(&self) -> &Cache;
 }
 
-pub trait ConfigMarker {}
+pub trait CacheManager {
+    fn clone_in_cache(&self, pipeline: &mut dyn Pipeline, seqs: &mut [&mut Sequence]);
+    fn clone_out_cache(&self, pipeline: &mut dyn Pipeline, seqs: &mut [&mut Sequence]);
+    fn set_none_cache(&self, pipeline: &mut dyn Pipeline);
+}
 
 pub trait NormalModelLoader {
     fn load(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
@@ -336,37 +400,38 @@
         xlora_config: Option<XLoraConfig>,
         xlora_ordering: Ordering,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         device: Device,
     ) -> Result<Box<dyn NormalModel + Send + Sync>>;
     fn is_gptx(&self) -> bool;
+    fn get_config_repr(&self, config: &str, use_flash_attn: bool) -> Result<Box<dyn Debug>>;
 }
 
 pub trait NormalModel {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         position_ids: Vec<usize>,
     ) -> candle_core::Result<Tensor>;
     #[allow(clippy::too_many_arguments)]
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         position_ids: Vec<usize>,
     ) -> candle_core::Result<Tensor>;
     fn is_xlora(&self) -> bool;
     fn device(&self) -> &Device;
     fn cache(&self) -> &Cache;
     fn max_seq_len(&self) -> usize;
     fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper);
@@ -411,20 +476,24 @@
         Ok(())
     }
 }
 
 struct InputMetadata {
     input: Tensor,
     positions: Vec<usize>,
-    positions_kernel: Tensor, // [bs, seq len]
-    context_lens: Vec<usize>,
+    positions_kernel: Tensor,          // [bs, seq len]
+    context_lens: Vec<(usize, usize)>, // (start index, len)
     position_ids: Vec<usize>,
 }
 
-fn get_prompt_input(input_seqs: &[&mut Sequence], device: &Device) -> Result<InputMetadata> {
+fn get_prompt_input(
+    input_seqs: &[&mut Sequence],
+    device: &Device,
+    last_n_context_len: Option<usize>,
+) -> Result<InputMetadata> {
     let max_len = input_seqs
         .iter()
         .map(|seq| seq.len())
         .max()
         .expect("No sequences");
     let padding_tok = 0;
     // Pad each sequence by the padding token to the max len.
@@ -433,15 +502,18 @@
     let mut context_lens = Vec::new();
     let mut position_ids = Vec::new();
     for seq in input_seqs.iter() {
         let mut ctxt = seq.get_toks().to_vec();
         seqlen_offsets.push(0);
 
         ctxt.extend(repeat(padding_tok).take(max_len.saturating_sub(ctxt.len())));
-        context_lens.push(seq.len() - 1);
+        context_lens.push((
+            seq.len() - 1 - last_n_context_len.map(|x| x - 1).unwrap_or(0),
+            last_n_context_len.unwrap_or(1),
+        ));
         position_ids.push(seq.len());
 
         seqs_tensors.push(Tensor::new(ctxt, device).unwrap().unsqueeze(0).unwrap());
     }
 
     let mut tmp = Vec::new();
     for pos in (0..seqs_tensors.len())
@@ -460,28 +532,29 @@
     })
 }
 
 fn get_completion_input(
     input_seqs: &[&mut Sequence],
     device: &Device,
     no_kv_cache: bool,
+    last_n_context_len: Option<usize>,
 ) -> Result<InputMetadata> {
     if no_kv_cache {
-        return get_prompt_input(input_seqs, device);
+        return get_prompt_input(input_seqs, device, last_n_context_len);
     }
     // Pad each sequence by the padding token to the max len.
     let mut seqs_tensors = Vec::new();
     let mut seqlen_offsets = Vec::new();
     let mut context_lens = Vec::new();
     let mut position_ids = Vec::new();
     for seq in input_seqs.iter() {
         let start_pos = seq.get_toks().len().saturating_sub(1);
         let ctxt = seq.get_toks()[start_pos..].to_vec();
         seqlen_offsets.push(start_pos);
-        context_lens.push(0);
+        context_lens.push((0, 1));
         position_ids.push(seq.len());
 
         seqs_tensors.push(Tensor::new(ctxt, device).unwrap().unsqueeze(0).unwrap());
     }
     let mut tmp = Vec::new();
     for pos in (0..seqs_tensors.len())
         .map(|i| vec![*seqlen_offsets.get(i).unwrap() as i64])
@@ -495,47 +568,49 @@
         positions: seqlen_offsets,
         positions_kernel,
         context_lens,
         position_ids,
     })
 }
 
-struct ModelInputs {
+#[derive(Clone)]
+pub struct ModelInputs {
     input_ids: Tensor,
     input_ids_full: Option<Tensor>,
     seqlen_offsets: Vec<usize>,
     seqlen_offsets_full: Option<Vec<usize>>,
     seqlen_offsets_kernel: Tensor,
     seqlen_offsets_kernel_full: Option<Tensor>,
-    context_lens: Vec<usize>,
+    context_lens: Vec<(usize, usize)>,
     position_ids: Vec<usize>,
 }
 
 fn calculate_inputs(
     input_seqs: &[&mut Sequence],
     is_prompt: bool,
     is_xlora: bool,
     device: &Device,
     no_kv_cache: bool,
+    last_n_context_len: Option<usize>,
 ) -> Result<ModelInputs> {
     if is_xlora && !is_prompt {
         let InputMetadata {
             input: input_ids_full,
             positions: seqlen_offsets_full,
             positions_kernel: seqlen_offsets_kernel_full,
             context_lens: _,
             position_ids,
-        } = get_prompt_input(input_seqs, device)?;
+        } = get_prompt_input(input_seqs, device, last_n_context_len)?;
         let InputMetadata {
             input: input_ids,
             positions: seqlen_offsets,
             positions_kernel: seqlen_offsets_kernel,
             context_lens,
             position_ids: _,
-        } = get_completion_input(input_seqs, device, no_kv_cache)?;
+        } = get_completion_input(input_seqs, device, no_kv_cache, last_n_context_len)?;
         Ok(ModelInputs {
             input_ids,
             input_ids_full: Some(input_ids_full),
             seqlen_offsets,
             seqlen_offsets_full: Some(seqlen_offsets_full),
             seqlen_offsets_kernel,
             seqlen_offsets_kernel_full: Some(seqlen_offsets_kernel_full),
@@ -545,15 +620,15 @@
     } else if is_xlora && is_prompt {
         let InputMetadata {
             input: input_ids,
             positions: seqlen_offsets,
             positions_kernel: seqlen_offsets_kernel,
             context_lens,
             position_ids,
-        } = get_prompt_input(input_seqs, device)?;
+        } = get_prompt_input(input_seqs, device, last_n_context_len)?;
         Ok(ModelInputs {
             input_ids: input_ids.clone(),
             input_ids_full: Some(input_ids),
             seqlen_offsets: seqlen_offsets.clone(),
             seqlen_offsets_full: Some(seqlen_offsets),
             seqlen_offsets_kernel: seqlen_offsets_kernel.clone(),
             seqlen_offsets_kernel_full: Some(seqlen_offsets_kernel),
@@ -563,15 +638,15 @@
     } else if is_prompt {
         let InputMetadata {
             input: input_ids,
             positions: seqlen_offsets,
             positions_kernel: seqlen_offsets_kernel,
             context_lens,
             position_ids,
-        } = get_prompt_input(input_seqs, device)?;
+        } = get_prompt_input(input_seqs, device, last_n_context_len)?;
         Ok(ModelInputs {
             input_ids,
             input_ids_full: None,
             seqlen_offsets,
             seqlen_offsets_full: None,
             seqlen_offsets_kernel,
             seqlen_offsets_kernel_full: None,
@@ -581,32 +656,35 @@
     } else {
         let InputMetadata {
             input: input_ids,
             positions: seqlen_offsets,
             positions_kernel: seqlen_offsets_kernel,
             context_lens,
             position_ids,
-        } = get_completion_input(input_seqs, device, no_kv_cache)?;
+        } = get_completion_input(input_seqs, device, no_kv_cache, last_n_context_len)?;
         Ok(ModelInputs {
             input_ids,
             input_ids_full: None,
             seqlen_offsets,
             seqlen_offsets_full: None,
             seqlen_offsets_kernel,
             seqlen_offsets_kernel_full: None,
             context_lens,
             position_ids,
         })
     }
 }
 
-pub fn extract_logits(logits: &Tensor, context_lens: Vec<usize>) -> candle_core::Result<Tensor> {
+pub fn extract_logits(
+    logits: &Tensor,
+    context_lens: Vec<(usize, usize)>,
+) -> candle_core::Result<Tensor> {
     let mut toks = Vec::new();
-    for (dim, start) in logits.chunk(logits.dims()[0], 0)?.iter().zip(context_lens) {
-        toks.push(dim.narrow(1, start, 1)?);
+    for (dim, (start, len)) in logits.chunk(logits.dims()[0], 0)?.iter().zip(context_lens) {
+        toks.push(dim.narrow(1, start, len)?);
     }
     Tensor::cat(&toks, 0)
 }
 
 struct XLoraPaths {
     adapter_configs: Option<Vec<(String, LoraConfig)>>,
     adapter_safetensors: Option<Vec<(String, PathBuf)>>,
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/prefix_cacher.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/prefix_cacher.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-use std::{cell::RefCell, rc::Rc};
+use std::sync::{Arc, Mutex};
 
 use candle_core::{Device, Result, Tensor};
 use radix_trie::{Trie, TrieCommon, TrieKey};
 
-use crate::{models::LayerCaches, sequence::Sequence};
+use crate::{get_mut_arcmutex, models::LayerCaches, sequence::Sequence};
 
 #[derive(PartialEq, Eq)]
 struct Tokens(Vec<u32>);
 
 impl TrieKey for Tokens {
     fn encode_bytes(&self) -> Vec<u8> {
         self.0
@@ -19,19 +19,19 @@
 
 impl From<Vec<u32>> for Tokens {
     fn from(value: Vec<u32>) -> Self {
         Self(value)
     }
 }
 
-type EvictionCacheGroup = (Rc<RefCell<LayerCaches>>, Option<Rc<RefCell<LayerCaches>>>);
+type EvictionCacheGroup = (Arc<Mutex<LayerCaches>>, Option<Arc<Mutex<LayerCaches>>>);
 
 pub struct PrefixCacheManager {
-    caches: Trie<Tokens, Rc<RefCell<LayerCaches>>>,
-    xlora_caches: Option<Trie<Tokens, Rc<RefCell<LayerCaches>>>>,
+    caches: Trie<Tokens, Arc<Mutex<LayerCaches>>>,
+    xlora_caches: Option<Trie<Tokens, Arc<Mutex<LayerCaches>>>>,
     device: Device,
     pub n_on_device: usize,
     no_prefix_cache: bool,
     eviction_cache_ptrs: Vec<EvictionCacheGroup>,
 }
 
 #[derive(Clone)]
@@ -55,19 +55,19 @@
 
     /// This always keeps the cache on the device. If later on, a new seq cannot be allocated due to memory shortage,
     /// some caches will be evicted.
     pub fn add_sequence(&mut self, seq: &mut Sequence) {
         if self.no_prefix_cache {
             return;
         }
-        let cache = Rc::new(RefCell::new(seq.cache().clone()));
+        let cache = Arc::new(Mutex::new(seq.cache().clone()));
         self.caches
             .insert(seq.get_toks().to_vec().into(), cache.clone());
         if seq.is_xlora() {
-            let xlora_cache = Rc::new(RefCell::new(seq.xlora_cache().clone()));
+            let xlora_cache = Arc::new(Mutex::new(seq.xlora_cache().clone()));
             self.xlora_caches
                 .as_mut()
                 .unwrap()
                 .insert(seq.get_toks().to_vec().into(), xlora_cache.clone());
             self.eviction_cache_ptrs.push((cache, Some(xlora_cache)));
         } else {
             self.eviction_cache_ptrs.push((cache, None));
@@ -91,32 +91,40 @@
     pub fn evict_to_cpu(&mut self) -> Result<usize> {
         if self.no_prefix_cache {
             return Ok(0);
         }
         let mut n_on_device = 0;
         for (cache, _) in &self.eviction_cache_ptrs {
             if !matches!(
-                cache.as_ref().borrow()[0].as_ref().unwrap().0.device(),
+                get_mut_arcmutex!(cache.as_ref())[0]
+                    .as_ref()
+                    .unwrap()
+                    .0
+                    .device(),
                 Device::Cpu
             ) {
                 n_on_device += 1;
             }
         }
         let mut n_evicted = 0;
         // Intentionally evict the first ones first, as they are the oldest
         for (cache, xlora_cache) in &self.eviction_cache_ptrs {
             if n_on_device - n_evicted == self.n_on_device {
                 break;
             }
             if !matches!(
-                cache.as_ref().borrow()[0].as_ref().unwrap().0.device(),
+                get_mut_arcmutex!(cache.as_ref())[0]
+                    .as_ref()
+                    .unwrap()
+                    .0
+                    .device(),
                 Device::Cpu
             ) {
-                let mut cache = cache.borrow_mut();
-                let mut xlora_cache = xlora_cache.as_ref().map(|c| c.borrow_mut());
+                let mut cache = get_mut_arcmutex!(cache);
+                let mut xlora_cache = xlora_cache.as_ref().map(|c| get_mut_arcmutex!(c));
 
                 Self::cache_to(cache.iter_mut(), &Device::Cpu)?;
                 if let Some(ref mut xlora_cache) = xlora_cache {
                     Self::cache_to(xlora_cache.iter_mut(), &Device::Cpu)?;
                 }
                 n_evicted += 1;
             }
@@ -128,19 +136,23 @@
     pub fn evict_all_to_cpu(&mut self) -> Result<usize> {
         if self.no_prefix_cache {
             return Ok(0);
         }
         // Intentionally evict the first ones first, as they are the oldest
         for (cache, xlora_cache) in &self.eviction_cache_ptrs {
             if !matches!(
-                cache.as_ref().borrow()[0].as_ref().unwrap().0.device(),
+                get_mut_arcmutex!(cache.as_ref())[0]
+                    .as_ref()
+                    .unwrap()
+                    .0
+                    .device(),
                 Device::Cpu
             ) {
-                let mut cache = cache.borrow_mut();
-                let mut xlora_cache = xlora_cache.as_ref().map(|c| c.borrow_mut());
+                let mut cache = get_mut_arcmutex!(cache);
+                let mut xlora_cache = xlora_cache.as_ref().map(|c| get_mut_arcmutex!(c));
 
                 Self::cache_to(cache.iter_mut(), &Device::Cpu)?;
                 if let Some(ref mut xlora_cache) = xlora_cache {
                     Self::cache_to(xlora_cache.iter_mut(), &Device::Cpu)?;
                 }
             }
         }
@@ -151,18 +163,18 @@
     pub fn search_for_matching_cache(&mut self, toks: &[u32]) -> Result<Option<MatchingCache>> {
         if self.no_prefix_cache {
             return Ok(None);
         }
 
         let toks = Tokens(toks.to_vec());
         if let Some(cache) = self.caches.get(&toks) {
-            Self::cache_to(cache.as_ref().borrow_mut().iter_mut(), &self.device)?;
-            let cache = cache.as_ref().borrow().clone();
+            Self::cache_to(get_mut_arcmutex!(cache.as_ref()).iter_mut(), &self.device)?;
+            let cache = get_mut_arcmutex!(cache.as_ref()).clone();
             let xlora_cache = if let Some(ref xlora_caches) = self.xlora_caches {
-                let mut xlora_cache = xlora_caches.get(&toks).unwrap().as_ref().borrow_mut();
+                let mut xlora_cache = get_mut_arcmutex!(xlora_caches.get(&toks).unwrap().as_ref());
                 Self::cache_to(xlora_cache.iter_mut(), &self.device)?;
                 Some(xlora_cache.clone())
             } else {
                 None
             };
             let ancestor = &self
                 .caches
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/request.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/request.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/response.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/response.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/sampler.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/sampler.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/scheduler.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/scheduler.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,30 @@
-use std::collections::{
-    vec_deque::{Iter, IterMut},
-    HashMap, VecDeque,
-};
+use std::collections::{vec_deque::Iter, HashMap, VecDeque};
 
 use crate::sequence::{Sequence, SequenceState};
 use range_checked::UsizeBounded;
 
 pub trait FcfsBacker: Default {
     fn new() -> Self;
-    fn next(&mut self) -> Option<Sequence>;
     fn add(&mut self, item: Sequence);
     fn into_iter(self) -> impl Iterator<Item = Sequence>;
     fn iter(&self) -> impl Iterator<Item = &Sequence>;
-    fn mut_iter(&mut self) -> impl Iterator<Item = &mut Sequence>;
     fn sort_ascending_ids(&mut self);
 }
 
 impl FcfsBacker for VecDeque<Sequence> {
     fn new() -> Self {
         Self::new()
     }
     fn add(&mut self, item: Sequence) {
         self.push_back(item)
     }
-    fn next(&mut self) -> Option<Sequence> {
-        self.pop_front()
-    }
     fn iter(&self) -> Iter<'_, Sequence> {
         self.iter()
     }
-    fn mut_iter(&mut self) -> IterMut<'_, Sequence> {
-        self.iter_mut()
-    }
     fn into_iter(self) -> impl Iterator<Item = Sequence> {
         <Self as IntoIterator>::into_iter(self)
     }
     fn sort_ascending_ids(&mut self) {
         let slice = self.make_contiguous();
         slice.sort_by_key(|seq| *seq.id());
     }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/sequence.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/sequence.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use std::{
-    cell::Cell,
-    sync::Arc,
+    fmt::Display,
+    sync::{Arc, RwLock},
     time::{SystemTime, UNIX_EPOCH},
 };
 use tokio::sync::{
     mpsc::{error::SendError, Sender},
     Mutex, MutexGuard,
 };
 
@@ -32,41 +32,41 @@
     StopString {
         stop_string_idx: usize,
         completion_bytes_pos: usize,
     },
     Canceled,
 }
 
-impl ToString for StopReason {
-    fn to_string(&self) -> String {
+impl Display for StopReason {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         match self {
-            StopReason::Eos => "stop".to_string(),
-            StopReason::Length(_) | StopReason::ModelLength(_) => "length".to_string(),
-            StopReason::StopTok(_) | StopReason::StopString { .. } => "stop".to_string(),
-            StopReason::Canceled => "canceled".to_string(),
+            StopReason::Eos => write!(f, "stop"),
+            StopReason::Length(_) | StopReason::ModelLength(_) => write!(f, "length"),
+            StopReason::StopTok(_) | StopReason::StopString { .. } => write!(f, "stop"),
+            StopReason::Canceled => write!(f, "canceled"),
         }
     }
 }
 
 #[derive(Clone, Copy, PartialEq)]
 pub enum SequenceState {
     Done(StopReason),
     RunningPrompt,
     RunningCompletion,
     Waiting,
     Error,
     RunningPrefillPrompt,
 }
 
-#[derive(Clone)]
 pub enum SequenceRecognizer {
     Regex(Box<StackRecognizer<StateID, RecRx>>),
     Cfg(Box<CfgParser>),
     None,
 }
+
 pub struct Sequence {
     // Metadata, const
     id: usize,
     prompt_len: usize,
     max_len: Option<usize>,
     timestamp: u128,
     sampler: Arc<Sampler>,
@@ -93,16 +93,17 @@
     stream_idx: usize,
     pub recognizer: SequenceRecognizer,
 
     // GPU things
     pub prompt_tok_per_sec: f32,
     pub prompt_timestamp: Option<u128>,
     group: Arc<Mutex<SequenceGroup>>,
-    state: Cell<SequenceState>,
+    state: RwLock<SequenceState>,
 }
+
 impl Sequence {
     #[allow(clippy::too_many_arguments)]
     pub fn new_waiting(
         tokens: Vec<u32>,
         id: usize,
         timestamp: u128,
         layers: usize,
@@ -123,15 +124,15 @@
         let prompt_len = tokens.len();
         Self {
             tokens,
             logprobs: Vec::new(),
             prompt_len,
             id,
             timestamp,
-            state: Cell::new(SequenceState::Waiting),
+            state: RwLock::new(SequenceState::Waiting),
             cache: vec![None; layers],
             xlora_cache: if is_xlora {
                 Some(vec![None; layers])
             } else {
                 None
             },
             responder,
@@ -190,30 +191,30 @@
     }
 
     pub fn id(&self) -> &usize {
         &self.id
     }
 
     pub fn is_running(&self) -> bool {
-        self.state.get() == SequenceState::RunningCompletion
-            || self.state.get() == SequenceState::RunningPrompt
-            || self.state.get() == SequenceState::RunningPrefillPrompt
+        *self.state.read().unwrap() == SequenceState::RunningCompletion
+            || *self.state.read().unwrap() == SequenceState::RunningPrompt
+            || *self.state.read().unwrap() == SequenceState::RunningPrefillPrompt
     }
 
     pub fn is_completion(&self) -> bool {
-        self.state.get() == SequenceState::RunningCompletion
+        *self.state.read().unwrap() == SequenceState::RunningCompletion
     }
 
     pub fn is_prompt(&self) -> bool {
-        self.state.get() == SequenceState::RunningPrompt
-            || self.state.get() == SequenceState::RunningPrefillPrompt
+        *self.state.read().unwrap() == SequenceState::RunningPrompt
+            || *self.state.read().unwrap() == SequenceState::RunningPrefillPrompt
     }
 
     pub fn is_waiting(&self) -> bool {
-        self.state.get() == SequenceState::Waiting
+        *self.state.read().unwrap() == SequenceState::Waiting
     }
 
     pub fn get_toks(&self) -> &[u32] {
         if let Some(toks) = &self.prefill_prompt_toks {
             return toks;
         }
         &self.tokens
@@ -239,14 +240,34 @@
         self.xlora_cache.is_some()
     }
 
     pub fn sampler(&mut self) -> Arc<Sampler> {
         self.sampler.clone()
     }
 
+    /// Add a some prefill tokens. Only meant for internal speculative decoding usage.
+    pub fn set_prefill_toks(&mut self, toks: Vec<u32>) {
+        self.prefill_prompt_toks = Some(toks)
+    }
+
+    /// Remove the prefill tokens.
+    pub fn reset_prefill_toks(&mut self) {
+        self.prefill_prompt_toks = None
+    }
+
+    /// Internal api.
+    pub fn add_tmp_tok(&mut self, tok: u32) {
+        self.tokens.push(tok);
+    }
+
+    /// Internal api.
+    pub fn remove_tmp_tok(&mut self, n: usize) {
+        self.tokens.truncate(self.tokens.len() - n);
+    }
+
     pub fn add_token(
         &mut self,
         tok: Logprobs,
         completion_bytes: Vec<u8>,
         is_done: &Option<StopReason>,
     ) {
         let stopped_by_token = matches!(
@@ -273,15 +294,15 @@
         self.creation_time
     }
 
     pub fn set_state(&self, state: SequenceState) {
         if matches!(state, SequenceState::Error) {
             get_mut_group!(self).n_choices -= 1;
         }
-        self.state.set(state);
+        *self.state.write().unwrap() = state;
     }
 
     pub fn is_done(
         &self,
         tok: u32,
         eos_tok: Option<&[u32]>,
         max_model_len: usize,
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/utils/mod.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/utils/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,14 @@
                     let pipeline = get_mut_arcmutex!($pipeline);
                     let pipeline_name = pipeline.name();
                     let tokenizer = pipeline.tokenizer();
                     (tokenizer, pipeline_name)
                 };
                 use $crate::response::Response;
                 use $crate::sequence::SequenceState;
-                use $crate::Engine;
                 use $crate::response::SYSTEM_FINGERPRINT;
                 use tracing::error;
                 error!("{} - Model failed with error: {:?}", $stage, &e);
                 for seq in $seq_slice.iter_mut() {
                     // Step 1: Add all choices to groups
                     let res = match tokenizer
                         .decode(&seq.get_toks()[seq.prompt_tokens()..], false)
@@ -156,15 +155,19 @@
                     }
                 }
                 for seq in $seq_slice.iter_mut() {
                     // Step 3: Set state - This cannot be done in Step 2 as `group` is locking the refcell
                     seq.set_state(SequenceState::Error);
                 }
 
-                Engine::set_none_cache(&mut *get_mut_arcmutex!($pipeline));
+                let mut p = get_mut_arcmutex!($pipeline);
+                // Also reset non granular state because:
+                // - The sequence is gone
+                // - We should reset the state then.
+                p.set_none_cache(true);
                 $prefix_cacher.evict_all_to_cpu().unwrap();
 
                 continue $label;
             }
         }
     };
 }
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/utils/tokens.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/utils/tokens.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/utils/varbuilder_utils.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/utils/varbuilder_utils.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/classifier.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/classifier.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/config.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/config.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/gemma.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/gemma.rs`

 * *Files 1% similar despite different names*

```diff
@@ -612,15 +612,15 @@
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
-                *self.cache.xlora_lock() = new_cache.clone();
+                self.cache.xlora_lock().clone_from(&new_cache);
             }
             self.cache.xlora_lock()
         } else {
             self.cache.lock()
         };
         let past_key_values_length =
             self.calculate_past_kv_len(seq_len, cache.first().as_ref().unwrap())?;
@@ -663,27 +663,27 @@
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         if self.xlora_classifier.is_some() {
             let scalings = self.get_scalings(
                 input_ids,
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
-                &context_lens,
+                &vec![usize::MAX; context_lens.len()],
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
@@ -738,30 +738,30 @@
 
 impl NormalModel for XLoraModel {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/llama.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/llama.rs`

 * *Files 1% similar despite different names*

```diff
@@ -472,15 +472,15 @@
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.kv_cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
-                *self.kv_cache.xlora_lock() = new_cache.clone();
+                self.kv_cache.xlora_lock().clone_from(&new_cache);
             }
             self.kv_cache.xlora_lock()
         } else {
             self.kv_cache.lock()
         };
         for (block_idx, block) in self.blocks.iter().enumerate() {
             x = self.mapper.map(x, block_idx)?;
@@ -510,27 +510,27 @@
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         if self.xlora_classifier.is_some() {
             let scalings = self.get_scalings(
                 input_ids,
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
-                &context_lens,
+                &vec![usize::MAX; context_lens.len()],
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
@@ -688,30 +688,30 @@
 
 impl NormalModel for XLoraLlama {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/mistral.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/mistral.rs`

 * *Files 2% similar despite different names*

```diff
@@ -616,15 +616,15 @@
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
-                *self.cache.xlora_lock() = new_cache.clone();
+                self.cache.xlora_lock().clone_from(&new_cache);
             }
             self.cache.xlora_lock()
         } else {
             self.cache.lock()
         };
         let past_key_values_length =
             self.calculate_past_kv_len(seq_len, cache.first().as_ref().unwrap())?;
@@ -666,27 +666,27 @@
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         if self.xlora_classifier.is_some() {
             let scalings = self.get_scalings(
                 input_ids,
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
-                &context_lens,
+                &vec![usize::MAX; context_lens.len()],
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
@@ -741,30 +741,30 @@
 
 impl NormalModel for XLoraModel {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/mixtral.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/mixtral.rs`

 * *Files 1% similar despite different names*

```diff
@@ -751,15 +751,15 @@
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
-                *self.cache.xlora_lock() = new_cache.clone();
+                self.cache.xlora_lock().clone_from(&new_cache);
             }
             self.cache.xlora_lock()
         } else {
             self.cache.lock()
         };
         let mut xs = self.embed_tokens.forward(input_ids)?;
         for (i, layer) in self.layers.iter_mut().enumerate() {
@@ -792,27 +792,27 @@
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         if self.xlora_classifier.is_some() {
             let scalings = self.get_scalings(
                 input_ids,
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
-                &context_lens,
+                &vec![usize::MAX; context_lens.len()],
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
@@ -867,30 +867,30 @@
 
 impl NormalModel for XLoraModel {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/mod.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 mod llama;
 mod mistral;
 mod mixtral;
 mod phi2;
 mod phi3;
 mod quantized_llama;
 
-use std::sync::{Arc, Mutex};
+use std::sync::Arc;
 
 use candle_core::{DType, Device, Result, Tensor};
 pub use config::XLoraConfig;
 pub use gemma::XLoraModel as XLoraGemma;
 pub use llama::XLoraLlama;
 pub use mistral::XLoraModel as XLoraMistral;
 use mistralrs_lora::Ordering;
 pub use mixtral::XLoraModel as XLoraMixtral;
 pub use phi2::Model as XLoraPhi2;
 pub use phi3::Model as XLoraPhi3;
 pub use quantized_llama::ModelWeights as XLoraModelWeights;
+use tokio::sync::Mutex;
 
 use crate::{get_mut_arcmutex, models::Cache};
 
 use self::classifier::XLoraClassifier;
 
 pub struct NonGranularState {
     pub non_granular_index: Arc<Mutex<usize>>,
@@ -95,15 +96,15 @@
             let mut new_cache = Vec::new();
             for _ in 0..self.get_cache().xlora_lock().len() {
                 new_cache.push(Some((
                     Tensor::zeros((1,), DType::U8, &Device::Cpu)?,
                     Tensor::zeros((1,), DType::U8, &Device::Cpu)?,
                 )));
             }
-            *self.get_cache().lock() = new_cache.clone();
+            self.get_cache().lock().clone_from(&new_cache);
 
             res
         } else {
             self.forward(
                 input_ids,
                 seqlen_offsets,
                 start_offsets_kernel.clone(),
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/phi2.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/phi2.rs`

 * *Files 2% similar despite different names*

```diff
@@ -555,15 +555,15 @@
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
-                *self.cache.xlora_lock() = new_cache.clone();
+                self.cache.xlora_lock().clone_from(&new_cache);
             }
             self.cache.xlora_lock()
         } else {
             self.cache.lock()
         };
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
@@ -594,27 +594,27 @@
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         if self.xlora_classifier.is_some() {
             let scalings = self.get_scalings(
                 input_ids,
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
-                &context_lens,
+                &vec![usize::MAX; context_lens.len()],
             )?;
 
             if no_kv_cache {
                 let mut res = self
                     .inner_forward(
                         input_ids_full,
                         seqlen_offsets_full,
@@ -669,30 +669,30 @@
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/phi3.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/phi3.rs`

 * *Files 0% similar despite different names*

```diff
@@ -569,15 +569,15 @@
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
-                *self.cache.xlora_lock() = new_cache.clone();
+                self.cache.xlora_lock().clone_from(&new_cache);
             }
             self.cache.xlora_lock()
         } else {
             self.cache.lock()
         };
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
@@ -609,15 +609,15 @@
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         if self.xlora_classifier.is_some() {
             let scalings = self.get_scalings(
                 input_ids,
                 input_ids_full,
                 seqlen_offsets,
@@ -685,30 +685,30 @@
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         _input_ids: &Tensor,
         _seqlen_offsets: &[usize],
         _start_offsets_kernel: Tensor,
-        _context_lens: Vec<usize>,
+        _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unreachable!()
     }
     fn xlora_forward(
         &mut self,
         input_ids: &Tensor,
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<crate::xlora_models::NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
         position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         self.forward(
             input_ids,
             input_ids_full,
             seqlen_offsets,
             seqlen_offsets_full,
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-core/src/xlora_models/quantized_llama.rs` & `mistralrs_cuda-0.1.4/mistralrs-core/src/xlora_models/quantized_llama.rs`

 * *Files 2% similar despite different names*

```diff
@@ -715,15 +715,15 @@
         let mut cache = if is_full_pass {
             if no_kv_cache {
                 let mut new_cache = Vec::new();
                 for _ in 0..self.cache.xlora_lock().len() {
                     new_cache.push(None);
                 }
 
-                *self.cache.xlora_lock() = new_cache.clone();
+                self.cache.xlora_lock().clone_from(&new_cache);
             }
             self.cache.xlora_lock()
         } else {
             self.cache.lock()
         };
         for (i, layer) in self.layers.iter_mut().enumerate() {
             if let Some(ref mapper) = self.mapper {
@@ -773,27 +773,27 @@
         input_ids_full: &Tensor,
         seqlen_offsets: &[usize],
         seqlen_offsets_full: &[usize],
         start_offsets_kernel: Tensor,
         start_offsets_kernel_full: Tensor,
         no_kv_cache: bool,
         non_granular_state: &Option<NonGranularState>,
-        context_lens: Vec<usize>,
+        context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         if self.xlora_classifier.is_some() {
             let scalings = self.get_scalings(
                 input_ids,
                 input_ids_full,
                 seqlen_offsets,
                 seqlen_offsets_full,
                 &start_offsets_kernel,
                 &start_offsets_kernel_full,
                 no_kv_cache,
                 non_granular_state,
-                &context_lens,
+                &vec![usize::MAX; context_lens.len()],
             )?;
 
             if no_kv_cache {
                 extract_logits(
                     &self
                         .inner_forward(
                             input_ids_full,
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-lora/Cargo.toml` & `mistralrs_cuda-0.1.4/mistralrs-lora/Cargo.toml`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-lora/src/layer.rs` & `mistralrs_cuda-0.1.4/mistralrs-lora/src/layer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-lora/src/lib.rs` & `mistralrs_cuda-0.1.4/mistralrs-lora/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-lora/src/loralinear.rs` & `mistralrs_cuda-0.1.4/mistralrs-lora/src/loralinear.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-lora/src/qloralinear.rs` & `mistralrs_cuda-0.1.4/mistralrs-lora/src/qloralinear.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-pyo3/Cargo.toml` & `mistralrs_cuda-0.1.4/mistralrs-pyo3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.3", path = "../mistralrs-core", features=["cuda"] }
+mistralrs-core = { version = "0.1.4", path = "../mistralrs-core", features=["cuda"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["cuda"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-pyo3/.gitignore` & `mistralrs_cuda-0.1.4/mistralrs-pyo3/.gitignore`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-pyo3/API.md` & `mistralrs_cuda-0.1.4/mistralrs-pyo3/API.md`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-pyo3/Cargo_template.toml` & `mistralrs_cuda-0.1.4/mistralrs-pyo3/Cargo_template.toml`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.3", path = "../mistralrs-core", features=["$feature_name"] }
+mistralrs-core = { version = "0.1.4", path = "../mistralrs-core", features=["$feature_name"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["$feature_name"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-pyo3/README.md` & `mistralrs_cuda-0.1.4/mistralrs-pyo3/README.md`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-pyo3/mistralrs.pyi` & `mistralrs_cuda-0.1.4/mistralrs-pyo3/mistralrs.pyi`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-pyo3/pyproject_template.toml` & `mistralrs_cuda-0.1.4/mistralrs-pyo3/pyproject_template.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
 name = "$name"
-version = "0.1.3"
+version = "0.1.4"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mistralrs_cuda-0.1.3/mistralrs-pyo3/src/lib.rs` & `mistralrs_cuda-0.1.4/mistralrs-pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-pyo3/src/stream.rs` & `mistralrs_cuda-0.1.4/mistralrs-pyo3/src/stream.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-pyo3/src/which.rs` & `mistralrs_cuda-0.1.4/mistralrs-pyo3/src/which.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/mistralrs-pyo3/upload.py` & `mistralrs_cuda-0.1.4/mistralrs-pyo3/upload.py`

 * *Files identical despite different names*

### Comparing `mistralrs_cuda-0.1.3/Cargo.lock` & `mistralrs_cuda-0.1.4/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -63,65 +63,66 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.13"
+version = "0.6.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
+checksum = "418c75fa768af9c03be99d17643f93f79bbba589895012a80e3452a19ddda15b"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
+ "is_terminal_polyfill",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+checksum = "c03a11a9034d92058ceb6ee011ce58af4a9bf61491aa7e1e59ecd24bd40d22d4"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+checksum = "a64c907d4e79225ac72e2a354c9ce84d50ebb4586dee56c82b3ee73004f537f5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+checksum = "61a38449feb7068f52bb06c12759005cf459ee52bb4adc1d5a7c4322d716fb19"
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.82"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
+checksum = "25bdb32cbbdce2b519a9cd7df3a678443100e265d5e25ca763b7572a5104f5f3"
 dependencies = [
  "backtrace",
 ]
 
 [[package]]
 name = "arbitrary"
 version = "1.3.2"
@@ -141,22 +142,22 @@
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "axum"
 version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3a6c9af12842a67734c9a2e355436e5d03b22383ed60cf13cd0c18fbfe3dcbcf"
 dependencies = [
@@ -314,15 +315,15 @@
 name = "bytemuck_derive"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
@@ -353,15 +354,15 @@
  "num_cpus",
  "rand",
  "rand_distr",
  "rayon",
  "safetensors",
  "thiserror",
  "yoke",
- "zip 1.1.3",
+ "zip 1.2.1",
 ]
 
 [[package]]
 name = "candle-flash-attn"
 version = "0.5.0"
 source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
 dependencies = [
@@ -440,29 +441,29 @@
  "serde_json",
  "serde_plain",
  "tracing",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.96"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
+checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cfgrammar"
-version = "0.13.4"
+version = "0.13.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "829b900c3abfb519f93fe713765625385117372cc83b9c68c22d3d8807d89440"
+checksum = "163348850b1cd34fa99ef1592b5d598ea7e6752f18aff2125b67537e887edb36"
 dependencies = [
  "indexmap",
  "lazy_static",
  "num-traits",
  "regex",
  "serde",
  "vob",
@@ -531,15 +532,15 @@
 version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
@@ -565,17 +566,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "colorchoice"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+checksum = "0b6a852b24ab71dffc585bcb46eaf7959d175cb865a7152e35b348d1b2960422"
 
 [[package]]
 name = "console"
 version = "0.15.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e1f83fc076bd6dd27517eacdf25fef6c4dfe5f1d7448bafaaf3a26f13b5e4eb"
 dependencies = [
@@ -768,15 +769,15 @@
 checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim 0.10.0",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "darling_macro"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
@@ -790,15 +791,15 @@
 name = "darling_macro"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core 0.20.8",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "defmac"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aafbece59594ed57696a1a69e8bb3ca1683fbc9cdb41d5c02726070b2cd8f19d"
@@ -807,15 +808,15 @@
 name = "derive_arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67e77553c4162a157adbf834ebae5b415acbecbeafc7a74b0e886657506a7611"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "derive_builder"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d67778784b508018359cbc8696edb3db78160bab2c2a28ba7f56ef6932997f8"
@@ -849,15 +850,15 @@
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d48cda787f839151732d396ac69e3473923d54312c070ee21e9effcaa8ca0b1d"
 dependencies = [
  "darling 0.20.8",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "derive_builder_macro"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ebcda35c7a396850a55ffeac740804b40ffec779b98fffbb1738f4033f0ee79e"
@@ -869,15 +870,15 @@
 [[package]]
 name = "derive_builder_macro"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "206868b8242f27cecce124c19fd88157fbd0dd334df2587f36417bafbc85097b"
 dependencies = [
  "derive_builder_core 0.20.0",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
@@ -913,14 +914,25 @@
  "libc",
  "option-ext",
  "redox_users",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "displaydoc"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "487585f4d0c6655fe74905e2504d8ad6908e4db67f744eb140876906c2f3175d"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.61",
+]
+
+[[package]]
 name = "dyn-fmt"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "79ef34f092abc832595d6e7b81a416403243ab94cc4c8262608aa4fddc95209a"
 
 [[package]]
 name = "dyn-stack"
@@ -958,15 +970,15 @@
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ffccbb6966c05b32ef8fbac435df276c4ae4d3dc55a8cd0eb9745e6c12f546a"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
@@ -1068,15 +1080,15 @@
 name = "foreign-types-macros"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a5c6c585bc94aaf2c7b51dd4c2ba22680844aba4c687be581871a6f518c5742"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
@@ -1148,15 +1160,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -1321,17 +1333,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -1602,14 +1614,20 @@
 dependencies = [
  "anyhow",
  "log",
  "walkdir",
 ]
 
 [[package]]
+name = "is_terminal_polyfill"
+version = "1.70.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8478577c03552c21db0e2724ffb8986a5ce7af88107e6be5d2ee6e158c12800"
+
+[[package]]
 name = "itertools"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
@@ -1686,17 +1704,17 @@
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "lrtable"
-version = "0.13.4"
+version = "0.13.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee337773c4a85c7a270fbc4ca500ece4abb288cd9c3ac60f642441b96b9f53a7"
+checksum = "ff5668c3bfd279ed24d5b0d24568c48dc993f9beabd51f74d1865a78c1d206ab"
 dependencies = [
  "cfgrammar",
  "fnv",
  "num-traits",
  "sparsevec",
  "vob",
 ]
@@ -1831,25 +1849,25 @@
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mistralrs"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "anyhow",
  "candle-core",
  "mistralrs-core",
  "tokio",
 ]
 
 [[package]]
 name = "mistralrs-bench"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "anyhow",
  "candle-core",
  "clap",
  "cli-table",
  "either",
  "mistralrs-core",
@@ -1858,18 +1876,19 @@
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-core"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "accelerate-src",
  "anyhow",
+ "async-trait",
  "bytemuck",
  "candle-core",
  "candle-flash-attn",
  "candle-nn",
  "candle-transformers",
  "cfgrammar",
  "chrono",
@@ -1903,28 +1922,28 @@
  "tqdm",
  "tracing",
  "vob",
 ]
 
 [[package]]
 name = "mistralrs-lora"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "candle-nn",
  "either",
  "intel-mkl-src",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "mistralrs-pyo3"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "either",
  "futures",
  "indexmap",
  "intel-mkl-src",
@@ -1933,15 +1952,15 @@
  "serde",
  "serde_json",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-server"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "axum",
  "candle-core",
  "clap",
  "dyn-fmt",
@@ -1958,31 +1977,31 @@
  "tracing-subscriber",
  "utoipa",
  "utoipa-swagger-ui",
 ]
 
 [[package]]
 name = "monostate"
-version = "0.1.12"
+version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a20fffcd8ca4c69d31e036a71abc400147b41f90895df4edcb36497a1f8af8bf"
+checksum = "0d208407d7552cd041d8cdb69a1bc3303e029c598738177a3d87082004dc0e1e"
 dependencies = [
  "monostate-impl",
  "serde",
 ]
 
 [[package]]
 name = "monostate-impl"
-version = "0.1.12"
+version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf307cbbbd777a9c10cec88ddafee572b3484caad5cce0c9236523c3803105a6"
+checksum = "a7ce64b975ed4f123575d11afd9491f2e37bbd5813fbfbc0f09ae1fbddea74e0"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
@@ -2026,28 +2045,27 @@
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "bytemuck",
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
@@ -2056,17 +2074,17 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -2075,14 +2093,35 @@
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
+name = "num_enum"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02339744ee7253741199f897151b38e72257d13802d4ee837285cc2990a90845"
+dependencies = [
+ "num_enum_derive",
+]
+
+[[package]]
+name = "num_enum_derive"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
+dependencies = [
+ "proc-macro-crate",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.61",
+]
+
+[[package]]
 name = "number_prefix"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
 
 [[package]]
 name = "objc"
@@ -2199,15 +2238,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -2267,26 +2306,26 @@
  "redox_syscall 0.5.1",
  "smallvec",
  "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "parse-zoneinfo"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
+checksum = "1f2a05b18d44e2957b88f96ba460715e295bc1d7510468a2f3d3b44535d26c24"
 dependencies = [
  "regex",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
@@ -2341,15 +2380,15 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
@@ -2375,14 +2414,23 @@
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
+name = "proc-macro-crate"
+version = "3.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
+dependencies = [
+ "toml_edit 0.21.1",
+]
+
+[[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
@@ -2400,17 +2448,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pulp"
 version = "0.18.10"
@@ -2478,28 +2526,28 @@
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
@@ -2721,15 +2769,15 @@
 version = "8.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b91ac2a3c6c0520a3fb3dd89321177c3c692937c4eb21893378219da10c44fc8"
 dependencies = [
  "proc-macro2",
  "quote",
  "rust-embed-utils",
- "syn 2.0.60",
+ "syn 2.0.61",
  "walkdir",
 ]
 
 [[package]]
 name = "rust-embed-utils"
 version = "8.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2747,17 +2795,17 @@
 dependencies = [
  "arrayvec",
  "num-traits",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
@@ -2795,40 +2843,40 @@
  "rustls-webpki",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.5.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
+checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
 
 [[package]]
 name = "rustls-webpki"
 version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.15"
+version = "1.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
+checksum = "092474d1a01ea8278f69e6a358998405fae5b8b963ddaeb2b0b04a128bf1dfb0"
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "safetensors"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ced76b22c7fba1162f11a5a75d9d8405264b467a07ae0c9c29be119b9297db9"
 dependencies = [
@@ -2858,72 +2906,72 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "security-framework"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
+checksum = "c627723fd09706bacdb5cf41499e95098555af3c3c29d014dc3c458ef6be11c0"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
+checksum = "317936bbbd05227752583946b9e66d7ce3b489f84e11a94a510b4437fef407d7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
+checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
+checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.116"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -3110,17 +3158,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3139,15 +3187,15 @@
 name = "synstructure"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8af7666ab7b6390ab78131fb5b0fce11d6b7a6951602017c35fa82800708971"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "sysctl"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec7dddc5f0fee506baf8b9fdb989e242f17e4b11c61dfbb0635b705217199eea"
@@ -3196,30 +3244,30 @@
 checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
@@ -3296,15 +3344,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "tokio-rayon"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7cf33a76e0b1dd03b778f83244137bd59887abf25c0e87bc3e7071105f457693"
@@ -3318,37 +3366,48 @@
 version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
- "toml_edit",
+ "toml_edit 0.22.12",
 ]
 
 [[package]]
 name = "toml_datetime"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
+version = "0.21.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6a8534fd7f78b5405e860340ad6575217ce99f38d4d5c8f2442cb5ecb50090e1"
+dependencies = [
+ "indexmap",
+ "toml_datetime",
+ "winnow 0.5.40",
+]
+
+[[package]]
+name = "toml_edit"
 version = "0.22.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3328d4f68a705b2a4498da1d580585d39a6510f98318a2cec3018a7ec61ddef"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
- "winnow",
+ "winnow 0.6.8",
 ]
 
 [[package]]
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
@@ -3418,15 +3477,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -3580,35 +3639,35 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "utoipa"
-version = "4.2.0"
+version = "4.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "272ebdfbc99111033031d2f10e018836056e4d2c8e2acda76450ec7974269fa7"
+checksum = "c5afb1a60e207dca502682537fefcfd9921e71d0b83e9576060f09abc6efab23"
 dependencies = [
  "indexmap",
  "serde",
  "serde_json",
  "utoipa-gen",
 ]
 
 [[package]]
 name = "utoipa-gen"
-version = "4.2.0"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3c9f4d08338c1bfa70dde39412a040a884c6f318b3d09aaaf3437a1e52027fc"
+checksum = "7bf0e16c02bc4bf5322ab65f10ab1149bdbcaa782cba66dc7057370a3f8190be"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "regex",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "utoipa-swagger-ui"
 version = "6.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b39868d43c011961e04b41623e050aedf2cc93652562ff7935ce0f819aaf2da"
@@ -3694,15 +3753,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3716,15 +3775,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -3917,17 +3976,26 @@
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
-version = "0.6.7"
+version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14b9415ee827af173ebb3f15f9083df5a122eb93572ec28741fb153356ea2578"
+checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
+name = "winnow"
+version = "0.6.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c3c52e9c97a68071b23e836c9380edae937f17b9c4667bd021973efc689f618d"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "xattr"
 version = "1.3.1"
@@ -3955,36 +4023,36 @@
 name = "yoke-derive"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e6936f0cce458098a201c245a11bef556c6a0181129c7034d10d76d1ec3a2b8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
  "synstructure",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
 ]
 
 [[package]]
 name = "zerofrom"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "655b0814c5c0b19ade497851070c640773304939a6c0fd5f5fb43da0696d05b7"
@@ -3996,15 +4064,15 @@
 name = "zerofrom-derive"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6a647510471d372f2e6c2e6b7219e44d8c574d24fdc11c610a61455782f18c3"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.61",
  "synstructure",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4020,16 +4088,19 @@
  "crc32fast",
  "crossbeam-utils",
  "flate2",
 ]
 
 [[package]]
 name = "zip"
-version = "1.1.3"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e6cb8909b2e8e6733c9ef67d35be1a27105644d362aafb5f8b2ba395727adf6"
+checksum = "006d078b7b6fc587bb25e022ad39e7086f44e5c4fef6076964ea601533241beb"
 dependencies = [
  "arbitrary",
- "byteorder",
  "crc32fast",
  "crossbeam-utils",
+ "displaydoc",
+ "indexmap",
+ "num_enum",
+ "thiserror",
 ]
```

### Comparing `mistralrs_cuda-0.1.3/Cargo.toml` & `mistralrs_cuda-0.1.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["mistralrs-core", "mistralrs-lora", "mistralrs-pyo3"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.3"
+version = "0.1.4"
 edition = "2021"
 description = "Fast and easy LLM serving."
 homepage = "https://github.com/EricLBuehler/mistral.rs"
 repository = "https://github.com/EricLBuehler/mistral.rs"
 keywords = ["machine-learning"]
 categories = ["science"]
 license = "MIT"
```

### Comparing `mistralrs_cuda-0.1.3/pyproject.toml` & `mistralrs_cuda-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
 name = "mistralrs-cuda"
-version = "0.1.3"
+version = "0.1.4"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mistralrs_cuda-0.1.3/PKG-INFO` & `mistralrs_cuda-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistralrs-cuda
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Rust
 Summary: Fast and easy LLM serving.
```

