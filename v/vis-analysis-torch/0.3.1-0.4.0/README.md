# Comparing `tmp/vis_analysis_torch-0.3.1.tar.gz` & `tmp/vis_analysis_torch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vis_analysis_torch-0.3.1.tar", last modified: Wed May  8 05:42:42 2024, max compression
+gzip compressed data, was "vis_analysis_torch-0.4.0.tar", last modified: Wed May  8 07:28:02 2024, max compression
```

## Comparing `vis_analysis_torch-0.3.1.tar` & `vis_analysis_torch-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 05:42:42.136011 vis_analysis_torch-0.3.1/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 05:42:42.136011 vis_analysis_torch-0.3.1/PKG-INFO
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       38 2024-05-08 05:42:42.136011 vis_analysis_torch-0.3.1/setup.cfg
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      498 2024-05-08 05:41:47.000000 vis_analysis_torch-0.3.1/setup.py
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 05:42:42.136011 vis_analysis_torch-0.3.1/vis_analysis_torch/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 03:28:25.000000 vis_analysis_torch-0.3.1/vis_analysis_torch/__init__.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 02:55:56.000000 vis_analysis_torch-0.3.1/vis_analysis_torch/common_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     5902 2024-05-08 05:42:32.000000 vis_analysis_torch-0.3.1/vis_analysis_torch/pose_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      611 2024-05-08 04:01:43.000000 vis_analysis_torch-0.3.1/vis_analysis_torch/utils.py
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 05:42:42.136011 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 05:42:42.000000 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/PKG-INFO
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      360 2024-05-08 05:42:42.000000 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/SOURCES.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        1 2024-05-08 05:42:42.000000 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/dependency_links.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       26 2024-05-08 05:42:42.000000 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/requires.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       19 2024-05-08 05:42:42.000000 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/top_level.txt
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 07:28:02.951342 vis_analysis_torch-0.4.0/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 07:28:02.951342 vis_analysis_torch-0.4.0/PKG-INFO
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       38 2024-05-08 07:28:02.951342 vis_analysis_torch-0.4.0/setup.cfg
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      498 2024-05-08 07:27:58.000000 vis_analysis_torch-0.4.0/setup.py
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 07:28:02.951342 vis_analysis_torch-0.4.0/vis_analysis_torch/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 03:28:25.000000 vis_analysis_torch-0.4.0/vis_analysis_torch/__init__.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     2410 2024-05-08 07:27:45.000000 vis_analysis_torch-0.4.0/vis_analysis_torch/bbox_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 02:55:56.000000 vis_analysis_torch-0.4.0/vis_analysis_torch/common_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     5421 2024-05-08 07:20:23.000000 vis_analysis_torch-0.4.0/vis_analysis_torch/pose_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     1503 2024-05-08 07:19:06.000000 vis_analysis_torch-0.4.0/vis_analysis_torch/utils.py
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 07:28:02.951342 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 07:28:02.000000 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/PKG-INFO
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      401 2024-05-08 07:28:02.000000 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/SOURCES.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        1 2024-05-08 07:28:02.000000 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/dependency_links.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       26 2024-05-08 07:28:02.000000 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/requires.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       19 2024-05-08 07:28:02.000000 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/top_level.txt
```

### Comparing `vis_analysis_torch-0.3.1/vis_analysis_torch/pose_visualization.py` & `vis_analysis_torch-0.4.0/vis_analysis_torch/pose_visualization.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 import torch
 import cv2
 import os
+
+from utils import convert_image
     
 def get_draw_preset(draw_preset):
     skeleton, kpt_color, skeleton_color = None, None, None
     if draw_preset == 'coco':
         skeleton = [[15, 13], [13, 11], [16, 14], [14, 12], 
                     [11, 12], [5, 11], [6, 12], [5, 6], 
                     [5, 7], [6, 8], [7, 9], [8, 10], 
@@ -65,26 +67,15 @@
 
     Args:
         img (np.array): img to draw pose
         pose (_type_): pose can be multiple person or single person
         save_dir (_type_): the dir to save the pose image
         dataset_category (dict, optional): dataset_category, it must contain skeleton at least. Defaults to COCO_CATEGORY.
     """
-    if normlization:
-        img = img * 255
-    
-    assert img.shape[2] == 3, "the last dimension of img must be 3. It means color channel"
-    assert (standardization_mean is None and standardization_std is None) \
-        or (standardization_mean is not None and standardization_std is not None), "standardization_mean and standardization_std must be None or not None at the same time"
-        
-    if standardization_mean is not None and standardization_std is not None:
-        img = img * standardization_std + standardization_mean
-    
-    if RGB2BGR:
-        input_tensor = cv2.cvtColor(input_tensor, cv2.COLOR_RGB2BGR)
+    img = convert_image(img, RGB2BGR, normlization, standardization_mean, standardization_std)
     
     if len(poses.shape) == 2:
         poses = poses[None, :]
     if poses.shape[2] == 3:
         poses = poses[:, :, :2]
     
     assert draw_preset in ['coco', 'sodpose', None], "draw_preset must be in ['coco', 'sodpose', None]"
@@ -115,8 +106,10 @@
                 
             # 绘制骨架
             cv2.circle(img, (int(x), int(y)), draw_point_size, draw_point_color[i], draw_point_thickness)
             
         for i, (s, e) in enumerate(skeleton): # draw skeleton
             cv2.line(img, (int(_pose[s][0]), int(_pose[s][1])), (int(_pose[e][0]),int(_pose[e][1])), draw_skeleton_color[i]) 
             
-    cv2.imwrite(save_img_dir, img)
+    cv2.imwrite(save_img_dir, img)
+    
+    return img
```

