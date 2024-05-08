# Comparing `tmp/TokenProbs-1.0.0.tar.gz` & `tmp/TokenProbs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TokenProbs-1.0.0.tar", last modified: Fri Apr 19 16:24:54 2024, max compression
+gzip compressed data, was "TokenProbs-1.0.1.tar", last modified: Wed May  8 14:26:21 2024, max compression
```

## Comparing `TokenProbs-1.0.0.tar` & `TokenProbs-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-19 16:24:54.869172 TokenProbs-1.0.0/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 TokenProbs-1.0.0/LICENSE
--rw-r--r--   0 faf32    (50383) faf32    (50391)     4009 2024-04-19 16:24:54.868597 TokenProbs-1.0.0/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     3449 2024-04-06 21:01:27.000000 TokenProbs-1.0.0/README.md
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-19 16:24:54.865633 TokenProbs-1.0.0/TokenProbs/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-06 19:12:30.000000 TokenProbs-1.0.0/TokenProbs/__init__.py
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     9799 2024-04-19 16:05:53.000000 TokenProbs-1.0.0/TokenProbs/logit_extraction.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-19 16:24:54.868070 TokenProbs-1.0.0/TokenProbs.egg-info/
--rw-r--r--   0 faf32    (50383) faf32    (50391)     4009 2024-04-19 16:24:54.866303 TokenProbs-1.0.0/TokenProbs.egg-info/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)      249 2024-04-19 16:24:54.866761 TokenProbs-1.0.0/TokenProbs.egg-info/SOURCES.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-19 16:24:54.867264 TokenProbs-1.0.0/TokenProbs.egg-info/dependency_links.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-19 16:24:54.867789 TokenProbs-1.0.0/TokenProbs.egg-info/requires.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-19 16:24:54.868164 TokenProbs-1.0.0/TokenProbs.egg-info/top_level.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-19 16:24:54.869273 TokenProbs-1.0.0/setup.cfg
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     1181 2024-04-19 16:24:30.000000 TokenProbs-1.0.0/setup.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-05-08 14:26:21.418437 TokenProbs-1.0.1/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 TokenProbs-1.0.1/LICENSE
+-rw-r--r--   0 faf32    (50383) faf32    (50391)     4427 2024-05-08 14:26:21.417673 TokenProbs-1.0.1/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     3867 2024-04-22 17:45:18.000000 TokenProbs-1.0.1/README.md
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-05-08 14:26:21.414139 TokenProbs-1.0.1/TokenProbs/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-06 19:12:30.000000 TokenProbs-1.0.1/TokenProbs/__init__.py
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     9824 2024-05-08 14:24:51.000000 TokenProbs-1.0.1/TokenProbs/logit_extraction.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-05-08 14:26:21.416676 TokenProbs-1.0.1/TokenProbs.egg-info/
+-rw-r--r--   0 faf32    (50383) faf32    (50391)     4427 2024-05-08 14:26:20.000000 TokenProbs-1.0.1/TokenProbs.egg-info/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)      249 2024-05-08 14:26:20.000000 TokenProbs-1.0.1/TokenProbs.egg-info/SOURCES.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-05-08 14:26:20.000000 TokenProbs-1.0.1/TokenProbs.egg-info/dependency_links.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-05-08 14:26:20.000000 TokenProbs-1.0.1/TokenProbs.egg-info/requires.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-05-08 14:26:20.000000 TokenProbs-1.0.1/TokenProbs.egg-info/top_level.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-05-08 14:26:21.418525 TokenProbs-1.0.1/setup.cfg
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     1181 2024-05-08 14:26:06.000000 TokenProbs-1.0.1/setup.py
```

### Comparing `TokenProbs-1.0.0/PKG-INFO` & `TokenProbs-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TokenProbs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,22 +20,35 @@
 # TokenProbs
 
 Extract token-level probability scores from generative language models (GLMs) without fine-tuning. Often times, it is relevent to request probability assessment to binary or multi-class outcomes. GLMs are not well-suited for this task. Instead, use `LogitExtractor` to obtain label probabilities without fine-tuning.
 
 
 ## Installation
 
+Install with `pip`:
+
+```bash
+conda create -n TokenProbs python=3.9
+conda activate TokenProbs
+pip3 install TokenProbs 
+```
+
+Install via Github Repository:
 ```bash
-conda create -n GenCasting python=3.9
-pip3 install GenCasting 
+conda create -n TokenProbs python=3.9
+conda activate TokenProbs
+
+git clone https://github.com/francescoafabozzi/TokenProbs.git
+cd TokenProbs
+pip3 install -e . # Install in editable mode 
 ```
 
 __Troubling Shooting__
 
