# Comparing `tmp/irisml_tasks_yolov9-0.0.1.tar.gz` & `tmp/irisml_tasks_yolov9-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml_tasks_yolov9-0.0.1.tar", last modified: Wed May  8 08:26:11 2024, max compression
+gzip compressed data, was "irisml_tasks_yolov9-0.0.2.tar", last modified: Wed May  8 16:39:01 2024, max compression
```

## Comparing `irisml_tasks_yolov9-0.0.1.tar` & `irisml_tasks_yolov9-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:26:11.589228 irisml_tasks_yolov9-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-08 08:24:02.000000 irisml_tasks_yolov9-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-08 08:26:11.589228 irisml_tasks_yolov9-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-08 08:24:02.000000 irisml_tasks_yolov9-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:26:11.585228 irisml_tasks_yolov9-0.0.1/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:26:11.585228 irisml_tasks_yolov9-0.0.1/irisml/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:26:11.589228 irisml_tasks_yolov9-0.0.1/irisml/tasks/create_yolov9_detection_model/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 08:24:02.000000 irisml_tasks_yolov9-0.0.1/irisml/tasks/create_yolov9_detection_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-08 08:24:02.000000 irisml_tasks_yolov9-0.0.1/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:26:11.589228 irisml_tasks_yolov9-0.0.1/irisml_tasks_yolov9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-08 08:26:11.000000 irisml_tasks_yolov9-0.0.1/irisml_tasks_yolov9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-08 08:26:11.000000 irisml_tasks_yolov9-0.0.1/irisml_tasks_yolov9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:26:11.000000 irisml_tasks_yolov9-0.0.1/irisml_tasks_yolov9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 08:26:11.000000 irisml_tasks_yolov9-0.0.1/irisml_tasks_yolov9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 08:26:11.000000 irisml_tasks_yolov9-0.0.1/irisml_tasks_yolov9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 08:24:02.000000 irisml_tasks_yolov9-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:26:11.589228 irisml_tasks_yolov9-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:26:11.589228 irisml_tasks_yolov9-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-08 08:24:02.000000 irisml_tasks_yolov9-0.0.1/test/test_create_yolov9_detection_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:01.607155 irisml_tasks_yolov9-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-08 16:36:50.000000 irisml_tasks_yolov9-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-08 16:39:01.607155 irisml_tasks_yolov9-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-08 16:36:50.000000 irisml_tasks_yolov9-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:01.603155 irisml_tasks_yolov9-0.0.2/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:01.603155 irisml_tasks_yolov9-0.0.2/irisml/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:01.607155 irisml_tasks_yolov9-0.0.2/irisml/tasks/create_yolov9_detection_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 16:36:50.000000 irisml_tasks_yolov9-0.0.2/irisml/tasks/create_yolov9_detection_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-08 16:36:50.000000 irisml_tasks_yolov9-0.0.2/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:01.607155 irisml_tasks_yolov9-0.0.2/irisml_tasks_yolov9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-08 16:39:01.000000 irisml_tasks_yolov9-0.0.2/irisml_tasks_yolov9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-08 16:39:01.000000 irisml_tasks_yolov9-0.0.2/irisml_tasks_yolov9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:39:01.000000 irisml_tasks_yolov9-0.0.2/irisml_tasks_yolov9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 16:39:01.000000 irisml_tasks_yolov9-0.0.2/irisml_tasks_yolov9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 16:39:01.000000 irisml_tasks_yolov9-0.0.2/irisml_tasks_yolov9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 16:36:50.000000 irisml_tasks_yolov9-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:39:01.607155 irisml_tasks_yolov9-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:01.607155 irisml_tasks_yolov9-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-08 16:36:50.000000 irisml_tasks_yolov9-0.0.2/test/test_create_yolov9_detection_model.py
```

### Comparing `irisml_tasks_yolov9-0.0.1/LICENSE` & `irisml_tasks_yolov9-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.1/PKG-INFO` & `irisml_tasks_yolov9-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-Metadata-Version: 2.1
-Name: irisml-tasks-yolov9
-Version: 0.0.1
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: irisml
-Requires-Dist: pyyolov9<1
-
 # irisml-tasks-yolov9
 
 This package is to integrate the [yolov9](https://github.com/WongKinYiu/yolov9) library into the [irisml](https://github.com/microsoft/irisml) framework.
 
+## Convert the official weights
+To load the offficial weights from the yolov9 repository, you can use the following script:
+```bash
+sys.path.append(<path to yolov9 repository>)
+model = torch.load('yolov9-c.pt', map_location='cpu')
+torch.save(model['model'].state_dict(), 'model.pth')
+```
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
 
 When you submit a pull request, a CLA bot will automatically determine whether you need to provide
```

### Comparing `irisml_tasks_yolov9-0.0.1/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py` & `irisml_tasks_yolov9-0.0.2/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         nms_iou_threshold (float): The IoU threshold for non-maximum suppression.
     """
 
     VERSION = '0.1.0'
 
     @dataclasses.dataclass
     class Config:
-        model_name: typing.Literal['yolov9-c', 'yolov9-e', 'yolov9', 'gelan-c', 'gelan-e', 'gelan']
+        model_name: typing.Literal['yolov9c', 'yolov9e', 'yolov9', 'gelanc', 'gelane', 'gelan']
         num_classes: int
         nms_conf_threshold: float = 0.001
         nms_iou_threshold: float = 0.7
 
     @dataclasses.dataclass
     class Outputs:
         model: torch.nn.Module
@@ -73,15 +73,15 @@
         features = self._model(inputs)
         loss, _ = self._loss(features, targets)
         return {'loss': loss}
 
     def prediction_step(self, inputs):
         pred = self._model(inputs)
         if self._has_dual_loss:
-            assert isinstance(pred, list)
+            assert isinstance(pred[0], list)
             pred = pred[0][1]
 
         yolo_predictions = yolov9.utils.general.non_max_suppression(pred, self._nms_conf_threshold, self._nms_iou_threshold, labels=[], multi_label=True, agnostic=False, max_det=300)
         for p in yolo_predictions:
             # Convert [x,y,x2,y2,conf,cls] to [cls,conf,x,y,x2,y2]
             p[:, [0, 1, 2, 3, 4, 5]] = p[:, [5, 4, 0, 1, 2, 3]]
             p[:, (2, 4)] /= inputs.shape[3]  # Normalize x
```

### Comparing `irisml_tasks_yolov9-0.0.1/irisml_tasks_yolov9.egg-info/PKG-INFO` & `irisml_tasks_yolov9-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-yolov9
-Version: 0.0.1
+Version: 0.0.2
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: irisml
 Requires-Dist: pyyolov9<1
 
 # irisml-tasks-yolov9
 
 This package is to integrate the [yolov9](https://github.com/WongKinYiu/yolov9) library into the [irisml](https://github.com/microsoft/irisml) framework.
 
+## Convert the official weights
+To load the offficial weights from the yolov9 repository, you can use the following script:
+```bash
+sys.path.append(<path to yolov9 repository>)
+model = torch.load('yolov9-c.pt', map_location='cpu')
+torch.save(model['model'].state_dict(), 'model.pth')
+```
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
 
 When you submit a pull request, a CLA bot will automatically determine whether you need to provide
```

### Comparing `irisml_tasks_yolov9-0.0.1/test/test_create_yolov9_detection_model.py` & `irisml_tasks_yolov9-0.0.2/test/test_create_yolov9_detection_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import unittest
 import torch
 from irisml.tasks.create_yolov9_detection_model import Task
 
 class TestCreateYolov9DetectionModel(unittest.TestCase):
     def test_yolov9(self):
-        model = Task(Task.Config(model_name='yolov9-c', num_classes=3)).execute(Task.Inputs()).model
+        model = Task(Task.Config(model_name='yolov9c', num_classes=3)).execute(Task.Inputs()).model
 
         self.assertIsInstance(model, torch.nn.Module)
         outputs = model.training_step(torch.rand(2, 3, 32, 32), [torch.zeros(0, 5), torch.tensor([[0, 0.0, 0.0, 1.0, 1.0]])])
         self.assertIsInstance(outputs, dict)
         self.assertIsInstance(outputs['loss'], torch.Tensor)
 
         outputs = model.prediction_step(torch.rand(2, 3, 32, 32))
         self.assertIsInstance(outputs, list)
         self.assertEqual(len(outputs), 2)
         self.assertIsInstance(outputs[0], torch.Tensor)
         self.assertIsInstance(outputs[1], torch.Tensor)
 
     def test_gelan(self):
-        model = Task(Task.Config(model_name='gelan-c', num_classes=3)).execute(Task.Inputs()).model
+        model = Task(Task.Config(model_name='gelanc', num_classes=3)).execute(Task.Inputs()).model
 
         self.assertIsInstance(model, torch.nn.Module)
         outputs = model.training_step(torch.rand(2, 3, 32, 32), [torch.zeros(0, 5), torch.tensor([[0, 0.0, 0.0, 1.0, 1.0]])])
         self.assertIsInstance(outputs, dict)
         self.assertIsInstance(outputs['loss'], torch.Tensor)
 
         outputs = model.prediction_step(torch.rand(2, 3, 32, 32))
```

