# Comparing `tmp/alegant-1.0.4.tar.gz` & `tmp/alegant-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dutir_exp_4t/zhuhaohao/Projects/alegant/dist/.tmp-17qgn74f/alegant-1.0.4.tar", last modified: Fri Jan 12 09:27:36 2024, max compression
+gzip compressed data, was "/home/dutir_exp_4t/zhuhaohao/Projects/alegant/dist/.tmp-_1iavo4m/alegant-1.0.5.tar", last modified: Wed May  8 17:48:53 2024, max compression
```

## Comparing `alegant-1.0.4.tar` & `alegant-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 zhuhaohao  (1019) dutir     (1000)        0 2024-01-12 09:27:36.000000 alegant-1.0.4/
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     1061 2024-01-12 06:46:10.000000 alegant-1.0.4/LICENSE
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     1963 2024-01-12 09:27:36.000000 alegant-1.0.4/PKG-INFO
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     1524 2024-01-12 08:03:26.000000 alegant-1.0.4/README.md
-drwxr-xr-x   0 zhuhaohao  (1019) dutir     (1000)        0 2024-01-12 09:27:36.000000 alegant-1.0.4/alegant/
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)      101 2024-01-12 06:51:31.000000 alegant-1.0.4/alegant/__init__.py
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     5155 2024-01-12 06:51:31.000000 alegant-1.0.4/alegant/data_module.py
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)    16806 2024-01-12 06:51:31.000000 alegant-1.0.4/alegant/trainer.py
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     1410 2024-01-12 06:51:31.000000 alegant-1.0.4/alegant/utils.py
-drwxr-xr-x   0 zhuhaohao  (1019) dutir     (1000)        0 2024-01-12 09:27:36.000000 alegant-1.0.4/alegant.egg-info/
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     1963 2024-01-12 09:27:36.000000 alegant-1.0.4/alegant.egg-info/PKG-INFO
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)      259 2024-01-12 09:27:36.000000 alegant-1.0.4/alegant.egg-info/SOURCES.txt
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)        1 2024-01-12 09:27:36.000000 alegant-1.0.4/alegant.egg-info/dependency_links.txt
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)       56 2024-01-12 09:27:36.000000 alegant-1.0.4/alegant.egg-info/requires.txt
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)        8 2024-01-12 09:27:36.000000 alegant-1.0.4/alegant.egg-info/top_level.txt
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)       38 2024-01-12 09:27:36.000000 alegant-1.0.4/setup.cfg
--rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     1040 2024-01-12 09:27:17.000000 alegant-1.0.4/setup.py
+drwxr-xr-x   0 zhuhaohao  (1019) dutir     (1000)        0 2024-05-08 17:48:53.000000 alegant-1.0.5/
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     1061 2024-01-12 06:46:10.000000 alegant-1.0.5/LICENSE
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     2503 2024-05-08 17:48:53.000000 alegant-1.0.5/PKG-INFO
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     2064 2024-01-15 06:08:11.000000 alegant-1.0.5/README.md
+drwxr-xr-x   0 zhuhaohao  (1019) dutir     (1000)        0 2024-05-08 17:48:53.000000 alegant-1.0.5/alegant/
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)      176 2024-01-14 03:17:37.000000 alegant-1.0.5/alegant/__init__.py
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     5399 2024-01-17 12:13:04.000000 alegant-1.0.5/alegant/data_module.py
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     3350 2024-04-04 11:42:35.000000 alegant-1.0.5/alegant/runner.py
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)    16857 2024-04-04 11:46:48.000000 alegant-1.0.5/alegant/trainer.py
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     1465 2024-01-12 11:41:49.000000 alegant-1.0.5/alegant/utils.py
+drwxr-xr-x   0 zhuhaohao  (1019) dutir     (1000)        0 2024-05-08 17:48:53.000000 alegant-1.0.5/alegant.egg-info/
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     2503 2024-05-08 17:48:53.000000 alegant-1.0.5/alegant.egg-info/PKG-INFO
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)      277 2024-05-08 17:48:53.000000 alegant-1.0.5/alegant.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)        1 2024-05-08 17:48:53.000000 alegant-1.0.5/alegant.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)       56 2024-05-08 17:48:53.000000 alegant-1.0.5/alegant.egg-info/requires.txt
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)        8 2024-05-08 17:48:53.000000 alegant-1.0.5/alegant.egg-info/top_level.txt
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)       38 2024-05-08 17:48:53.000000 alegant-1.0.5/setup.cfg
+-rw-r--r--   0 zhuhaohao  (1019) dutir     (1000)     1048 2024-01-13 12:49:11.000000 alegant-1.0.5/setup.py
```

### Comparing `alegant-1.0.4/LICENSE` & `alegant-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alegant-1.0.4/README.md` & `alegant-1.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,90 @@
+Metadata-Version: 2.1
+Name: alegant
+Version: 1.0.5
+Summary: Alegant: a elegant training framework
+Home-page: https://github.com/Hugo-Zhu/alegant
+Author: Haohao Zhu
+Author-email: zhuhh17@qq.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Alegant
 
 Alegant is an elegant training framework for PyTorch models.
 
 ## Install Alegant
 
 Before installing Alegant, please make sure you have the following requirements:
 - Python >= 3.7
 - torch >= 1.9
 
 Simple installation from PyPI
 ```bash
 pip install alegant
 ```
