# Comparing `tmp/dragon_baseline-0.2.0.tar.gz` & `tmp/dragon_baseline-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragon_baseline-0.2.0.tar", last modified: Fri May  3 12:01:10 2024, max compression
+gzip compressed data, was "dragon_baseline-0.2.1.tar", last modified: Wed May  8 12:37:53 2024, max compression
```

## Comparing `dragon_baseline-0.2.0.tar` & `dragon_baseline-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 12:01:10.969351 dragon_baseline-0.2.0/
--rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2023-10-10 15:36:12.000000 dragon_baseline-0.2.0/LICENSE
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1428 2024-05-03 12:01:10.969283 dragon_baseline-0.2.0/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)      136 2023-11-13 10:41:08.000000 dragon_baseline-0.2.0/README.md
--rw-r--r--   0 joeranbosma   (501) staff       (20)      504 2023-11-02 16:39:08.000000 dragon_baseline-0.2.0/pyproject.toml
--rw-r--r--   0 joeranbosma   (501) staff       (20)      879 2024-05-03 12:01:10.969712 dragon_baseline-0.2.0/setup.cfg
--rw-r--r--   0 joeranbosma   (501) staff       (20)      736 2024-05-03 11:58:27.000000 dragon_baseline-0.2.0/setup.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 12:01:10.962697 dragon_baseline-0.2.0/src/
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 12:01:10.966286 dragon_baseline-0.2.0/src/dragon_baseline/
--rw-r--r--   0 joeranbosma   (501) staff       (20)       85 2023-11-13 10:46:15.000000 dragon_baseline-0.2.0/src/dragon_baseline/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1346 2024-03-05 15:10:45.000000 dragon_baseline-0.2.0/src/dragon_baseline/__main__.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 12:01:10.968241 dragon_baseline-0.2.0/src/dragon_baseline/architectures/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2023-11-13 10:43:50.000000 dragon_baseline-0.2.0/src/dragon_baseline/architectures/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5957 2023-11-13 10:46:35.000000 dragon_baseline-0.2.0/src/dragon_baseline/architectures/clf_multi_head.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7494 2023-11-13 10:47:28.000000 dragon_baseline-0.2.0/src/dragon_baseline/architectures/ner_multi_head.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5752 2023-11-13 10:47:35.000000 dragon_baseline-0.2.0/src/dragon_baseline/architectures/reg_multi_head.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    33112 2024-05-03 11:54:34.000000 dragon_baseline-0.2.0/src/dragon_baseline/main.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    18567 2024-03-05 15:10:45.000000 dragon_baseline-0.2.0/src/dragon_baseline/nlp_algorithm.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    34016 2023-11-02 16:39:08.000000 dragon_baseline-0.2.0/src/dragon_baseline/run_classification.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    35990 2023-11-02 16:39:08.000000 dragon_baseline-0.2.0/src/dragon_baseline/run_classification_multi_label.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    29097 2023-11-02 16:39:08.000000 dragon_baseline-0.2.0/src/dragon_baseline/run_ner.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-03 12:01:10.968600 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1428 2024-05-03 12:01:10.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)      765 2024-05-03 12:01:10.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/SOURCES.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2024-05-03 12:01:10.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/dependency_links.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-11-13 11:58:50.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/not-zip-safe
--rw-r--r--   0 joeranbosma   (501) staff       (20)      177 2024-05-03 12:01:10.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/requires.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)       16 2024-05-03 12:01:10.000000 dragon_baseline-0.2.0/src/dragon_baseline.egg-info/top_level.txt
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-08 12:37:53.329367 dragon_baseline-0.2.1/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2023-10-10 15:36:12.000000 dragon_baseline-0.2.1/LICENSE
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1428 2024-05-08 12:37:53.329284 dragon_baseline-0.2.1/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      136 2024-05-08 11:38:49.000000 dragon_baseline-0.2.1/README.md
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      504 2023-11-02 16:39:08.000000 dragon_baseline-0.2.1/pyproject.toml
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      879 2024-05-08 12:37:53.329818 dragon_baseline-0.2.1/setup.cfg
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      736 2024-05-08 11:41:02.000000 dragon_baseline-0.2.1/setup.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-08 12:37:53.321778 dragon_baseline-0.2.1/src/
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-08 12:37:53.325708 dragon_baseline-0.2.1/src/dragon_baseline/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       85 2023-11-13 10:46:15.000000 dragon_baseline-0.2.1/src/dragon_baseline/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1346 2024-03-05 15:10:45.000000 dragon_baseline-0.2.1/src/dragon_baseline/__main__.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-08 12:37:53.328268 dragon_baseline-0.2.1/src/dragon_baseline/architectures/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2023-11-13 10:43:50.000000 dragon_baseline-0.2.1/src/dragon_baseline/architectures/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     6028 2024-05-08 12:32:22.000000 dragon_baseline-0.2.1/src/dragon_baseline/architectures/clf_multi_head.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7565 2024-05-08 12:32:27.000000 dragon_baseline-0.2.1/src/dragon_baseline/architectures/ner_multi_head.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5823 2024-05-08 12:32:09.000000 dragon_baseline-0.2.1/src/dragon_baseline/architectures/reg_multi_head.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    32960 2024-05-08 12:33:21.000000 dragon_baseline-0.2.1/src/dragon_baseline/main.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    18567 2024-03-05 15:10:45.000000 dragon_baseline-0.2.1/src/dragon_baseline/nlp_algorithm.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    34016 2023-11-02 16:39:08.000000 dragon_baseline-0.2.1/src/dragon_baseline/run_classification.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    35990 2023-11-02 16:39:08.000000 dragon_baseline-0.2.1/src/dragon_baseline/run_classification_multi_label.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    29174 2024-05-08 11:34:55.000000 dragon_baseline-0.2.1/src/dragon_baseline/run_ner.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-08 12:37:53.328470 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1428 2024-05-08 12:37:53.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      765 2024-05-08 12:37:53.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/SOURCES.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2024-05-08 12:37:53.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/dependency_links.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-11-13 11:58:50.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/not-zip-safe
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      177 2024-05-08 12:37:53.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/requires.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       16 2024-05-08 12:37:53.000000 dragon_baseline-0.2.1/src/dragon_baseline.egg-info/top_level.txt
```

### Comparing `dragon_baseline-0.2.0/LICENSE` & `dragon_baseline-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.0/PKG-INFO` & `dragon_baseline-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragon_baseline
-Version: 0.2.0
+Version: 0.2.1
 Summary: Baseline training algorithm for the DRAGON Challenge
 Home-page: https://github.com/DIAGNijmegen/dragon_baseline
 Author: Joeran Bosma
 Author-email: Joeran.Bosma@radboudumc.nl
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dragon_baseline/issues
 Platform: unix
 Platform: linux
