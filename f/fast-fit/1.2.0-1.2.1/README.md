# Comparing `tmp/fast-fit-1.2.0.tar.gz` & `tmp/fast_fit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-fit-1.2.0.tar", last modified: Thu Feb 29 13:32:29 2024, max compression
+gzip compressed data, was "fast_fit-1.2.1.tar", last modified: Wed May  8 20:54:50 2024, max compression
```

## Comparing `fast-fit-1.2.0.tar` & `fast_fit-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:32:29.956027 fast-fit-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-29 13:32:26.000000 fast-fit-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-02-29 13:32:29.956027 fast-fit-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-02-29 13:32:26.000000 fast-fit-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:32:29.956027 fast-fit-1.2.0/fast_fit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-02-29 13:32:29.000000 fast-fit-1.2.0/fast_fit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-29 13:32:29.000000 fast-fit-1.2.0/fast_fit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 13:32:29.000000 fast-fit-1.2.0/fast_fit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-29 13:32:29.000000 fast-fit-1.2.0/fast_fit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-29 13:32:29.000000 fast-fit-1.2.0/fast_fit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-29 13:32:29.000000 fast-fit-1.2.0/fast_fit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 13:32:29.956027 fast-fit-1.2.0/fastfit/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-29 13:32:26.000000 fast-fit-1.2.0/fastfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-02-29 13:32:26.000000 fast-fit-1.2.0/fastfit/modeling.py
--rw-r--r--   0 runner    (1001) docker     (127)    41686 2024-02-29 13:32:26.000000 fast-fit-1.2.0/fastfit/train.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-29 13:32:26.000000 fast-fit-1.2.0/fastfit/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 13:32:29.956027 fast-fit-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-29 13:32:26.000000 fast-fit-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:54:50.532426 fast_fit-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 20:54:47.000000 fast_fit-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-05-08 20:54:50.532426 fast_fit-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-05-08 20:54:47.000000 fast_fit-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:54:50.532426 fast_fit-1.2.1/fast_fit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-05-08 20:54:50.000000 fast_fit-1.2.1/fast_fit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-08 20:54:50.000000 fast_fit-1.2.1/fast_fit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:54:50.000000 fast_fit-1.2.1/fast_fit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 20:54:50.000000 fast_fit-1.2.1/fast_fit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 20:54:50.000000 fast_fit-1.2.1/fast_fit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 20:54:50.000000 fast_fit-1.2.1/fast_fit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:54:50.532426 fast_fit-1.2.1/fastfit/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-08 20:54:47.000000 fast_fit-1.2.1/fastfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30997 2024-05-08 20:54:47.000000 fast_fit-1.2.1/fastfit/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41944 2024-05-08 20:54:47.000000 fast_fit-1.2.1/fastfit/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-08 20:54:47.000000 fast_fit-1.2.1/fastfit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:54:50.532426 fast_fit-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-08 20:54:47.000000 fast_fit-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:54:50.532426 fast_fit-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-08 20:54:47.000000 fast_fit-1.2.1/tests/test_full_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-08 20:54:47.000000 fast_fit-1.2.1/tests/test_inference_pipeline.py
```

### Comparing `fast-fit-1.2.0/LICENSE` & `fast_fit-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-fit-1.2.0/PKG-INFO` & `fast_fit-1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,10 @@
-Metadata-Version: 2.1
-Name: fast-fit
-Version: 1.2.0
-Summary: Fast and effective approach for few shot with many classes
-Home-page: https://github.com/IBM/fastfit
-Author: Elron Bandel & Asaf Yehudai
-Author-email: elron.bandel@ibm.com
-License: Apache 2.0
-Project-URL: Source, https://github.com/IBM/fastfit/
-Keywords: text classification machine learning NLP
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: transformers
-Provides-Extra: dev
-Requires-Dist: check-manifest; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Provides-Extra: test
-Requires-Dist: coverage; extra == "test"
+![fastfit_banner_white](https://github.com/IBM/fastfit/assets/23455264/a4de0a5e-b43a-462b-b1f2-9509ec873e76)
+
+FastFit, a method, and a Python package design to provide fast and accurate few-shot classification, especially for scenarios with many semantically similar classes. FastFit utilizes a novel approach integrating batch contrastive learning and token-level similarity score.  Compared to existing few-shot learning packages, such as SetFit, Transformers, or few-shot prompting of large language models via API calls, FastFit significantly improves multi-class classification performance in speed and accuracy across FewMany, our newly curated English benchmark, and Multilingual datasets. FastFit demonstrates a 3-20x improvement in training speed, completing training in just a few seconds.
 
 ## Running the Training Script
 
 Our package provides a convenient command-line tool `train_fastfit` to train text classification models. This tool comes with a variety of configurable parameters to customize your training process.
 
 ### Prerequisites
 
@@ -82,23 +57,23 @@
 You can simply run it with your python
 
 ```python
 from datasets import load_dataset
 from fastfit import FastFitTrainer, sample_dataset
 
 # Load a dataset from the Hugging Face Hub
-dataset = load_dataset("mteb/banking77")
+dataset = load_dataset("FastFit/banking_77")
 dataset["validation"] = dataset["test"]
 
 # Down sample the train data for 5-shot training
-dataset["train"] = sample_dataset(dataset["train"], label_column="label_text", num_samples_per_label=5)
+dataset["train"] = sample_dataset(dataset["train"], label_column="label", num_samples_per_label=5)
 
 trainer = FastFitTrainer(
     model_name_or_path="roberta-base",
-    label_column_name="label_text",
+    label_column_name="label",
     text_column_name="text",
     num_train_epochs=40,
     per_device_train_batch_size=32,
     per_device_eval_batch_size=64,
     max_text_length=128,
     dataloader_drop_last=False,
     num_repeats=4,
```

### Comparing `fast-fit-1.2.0/README.md` & `fast_fit-1.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: fast-fit
+Version: 1.2.1
+Summary: Fast and effective approach for few shot with many classes
+Home-page: https://github.com/IBM/fastfit
+Author: Elron Bandel & Asaf Yehudai
+Author-email: elron.bandel@ibm.com
+License: Apache 2.0
+Project-URL: Source, https://github.com/IBM/fastfit/
+Keywords: text classification machine learning NLP
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: transformers[torch]
+Requires-Dist: scikit-learn
+Requires-Dist: datasets
+Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+
+![fastfit_banner_white](https://github.com/IBM/fastfit/assets/23455264/a4de0a5e-b43a-462b-b1f2-9509ec873e76)
+
+FastFit, a method, and a Python package design to provide fast and accurate few-shot classification, especially for scenarios with many semantically similar classes. FastFit utilizes a novel approach integrating batch contrastive learning and token-level similarity score.  Compared to existing few-shot learning packages, such as SetFit, Transformers, or few-shot prompting of large language models via API calls, FastFit significantly improves multi-class classification performance in speed and accuracy across FewMany, our newly curated English benchmark, and Multilingual datasets. FastFit demonstrates a 3-20x improvement in training speed, completing training in just a few seconds.
+
 ## Running the Training Script
 
 Our package provides a convenient command-line tool `train_fastfit` to train text classification models. This tool comes with a variety of configurable parameters to customize your training process.
 
 ### Prerequisites
 
 Before running the training script, ensure you have Python installed along with our package and its dependencies. If you haven't already installed our package, you can do so using pip:
@@ -53,23 +88,23 @@
 You can simply run it with your python
 
 ```python
 from datasets import load_dataset
 from fastfit import FastFitTrainer, sample_dataset
 
 # Load a dataset from the Hugging Face Hub
-dataset = load_dataset("mteb/banking77")
+dataset = load_dataset("FastFit/banking_77")
 dataset["validation"] = dataset["test"]
 
 # Down sample the train data for 5-shot training
-dataset["train"] = sample_dataset(dataset["train"], label_column="label_text", num_samples_per_label=5)
+dataset["train"] = sample_dataset(dataset["train"], label_column="label", num_samples_per_label=5)
 
 trainer = FastFitTrainer(
     model_name_or_path="roberta-base",
-    label_column_name="label_text",
+    label_column_name="label",
     text_column_name="text",
     num_train_epochs=40,
     per_device_train_batch_size=32,
     per_device_eval_batch_size=64,
     max_text_length=128,
     dataloader_drop_last=False,
     num_repeats=4,
```

### Comparing `fast-fit-1.2.0/fast_fit.egg-info/PKG-INFO` & `fast_fit-1.2.1/fast_fit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-fit
-Version: 1.2.0
+Version: 1.2.1
 Summary: Fast and effective approach for few shot with many classes
 Home-page: https://github.com/IBM/fastfit
 Author: Elron Bandel & Asaf Yehudai
 Author-email: elron.bandel@ibm.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/IBM/fastfit/
 Keywords: text classification machine learning NLP
@@ -16,21 +16,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
-Requires-Dist: transformers
+Requires-Dist: transformers[torch]
+Requires-Dist: scikit-learn
+Requires-Dist: datasets
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
+![fastfit_banner_white](https://github.com/IBM/fastfit/assets/23455264/a4de0a5e-b43a-462b-b1f2-9509ec873e76)
+
+FastFit, a method, and a Python package design to provide fast and accurate few-shot classification, especially for scenarios with many semantically similar classes. FastFit utilizes a novel approach integrating batch contrastive learning and token-level similarity score.  Compared to existing few-shot learning packages, such as SetFit, Transformers, or few-shot prompting of large language models via API calls, FastFit significantly improves multi-class classification performance in speed and accuracy across FewMany, our newly curated English benchmark, and Multilingual datasets. FastFit demonstrates a 3-20x improvement in training speed, completing training in just a few seconds.
+
 ## Running the Training Script
 
 Our package provides a convenient command-line tool `train_fastfit` to train text classification models. This tool comes with a variety of configurable parameters to customize your training process.
 
 ### Prerequisites
 
 Before running the training script, ensure you have Python installed along with our package and its dependencies. If you haven't already installed our package, you can do so using pip:
@@ -82,23 +88,23 @@
 You can simply run it with your python
 
 ```python
 from datasets import load_dataset
 from fastfit import FastFitTrainer, sample_dataset
 
 # Load a dataset from the Hugging Face Hub
-dataset = load_dataset("mteb/banking77")
+dataset = load_dataset("FastFit/banking_77")
 dataset["validation"] = dataset["test"]
 
 # Down sample the train data for 5-shot training
-dataset["train"] = sample_dataset(dataset["train"], label_column="label_text", num_samples_per_label=5)
+dataset["train"] = sample_dataset(dataset["train"], label_column="label", num_samples_per_label=5)
 
 trainer = FastFitTrainer(
     model_name_or_path="roberta-base",
-    label_column_name="label_text",
+    label_column_name="label",
     text_column_name="text",
     num_train_epochs=40,
     per_device_train_batch_size=32,
     per_device_eval_batch_size=64,
     max_text_length=128,
     dataloader_drop_last=False,
     num_repeats=4,
```

### Comparing `fast-fit-1.2.0/fastfit/modeling.py` & `fast_fit-1.2.1/fastfit/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from transformers import (
     AutoModel,
     AutoConfig,
     AutoTokenizer,
     PreTrainedModel,
     AutoModelForMaskedLM,
 )
+from transformers.modeling_outputs import SequenceClassifierOutput
 
 from transformers.configuration_utils import PretrainedConfig
 from transformers.utils import logging
 
 logger = logging.get_logger(__name__)
 
 
@@ -148,24 +149,31 @@
     )
     pretrain_mode: Optional[bool] = field(
         default=False, metadata={"help": "Whether to do pre-training."}
     )
     inference_type: Optional[str] = field(
         default="sim", metadata={"help": "The inference type to be used."}
     )
+    inference_direction: Optional[str] = field(
+        default="doc", metadata={"help": "The inference direction to be used from doc/query/both."}
+    )
     rep_tokens: Optional[str] = field(
         default="all",
         metadata={
             "help": "The tokens to use for representation when calculating the similarity in training and inference."
         },
     )
     length_norm: Optional[bool] = field(
         default=True,
         metadata={"help": "Whether to normalize by length while considering pad"},
     )
+    length_norm_at_inference: Optional[bool] = field(
+        default=False,
+        metadata={"help": "Whether to normalize by length at inference"},
+    )
     mlm_factor: Optional[float] = field(
         default=0.0, metadata={"help": "The factor to scale the MLM loss."}
     )
     mask_prob: Optional[float] = field(
         default=0.0, metadata={"help": "The probability of masking a token."}
     )
     clf_level: Optional[str] = field(
@@ -211,14 +219,15 @@
         mlm_factor=0.0,
         mask_prob=0.15,
         pretrain_mode=False,
         length_norm=True,  # wether to noramlize scores by length
         scores_temp=0.07,
         inference_direction="doc",
         symetric_mode=True,
+        length_norm_at_inference=False,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.all_docs = all_docs
         self.num_repeats = num_repeats
         self.rep_tokens = rep_tokens
@@ -240,14 +249,15 @@
         self.pretrain_mode = pretrain_mode
         self.length_norm = length_norm
         self.scores_temp = scores_temp
         self.inference_direction = inference_direction
         self.mlm_prob = mask_prob
         self.mask_prob = mask_prob
         self.symetric_mode = symetric_mode
+        self.length_norm_at_inference = length_norm_at_inference
 
         assert inference_direction in ["query", "doc", "both"]
         assert "encoder" in kwargs, "Config has to be initialized with encoder config"
         encoder_config = kwargs.pop("encoder")
         encoder_model_type = encoder_config.pop("model_type")
         self.encoder = AutoConfig.for_model(encoder_model_type, **encoder_config)
         self.hidden_size = self.encoder.hidden_size
@@ -456,48 +466,45 @@
 
                 if self.config.inference_direction == "query":
                     scores = self.tokens_similarity(
                         query,
                         doc,
                         query_attention_mask,
                         doc_attention_mask,
-                        with_lens_norm=False,
+                        with_lens_norm=self.config.length_norm_at_inference,
                     ).T
                 elif self.config.inference_direction == "doc":
                     scores = self.tokens_similarity(
                         doc,
                         query,
                         doc_attention_mask,
                         query_attention_mask,
-                        with_lens_norm=False,
+                        with_lens_norm=self.config.length_norm_at_inference,
                     )
                 elif self.config.inference_direction == "both":
                     first = self.tokens_similarity(
                         query,
                         doc,
                         query_attention_mask,
                         doc_attention_mask,
-                        with_lens_norm=False,
+                        with_lens_norm=self.config.length_norm_at_inference,
                     ).T
                     second = self.tokens_similarity(
                         doc,
                         query,
                         doc_attention_mask,
                         query_attention_mask,
-                        with_lens_norm=False,
+                        with_lens_norm=self.config.length_norm_at_inference,
                     )
                     scores = (first + second) / 2
 
             elif self.config.inference_type == "clf":
-                _, scores = self.clf_loss(
+                scores = self.clf_loss(
                     query_encodings,
-                    doc_encodings,
                     query_attention_mask,
-                    doc_attention_mask,
-                    return_scores=True,
                 )
 
         return scores
 
     def prepare_inputs(
         self,
         query_input_ids,
@@ -535,16 +542,16 @@
 
         return self.normalize(projected)
 
     def forward(
         self,
         query_input_ids,
         query_attention_mask,
-        doc_input_ids,
-        doc_attention_mask,
+        doc_input_ids=None,
+        doc_attention_mask=None,
         labels=None,
     ):
         scores = None
         if not self.training:
             scores = self.inference_forward(query_input_ids, query_attention_mask)
 
         (
@@ -589,15 +596,18 @@
             mlm_loss = self.mlm_loss(query_encodings, mlm_labels)
             total_loss += mlm_loss * self.config.mlm_factor
 
         if self.config.clf_factor > 0.0 and not self.config.pretrain_mode:
             clf_loss = self.clf_loss(query_encodings, query_attention_mask, labels)
             total_loss += clf_loss * self.config.clf_factor
 
-        return total_loss, scores
+        return SequenceClassifierOutput(
+            loss=total_loss,
+            logits=scores,
+        )
 
     def sim_loss(
         self,
         query_projections,
         doc_projections,
         query_attention_mask,
         doc_attention_mask,
@@ -636,15 +646,15 @@
         input_mask_expanded = (
             attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
         )
         return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(
             input_mask_expanded.sum(1), min=1e-9
         )
 
-    def clf_loss(self, encodings, attention_mask, labels, return_scores=False):
+    def clf_loss(self, encodings, attention_mask, labels=None):
         if self.config.clf_level == "token":
             x = (encodings.last_hidden_state).permute(0, 2, 1)
             logits = (
                 (
                     self.clf.weight.view(
                         self.config.head_token_size, self.inner_dim, -1
                     ).permute(2, 0, 1)
@@ -664,20 +674,19 @@
             cls = self.mean_pooling(encodings, attention_mask)
             cls = torch.nn.functional.normalize(cls, p=2, dim=1)
             logits = self.clf(cls)
         else:
             raise ValueError("Unknown clf level: {}".format(self.config.clf_level))
 
         clf_scores = logits / self.config.clf_dim
-        clf_loss = self.clf_criterion(clf_scores, labels)
 
-        if return_scores:
-            return clf_loss, clf_scores
+        if labels is None:
+            return clf_scores
 
-        return clf_loss
+        return self.clf_criterion(clf_scores, labels)
 
     def mlm_loss(self, encodings, mlm_lables):
         sequence_output = encodings[0]
         prediction_scores = self.lm_head(sequence_output)
         vocab_size = (
             self.tokenizer.vocab_size
             if self.encoder.config.model_type != "deberta-v2"
@@ -823,14 +832,16 @@
 
         # The rest of the time (10% of the time) we keep the masked input tokens unchanged
         return inputs, labels
 
 
 class FastFit(FastFitTrainable):
     def forward(self, input_ids, attention_mask, labels=None):
-        return {"logits": [super().inference_forward(input_ids, attention_mask)]}
+        return SequenceClassifierOutput(
+            logits=self.inference_forward(input_ids, attention_mask),
+        )
 
 
 # main tests:
 
 if __name__ == "__main__":
     model = FastFitTrainable.from_pretrined_encoder("roberta-base")
```

### Comparing `fast-fit-1.2.0/fastfit/train.py` & `fast_fit-1.2.1/fastfit/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import random
 import sys
 import json
 import math
 import tempfile
+import uuid
 
 from dataclasses import dataclass, field
 from collections import Counter, defaultdict
 from typing import Optional
 
 import torch
 import datasets
@@ -28,15 +29,15 @@
     set_seed,
 )
 from transformers.trainer_utils import get_last_checkpoint
 from transformers.utils.versions import require_version
 
 from transformers.integrations import INTEGRATION_TO_CALLBACK
 from .modeling import ConfigArguments
-from .modeling import FastFitTrainable, FastFitConfig
+from .modeling import FastFitTrainable, FastFit, FastFitConfig
 
 INTEGRATION_TO_CALLBACK["clearml"] = INTEGRATION_TO_CALLBACK["tensorboard"]
 
 require_version(
     "datasets>=1.8.0",
     "To fix: pip install -r examples/pytorch/text-classification/requirements.txt",
 )
@@ -871,15 +872,15 @@
         if self.training_args.do_train:
             for index in random.sample(range(len(self.train_dataset)), 3):
                 logger.info(
                     f"Sample {index} of the training set: {self.train_dataset[index]}."
                 )
 
     def set_trainer(self):
-        metric = load_metric(self.data_args.metric_name)
+        metric = load_metric(self.data_args.metric_name, experiment_id=uuid.uuid4())
 
         # You can define your custom compute_metrics function. It takes an `EvalPrediction` object (a namedtuple with a
         # predictions and label_ids field) and has to return a dictionary string to float.
         def compute_metrics(p: EvalPrediction):
             predictions = (
                 p.predictions[0] if isinstance(p.predictions, tuple) else p.predictions
             )
@@ -954,14 +955,20 @@
         self.set_seed()
         self.set_data()
         self.set_tokenizer()
         self.set_model()
         self.preprocess_data()
         self.set_trainer()
 
+    def export_model(self):
+        with tempfile.TemporaryDirectory() as temp_dir:
+            self.model.save_pretrained(temp_dir)
+            model = FastFit.from_pretrained(temp_dir)
+        return model
+
     def train(self):
         # Training
         if self.training_args.do_train:
             train_result = self.trainer.train(
                 resume_from_checkpoint=self.checkpoint,
                 ignore_keys_for_eval={"doc_input_ids", "doc_attention_mask", "labels"},
             )
```

### Comparing `fast-fit-1.2.0/fastfit/utils.py` & `fast_fit-1.2.1/fastfit/utils.py`

 * *Files identical despite different names*

### Comparing `fast-fit-1.2.0/setup.py` & `fast_fit-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read requirements.txt and use it for the install_requires parameter
 with open("./requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="fast-fit",
-    version="1.2.0",
+    version="1.2.1",
     description="Fast and effective approach for few shot with many classes",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/IBM/fastfit",
     author="Elron Bandel & Asaf Yehudai",
     author_email="elron.bandel@ibm.com",
     license="Apache 2.0",
```