-If recieving `CUDA Setup failed despite GPU being available.` Identify the location of the cuda driver, typically found under `/usr/local/` and input the following commands via the command line. The example below shows this for cuda-12.3.:
+If recieving `CUDA Setup failed despite GPU being available.` error, identify the location of the cuda driver, typically found under `/usr/local/` and input the following commands via the command line. The example below shows this for cuda-12.3.:
 
 ```bash
 export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/cuda-12.3 # change 12.3 to appropriate location
 export BNB_CUDA_VERSION=123 # 123 (i.e., 12.3) also needs to be changed
 ```
 
 ## Usage
@@ -76,14 +89,16 @@
 text_output = extractor.text_generation(input_data,batch_size=1)
 ```
 
 ## Additional Features
 
 `LogitExtractor` also provides functionality for applying Low-rank Adaptation (LoRA) fine-tuning tailored to extracting logit scores for next-token predictions.
 
+Below is an example of fine-tuning Mistral on Financial Phrasebank, a financial sentiment classification dataset.
+
 ```python
 from datasets import load_dataset
 from TokenProbs import LogitExtractor
 
 # Load dataset
 dataset = load_dataset("financial_phrasebank",'sentences_50agree')['train']
 # Apply training and test split
@@ -120,13 +135,13 @@
 # Load model later
 trained_model = extractor(
     model_name = '<HF_USERNAME>/<MODEL_NAME>',
     quantization="8bit"
 )
 ```
 
-## Examples
+<!-- ## Examples -->
 
-Coming soon.
+<!-- Coming soon. -->
```

### Comparing `TokenProbs-1.0.0/README.md` & `TokenProbs-1.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 # TokenProbs
 
 Extract token-level probability scores from generative language models (GLMs) without fine-tuning. Often times, it is relevent to request probability assessment to binary or multi-class outcomes. GLMs are not well-suited for this task. Instead, use `LogitExtractor` to obtain label probabilities without fine-tuning.
 
 
 ## Installation
 
+Install with `pip`:
+
+```bash
+conda create -n TokenProbs python=3.9
+conda activate TokenProbs
+pip3 install TokenProbs 
+```
+
+Install via Github Repository:
 ```bash
-conda create -n GenCasting python=3.9
-pip3 install GenCasting 
+conda create -n TokenProbs python=3.9
+conda activate TokenProbs
+
+git clone https://github.com/francescoafabozzi/TokenProbs.git
+cd TokenProbs
+pip3 install -e . # Install in editable mode 
 ```
 
 __Troubling Shooting__
 
-If recieving `CUDA Setup failed despite GPU being available.` Identify the location of the cuda driver, typically found under `/usr/local/` and input the following commands via the command line. The example below shows this for cuda-12.3.:
+If recieving `CUDA Setup failed despite GPU being available.` error, identify the location of the cuda driver, typically found under `/usr/local/` and input the following commands via the command line. The example below shows this for cuda-12.3.:
 
 ```bash
 export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/cuda-12.3 # change 12.3 to appropriate location
 export BNB_CUDA_VERSION=123 # 123 (i.e., 12.3) also needs to be changed
 ```
 
 ## Usage
@@ -57,14 +70,16 @@
 text_output = extractor.text_generation(input_data,batch_size=1)
 ```
 
 ## Additional Features
 
 `LogitExtractor` also provides functionality for applying Low-rank Adaptation (LoRA) fine-tuning tailored to extracting logit scores for next-token predictions.
 
+Below is an example of fine-tuning Mistral on Financial Phrasebank, a financial sentiment classification dataset.
+
 ```python
 from datasets import load_dataset
 from TokenProbs import LogitExtractor
 
 # Load dataset
 dataset = load_dataset("financial_phrasebank",'sentences_50agree')['train']
 # Apply training and test split
@@ -101,13 +116,13 @@
 # Load model later
 trained_model = extractor(
     model_name = '<HF_USERNAME>/<MODEL_NAME>',
     quantization="8bit"
 )
 ```
 
-## Examples
+<!-- ## Examples -->
 
-Coming soon.
+<!-- Coming soon. -->
```

### Comparing `TokenProbs-1.0.0/TokenProbs/logit_extraction.py` & `TokenProbs-1.0.1/TokenProbs/logit_extraction.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
         ds = GenerativeDataset(input_text,self.tokenizer)
         collator = DataCollatorWithPadding(self.tokenizer)
         dataloader = DataLoader(ds,batch_size=batch_size,collate_fn=collator)
         
         return dataloader
 
-    def logit_extraction(self,input_data,tokens,batch_size=1):
+    def logit_extraction(self,input_data,tokens,batch_size=1,save=False):
         self.token_dict = self.identify_tokens(tokens)
         
         if type(input_data) == list:
             try:
                 input_data = self.get_dataloader(input_data,batch_size=batch_size)
             except:
                 raise ValueError('Batch size must be specified if text list is provided.')
@@ -155,20 +155,22 @@
                 # Extract predictions following end of prompt
                 generated = torch.vstack(
                     [output[i,batch['length'][i]-1,:] for i in range(len(batch['length']))]
                 )
                 preds.append(
                     softmax(generated[:,list(self.token_dict.values())],dim=-1).numpy()
                 )
