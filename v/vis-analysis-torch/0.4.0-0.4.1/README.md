# Comparing `tmp/vis_analysis_torch-0.4.0.tar.gz` & `tmp/vis_analysis_torch-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vis_analysis_torch-0.4.0.tar", last modified: Wed May  8 07:28:02 2024, max compression
+gzip compressed data, was "vis_analysis_torch-0.4.1.tar", last modified: Wed May  8 08:11:57 2024, max compression
```

## Comparing `vis_analysis_torch-0.4.0.tar` & `vis_analysis_torch-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 07:28:02.951342 vis_analysis_torch-0.4.0/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 07:28:02.951342 vis_analysis_torch-0.4.0/PKG-INFO
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       38 2024-05-08 07:28:02.951342 vis_analysis_torch-0.4.0/setup.cfg
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      498 2024-05-08 07:27:58.000000 vis_analysis_torch-0.4.0/setup.py
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 07:28:02.951342 vis_analysis_torch-0.4.0/vis_analysis_torch/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 03:28:25.000000 vis_analysis_torch-0.4.0/vis_analysis_torch/__init__.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     2410 2024-05-08 07:27:45.000000 vis_analysis_torch-0.4.0/vis_analysis_torch/bbox_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 02:55:56.000000 vis_analysis_torch-0.4.0/vis_analysis_torch/common_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     5421 2024-05-08 07:20:23.000000 vis_analysis_torch-0.4.0/vis_analysis_torch/pose_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     1503 2024-05-08 07:19:06.000000 vis_analysis_torch-0.4.0/vis_analysis_torch/utils.py
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 07:28:02.951342 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 07:28:02.000000 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/PKG-INFO
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      401 2024-05-08 07:28:02.000000 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/SOURCES.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        1 2024-05-08 07:28:02.000000 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/dependency_links.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       26 2024-05-08 07:28:02.000000 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/requires.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       19 2024-05-08 07:28:02.000000 vis_analysis_torch-0.4.0/vis_analysis_torch.egg-info/top_level.txt
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:11:57.948718 vis_analysis_torch-0.4.1/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 08:11:57.948718 vis_analysis_torch-0.4.1/PKG-INFO
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       38 2024-05-08 08:11:57.948718 vis_analysis_torch-0.4.1/setup.cfg
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      498 2024-05-08 08:11:54.000000 vis_analysis_torch-0.4.1/setup.py
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:11:57.948718 vis_analysis_torch-0.4.1/vis_analysis_torch/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 03:28:25.000000 vis_analysis_torch-0.4.1/vis_analysis_torch/__init__.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     3338 2024-05-08 08:11:41.000000 vis_analysis_torch-0.4.1/vis_analysis_torch/bbox_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 02:55:56.000000 vis_analysis_torch-0.4.1/vis_analysis_torch/common_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     7369 2024-05-08 08:11:50.000000 vis_analysis_torch-0.4.1/vis_analysis_torch/pose_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     2776 2024-05-08 07:55:53.000000 vis_analysis_torch-0.4.1/vis_analysis_torch/utils.py
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:11:57.948718 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 08:11:57.000000 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/PKG-INFO
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      401 2024-05-08 08:11:57.000000 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/SOURCES.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        1 2024-05-08 08:11:57.000000 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/dependency_links.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       26 2024-05-08 08:11:57.000000 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/requires.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       19 2024-05-08 08:11:57.000000 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/top_level.txt
```

### Comparing `vis_analysis_torch-0.4.0/vis_analysis_torch/bbox_visualization.py` & `vis_analysis_torch-0.4.1/vis_analysis_torch/bbox_visualization.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 import numpy as np
 import cv2
 import os
 
-from utils import convert_image
-
-# 读取图像
-image = cv2.imread('example.jpg')
-
-# 定义矩形框的左上角和右下角坐标
-x1, y1 = 100, 100  # 左上角坐标
-x2, y2 = 300, 300  # 右下角坐标
-
-# 定义矩形框的颜色（BGR 格式）
-color =   # 这里是绿色
-
-# 画矩形框
-
-
-# 显示图像
-cv2.imshow('Rectangle', image)
-cv2.waitKey(0)
-cv2.destroyAllWindows()
-
+from .utils import convert_image
 
 def draw_bbox_in_image(img: np.array, 
-                       bboxes,
+                       bboxes: np.array, 
+                       xyxy: bool = False,
                        save_root_dir: str = "./",
-                       save_img_name: str = "origin-draw-pose-img.jpg", 
+                       save_img_name: str = "origin-draw-bbox-img.jpg", 
                        RGB2BGR: bool = False,
                        normlization: bool = False,
                        standardization_mean: np.array = None,
                        standardization_std: np.array = None,
                        draw_bboxes_color: tuple = (0, 255, 0),
-                       draw_bboxes_thickness: int = 2):
-    """draw pose in image and save it in save_dir
+                       draw_bboxes_thickness: int = 2) -> np.array:
+    """在给定的图片中绘制bbox，并保存
 
     Args:
