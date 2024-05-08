# Comparing `tmp/magvit2_pytorch-0.4.3.tar.gz` & `tmp/magvit2_pytorch-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magvit2_pytorch-0.4.3.tar", last modified: Tue May  7 14:16:40 2024, max compression
+gzip compressed data, was "magvit2_pytorch-0.4.4.tar", last modified: Wed May  8 14:20:56 2024, max compression
```

## Comparing `magvit2_pytorch-0.4.3.tar` & `magvit2_pytorch-0.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:16:40.628078 magvit2_pytorch-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-07 14:16:40.628078 magvit2_pytorch-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:16:40.624078 magvit2_pytorch-0.4.3/magvit2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    56410 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/magvit2_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/magvit2_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:16:40.628078 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-07 14:16:40.000000 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 14:16:40.000000 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:16:40.000000 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 14:16:40.000000 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 14:16:40.000000 magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:16:40.628078 magvit2_pytorch-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-07 14:16:36.000000 magvit2_pytorch-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:56.124939 magvit2_pytorch-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-08 14:20:56.124939 magvit2_pytorch-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:56.120939 magvit2_pytorch-0.4.4/magvit2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56521 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/magvit2_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/magvit2_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:56.120939 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-08 14:20:56.000000 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-08 14:20:56.000000 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:20:56.000000 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 14:20:56.000000 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 14:20:56.000000 magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:20:56.124939 magvit2_pytorch-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-08 14:20:52.000000 magvit2_pytorch-0.4.4/setup.py
```

### Comparing `magvit2_pytorch-0.4.3/LICENSE` & `magvit2_pytorch-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.3/PKG-INFO` & `magvit2_pytorch-0.4.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magvit2-pytorch
-Version: 0.4.3
+Version: 0.4.4
 Summary: MagViT2 - Pytorch
 Home-page: https://github.com/lucidrains/magvit2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,attention mechanisms,generative video model
 Classifier: Development Status :: 4 - Beta
@@ -21,12 +21,12 @@
 Requires-Dist: pytorch-warmup
 Requires-Dist: gateloop-transformer>=0.2.2
 Requires-Dist: kornia
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 Requires-Dist: pytorch-custom-utils>=0.0.9
 Requires-Dist: numpy
-Requires-Dist: vector-quantize-pytorch>=1.14.10
+Requires-Dist: vector-quantize-pytorch>=1.14.20
 Requires-Dist: taylor-series-linear-attention>=0.1.5
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: x-transformers
```

### Comparing `magvit2_pytorch-0.4.3/README.md` & `magvit2_pytorch-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.3/magvit2_pytorch/attend.py` & `magvit2_pytorch-0.4.4/magvit2_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.3/magvit2_pytorch/data.py` & `magvit2_pytorch-0.4.4/magvit2_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.3/magvit2_pytorch/magvit2_pytorch.py` & `magvit2_pytorch-0.4.4/magvit2_pytorch/magvit2_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1061,14 +1061,15 @@
         input_conv_kernel_size: Tuple[int, int, int] = (7, 7, 7),
         output_conv_kernel_size: Tuple[int, int, int] = (3, 3, 3),
         pad_mode: str = 'constant',
         lfq_entropy_loss_weight = 0.1,
         lfq_commitment_loss_weight = 1.,
         lfq_diversity_gamma = 2.5,
         quantizer_aux_loss_weight = 1.,
+        lfq_soft_clamp_input_value = 10.,
         lfq_activation = nn.Identity(),
         use_fsq = False,
         fsq_levels: Optional[List[int]] = None,
         attn_dim_head = 32,
         attn_heads = 8,
         attn_dropout = 0.,
         linear_attn_dim_head = 8,
@@ -1358,15 +1359,16 @@
 
             self.quantizers = LFQ(
                 dim = dim,
                 codebook_size = codebook_size,
                 num_codebooks = num_codebooks,
                 entropy_loss_weight = lfq_entropy_loss_weight,
                 commitment_loss_weight = lfq_commitment_loss_weight,
-                diversity_gamma = lfq_diversity_gamma
+                diversity_gamma = lfq_diversity_gamma,
+                soft_clamp_input_value = lfq_soft_clamp_input_value
             )
 
         else:
             assert not exists(codebook_size) and exists(fsq_levels), 'if use_fsq is set to True, `fsq_levels` must be set (and not `codebook_size`). the effective codebook size is the cumulative product of all the FSQ levels'
 
             self.quantizers = FSQ(
                 fsq_levels,
```

### Comparing `magvit2_pytorch-0.4.3/magvit2_pytorch/optimizer.py` & `magvit2_pytorch-0.4.4/magvit2_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.3/magvit2_pytorch/trainer.py` & `magvit2_pytorch-0.4.4/magvit2_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `magvit2_pytorch-0.4.3/magvit2_pytorch.egg-info/PKG-INFO` & `magvit2_pytorch-0.4.4/magvit2_pytorch.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magvit2-pytorch
-Version: 0.4.3
+Version: 0.4.4
 Summary: MagViT2 - Pytorch
 Home-page: https://github.com/lucidrains/magvit2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,attention mechanisms,generative video model
 Classifier: Development Status :: 4 - Beta
@@ -21,12 +21,12 @@
 Requires-Dist: pytorch-warmup
 Requires-Dist: gateloop-transformer>=0.2.2
 Requires-Dist: kornia
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 Requires-Dist: pytorch-custom-utils>=0.0.9
 Requires-Dist: numpy
-Requires-Dist: vector-quantize-pytorch>=1.14.10
+Requires-Dist: vector-quantize-pytorch>=1.14.20
 Requires-Dist: taylor-series-linear-attention>=0.1.5
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: x-transformers
```

### Comparing `magvit2_pytorch-0.4.3/setup.py` & `magvit2_pytorch-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     'pytorch-warmup',
     'gateloop-transformer>=0.2.2',
     'kornia',
     'opencv-python',
     'pillow',
     'pytorch-custom-utils>=0.0.9',
     'numpy',
-    'vector-quantize-pytorch>=1.14.10',
+    'vector-quantize-pytorch>=1.14.20',
     'taylor-series-linear-attention>=0.1.5',
     'torch',
     'torchvision',
     'x-transformers'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
```