```

### Comparing `dragon_baseline-0.2.0/setup.cfg` & `dragon_baseline-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.0/setup.py` & `dragon_baseline-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 if __name__ == "__main__":
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
-        version="0.2.0",
+        version="0.2.1",
         author_email="Joeran.Bosma@radboudumc.nl",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/DIAGNijmegen/dragon_baseline",
         project_urls={
             "Bug Tracker": "https://github.com/DIAGNijmegen/dragon_baseline/issues"
         },
```

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline/__main__.py` & `dragon_baseline-0.2.1/src/dragon_baseline/__main__.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline/architectures/__init__.py` & `dragon_baseline-0.2.1/src/dragon_baseline/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline/architectures/clf_multi_head.py` & `dragon_baseline-0.2.1/src/dragon_baseline/architectures/clf_multi_head.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,25 @@
 from transformers import (AutoConfig, AutoModel,
                           AutoModelForSequenceClassification, PretrainedConfig,
                           PreTrainedModel)
 from transformers.modeling_outputs import SequenceClassifierOutput
 
 
 class AutoModelForMultiHeadSequenceClassificationConfig(PretrainedConfig):
-    model_type="AutoModelForMultiHeadSequenceClassification"
+    model_type = "AutoModelForMultiHeadSequenceClassification"
 
     def __init__(self, pretrained_model_name_or_path: Union[Path, str] = "bert-base-multilingual-cased", num_classes_per_label: Iterable[int] = (5, 7), **kwargs):
         super().__init__(num_labels=sum(num_classes_per_label), **kwargs)
         self.num_classes_per_label = num_classes_per_label
         self.pretrained_model_name_or_path = pretrained_model_name_or_path
 
 
 class AutoModelForMultiHeadSequenceClassification(PreTrainedModel):
     config_class = AutoModelForMultiHeadSequenceClassificationConfig
+    supports_gradient_checkpointing = True
 
     """
     This class is a wrapper around the AutoModelForSequenceClassification class
     that allows for multi-head classification with two sets of labels.
     """
 
     def __init__(self, config: AutoModelForMultiHeadSequenceClassificationConfig, *args, **kwargs):
@@ -49,14 +50,16 @@
         self.model = AutoModelForSequenceClassification.from_pretrained(
             config.pretrained_model_name_or_path,
             num_labels=config.num_labels,
             ignore_mismatched_sizes=True,
             *args, **kwargs
         )
 
+        self.post_init()
+
     # adapted from https://github.com/huggingface/transformers/blob/faed2ca46fb163082d154aa234fd5d30682d6bf1/src/transformers/models/bert/modeling_bert.py#L1541
     def forward(
         self,
         input_ids: Optional[torch.Tensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
         token_type_ids: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.Tensor] = None,
```

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline/architectures/ner_multi_head.py` & `dragon_baseline-0.2.1/src/dragon_baseline/architectures/ner_multi_head.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,25 +70,26 @@
                 decoded_label.append(id2label[lbl])
         decoded_labels.append(decoded_label)
 
     return decoded_labels
 
 
 class AutoModelForMultiHeadTokenClassificationConfig(PretrainedConfig):