-        img (np.array): img to draw pose
-        pose (_type_): pose can be multiple person or single person
-        save_dir (_type_): the dir to save the pose image
-        dataset_category (dict, optional): dataset_category, it must contain skeleton at least. Defaults to COCO_CATEGORY.
+        img (np.array): 绘制图片，尺寸为(H, W, C)
+        bboxes (_type_): bbox坐标，可以是多个bbox，shape为(N, 4)或(4,)
+        xyxy (bool, optional): 是否为左上右下坐标的格式，否则认定为左上宽高的格式. Defaults to True.
+        save_root_dir (str, optional): 绘制后图片保存的根路径. Defaults to "./".
+        save_img_name (str, optional): 保存图片的名称. Defaults to "origin-draw-bbox-img.jpg".
+        RGB2BGR (bool, optional): 是否进行RGB2BGR的转换. Defaults to False.
+        normlization (bool, optional): 是否需要逆归一化. Defaults to False.
+        standardization_mean (np.array, optional): 是否需要逆标准化，需要同时传入方差和标准差的值. Defaults to None.
+        standardization_std (np.array, optional): 是否需要逆标准化，需要同时传入方差和标准差的值. Defaults to None.
+        draw_bboxes_color (tuple, optional): bbox绘制颜色，传参时尺寸要求为[N, 3]. Defaults to (0, 255, 0).
+        draw_bboxes_thickness (int, optional): bbox绘制粗细. Defaults to 2.
+
+    Returns:
+        np.array: 绘制好的图片
     """
+    
     img = convert_image(img, RGB2BGR, normlization, standardization_mean, standardization_std)
     
-    bboxes = np.array(bboxes)
-    assert bboxes.shape[-1] == 4, "the last dimension of bboxes must be 4. It means (x, y, w, h)"
+    assert isinstance(bboxes, np.array), "bboxes must be np.array"
+    if len(bboxes.shape) == 1: # (4,) -> (1, 4)
+        bboxes = bboxes[None, :]
+        
+    assert bboxes.shape[-1] == 4, "the last dimension of bboxes must be 4. It means (x1, y1, x2, x2) or (x, y, w, h)"
     
+    if not xyxy: # 将左上宽高转为左上右下
+        # xywh2xyxy
+        bboxes[:, 2] += bboxes[:, 0]
+        bboxes[:, 3] += bboxes[:, 1]
+        
     if not os.path.isdir(save_root_dir):
         # 创建文件夹
         os.makedirs(save_root_dir)
             
     save_img_dir = os.path.join(save_root_dir, save_img_name)
 
     if isinstance(draw_bboxes_color, tuple):
         draw_bboxes_color = [draw_bboxes_color for _ in range(bboxes.shape[0])]
-        
+    assert len(draw_bboxes_color) == bboxes.shape[0], "the length of draw_bboxes_color must equal to the number of bboxes"
+    
     for i, _bbox in enumerate(bboxes):
-        x, y, w, h = _bbox
-        
-        tl_x, tl_y = x - w / 2, y - h / 2
-        br_x, br_y = x + w / 2, y + h / 2
+        tl_x, tl_y, br_x, br_y = _bbox
         
         # 判断左上角和右下角是否在图像内
         if tl_x < 0 or tl_y < 0 or br_x >= img.shape[1] or br_y >= img.shape[0]:
             continue
         
-        # 绘制
-        cv2.rectangle(image, (int(tl_x), int(tl_y)), (int(br_x), int(br_y)), draw_bboxes_color[i], thickness=draw_bboxes_thickness)
-            
+        # 绘制矩形框
+        cv2.rectangle(img, (int(tl_x), int(tl_y)), (int(br_x), int(br_y)), draw_bboxes_color[i], thickness=draw_bboxes_thickness)
+
     cv2.imwrite(save_img_dir, img)
     
     return img
```