-To install fairseq and develop locally:
+To install Alegant and develop locally:
 ```bash
 python setup.py develop
 ```
+
+## Example
+
+For examples on how to use elegant, please refer to the examples directory in this repository. It contains sample configuration files and code snippets to help you get started.
+
 ## Usage
-To use alegant, follow the steps below:
+
+To use Alegant, follow the steps below:
 
 1. Define your Model.
 2. Define your DataModule.
 3. Define your Trainer.
-4. Run the training script using the following command:
+4. Set your configuration.
+5. Run the training script using the following command:
 
-```python
-python --config_file run.py
+```bash
+cd alegant/example
+python example_main.py  # for simply use the DataModule and Trainer
+python example_runner.py # for using the runner from Alegant
 ```
-Make sure to replace config_file with the path to your configuration file.
 
 ## Configuration
 To customize the training process, you need to provide a configuration file. This file specifies various parameters such as dataset paths, model architecture, hyperparameters, etc. Make sure to create a valid configuration file before running the framework.
 
 ## Project Structure
 
 ```plaintext
 alegant
-├── tensorboard
-├── data
 ├── alegant
+│   ├── __init__.py
+│   ├── runner.py
+│   ├── trainer.py
 │   ├── data_module.py
-│   ├── trainer.py
-│   └── utils.py
-├── src
-│   ├── dataset.py
-│   ├── loss.py
-│   ├── model
-│   │   ├── modeling.py
-│   │   ├── poolers.py
-│   ├── trainer.py
-│   └── utils.py
-├── config.yaml
-├── run.py
+│   ├── utils.py
+│   └── example
+│       ├── data
+│       ├── config.yaml
+│       ├── example_main.py
+│       ├── example_runner.py
+│       ├── logs
+│       ├── README.md
+│       ├── src
+│       │   ├── dataset.py
+│       │   ├── loss.py
+│       │   ├── model
+│       │   │   ├── modeling.py
+│       │   │   ├── poolers.py
+│       │   ├── trainer.py
+│       │   └── utils.py
+│       └── tensorboard
 └── setup.py
 ```
 
 ## Contact
 If you have any questions or inquiries, please contact us at zhuhh17@qq.com
 
-Thank you for using Alegant! Happy training!
+Thank you for using Alegant! Happy training!
```

