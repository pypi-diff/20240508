# Comparing `tmp/llm2vec-0.1.5.tar.gz` & `tmp/llm2vec-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm2vec-0.1.5.tar", last modified: Tue Apr 30 22:32:19 2024, max compression
+gzip compressed data, was "llm2vec-0.1.6.tar", last modified: Wed May  8 16:29:59 2024, max compression
```

## Comparing `llm2vec-0.1.5.tar` & `llm2vec-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.870986 llm2vec-0.1.5/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-08 21:09:47.000000 llm2vec-0.1.5/LICENSE
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     8941 2024-04-30 22:32:19.871323 llm2vec-0.1.5/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     8491 2024-04-30 22:31:54.000000 llm2vec-0.1.5/README.md
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.852001 llm2vec-0.1.5/llm2vec/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       29 2024-04-16 16:56:44.000000 llm2vec-0.1.5/llm2vec/__init__.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.861701 llm2vec-0.1.5/llm2vec/dataset/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6340 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/dataset/E5Data.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       26 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/dataset/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1123 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/dataset/dataset.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      723 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/dataset/utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     2417 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/experiment_utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    15447 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/llm2vec.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.865363 llm2vec-0.1.5/llm2vec/loss/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1478 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/loss/HardNegativeNLLLoss.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       52 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/loss/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     3080 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/loss/loss_utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      289 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/loss/utils.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.869896 llm2vec-0.1.5/llm2vec/models/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      130 2024-04-16 16:56:44.000000 llm2vec-0.1.5/llm2vec/models/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7620 2024-04-16 16:56:44.000000 llm2vec-0.1.5/llm2vec/models/attn_mask_utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7760 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/models/bidirectional_llama.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10368 2024-04-17 17:32:47.000000 llm2vec-0.1.5/llm2vec/models/bidirectional_mistral.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-04-30 22:31:54.000000 llm2vec-0.1.5/llm2vec/version.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-30 22:32:19.857753 llm2vec-0.1.5/llm2vec.egg-info/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     8941 2024-04-30 22:32:19.000000 llm2vec-0.1.5/llm2vec.egg-info/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      661 2024-04-30 22:32:19.000000 llm2vec-0.1.5/llm2vec.egg-info/SOURCES.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-30 22:32:19.000000 llm2vec-0.1.5/llm2vec.egg-info/dependency_links.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.5/llm2vec.egg-info/not-zip-safe
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       74 2024-04-30 22:32:19.000000 llm2vec-0.1.5/llm2vec.egg-info/requires.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-04-30 22:32:19.000000 llm2vec-0.1.5/llm2vec.egg-info/top_level.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-04-30 22:32:19.872548 llm2vec-0.1.5/setup.cfg
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1089 2024-04-17 17:32:47.000000 llm2vec-0.1.5/setup.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.721398 llm2vec-0.1.6/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-08 21:09:47.000000 llm2vec-0.1.6/LICENSE
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    12628 2024-05-08 16:29:59.721661 llm2vec-0.1.6/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    12178 2024-05-08 16:25:06.000000 llm2vec-0.1.6/README.md
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.703822 llm2vec-0.1.6/llm2vec/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       29 2024-04-16 16:56:44.000000 llm2vec-0.1.6/llm2vec/__init__.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.711660 llm2vec-0.1.6/llm2vec/dataset/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6148 2024-05-08 16:25:06.000000 llm2vec-0.1.6/llm2vec/dataset/E5Data.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       26 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/dataset/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1123 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/dataset/dataset.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      723 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/dataset/utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     2417 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/experiment_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    16774 2024-05-08 16:25:06.000000 llm2vec-0.1.6/llm2vec/llm2vec.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.715280 llm2vec-0.1.6/llm2vec/loss/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1478 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/loss/HardNegativeNLLLoss.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       52 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/loss/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     3080 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/loss/loss_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      289 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/loss/utils.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.720316 llm2vec-0.1.6/llm2vec/models/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      130 2024-04-16 16:56:44.000000 llm2vec-0.1.6/llm2vec/models/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7620 2024-04-16 16:56:44.000000 llm2vec-0.1.6/llm2vec/models/attn_mask_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7760 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/models/bidirectional_llama.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10368 2024-04-17 17:32:47.000000 llm2vec-0.1.6/llm2vec/models/bidirectional_mistral.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-05-08 16:29:50.000000 llm2vec-0.1.6/llm2vec/version.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.708107 llm2vec-0.1.6/llm2vec.egg-info/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    12628 2024-05-08 16:29:59.000000 llm2vec-0.1.6/llm2vec.egg-info/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      661 2024-05-08 16:29:59.000000 llm2vec-0.1.6/llm2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-05-08 16:29:59.000000 llm2vec-0.1.6/llm2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.6/llm2vec.egg-info/not-zip-safe
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       74 2024-05-08 16:29:59.000000 llm2vec-0.1.6/llm2vec.egg-info/requires.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-05-08 16:29:59.000000 llm2vec-0.1.6/llm2vec.egg-info/top_level.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-05-08 16:29:59.722725 llm2vec-0.1.6/setup.cfg
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1089 2024-04-17 17:32:47.000000 llm2vec-0.1.6/setup.py
```

### Comparing `llm2vec-0.1.5/LICENSE` & `llm2vec-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.5/PKG-INFO` & `llm2vec-0.1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm2vec
-Version: 0.1.5
+Version: 0.1.6
 Summary: The official llm2vec library
 Home-page: https://github.com/McGill-NLP/llm2vec
 Author: McGill NLP
 Author-email: parishad.behnamghader@mila.quebec
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *LLM2Vec: Large Language Models Are Secretly Powerful Text Encoders* 
 
 [![arxiv](https://img.shields.io/badge/arXiv-2404.05961-b31b1b.svg)](https://arxiv.org/abs/2404.05961)
 [![PyPi](https://img.shields.io/pypi/v/llm2vec)](https://pypi.org/project/llm2vec/)
-[![HF](https://img.shields.io/badge/HF%20Models-LLM2Vec-FFD21E.svg)](https://huggingface.co/collections/McGill-NLP/llm2vec-660e14f536b3c8d10b3f1c34)
+[![HF Link](https://img.shields.io/badge/HF%20Models-LLM2Vec-FFD21E.svg)](https://huggingface.co/collections/McGill-NLP/llm2vec-660e14f536b3c8d10b3f1c34)
 
 
 
 
 LLM2Vec is a simple recipe to convert decoder-only LLMs into text encoders. It consists of 3 simple steps: 1) enabling bidirectional attention, 2) training with masked next token prediction, and 3) unsupervised contrastive learning. The model can be further fine-tuned to achieve state-of-the-art performance.
 
 <p align="center">
@@ -115,30 +115,24 @@
         [0.0565, 0.5425]])
 """
 ```
 
 More examples of classification, clustering, sentence similarity etc are present in [examples](examples) directory.
 
 ## Model List
-- ### Meta-Llama-3-8B
-  - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp)
-  - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse)
-  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised) (state-of-the-art on MTEB among models trained on public data)
-- ### Mistral-7B
-  - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp)
-  - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-unsup-simcse) (Unsupervised state-of-the-art on MTEB)
-  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised)
-- ### Llama-2-7B
-  - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp)
-  - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-unsup-simcse)
-  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp-supervised)
-- ### Sheared-Llama-1.3B
-  - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp)
-  - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-unsup-simcse)
-  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp-supervised)
+
+|  | Meta-Llama-3-8B | Mistral-7B | Llama-2-7B | Sheared-Llama-1.3B |
+|----|------------------|------------|------------|---------------------|
+| Bi + MNTP | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp) |
+| Bi + MNTP + SimCSE | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-unsup-simcse)** | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-unsup-simcse) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-unsup-simcse) |
+| Bi + MNTP + Supervised | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised)* | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp-supervised) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp-supervised) |
+
+\* State-of-the-art on MTEB among models trained on public data
+
+\*\* Unsupervised state-of-the-art on MTEB
 
 ## Training 
 ### MNTP training
 To train the model with Masked Next Token Prediction (MNTP), you can use the `experiments/run_mntp.py` script. It is adapted from HuggingFace Masked Language Modeling (MLM) [script](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/examples/pytorch/language-modeling/run_mlm.py). To train the Mistral-7B model with MNTP, run the following command:
 
 ```bash
 python experiments/run_mntp.py train_configs/mntp/Mistral.json
@@ -157,15 +151,88 @@
     "gradient_checkpointing": true,
     "torch_dtype": "bfloat16",
     "attn_implementation": "flash_attention_2"
     // ....
 }
 ```
 
-Similar configurations are also available for [Llama-2-7B](train_configs/mntp/Llama.json) and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
+Similar configurations are also available for[Meta-Llama-3-8B](train_configs/mntp/MetaLlama3.json), [Llama-2-7B](train_configs/mntp/Llama2.json), and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
+
+### Unsupervised contrastive training (SimCSE)
+COMING SOON
+
+### Supervised contrastive training
+For supervised contrastive training, we use the public portion of dataset used in [Improving Text Embeddings with Large Language Models](https://arxiv.org/abs/2401.00368), curated by authors of [Repetition Improves Language Model Embeddings](https://arxiv.org/abs/2402.15449). The dataset can be downloaded from the [GitHub page of Echo embeddings repository](https://github.com/jakespringer/echo-embeddings#training). To use the training script, the downloaded dataset should be placed in the `cache` directory. The directory layout should be as follows:
+
+```
+cache
+└── echo-data
+    ├── allnli_split1.jsonl
+    ├── allnli_split2.jsonl
+    ├── allnli.jsonl
+    ├── dureader.jsonl
+    ...
+```
+If the dataset is placed in a different directory, please change the `dataset_file_path` in the training configuration accordingly. 
+
+To train the Mistral-7B model with supervised contrastive learning, run the following command:
+
+```bash
+torchrun --nproc_per_node=8 experiments/run_supervised.py train_configs/supervised/Mistral.json
+```
+The number of GPUs can be changed by modifying the `--nproc_per_node` argument.
+
+The Mistral training configuration [file](train_configs/supervised/Mistral.json) contains all the training hyperparameters and configurations used in our paper. 
+```json
+{
+    "model_name_or_path": "mistralai/Mistral-7B-Instruct-v0.2",
+    "peft_model_name_or_path": "McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp",
+    "bidirectional": true,
+    "pooling_mode": "mean",
+    "dataset_name": "E5",
+    "dataset_file_path": "cache/echo-data",
+    "learning_rate": 2e-4,
+    "num_train_epochs": 3,
+    "warmup_steps": 300,
+    "per_device_train_batch_size": 64,
+    "lora_r": 16,
+    "gradient_checkpointing": true,
+    "torch_dtype": "bfloat16",
+    "attn_implementation": "flash_attention_2"
+    // ....
+}
+```
+Similar configurations are also available for [Meta-Llama-3-8B](train_configs/supervised/MetaLlama3.json), [Llama-2-7B](train_configs/supervised/Llama2.json), and [Sheared-Llama-1.3B](train_configs/supervised/Sheared-Llama.json) models.
+
+
+### Word-level tasks training
+
+To tune the model for word-level tasks, we define a classifier on top of the models, and only train the classifier weights. The code is adapted from HuggingFace token classification [example](https://huggingface.co/docs/transformers/en/tasks/token_classification). To train and test the classifier for Llama-2-7B MNTP model on `pos_tags` task, run the following command:
+```bash
+python experiments/run_word_task.py train_configs/word-task/Llama2-bi-mntp.json
+python experiments/test_word_task.py --config_file test_configs/word-task/Llama2-bi-mntp.json
+```
+The config files contain all the parameters and configurations used in our paper. For instance, `Llama2-bi-mntp.json` includes:
+```json
+{
+    "model_name_or_path": "meta-llama/Llama-2-7b-chat-hf",
+    "peft_addr": "McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp", // or any local directory containing `adapter_model` files.
+    "model_class": "custom",
+    "bidirectional": true,
+    "classifier_dropout": 0.1,
+    "merge_subwords": true,
+    "retroactive_labels": "next_token",
+    "output_dir": "output/word-task/pos_tags/Llama2/bi-mntp",
+    "dataset_name": "conll2003",
+    "task": "pos_tags", // or ner_tags, or chunk_tags
+    // ....
+}
+``` 
+[train_configs/word-task](train_configs/word-task) and [test_configs/word-task](train_configs/word-task) contain similar configurations for Llama-2-7B, Mistral-7B, and Sheared-Llama-1.3B for all Uni, Bi, Bi-MNTP, and Bi-MNTP-SimCSE (LLM2Vec) variants. 
+
 
 ## Citation
 If you find our work helpful, please cite us:
 ```bibtex
 @article{llm2vec,
       title={{LLM2Vec}: {L}arge Language Models Are Secretly Powerful Text Encoders}, 
       author={Parishad BehnamGhader and Vaibhav Adlakha and Marius Mosbach and Dzmitry Bahdanau and Nicolas Chapados and Siva Reddy},
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llm2vec-0.1.5/README.md` & `llm2vec-0.1.6/llm2vec.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,27 @@
+Metadata-Version: 2.1
+Name: llm2vec
+Version: 0.1.6
+Summary: The official llm2vec library
+Home-page: https://github.com/McGill-NLP/llm2vec
+Author: McGill NLP
+Author-email: parishad.behnamghader@mila.quebec
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # *LLM2Vec: Large Language Models Are Secretly Powerful Text Encoders* 
 
 [![arxiv](https://img.shields.io/badge/arXiv-2404.05961-b31b1b.svg)](https://arxiv.org/abs/2404.05961)
 [![PyPi](https://img.shields.io/pypi/v/llm2vec)](https://pypi.org/project/llm2vec/)
-[![HF](https://img.shields.io/badge/HF%20Models-LLM2Vec-FFD21E.svg)](https://huggingface.co/collections/McGill-NLP/llm2vec-660e14f536b3c8d10b3f1c34)
+[![HF Link](https://img.shields.io/badge/HF%20Models-LLM2Vec-FFD21E.svg)](https://huggingface.co/collections/McGill-NLP/llm2vec-660e14f536b3c8d10b3f1c34)
 
 
 
 
 LLM2Vec is a simple recipe to convert decoder-only LLMs into text encoders. It consists of 3 simple steps: 1) enabling bidirectional attention, 2) training with masked next token prediction, and 3) unsupervised contrastive learning. The model can be further fine-tuned to achieve state-of-the-art performance.
 
 <p align="center">
@@ -100,30 +115,24 @@
         [0.0565, 0.5425]])
 """
 ```
 
 More examples of classification, clustering, sentence similarity etc are present in [examples](examples) directory.
 
 ## Model List
-- ### Meta-Llama-3-8B
-  - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp)
-  - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse)
-  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised) (state-of-the-art on MTEB among models trained on public data)
-- ### Mistral-7B
-  - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp)
-  - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-unsup-simcse) (Unsupervised state-of-the-art on MTEB)
-  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised)
-- ### Llama-2-7B
-  - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp)
-  - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-unsup-simcse)
-  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp-supervised)
-- ### Sheared-Llama-1.3B
-  - ### [Bi + MNTP](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp)
-  - ### [Bi + MNTP + SimCSE](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-unsup-simcse)
-  - ### [Bi + MNTP + Supervised](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp-supervised)
+
+|  | Meta-Llama-3-8B | Mistral-7B | Llama-2-7B | Sheared-Llama-1.3B |
+|----|------------------|------------|------------|---------------------|
+| Bi + MNTP | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp) |
+| Bi + MNTP + SimCSE | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-unsup-simcse)** | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-unsup-simcse) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-unsup-simcse) |
+| Bi + MNTP + Supervised | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised)* | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp-supervised) | [HF Link](https://huggingface.co/McGill-NLP/LLM2Vec-Sheared-LLaMA-mntp-supervised) |
+
+\* State-of-the-art on MTEB among models trained on public data
+
+\*\* Unsupervised state-of-the-art on MTEB
 
 ## Training 
 ### MNTP training
 To train the model with Masked Next Token Prediction (MNTP), you can use the `experiments/run_mntp.py` script. It is adapted from HuggingFace Masked Language Modeling (MLM) [script](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/examples/pytorch/language-modeling/run_mlm.py). To train the Mistral-7B model with MNTP, run the following command:
 
 ```bash
 python experiments/run_mntp.py train_configs/mntp/Mistral.json
@@ -142,15 +151,88 @@
     "gradient_checkpointing": true,
     "torch_dtype": "bfloat16",
     "attn_implementation": "flash_attention_2"
     // ....
 }
 ```
 
-Similar configurations are also available for [Llama-2-7B](train_configs/mntp/Llama.json) and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
+Similar configurations are also available for[Meta-Llama-3-8B](train_configs/mntp/MetaLlama3.json), [Llama-2-7B](train_configs/mntp/Llama2.json), and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
+
+### Unsupervised contrastive training (SimCSE)
+COMING SOON
+
+### Supervised contrastive training
+For supervised contrastive training, we use the public portion of dataset used in [Improving Text Embeddings with Large Language Models](https://arxiv.org/abs/2401.00368), curated by authors of [Repetition Improves Language Model Embeddings](https://arxiv.org/abs/2402.15449). The dataset can be downloaded from the [GitHub page of Echo embeddings repository](https://github.com/jakespringer/echo-embeddings#training). To use the training script, the downloaded dataset should be placed in the `cache` directory. The directory layout should be as follows:
+
+```
+cache
+└── echo-data
+    ├── allnli_split1.jsonl
+    ├── allnli_split2.jsonl
+    ├── allnli.jsonl
+    ├── dureader.jsonl
+    ...
+```
+If the dataset is placed in a different directory, please change the `dataset_file_path` in the training configuration accordingly. 
+
+To train the Mistral-7B model with supervised contrastive learning, run the following command:
+
+```bash
+torchrun --nproc_per_node=8 experiments/run_supervised.py train_configs/supervised/Mistral.json
+```
+The number of GPUs can be changed by modifying the `--nproc_per_node` argument.
+
+The Mistral training configuration [file](train_configs/supervised/Mistral.json) contains all the training hyperparameters and configurations used in our paper. 
+```json
+{
+    "model_name_or_path": "mistralai/Mistral-7B-Instruct-v0.2",
+    "peft_model_name_or_path": "McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp",
+    "bidirectional": true,
+    "pooling_mode": "mean",
+    "dataset_name": "E5",
+    "dataset_file_path": "cache/echo-data",
+    "learning_rate": 2e-4,
+    "num_train_epochs": 3,
+    "warmup_steps": 300,
+    "per_device_train_batch_size": 64,
+    "lora_r": 16,
+    "gradient_checkpointing": true,
+    "torch_dtype": "bfloat16",
+    "attn_implementation": "flash_attention_2"
+    // ....
+}
+```
+Similar configurations are also available for [Meta-Llama-3-8B](train_configs/supervised/MetaLlama3.json), [Llama-2-7B](train_configs/supervised/Llama2.json), and [Sheared-Llama-1.3B](train_configs/supervised/Sheared-Llama.json) models.
+
+
+### Word-level tasks training
+
+To tune the model for word-level tasks, we define a classifier on top of the models, and only train the classifier weights. The code is adapted from HuggingFace token classification [example](https://huggingface.co/docs/transformers/en/tasks/token_classification). To train and test the classifier for Llama-2-7B MNTP model on `pos_tags` task, run the following command:
+```bash
+python experiments/run_word_task.py train_configs/word-task/Llama2-bi-mntp.json
+python experiments/test_word_task.py --config_file test_configs/word-task/Llama2-bi-mntp.json
+```
+The config files contain all the parameters and configurations used in our paper. For instance, `Llama2-bi-mntp.json` includes:
+```json
+{
+    "model_name_or_path": "meta-llama/Llama-2-7b-chat-hf",
+    "peft_addr": "McGill-NLP/LLM2Vec-Llama-2-7b-chat-hf-mntp", // or any local directory containing `adapter_model` files.
+    "model_class": "custom",
+    "bidirectional": true,
+    "classifier_dropout": 0.1,
+    "merge_subwords": true,
+    "retroactive_labels": "next_token",
+    "output_dir": "output/word-task/pos_tags/Llama2/bi-mntp",
+    "dataset_name": "conll2003",
+    "task": "pos_tags", // or ner_tags, or chunk_tags
+    // ....
+}
+``` 
+[train_configs/word-task](train_configs/word-task) and [test_configs/word-task](train_configs/word-task) contain similar configurations for Llama-2-7B, Mistral-7B, and Sheared-Llama-1.3B for all Uni, Bi, Bi-MNTP, and Bi-MNTP-SimCSE (LLM2Vec) variants. 
+
 
 ## Citation
 If you find our work helpful, please cite us:
 ```bibtex
 @article{llm2vec,
       title={{LLM2Vec}: {L}arge Language Models Are Secretly Powerful Text Encoders}, 
       author={Parishad BehnamGhader and Vaibhav Adlakha and Marius Mosbach and Dzmitry Bahdanau and Nicolas Chapados and Siva Reddy},
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llm2vec-0.1.5/llm2vec/dataset/E5Data.py` & `llm2vec-0.1.6/llm2vec/dataset/E5Data.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,47 +3,32 @@
 import os
 
 from .dataset import DataSample, TrainSample, Dataset
 from accelerate.logging import get_logger
 
 logger = get_logger(__name__, log_level="INFO")
 
-datasets_list = [
-    "allnli_split1",
-    "allnli_split2",
-    "dureader",
-    "eli5_question_answer",
-    "fever",
-    "hotpot_qa",
-    "miracl",
-    "mrtydi",
-    "msmarco_passage",
-    "msmarco_document",
-    "nq",
-    "quora_duplicates_split1",
-    "quora_duplicates_split2",
-    "squad",
-    "t2ranking",
-    "trivia_qa",
-]
-
 E5_EMBEDDING_PROMPTS = {
-    "allnli_split1": "Given a premise, retrieve a hypothesis that is entailed by the premise",
-    "allnli_split2": "Retrieve semantically similar text",
+    "allnli": [
+        "Given a premise, retrieve a hypothesis that is entailed by the premise",
+        "Retrieve semantically similar text",
+    ],
     "dureader": "Given a Chinese search query, retrieve web passages that answer the question",
     "eli5_question_answer": "Provided a user question, retrieve the highest voted answers on Reddit ELI5 forum",
     "fever": "Given a claim, retrieve documents that support or refute the claim",
     "hotpot_qa": "Given a multi-hop question, retrieve documents that can help answer the question",
     "miracl": "Given a question, retrieve Wikipedia passages that answer the question",
     "mrtydi": "Given a question, retrieve Wikipedia passages that answer the question",
     "msmarco_passage": "Given a web search query, retrieve relevant passages that answer the query",
     "msmarco_document": "Given a web search query, retrieve relevant documents that answer the query",
     "nq": "Given a question, retrieve Wikipedia passages that answer the question",
-    "quora_duplicates_split1": "Given a question, retrieve questions that are semantically equivalent to the given question",
-    "quora_duplicates_split2": "Find questions that have the same meaning as the input question",
+    "quora_duplicates": [
+        "Given a question, retrieve questions that are semantically equivalent to the given question",
+        "Find questions that have the same meaning as the input question",
+    ],
     "squad": "Retrieve Wikipedia passages that answer the question",
     "t2ranking": "Given a Chinese search query, retrieve web passages that answer the question",
     "trivia_qa": "Retrieve Wikipedia passages that answer the question",
 }
 
 
 class E5Data(Dataset):
@@ -71,29 +56,30 @@
     def load_data(self, file_path: str = None):
         logger.info(f"Loading E5 data from {file_path}...")
         # file path is actually a directory
 
         data_map = {}
         all_samples = []
         id_ = 0
-        for dataset in datasets_list:
+        for dataset in E5_EMBEDDING_PROMPTS:
             logger.info(f"Loading dataset {dataset}...")
             if dataset not in data_map:
                 data_map[dataset] = []
             with open(os.path.join(file_path, f"{dataset}.jsonl"), "r") as f:
                 dataset_samples = f.readlines()
 
             dataset_samples = [json.loads(d) for d in dataset_samples]
 
-            for sample in dataset_samples:
-                query = (
-                    f"{E5_EMBEDDING_PROMPTS[dataset]}; "
-                    + self.separator
-                    + sample["query"]
+            for i, sample in enumerate(dataset_samples):
+                instruction = (
+                    E5_EMBEDDING_PROMPTS[dataset]
+                    if isinstance(E5_EMBEDDING_PROMPTS[dataset], str)
+                    else E5_EMBEDDING_PROMPTS[dataset][i % 2]
                 )
+                query = f"{instruction}; " + self.separator + sample["query"]
                 if dataset in [
                     "allnli_split2",
                     "quora_duplicates_split1",
                     "quora_duplicates_split2",
                 ]:
                     pos = (
                         f"{E5_EMBEDDING_PROMPTS[dataset]}; "
```

### Comparing `llm2vec-0.1.5/llm2vec/dataset/dataset.py` & `llm2vec-0.1.6/llm2vec/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.5/llm2vec/dataset/utils.py` & `llm2vec-0.1.6/llm2vec/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.5/llm2vec/experiment_utils.py` & `llm2vec-0.1.6/llm2vec/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.5/llm2vec/llm2vec.py` & `llm2vec-0.1.6/llm2vec/llm2vec.py`

 * *Files 4% similar despite different names*

```diff
@@ -273,21 +273,40 @@
     def encode(
         self,
         sentences: Union[str, List[str]],
         batch_size: int = 32,
         show_progress_bar: bool = True,
         convert_to_numpy: bool = False,
         convert_to_tensor: bool = False,
+        device: Optional[str] = None,
     ):
+        """
+        Encode a list of sentences to their respective embeddings. The sentences can be a list of strings or a string.
+        Args:
+            sentences: sentence or sentences to encode.
+            batch_size: batch size for turning sentence tokens into embeddings.
+            show_progress_bar: whether to show progress bars during encoding steps.
+            convert_to_numpy: If true, return numpy arrays instead of torch tensors.
+            convert_to_tensor: If true, return torch tensors (default).
+            device: torch backend device identifier (e.g., 'cuda', 'cpu','mps' etc.). If not specified,
+            the default is to use cuda when available, otherwise cpu. Note that only the choice of 'cuda' supports
+            multiprocessing as currently implemented.
+
+        Returns: embeddings of the sentences.
+
+        """
         if isinstance(sentences[0], str) and isinstance(sentences[-1], int):
             sentences = [sentences]
         # required for MEDI version of MTEB
         if isinstance(sentences[0], str):
             sentences = [[""] + [sentence] for sentence in sentences]
 
+        if device is None:
+                device = "cuda" if torch.cuda.is_available() else "cpu"
+
         concatenated_input_texts = []
         for sentence in sentences:
             assert isinstance(sentence[0], str)
             assert isinstance(sentence[1], str)
             concatenated_input_texts.append(
                 self._convert_to_str(sentence[0], sentence[1])
             )
@@ -299,15 +318,15 @@
             convert_to_numpy = False
 
         length_sorted_idx = np.argsort([-self._text_length(sen) for sen in sentences])
         sentences_sorted = [sentences[idx] for idx in length_sorted_idx]
         all_embeddings = []
 
         if torch.cuda.device_count() <= 1:
-            device = "cuda" if torch.cuda.is_available() else "cpu"
+            # This branch also support mps devices
             self.to(device)
             for start_index in trange(
                 0,
                 len(sentences),
                 batch_size,
                 desc="Batches",
                 disable=not show_progress_bar,
@@ -316,24 +335,27 @@
                     start_index : start_index + batch_size
                 ]
                 embeddings = self._encode(
                     sentences_batch, device=device, convert_to_numpy=convert_to_numpy
                 )
                 all_embeddings.append(embeddings)
         else:
+
             num_proc = torch.cuda.device_count()
             cuda_compatible_multiprocess = mp.get_context("spawn")
             with cuda_compatible_multiprocess.Pool(num_proc) as p:
                 sentences_batches = [
                     sentences_sorted[start_index : start_index + batch_size]
                     for start_index in trange(0, len(sentences), batch_size)
                 ]
                 for result in p.map(
                     partial(
                         self._encode,
+                        # This branch only supports CUDA devices, so we ignore the value of device
+                        # and let _encode determine it based on rank.
                         device=None,
                         convert_to_numpy=convert_to_numpy,
                         multiprocessing=True,
                     ),
                     sentences_batches,
                 ):
                     all_embeddings.append(result)
@@ -363,16 +385,18 @@
         }
 
         if save_config:
             os.makedirs(output_path, exist_ok=True)
             with open(f"{output_path}/llm2vec_config.json", "w") as fOut:
                 json.dump(llm2vec_config, fOut, indent=4)
 
-    def _encode(self, sentences_batch, device, convert_to_numpy, multiprocessing=False):
+    def _encode(self, sentences_batch, device:Optional[str]=None, convert_to_numpy:bool=False, multiprocessing=False):
         if multiprocessing:
+            # multiprocessing only supports CUDA devices at this time, so we ignore the value of device
+            # and use cuda:rank for the device
             rank = mp.current_process()._identity[0]
             if device is None and torch.cuda.is_available():
                 device = f"cuda:{rank % torch.cuda.device_count()}"
 
         self.to(device)
         features = self.tokenize(
             [self.prepare_for_tokenization(sentence) for sentence in sentences_batch]
```

### Comparing `llm2vec-0.1.5/llm2vec/loss/HardNegativeNLLLoss.py` & `llm2vec-0.1.6/llm2vec/loss/HardNegativeNLLLoss.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.5/llm2vec/loss/loss_utils.py` & `llm2vec-0.1.6/llm2vec/loss/loss_utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.5/llm2vec/models/attn_mask_utils.py` & `llm2vec-0.1.6/llm2vec/models/attn_mask_utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.5/llm2vec/models/bidirectional_llama.py` & `llm2vec-0.1.6/llm2vec/models/bidirectional_llama.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.5/llm2vec/models/bidirectional_mistral.py` & `llm2vec-0.1.6/llm2vec/models/bidirectional_mistral.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.5/llm2vec.egg-info/SOURCES.txt` & `llm2vec-0.1.6/llm2vec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.5/setup.py` & `llm2vec-0.1.6/setup.py`

 * *Files identical despite different names*

