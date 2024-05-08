# Comparing `tmp/vis_analysis_torch-0.3.tar.gz` & `tmp/vis_analysis_torch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vis_analysis_torch-0.3.tar", last modified: Wed May  8 05:30:32 2024, max compression
+gzip compressed data, was "vis_analysis_torch-0.3.1.tar", last modified: Wed May  8 05:42:42 2024, max compression
```

## Comparing `vis_analysis_torch-0.3.tar` & `vis_analysis_torch-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 05:30:32.454025 vis_analysis_torch-0.3/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      330 2024-05-08 05:30:32.454025 vis_analysis_torch-0.3/PKG-INFO
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       38 2024-05-08 05:30:32.454025 vis_analysis_torch-0.3/setup.cfg
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      496 2024-05-08 05:30:24.000000 vis_analysis_torch-0.3/setup.py
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 05:30:32.454025 vis_analysis_torch-0.3/vis_analysis_torch/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 03:28:25.000000 vis_analysis_torch-0.3/vis_analysis_torch/__init__.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 02:55:56.000000 vis_analysis_torch-0.3/vis_analysis_torch/common_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     5895 2024-05-08 04:00:11.000000 vis_analysis_torch-0.3/vis_analysis_torch/pose_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      611 2024-05-08 04:01:43.000000 vis_analysis_torch-0.3/vis_analysis_torch/utils.py
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 05:30:32.454025 vis_analysis_torch-0.3/vis_analysis_torch.egg-info/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      330 2024-05-08 05:30:32.000000 vis_analysis_torch-0.3/vis_analysis_torch.egg-info/PKG-INFO
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      360 2024-05-08 05:30:32.000000 vis_analysis_torch-0.3/vis_analysis_torch.egg-info/SOURCES.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        1 2024-05-08 05:30:32.000000 vis_analysis_torch-0.3/vis_analysis_torch.egg-info/dependency_links.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       26 2024-05-08 05:30:32.000000 vis_analysis_torch-0.3/vis_analysis_torch.egg-info/requires.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       19 2024-05-08 05:30:32.000000 vis_analysis_torch-0.3/vis_analysis_torch.egg-info/top_level.txt
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 05:42:42.136011 vis_analysis_torch-0.3.1/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 05:42:42.136011 vis_analysis_torch-0.3.1/PKG-INFO
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       38 2024-05-08 05:42:42.136011 vis_analysis_torch-0.3.1/setup.cfg
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      498 2024-05-08 05:41:47.000000 vis_analysis_torch-0.3.1/setup.py
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 05:42:42.136011 vis_analysis_torch-0.3.1/vis_analysis_torch/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 03:28:25.000000 vis_analysis_torch-0.3.1/vis_analysis_torch/__init__.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 02:55:56.000000 vis_analysis_torch-0.3.1/vis_analysis_torch/common_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     5902 2024-05-08 05:42:32.000000 vis_analysis_torch-0.3.1/vis_analysis_torch/pose_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      611 2024-05-08 04:01:43.000000 vis_analysis_torch-0.3.1/vis_analysis_torch/utils.py
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 05:42:42.136011 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 05:42:42.000000 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/PKG-INFO
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      360 2024-05-08 05:42:42.000000 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/SOURCES.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        1 2024-05-08 05:42:42.000000 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/dependency_links.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       26 2024-05-08 05:42:42.000000 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/requires.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       19 2024-05-08 05:42:42.000000 vis_analysis_torch-0.3.1/vis_analysis_torch.egg-info/top_level.txt
```

### Comparing `vis_analysis_torch-0.3/vis_analysis_torch/pose_visualization.py` & `vis_analysis_torch-0.3.1/vis_analysis_torch/pose_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,31 +78,31 @@
         
     if standardization_mean is not None and standardization_std is not None:
         img = img * standardization_std + standardization_mean
     
     if RGB2BGR:
         input_tensor = cv2.cvtColor(input_tensor, cv2.COLOR_RGB2BGR)
     
-    if len(pose.shape) == 2:
-        pose = pose[None, :]
-    if pose.shape[2] == 3:
-        pose = pose[:, :, :2]
+    if len(poses.shape) == 2:
+        poses = poses[None, :]
+    if poses.shape[2] == 3:
+        poses = poses[:, :, :2]
     
     assert draw_preset in ['coco', 'sodpose', None], "draw_preset must be in ['coco', 'sodpose', None]"
     
     if draw_preset:
         skeleton, draw_point_color, draw_skeleton_color = get_draw_preset(draw_preset)
     else:
         assert skeleton is not None, "skeleton must be provided when draw_preset is None"
         
         min_kpt_id = np.min(skeleton.flatten())
         assert min_kpt_id == 1, "the keypoint id must be starting from 0"
         
         if isinstance(draw_point_color, tuple):
-            draw_point_color = [draw_point_color for _ in range(pose.shape[1])]
+            draw_point_color = [draw_point_color for _ in range(poses.shape[1])]
         if isinstance(draw_skeleton_color, tuple):
             draw_skeleton_color = [draw_skeleton_color for _ in range(len(skeleton))]
     
     if not os.path.isdir(save_root_dir):
         # 创建文件夹
         os.makedirs(save_root_dir)
```

### Comparing `vis_analysis_torch-0.3/vis_analysis_torch/utils.py` & `vis_analysis_torch-0.3.1/vis_analysis_torch/utils.py`

 * *Files identical despite different names*