+                if save != False:
+                    pd.to_pickle(save)
 
         output_df = pd.DataFrame(np.vstack(preds),columns=list(self.token_dict.keys()))
 
         return output_df
 
-    def text_generation(self,input_data,batch_size=1,max_new_tokens=100):
+    def text_generation(self,input_data,batch_size=1,max_new_tokens=100,save=False):
         self.tokenizer.padding_side = "left"
         if (type(input_data) == list) or (type(input_data) == pd.DataFrame):
             try:
                 input_data = self.get_dataloader(input_data,batch_size=batch_size)
             except:
                 raise ValueError('Batch size must be specified if text list is provided.')
         
@@ -189,24 +191,23 @@
             for batch in tqdm(input_data):
                 output = self.model.generate(
                     input_ids = batch['input_ids'].to('cuda'),
                     attention_mask = batch['attention_mask'].to('cuda'),
                     max_new_tokens = max_new_tokens
                 )
     
-                preds.extend(
-                    self.tokenizer.batch_decode(
-                        [output[i,batch['length'][i]:] for i in range(len(batch['length']))]
-                    )
-                )
+                preds.extend(self.tokenizer.batch_decode(output))
 
                 torch.cuda.empty_cache()
 
-        self.tokenizer.padding_side = "right"
-        preds = [i.replace('</s>','').replace('<s>','') for i in preds]
+                if save != False:
+                    pd.to_pickle(save)
+
+        #self.tokenizer.padding_side = "right"
+        #preds = [i.replace('</s>','').replace('<s>','') for i in preds]
         return preds
 
     def get_response_seq(self,response_seq):
         if type(response_seq) == list:
             return response_seq
         else:
             return self.tokenizer(response_seq)['input_ids'][1:]
```

### Comparing `TokenProbs-1.0.0/TokenProbs.egg-info/PKG-INFO` & `TokenProbs-1.0.1/TokenProbs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TokenProbs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,22 +20,35 @@
 # TokenProbs
 
 Extract token-level probability scores from generative language models (GLMs) without fine-tuning. Often times, it is relevent to request probability assessment to binary or multi-class outcomes. GLMs are not well-suited for this task. Instead, use `LogitExtractor` to obtain label probabilities without fine-tuning.
 
 
 ## Installation
 
+Install with `pip`:
+
+```bash
+conda create -n TokenProbs python=3.9
+conda activate TokenProbs
+pip3 install TokenProbs 
+```
+
+Install via Github Repository:
 ```bash
-conda create -n GenCasting python=3.9
-pip3 install GenCasting 
+conda create -n TokenProbs python=3.9
+conda activate TokenProbs
+
+git clone https://github.com/francescoafabozzi/TokenProbs.git
+cd TokenProbs
+pip3 install -e . # Install in editable mode 
 ```
 
 __Troubling Shooting__
 
-If recieving `CUDA Setup failed despite GPU being available.` Identify the location of the cuda driver, typically found under `/usr/local/` and input the following commands via the command line. The example below shows this for cuda-12.3.:
+If recieving `CUDA Setup failed despite GPU being available.` error, identify the location of the cuda driver, typically found under `/usr/local/` and input the following commands via the command line. The example below shows this for cuda-12.3.:
 
 ```bash
 export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/cuda-12.3 # change 12.3 to appropriate location
 export BNB_CUDA_VERSION=123 # 123 (i.e., 12.3) also needs to be changed
 ```
 
 ## Usage
@@ -76,14 +89,16 @@
 text_output = extractor.text_generation(input_data,batch_size=1)
 ```
 
 ## Additional Features
 
 `LogitExtractor` also provides functionality for applying Low-rank Adaptation (LoRA) fine-tuning tailored to extracting logit scores for next-token predictions.
 
+Below is an example of fine-tuning Mistral on Financial Phrasebank, a financial sentiment classification dataset.
+
 ```python
 from datasets import load_dataset
 from TokenProbs import LogitExtractor
 
 # Load dataset
 dataset = load_dataset("financial_phrasebank",'sentences_50agree')['train']
 # Apply training and test split
@@ -120,13 +135,13 @@
 # Load model later
 trained_model = extractor(
     model_name = '<HF_USERNAME>/<MODEL_NAME>',
     quantization="8bit"
 )
 ```
 
-## Examples
+<!-- ## Examples -->
 
-Coming soon.
+<!-- Coming soon. -->
```

### Comparing `TokenProbs-1.0.0/setup.py` & `TokenProbs-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'Extract token-level probabilities from LLMs for classification-type outputs.'
 LONG_DESCRIPTION = 'A package that allows one to extract token-level probabilities. This method can be used for example to extract sentiment class probabilities or other probability-based queries instead of parsing text-generation outputs.'
 
 # Setting up
 setup(
     name="TokenProbs",
     version=VERSION,
```

