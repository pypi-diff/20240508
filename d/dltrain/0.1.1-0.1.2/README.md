# Comparing `tmp/dltrain-0.1.1.tar.gz` & `tmp/dltrain-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dltrain-0.1.1.tar", last modified: Tue May  7 05:14:44 2024, max compression
+gzip compressed data, was "dltrain-0.1.2.tar", last modified: Wed May  8 06:35:18 2024, max compression
```

## Comparing `dltrain-0.1.1.tar` & `dltrain-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 05:14:44.934664 dltrain-0.1.1/
--rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6385 2024-05-07 05:14:44.928143 dltrain-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5748 2024-05-07 05:10:29.000000 dltrain-0.1.1/README.md
--rw-rw-rw-   0        0        0      625 2024-05-07 05:14:37.000000 dltrain-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 05:14:44.934664 dltrain-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 05:14:44.791124 dltrain-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 05:14:44.846125 dltrain-0.1.1/src/dltrain/
--rw-rw-rw-   0        0        0      229 2024-05-05 13:13:52.000000 dltrain-0.1.1/src/dltrain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 05:14:44.927133 dltrain-0.1.1/src/dltrain/builder/
--rw-rw-rw-   0        0        0       32 2024-05-04 13:43:22.000000 dltrain-0.1.1/src/dltrain/builder/__init__.py
--rw-rw-rw-   0        0        0     1207 2024-05-07 01:28:09.000000 dltrain-0.1.1/src/dltrain/builder/base.py
--rw-rw-rw-   0        0        0     3219 2024-05-07 03:07:53.000000 dltrain-0.1.1/src/dltrain/builder/builder.py
--rw-rw-rw-   0        0        0      212 2024-05-04 13:37:24.000000 dltrain-0.1.1/src/dltrain/builder/core.py
--rw-rw-rw-   0        0        0      714 2024-05-05 13:08:13.000000 dltrain-0.1.1/src/dltrain/builder/criterion.py
--rw-rw-rw-   0        0        0     1177 2024-05-05 13:08:13.000000 dltrain-0.1.1/src/dltrain/builder/dataset.py
--rw-rw-rw-   0        0        0      721 2024-05-05 13:08:13.000000 dltrain-0.1.1/src/dltrain/builder/delineator.py
--rw-rw-rw-   0        0        0     1556 2024-05-05 13:08:13.000000 dltrain-0.1.1/src/dltrain/builder/evaluation.py
--rw-rw-rw-   0        0        0      488 2024-05-07 01:12:49.000000 dltrain-0.1.1/src/dltrain/builder/forward.py
--rw-rw-rw-   0        0        0      281 2024-05-07 03:07:32.000000 dltrain-0.1.1/src/dltrain/builder/inject.py
--rw-rw-rw-   0        0        0      840 2024-05-05 13:08:13.000000 dltrain-0.1.1/src/dltrain/builder/model.py
--rw-rw-rw-   0        0        0     1169 2024-05-07 01:28:56.000000 dltrain-0.1.1/src/dltrain/builder/optimizer.py
--rw-rw-rw-   0        0        0      533 2024-05-04 13:52:21.000000 dltrain-0.1.1/src/dltrain/builder/scheduler.py
--rw-rw-rw-   0        0        0      718 2024-05-05 13:08:13.000000 dltrain-0.1.1/src/dltrain/builder/transforms.py
--rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.1.1/src/dltrain/checkpoint.py
--rw-rw-rw-   0        0        0     5177 2024-05-05 13:08:13.000000 dltrain-0.1.1/src/dltrain/dataset.py
--rw-rw-rw-   0        0        0     1300 2024-05-05 13:08:13.000000 dltrain-0.1.1/src/dltrain/delineator.py
--rw-rw-rw-   0        0        0      935 2024-05-03 11:30:58.000000 dltrain-0.1.1/src/dltrain/error.py
--rw-rw-rw-   0        0        0     3949 2024-05-05 13:08:13.000000 dltrain-0.1.1/src/dltrain/evaluation.py
--rw-rw-rw-   0        0        0     6478 2024-05-07 02:10:02.000000 dltrain-0.1.1/src/dltrain/forward.py
--rw-rw-rw-   0        0        0     1203 2024-05-07 03:07:32.000000 dltrain-0.1.1/src/dltrain/inject.py
--rw-rw-rw-   0        0        0     4523 2024-05-07 02:14:49.000000 dltrain-0.1.1/src/dltrain/models.py
--rw-rw-rw-   0        0        0     1290 2024-04-07 09:09:29.000000 dltrain-0.1.1/src/dltrain/options.py
--rw-rw-rw-   0        0        0    11930 2024-05-07 02:10:30.000000 dltrain-0.1.1/src/dltrain/train.py
--rw-rw-rw-   0        0        0     1145 2024-04-07 09:09:29.000000 dltrain-0.1.1/src/dltrain/transform.py
--rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.1.1/src/dltrain/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 05:14:44.928143 dltrain-0.1.1/src/dltrain.egg-info/
--rw-rw-rw-   0        0        0     6385 2024-05-07 05:14:44.000000 dltrain-0.1.1/src/dltrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      916 2024-05-07 05:14:44.000000 dltrain-0.1.1/src/dltrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 05:14:44.000000 dltrain-0.1.1/src/dltrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 05:14:44.000000 dltrain-0.1.1/src/dltrain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.815354 dltrain-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6714 2024-05-08 06:35:18.814354 dltrain-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6077 2024-05-08 06:33:51.000000 dltrain-0.1.2/README.md
+-rw-rw-rw-   0        0        0      625 2024-05-08 02:25:24.000000 dltrain-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 06:35:18.815354 dltrain-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.579814 dltrain-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.678369 dltrain-0.1.2/src/dltrain/
+-rw-rw-rw-   0        0        0      229 2024-05-05 13:13:52.000000 dltrain-0.1.2/src/dltrain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.788369 dltrain-0.1.2/src/dltrain/builder/
+-rw-rw-rw-   0        0        0       32 2024-05-04 13:43:22.000000 dltrain-0.1.2/src/dltrain/builder/__init__.py
+-rw-rw-rw-   0        0        0     1207 2024-05-07 01:28:09.000000 dltrain-0.1.2/src/dltrain/builder/base.py
+-rw-rw-rw-   0        0        0     3219 2024-05-07 03:07:53.000000 dltrain-0.1.2/src/dltrain/builder/builder.py
+-rw-rw-rw-   0        0        0      212 2024-05-04 13:37:24.000000 dltrain-0.1.2/src/dltrain/builder/core.py
+-rw-rw-rw-   0        0        0      714 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/builder/criterion.py
+-rw-rw-rw-   0        0        0     2264 2024-05-08 02:25:24.000000 dltrain-0.1.2/src/dltrain/builder/dataset.py
+-rw-rw-rw-   0        0        0      721 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/builder/delineator.py
+-rw-rw-rw-   0        0        0     1556 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/builder/evaluation.py
+-rw-rw-rw-   0        0        0      488 2024-05-07 01:12:49.000000 dltrain-0.1.2/src/dltrain/builder/forward.py
+-rw-rw-rw-   0        0        0      281 2024-05-07 03:07:32.000000 dltrain-0.1.2/src/dltrain/builder/inject.py
+-rw-rw-rw-   0        0        0      861 2024-05-08 02:46:50.000000 dltrain-0.1.2/src/dltrain/builder/model.py
+-rw-rw-rw-   0        0        0     1169 2024-05-07 01:28:56.000000 dltrain-0.1.2/src/dltrain/builder/optimizer.py
+-rw-rw-rw-   0        0        0      533 2024-05-04 13:52:21.000000 dltrain-0.1.2/src/dltrain/builder/scheduler.py
+-rw-rw-rw-   0        0        0      834 2024-05-08 02:35:03.000000 dltrain-0.1.2/src/dltrain/builder/transforms.py
+-rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.1.2/src/dltrain/checkpoint.py
+-rw-rw-rw-   0        0        0     5177 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/dataset.py
+-rw-rw-rw-   0        0        0     1300 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/delineator.py
+-rw-rw-rw-   0        0        0      935 2024-05-03 11:30:58.000000 dltrain-0.1.2/src/dltrain/error.py
+-rw-rw-rw-   0        0        0     3949 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/evaluation.py
+-rw-rw-rw-   0        0        0     6478 2024-05-07 02:10:02.000000 dltrain-0.1.2/src/dltrain/forward.py
+-rw-rw-rw-   0        0        0     1203 2024-05-07 03:07:32.000000 dltrain-0.1.2/src/dltrain/inject.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.811359 dltrain-0.1.2/src/dltrain/models/
+-rw-rw-rw-   0        0        0      101 2024-05-08 02:46:50.000000 dltrain-0.1.2/src/dltrain/models/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-05-08 06:15:11.000000 dltrain-0.1.2/src/dltrain/models/component.py
+-rw-rw-rw-   0        0        0     1607 2024-05-08 02:46:50.000000 dltrain-0.1.2/src/dltrain/models/model.py
+-rw-rw-rw-   0        0        0     3040 2024-05-08 02:46:50.000000 dltrain-0.1.2/src/dltrain/models/wrapper.py
+-rw-rw-rw-   0        0        0     1290 2024-04-07 09:09:29.000000 dltrain-0.1.2/src/dltrain/options.py
+-rw-rw-rw-   0        0        0    11930 2024-05-07 02:10:30.000000 dltrain-0.1.2/src/dltrain/train.py
+-rw-rw-rw-   0        0        0     1405 2024-05-08 02:35:03.000000 dltrain-0.1.2/src/dltrain/transform.py
+-rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.1.2/src/dltrain/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.813355 dltrain-0.1.2/src/dltrain.egg-info/
+-rw-rw-rw-   0        0        0     6714 2024-05-08 06:35:18.000000 dltrain-0.1.2/src/dltrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1015 2024-05-08 06:35:18.000000 dltrain-0.1.2/src/dltrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 06:35:18.000000 dltrain-0.1.2/src/dltrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-08 06:35:18.000000 dltrain-0.1.2/src/dltrain.egg-info/top_level.txt
```

### Comparing `dltrain-0.1.1/LICENSE` & `dltrain-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/PKG-INFO` & `dltrain-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -148,7 +148,16 @@
 | seed             | 3407                                               |
 | device           | cpu                                                |
 | save_checkpoint  | False                                              |
 | start_checkpoint | User-set                                           |
 | delineator*      | None,Must be specified by the user                 |
 | forward          | SimpleForward                                      |
 | trainer          | SimpleTrainer                                      |
