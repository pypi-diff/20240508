# Comparing `tmp/infini_transformer_pytorch-0.0.8.tar.gz` & `tmp/infini_transformer_pytorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infini_transformer_pytorch-0.0.8.tar", last modified: Thu May  2 16:29:45 2024, max compression
+gzip compressed data, was "infini_transformer_pytorch-0.0.9.tar", last modified: Thu May  2 16:34:37 2024, max compression
```

## Comparing `infini_transformer_pytorch-0.0.8.tar` & `infini_transformer_pytorch-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:29:45.349289 infini_transformer_pytorch-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 16:29:41.000000 infini_transformer_pytorch-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 16:29:45.349289 infini_transformer_pytorch-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-02 16:29:41.000000 infini_transformer_pytorch-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:29:45.349289 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 16:29:41.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-02 16:29:41.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch/infini_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:29:45.349289 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 16:29:45.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 16:29:45.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:29:45.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 16:29:45.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 16:29:45.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:29:45.349289 infini_transformer_pytorch-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 16:29:41.000000 infini_transformer_pytorch-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:34:37.077998 infini_transformer_pytorch-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 16:34:32.000000 infini_transformer_pytorch-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 16:34:37.073998 infini_transformer_pytorch-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-02 16:34:32.000000 infini_transformer_pytorch-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:34:37.073998 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 16:34:32.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-02 16:34:32.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch/infini_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:34:37.073998 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 16:34:37.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 16:34:37.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:34:37.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 16:34:37.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 16:34:37.000000 infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:34:37.077998 infini_transformer_pytorch-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 16:34:32.000000 infini_transformer_pytorch-0.0.9/setup.py
```

### Comparing `infini_transformer_pytorch-0.0.8/LICENSE` & `infini_transformer_pytorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.8/PKG-INFO` & `infini_transformer_pytorch-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.8/README.md` & `infini_transformer_pytorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.8/infini_transformer_pytorch/infini_transformer.py` & `infini_transformer_pytorch-0.0.9/infini_transformer_pytorch/infini_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,17 @@
 def exists(v):
     return v
 
 def default(v, d):
     return v if exists(v) else d
 
 def detach_memories_(memories: Memories):
-    if detach_memories:
-        for (mem_kv, mem_norm) in memories:
-            mem_kv.detach_()
-            mem_norm.detach_()
+    for (mem_kv, mem_norm) in memories:
+        mem_kv.detach_()
+        mem_norm.detach_()
 
 # classes
 
 class RMSNorm(Module):
     def __init__(self, dim):
         super().__init__()
         self.scale = dim ** 0.5
```

### Comparing `infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/PKG-INFO` & `infini_transformer_pytorch-0.0.9/infini_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.8/setup.py` & `infini_transformer_pytorch-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'infini-transformer-pytorch',
   packages = find_packages(exclude = []),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Infini-Transformer in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/infini-transformer-pytorch',
   keywords = [
```