### Comparing `alegant-1.0.4/alegant/data_module.py` & `alegant-1.0.5/alegant/data_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,17 @@
         train_batch_size (Optional[int]): Batch size for training data. Defaults to 32.
         train_limit_batches (Optional[float]): Batch limit ratio for training data. Defaults to 1.0.
         val_batch_size (Optional[int]): Batch size for validation data. Defaults to 32.
         val_limit_batches (Optional[float]): Batch limit ratio for validation data. Defaults to 1.0.
         test_batch_size (Optional[int]): Batch size for test data. Defaults to 32.
         test_limit_batches (Optional[float]): Batch limit ratio for test data. Defaults to 1.0.
     """
-    train_data_path: str
-    val_data_path: str
-    test_data_path: str
+    train_data_path: str = field(default=None, metadata={"description": "File path to the training data"})
+    val_data_path: str = field(default=None, metadata={"description": "File path to the validation data"})
+    test_data_path: str = field(default=None, metadata={"description": "File path to the test data"})
     do_setup: bool = field(default=True, metadata={"description": "Whether prepare datasets from data_paths"})
     cache_dir: str = field(default=None, metadata={"description": "Path to cache the datasets"})
     
     train_batch_size: int = field(default=32, metadata={"description": "Batch size for training data"})
     train_limit_batches: float = field(default=1.0, metadata={"description": "Batch limit ratio for training data"})
     val_batch_size: int = field(default=32, metadata={"description": "Batch size for validation data"})
     val_limit_batches: float = field(default=1.0, metadata={"description": "Batch limit ratio for validation data"})
```

### Comparing `alegant-1.0.4/alegant/trainer.py` & `alegant-1.0.5/alegant/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         else: self.model = self.model.to(self.args.device)
         
         scaler = GradScaler(enabled=self.args.amp)
 
         # Start train loop
         for self.epoch in range(self.start_epoch, self.args.epochs):
             self.model.train()
-            for batch_idx, batch in tqdm(enumerate(train_dataloader), f"Epoch: {self.epoch}", total=len(train_dataloader), miniters=len(train_dataloader)*0.1, maxinterval=float("inf")):
+            for batch_idx, batch in tqdm(enumerate(train_dataloader), f"EPOCH: {self.epoch}", total=len(train_dataloader), miniters=len(train_dataloader)*0.1, maxinterval=float("inf")):
                 outputs = self.training_step(batch, batch_idx)
                 loss = outputs.get("loss")/self.args.accumulation_steps     # 除不除accumulation_steps对结果有影响
                 # loss.backward()
                 scaler.scale(loss).backward()
                 
                 # Clip gradients for each parameter group in the optimizer
                 if self.args.max_norm is not None:
@@ -143,14 +143,15 @@
                     self.optimizer.zero_grad()
                 
                 # Evaluation loop
                 if (batch_idx+1) % self.args.eval_steps == 0 or (batch_idx+1)==len(train_dataloader):
                     self.validation(eval_dataloader)
             
             self.training_epoch_end()
+        logger.success(f"best_f1: {self.best_f1:.5f}")
         self.logger.close()
     
 
     @torch.no_grad()
     def validation(self, eval_dataloader):
         """
         Perform model validation.
@@ -158,15 +159,15 @@
         Args:
             eval_dataloader: Dataloader for evaluation.
         """
         self.model.eval()
         eval_outputs = []
         
         self.num_eval += 1
-        for batch_idx_eval, batch_eval in tqdm(enumerate(eval_dataloader), "evalation", total=len(eval_dataloader), miniters=len(eval_dataloader)*0.1, maxinterval=float("inf")):
+        for batch_idx_eval, batch_eval in tqdm(enumerate(eval_dataloader), "EVALUATING", total=len(eval_dataloader), miniters=len(eval_dataloader)*0.1, maxinterval=float("inf")):
             outputs = self.validation_step(batch_eval, batch_idx_eval)
             loss = outputs.get("loss")
             eval_outputs.append(outputs)
             self.num_eval_step += 1
             self.logger.add_scalar(f"eval_loss", loss.item(), self.num_eval_step)
         
         self.validation_epoch_end(eval_outputs)
@@ -181,26 +182,27 @@
             checkpoint (str): Path to the checkpoint file.
         Returns:
             float: Test accuracy.
         """
         self.model.to(self.args.device)
         # Load the checkpoint
         if checkpoint is None:
-            logger.warning("Checkpoint is None during TESTING !!!")
+            logger.error("Checkpoint is None during TESTING !!!")
+            raise Exception
         else:
             logger.info(f"Loading checkpoint from {checkpoint} ...")
             checkpoint = torch.load(checkpoint, map_location=self.args.device)
             self.model.load_state_dict(checkpoint['model_state_dict'])
         # Initialize the test dataloader
         dataloader = self.data_module.test_dataloader()
         
         self.model.eval()
         test_outputs = []
         num_test_step = 0