+
+## Version Log
+- 0.0.1<br/>
+1、构造整体模型框架
+- 0.0.2<br/>
+1、加入了TaskBuilder方便构造模型
+- 0.1.2<br/>
+1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)
+2、将models.py封装到models包，添加了许多拆箱可用模型
```

### Comparing `dltrain-0.1.1/README.md` & `dltrain-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -134,7 +134,16 @@
 | seed             | 3407                                               |
 | device           | cpu                                                |
 | save_checkpoint  | False                                              |
 | start_checkpoint | User-set                                           |
 | delineator*      | None,Must be specified by the user                 |
 | forward          | SimpleForward                                      |
 | trainer          | SimpleTrainer                                      |
+
+## Version Log
+- 0.0.1<br/>
+1、构造整体模型框架
+- 0.0.2<br/>
+1、加入了TaskBuilder方便构造模型
+- 0.1.2<br/>
+1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)
+2、将models.py封装到models包，添加了许多拆箱可用模型
```

### Comparing `dltrain-0.1.1/pyproject.toml` & `dltrain-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dltrain"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="XiaosYu", email="lijingyu_ai@163.com" },
 ]
 description = "This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dltrain-0.1.1/src/dltrain/builder/base.py` & `dltrain-0.1.2/src/dltrain/builder/base.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/builder/builder.py` & `dltrain-0.1.2/src/dltrain/builder/builder.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/builder/criterion.py` & `dltrain-0.1.2/src/dltrain/builder/criterion.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/builder/delineator.py` & `dltrain-0.1.2/src/dltrain/builder/delineator.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/builder/evaluation.py` & `dltrain-0.1.2/src/dltrain/builder/evaluation.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/builder/model.py` & `dltrain-0.1.2/src/dltrain/builder/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .core import Wizard