-    model_type="AutoModelForMultiHeadTokenClassification"
+    model_type = "AutoModelForMultiHeadTokenClassification"
 
     def __init__(self, pretrained_model_name_or_path: Union[Path, str] = "bert-base-multilingual-cased", num_labels: int = 5, **kwargs):
         # don't change the order of the lines below
         super().__init__(num_labels=num_labels, **kwargs)
         self.pretrained_model_name_or_path = pretrained_model_name_or_path
         self.real_num_labels = num_labels
 
 
 class AutoModelForMultiHeadTokenClassification(PreTrainedModel):
     config_class = AutoModelForMultiHeadTokenClassificationConfig
+    supports_gradient_checkpointing = True
 
     """
     This class is a wrapper around the AutoModelForTokenClassification class
     that allows for multi-head binary named entity recognition..
     """
 
     def __init__(self, config: AutoModelForMultiHeadTokenClassificationConfig, *args, **kwargs):
@@ -98,14 +99,16 @@
         self.model = AutoModelForTokenClassification.from_pretrained(
             config.pretrained_model_name_or_path,
             num_labels=config.num_labels,
             ignore_mismatched_sizes=True,
             *args, **kwargs
         )
 
+        self.post_init()
+
         self.id2label = generate_id_to_label_dict(config.num_labels)
 
 
     # adapted from https://github.com/huggingface/transformers/blob/faed2ca46fb163082d154aa234fd5d30682d6bf1/src/transformers/models/bert/modeling_bert.py#L1541
     def forward(
         self,
         input_ids: Optional[torch.Tensor] = None,
```

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline/architectures/reg_multi_head.py` & `dragon_baseline-0.2.1/src/dragon_baseline/architectures/reg_multi_head.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,25 @@
 from transformers.modeling_outputs import SequenceClassifierOutput
 
 # For documentation on sharing custom models, plaese see:
 # https://huggingface.co/docs/transformers/custom_models#registering-a-model-with-custom-code-to-the-auto-classes
 
 
 class AutoModelForMultiHeadSequenceRegressionConfig(PretrainedConfig):
-    model_type="AutoModelForMultiHeadSequenceRegression"
+    model_type = "AutoModelForMultiHeadSequenceRegression"
 
     def __init__(self, pretrained_model_name_or_path: Union[Path, str] = "bert-base-multilingual-cased", num_labels: int = 5, filter_targets: bool = True, **kwargs):
         super().__init__(num_labels=num_labels, **kwargs)
         self.pretrained_model_name_or_path = pretrained_model_name_or_path
         self.filter_targets = filter_targets
 
 
 class AutoModelForMultiHeadSequenceRegression(PreTrainedModel):
     config_class = AutoModelForMultiHeadSequenceRegressionConfig
+    supports_gradient_checkpointing = True
 
     """
     This class is a wrapper around the AutoModelForSequenceClassification class
     that allows for multi-head regression with multiple sets of labels.
     """
 
     def __init__(self, config: AutoModelForMultiHeadSequenceRegressionConfig, *args, **kwargs):
@@ -51,14 +52,16 @@
         self.model = AutoModelForSequenceClassification.from_pretrained(
             config.pretrained_model_name_or_path,
             num_labels=config.num_labels,
             ignore_mismatched_sizes=True,
             *args, **kwargs
         )
 
+        self.post_init()
+
     # adapted from https://github.com/huggingface/transformers/blob/faed2ca46fb163082d154aa234fd5d30682d6bf1/src/transformers/models/bert/modeling_bert.py#L1541
     def forward(
         self,
         input_ids: Optional[torch.Tensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
         token_type_ids: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.Tensor] = None,
```

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline/main.py` & `dragon_baseline-0.2.1/src/dragon_baseline/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,24 +27,21 @@
 from transformers import (AutoModelForSequenceClassification,
                           AutoModelForTokenClassification, AutoTokenizer,
                           TokenClassificationPipeline)
 from transformers.modeling_outputs import SequenceClassifierOutput
 
 from dragon_baseline.architectures.clf_multi_head import \
     AutoModelForMultiHeadSequenceClassification
-from dragon_baseline.architectures.ner_multi_head import \
-    AutoModelForMultiHeadTokenClassification
 from dragon_baseline.architectures.reg_multi_head import \
     AutoModelForMultiHeadSequenceRegression
 from dragon_baseline.nlp_algorithm import NLPAlgorithm, ProblemType
 
 __all__ = [
     # expose the algorithm classes
     "AutoModelForMultiHeadSequenceClassification",
-    "AutoModelForMultiHeadTokenClassification",
     "AutoModelForMultiHeadSequenceRegression",
 ]
 
 class CustomLogScaler(TransformerMixin, BaseEstimator):
     def __init__(self):
         self.standard_scaler = StandardScaler()
```

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline/nlp_algorithm.py` & `dragon_baseline-0.2.1/src/dragon_baseline/nlp_algorithm.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline/run_classification.py` & `dragon_baseline-0.2.1/src/dragon_baseline/run_classification.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline/run_classification_multi_label.py` & `dragon_baseline-0.2.1/src/dragon_baseline/run_classification_multi_label.py`

 * *Files identical despite different names*

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline/run_ner.py` & `dragon_baseline-0.2.1/src/dragon_baseline/run_ner.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
         cache_dir=model_args.cache_dir,
         revision=model_args.model_revision,
         token=model_args.token,
         trust_remote_code=model_args.trust_remote_code,
     )
 
     tokenizer_name_or_path = model_args.tokenizer_name if model_args.tokenizer_name else model_args.model_name_or_path