-        for batch_idx_test, batch_test in tqdm(enumerate(dataloader), "test", total=len(dataloader)):
+        for batch_idx_test, batch_test in tqdm(enumerate(dataloader), "TESTING", total=len(dataloader)):
             outputs = self.test_step(batch_test, batch_idx_test)
             loss = outputs.get("loss")
             test_outputs.append(outputs)
             num_test_step += 1
             self.logger.add_scalar(f"test_loss", loss.item(), num_test_step)
 
         self.test_epoch_end(test_outputs)
@@ -215,22 +217,22 @@
         Args:
             batch: Batch of training data.
             batch_idx (int): Index of the batch.
 
         Returns:
             dict: Dictionary containing the training step outputs.
         """
-        # 获取数据并移动到设备
+        # load data & to device
         input_ids = batch['input_ids'].to(self.args.device)
         label = batch['label'].to(self.args.device)
         
         with autocast(enabled=self.args.amp):
-            # 前向传播
+            # forward
             logits = self.model(input_ids)
-            # 计算损失
+            # calculate loss
             loss = self.criterion(logits, label)
         
         return {"loss": loss}
 
     def training_epoch_end(self):
         """
         Perform operations at the end of each training epoch.
@@ -245,15 +247,15 @@
         Args:
             batch: Batch of validation data.
             batch_idx (int): Index of the batch.
 
         Returns:
             dict: Dictionary containing the validation step outputs.
         """
-        # 获取数据并移动到设备 -> 前向传播 -> 计算损失 -> 记录评价指标
+        # load data & to device -> forward -> calculate loss -> log metrics
         input_ids = batch['input_ids'].to(self.args.device)
         label = batch['label'].to(self.args.device)
         with autocast(enabled=self.args.amp):
             logits = self.model(input_ids)
             loss = self.criterion(logits, label)
         predictions = torch.argmax(logits, dim=-1)
         batch_errors = (predictions != label)
@@ -280,15 +282,15 @@
         metrics = self.compute_metrics(preds_list, label_list)
         accuracy = metrics.get("accuracy")
         self.logger.add_scalar("accuracy", accuracy, self.num_eval)
         if accuracy > self.best_acc:
             self.best_acc = accuracy
             if self.args.do_save:
                 self.save_checkpoint()
-        logger.success(f"acc: {accuracy}, best_acc: {self.best_acc}")
+        logger.info(f"acc: {accuracy}; best_acc: {self.best_acc}")
 
 
     def test_step(self, batch, batch_idx):
         return self.validation_step(batch, batch_idx)
 
 
     def test_epoch_end(self, outputs):
@@ -306,15 +308,15 @@
 
         preds_list = torch.argmax(F.softmax(logits_list, dim=-1), dim=-1)
         preds_list = torch.cat(preds_list, dim=0)
         label_list = torch.cat(label_list, dim=0)
 
         metrics = self.compute_metrics(preds_list, label_list)
         accuracy = metrics.get("accuracy")
-        logger.info(f"acc: {accuracy}")
+        logger.info(f"Acc: {accuracy}")
 
     @abstractmethod
     def configure_optimizers(self, num_training_steps):
         """
         Configure the optimizer and learning rate scheduler.
 
         Args:
```

### Comparing `alegant-1.0.4/alegant/utils.py` & `alegant-1.0.5/alegant/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import torch
 import random
 import argparse
 import numpy as np
 from loguru import logger
 from attrdict import AttrDict
 
+__all__ = [
+    "parse_args",
+    "seed_everything",
+]
 
 def parse_args():
     """
     Parse command-line arguments and load the configuration file.
 
     Returns:
         config (AttrDict): Configuration loaded from the file and command-line arguments.
```

### Comparing `alegant-1.0.4/setup.py` & `alegant-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='alegant',
-    version='1.0.4',
-    packages=find_packages(exclude=["dist.*", "dist", "*tests*", "*script*", "*cache*"]),
+    version='1.0.5',
+    packages=find_packages(exclude=["dist.*", "dist", "*tests*", "*script*", "*cache*", "data"]),
     url='https://github.com/Hugo-Zhu/alegant',
     license='MIT',
     author='Haohao Zhu',
     author_email='zhuhh17@qq.com',
     description='Alegant: a elegant training framework',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