-from ..models import MultilayerPerceptron, PyTorchNativeCNN, create_native_model, Module
+from ..models import MultilayerPerceptron, PyTorchNativeCNN, create_native_model
+from torch.nn import Module
 
 
 class ModelWizard(Wizard):
     def __init__(self):
         self._model = None
 
     def use_model(self, model: Module):
```

### Comparing `dltrain-0.1.1/src/dltrain/builder/optimizer.py` & `dltrain-0.1.2/src/dltrain/builder/optimizer.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/builder/scheduler.py` & `dltrain-0.1.2/src/dltrain/builder/scheduler.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/builder/transforms.py` & `dltrain-0.1.2/src/dltrain/builder/transforms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..transform import Transform, Standardize, Resize
+from ..transform import Transform, Standardize, Resize, Noise
 from .core import Wizard
 
 
 class TransformWizard(Wizard):
     def __init__(self):
         self._features_transform = []
         self._targets_transform = []
@@ -15,10 +15,13 @@
 
         return self
 
     def add_resize(self, size, is_feature=True):
         self.add_transform(Resize(size), is_feature)
         return self
 
+    def add_noise(self, rate=0.01, is_feature=True):
+        self.add_transform(Noise(rate), is_feature)
+
     def add_standardize(self, is_feature=True):
         self.add_transform(Standardize(), is_feature)
         return self