-    if config.model_type in {"bloom", "gpt2", "roberta"}:
+    if config.model_type in {"bloom", "gpt2", "roberta", "longformer", "bert"}:
         tokenizer = AutoTokenizer.from_pretrained(
             tokenizer_name_or_path,
             cache_dir=model_args.cache_dir,
             use_fast=True,
             revision=model_args.model_revision,
             token=model_args.token,
             trust_remote_code=model_args.trust_remote_code,
@@ -406,14 +406,15 @@
         tokenizer = AutoTokenizer.from_pretrained(
             tokenizer_name_or_path,
             cache_dir=model_args.cache_dir,
             use_fast=True,
             revision=model_args.model_revision,
             token=model_args.token,
             trust_remote_code=model_args.trust_remote_code,
+            truncation_side=data_args.truncation_side,
         )
 
     model = AutoModelForTokenClassification.from_pretrained(
         model_args.model_name_or_path,
         from_tf=bool(".ckpt" in model_args.model_name_or_path),
         config=config,
         cache_dir=model_args.cache_dir,
```

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline.egg-info/PKG-INFO` & `dragon_baseline-0.2.1/src/dragon_baseline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragon_baseline
-Version: 0.2.0
+Version: 0.2.1
 Summary: Baseline training algorithm for the DRAGON Challenge
 Home-page: https://github.com/DIAGNijmegen/dragon_baseline
 Author: Joeran Bosma
 Author-email: Joeran.Bosma@radboudumc.nl
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dragon_baseline/issues
 Platform: unix
 Platform: linux
```

### Comparing `dragon_baseline-0.2.0/src/dragon_baseline.egg-info/SOURCES.txt` & `dragon_baseline-0.2.1/src/dragon_baseline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

