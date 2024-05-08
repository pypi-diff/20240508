# Comparing `tmp/RViT-1.0.0.tar.gz` & `tmp/rvit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RViT-1.0.0.tar", last modified: Wed May  8 12:16:26 2024, max compression
+gzip compressed data, was "rvit-1.0.1.tar", last modified: Wed May  8 12:27:46 2024, max compression
```

## Comparing `RViT-1.0.0.tar` & `rvit-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 12:16:26.750945 RViT-1.0.0/
--rw-rw-rw-   0        0        0     1083 2024-05-08 12:16:26.750945 RViT-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-05-08 12:13:12.000000 RViT-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 12:16:26.741944 RViT-1.0.0/RViT/
--rw-rw-rw-   0        0        0       60 2024-05-08 12:01:57.000000 RViT-1.0.0/RViT/__init__.py
--rw-rw-rw-   0        0        0     3740 2024-05-08 12:00:48.000000 RViT-1.0.0/RViT/r_vision_transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:16:26.749945 RViT-1.0.0/RViT.egg-info/
--rw-rw-rw-   0        0        0     1083 2024-05-08 12:16:26.000000 RViT-1.0.0/RViT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-05-08 12:16:26.000000 RViT-1.0.0/RViT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 12:16:26.000000 RViT-1.0.0/RViT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-08 12:16:26.000000 RViT-1.0.0/RViT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-08 12:16:26.000000 RViT-1.0.0/RViT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 12:16:26.750945 RViT-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1048 2024-05-08 12:16:19.000000 RViT-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:27:46.102253 rvit-1.0.1/
+-rw-rw-rw-   0        0        0     1135 2024-05-08 12:27:46.102253 rvit-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2024-05-08 12:21:15.000000 rvit-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 12:27:46.100253 rvit-1.0.1/RViT/
+-rw-rw-rw-   0        0        0       74 2024-05-08 12:24:16.000000 rvit-1.0.1/RViT/__init__.py
+-rw-rw-rw-   0        0        0     3740 2024-05-08 12:00:48.000000 rvit-1.0.1/RViT/registered_vision_transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-08 12:27:46.100253 rvit-1.0.1/RViT.egg-info/
+-rw-rw-rw-   0        0        0     1135 2024-05-08 12:27:46.000000 rvit-1.0.1/RViT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-05-08 12:27:46.000000 rvit-1.0.1/RViT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 12:27:46.000000 rvit-1.0.1/RViT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 12:27:46.000000 rvit-1.0.1/RViT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-08 12:27:46.000000 rvit-1.0.1/RViT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 12:27:46.102253 rvit-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2024-05-08 12:27:27.000000 rvit-1.0.1/setup.py
```

### Comparing `RViT-1.0.0/PKG-INFO` & `rvit-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: RViT
-Version: 1.0.0
+Name: rvit
+Version: 1.0.1
 Summary: Vision Transformer with Registers
 Author: Joe Griffith
 Author-email: <joeagriffith@gmail.com
 Keywords: python,pytorch,vision transformer,register,registers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -15,8 +15,13 @@
 
 
 A simple augmentation of PyTorch's VisionTransform class from torchvision.models to include registers, as per: https://arxiv.org/abs/2309.16588
 
 Introduces registers to the encoder that are appended as tokens to the 'patchified' sequence, and excluded in the output.
 The tokens are learnable parameters and do not receive positional embeddings.
 
-The API of the class is identical with VisionTransformer, except the additional init argument for 'num_registers', which specifies the number of register tokens.
+The API of the class is identical with VisionTransformer, except the additional init argument for 'num_registers', which specifies the number of register tokens.
+
+## Installation
+```
+pip install rvit
+```
```

### Comparing `RViT-1.0.0/README.md` & `rvit-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,6 +1,11 @@
 A simple augmentation of PyTorch's VisionTransform class from torchvision.models to include registers, as per: https://arxiv.org/abs/2309.16588
 
 Introduces registers to the encoder that are appended as tokens to the 'patchified' sequence, and excluded in the output.
 The tokens are learnable parameters and do not receive positional embeddings.
 
-The API of the class is identical with VisionTransformer, except the additional init argument for 'num_registers', which specifies the number of register tokens.
+The API of the class is identical with VisionTransformer, except the additional init argument for 'num_registers', which specifies the number of register tokens.
+
+## Installation
+```
+pip install rvit
+```
```

### Comparing `RViT-1.0.0/RViT/r_vision_transformer.py` & `rvit-1.0.1/RViT/registered_vision_transformer.py`

 * *Files identical despite different names*

### Comparing `RViT-1.0.0/RViT.egg-info/PKG-INFO` & `rvit-1.0.1/RViT.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: RViT
-Version: 1.0.0
+Name: rvit
+Version: 1.0.1
 Summary: Vision Transformer with Registers
 Author: Joe Griffith
 Author-email: <joeagriffith@gmail.com
 Keywords: python,pytorch,vision transformer,register,registers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -15,8 +15,13 @@
 
 
 A simple augmentation of PyTorch's VisionTransform class from torchvision.models to include registers, as per: https://arxiv.org/abs/2309.16588
 
 Introduces registers to the encoder that are appended as tokens to the 'patchified' sequence, and excluded in the output.
 The tokens are learnable parameters and do not receive positional embeddings.
 
-The API of the class is identical with VisionTransformer, except the additional init argument for 'num_registers', which specifies the number of register tokens.
+The API of the class is identical with VisionTransformer, except the additional init argument for 'num_registers', which specifies the number of register tokens.
+
+## Installation
+```
+pip install rvit
+```
```

### Comparing `RViT-1.0.0/setup.py` & `rvit-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'Vision Transformer with Registers'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
-    name="RViT",
+    name="rvit",
     version=VERSION,
     author="Joe Griffith",
     author_email="<joeagriffith@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