```

### Comparing `dltrain-0.1.1/src/dltrain/checkpoint.py` & `dltrain-0.1.2/src/dltrain/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/dataset.py` & `dltrain-0.1.2/src/dltrain/dataset.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/delineator.py` & `dltrain-0.1.2/src/dltrain/delineator.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/error.py` & `dltrain-0.1.2/src/dltrain/error.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/evaluation.py` & `dltrain-0.1.2/src/dltrain/evaluation.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/forward.py` & `dltrain-0.1.2/src/dltrain/forward.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/inject.py` & `dltrain-0.1.2/src/dltrain/inject.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/options.py` & `dltrain-0.1.2/src/dltrain/options.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/train.py` & `dltrain-0.1.2/src/dltrain/train.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain/transform.py` & `dltrain-0.1.2/src/dltrain/transform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 from abc import ABCMeta, abstractmethod
+
+import torch
 from torch import Tensor
 
 __all__ = [
     'Transform',
     'Container',
     'Resize',
+    'Noise',
     'Standardize'
 ]
 
 class Transform(metaclass=ABCMeta):
     def __call__(self, *args, **kwargs):
         return self.transform(*args, **kwargs)
 
     @abstractmethod
     def transform(self, data: Tensor):
         pass
 
 
+class Noise(Transform):
+    def __init__(self, rate=0.01):
+        self.rate = rate
+
+    def transform(self, data: Tensor):
+        noise = torch.rand(data.shape).to(data.device) * self.rate
+        return data + noise
+
+
 class Container(Transform):
     def __init__(self, transforms):
         self.transforms = transforms
 
     def transform(self, data: Tensor):
         if self.transforms is None:
             return data
```

### Comparing `dltrain-0.1.1/src/dltrain/utils.py` & `dltrain-0.1.2/src/dltrain/utils.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.1/src/dltrain.egg-info/PKG-INFO` & `dltrain-0.1.2/src/dltrain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -148,7 +148,16 @@
 | seed             | 3407                                               |
 | device           | cpu                                                |
 | save_checkpoint  | False                                              |
 | start_checkpoint | User-set                                           |
 | delineator*      | None,Must be specified by the user                 |
 | forward          | SimpleForward                                      |
 | trainer          | SimpleTrainer                                      |
+
+## Version Log
+- 0.0.1<br/>
+1、构造整体模型框架
+- 0.0.2<br/>
+1、加入了TaskBuilder方便构造模型
+- 0.1.2<br/>
+1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)
+2、将models.py封装到models包，添加了许多拆箱可用模型
```

### Comparing `dltrain-0.1.1/src/dltrain.egg-info/SOURCES.txt` & `dltrain-0.1.2/src/dltrain.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 src/dltrain/checkpoint.py
 src/dltrain/dataset.py
 src/dltrain/delineator.py
 src/dltrain/error.py
 src/dltrain/evaluation.py
 src/dltrain/forward.py
 src/dltrain/inject.py
-src/dltrain/models.py
 src/dltrain/options.py
 src/dltrain/train.py
 src/dltrain/transform.py
 src/dltrain/utils.py
 src/dltrain.egg-info/PKG-INFO
 src/dltrain.egg-info/SOURCES.txt
 src/dltrain.egg-info/dependency_links.txt
@@ -27,8 +26,12 @@
 src/dltrain/builder/delineator.py
 src/dltrain/builder/evaluation.py
 src/dltrain/builder/forward.py
 src/dltrain/builder/inject.py
 src/dltrain/builder/model.py
 src/dltrain/builder/optimizer.py
 src/dltrain/builder/scheduler.py
-src/dltrain/builder/transforms.py
+src/dltrain/builder/transforms.py
+src/dltrain/models/__init__.py
+src/dltrain/models/component.py
+src/dltrain/models/model.py
+src/dltrain/models/wrapper.py
```

