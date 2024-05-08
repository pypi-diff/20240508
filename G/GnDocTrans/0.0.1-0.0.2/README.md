# Comparing `tmp/GnDocTrans-0.0.1.tar.gz` & `tmp/GnDocTrans-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GnDocTrans-0.0.1.tar", last modified: Tue May  7 07:56:35 2024, max compression
+gzip compressed data, was "GnDocTrans-0.0.2.tar", last modified: Wed May  8 03:24:04 2024, max compression
```

## Comparing `GnDocTrans-0.0.1.tar` & `GnDocTrans-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-07 07:56:35.379974 GnDocTrans-0.0.1/
-drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-07 07:56:35.379974 GnDocTrans-0.0.1/GnDocTrans/
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       30 2024-05-07 06:57:19.000000 GnDocTrans-0.0.1/GnDocTrans/__init__.py
--rw-rw-r--   0 fusen     (1000) fusen     (1000)    16822 2024-05-07 06:56:28.000000 GnDocTrans-0.0.1/GnDocTrans/tri_derive_tile.py
-drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-07 07:56:35.379974 GnDocTrans-0.0.1/GnDocTrans.egg-info/
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-07 07:56:35.000000 GnDocTrans-0.0.1/GnDocTrans.egg-info/PKG-INFO
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      230 2024-05-07 07:56:35.000000 GnDocTrans-0.0.1/GnDocTrans.egg-info/SOURCES.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)        1 2024-05-07 07:56:35.000000 GnDocTrans-0.0.1/GnDocTrans.egg-info/dependency_links.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       20 2024-05-07 07:56:35.000000 GnDocTrans-0.0.1/GnDocTrans.egg-info/requires.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       11 2024-05-07 07:56:35.000000 GnDocTrans-0.0.1/GnDocTrans.egg-info/top_level.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-07 07:56:35.379974 GnDocTrans-0.0.1/PKG-INFO
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       38 2024-05-07 07:56:35.379974 GnDocTrans-0.0.1/setup.cfg
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      501 2024-05-07 07:15:53.000000 GnDocTrans-0.0.1/setup.py
+drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-08 03:24:04.553559 GnDocTrans-0.0.2/
+drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-08 03:24:04.553559 GnDocTrans-0.0.2/GnDocTrans/
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       30 2024-05-07 06:57:19.000000 GnDocTrans-0.0.2/GnDocTrans/__init__.py
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)    17814 2024-05-08 03:22:06.000000 GnDocTrans-0.0.2/GnDocTrans/tri_derive_tile.py
+drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-08 03:24:04.553559 GnDocTrans-0.0.2/GnDocTrans.egg-info/
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-08 03:24:04.000000 GnDocTrans-0.0.2/GnDocTrans.egg-info/PKG-INFO
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      230 2024-05-08 03:24:04.000000 GnDocTrans-0.0.2/GnDocTrans.egg-info/SOURCES.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)        1 2024-05-08 03:24:04.000000 GnDocTrans-0.0.2/GnDocTrans.egg-info/dependency_links.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       20 2024-05-08 03:24:04.000000 GnDocTrans-0.0.2/GnDocTrans.egg-info/requires.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       11 2024-05-08 03:24:04.000000 GnDocTrans-0.0.2/GnDocTrans.egg-info/top_level.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-08 03:24:04.553559 GnDocTrans-0.0.2/PKG-INFO
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       38 2024-05-08 03:24:04.553559 GnDocTrans-0.0.2/setup.cfg
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      501 2024-05-08 03:22:16.000000 GnDocTrans-0.0.2/setup.py
```

### Comparing `GnDocTrans-0.0.1/GnDocTrans/tri_derive_tile.py` & `GnDocTrans-0.0.2/GnDocTrans/tri_derive_tile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __all__ = [
     'tileWithTri'
 ]
 
 
+
 import cv2
 import numpy as np
 from numpy import ndarray
 import base64
 from typing import Literal
 import math
 import copy
@@ -153,25 +154,44 @@
     return {
         'islet': boxes_of_islet,
         'sector': boxes_of_sector,
     }
 
 
 
-def randBoxes(cell_w: int, cell_h: int, rows: int, cols: int, probability: float) -> dict[str, list[list]]:
+def randBoxes(cell_w: int, cell_h: int, rows: int, cols: int, probability: float, exist_boxes: dict[str, list[list]]) -> dict[str, list[list]]:
     random.seed(time.time())
     probability = 0 if probability < 0 else probability
     probability = 1 if probability > 1 else probability
     half_cell_w = cell_w / 2
     boxes_of_random: list[list] = []
+    flags_dict: dict[str, list[bool]] = {
+        'islet': [False]*len(exist_boxes['islet'])
+    }
     for row in range(rows):
         col_shift = half_cell_w if row%2 else 0
         for col in range(cols+(row%2)):
             if random.random() < probability:
-                boxes_of_random.append([col*cell_w - col_shift, row*cell_h, cell_w, cell_h])
+                tl_x = col*cell_w - col_shift
+                tl_y = row*cell_h
+                center_x = tl_x + cell_w / 2
+                center_y = tl_y + cell_h / 2
+                is_in_box: bool = False
+                for name, flag_list in flags_dict.items():
+                    for index, flag in enumerate(flag_list):
+                        if flag:
+                            continue
+                        is_in_box = (exist_boxes[name][index][0] < center_x and center_x < exist_boxes[name][index][0]+exist_boxes[name][index][2]) and \
+                            (exist_boxes[name][index][1] < center_y and center_y < exist_boxes[name][index][1]+exist_boxes[name][index][3])
+                        if is_in_box:
+                            break
+                    if is_in_box:
+                        break
+                if not is_in_box:
+                    boxes_of_random.append([tl_x, tl_y, cell_w, cell_h])
     return {
         'random': boxes_of_random
     }
     
 
 
 
@@ -306,15 +326,15 @@
     else:
         if 'left' == direction:
             shift_x = int(math.floor(sandbox_width * reference_cx))
         else:
             shift_x = int(math.ceil(sandbox_width * reference_cx))
         shift_x = shift_x // cell_width * cell_width
     boxes_raw = shiftBoxes(boxes_raw, shift_x, shift_y)
-    boxes_rand = randBoxes(cell_width, cell_height, cell_rows, cell_cols, probability)
+    boxes_rand = randBoxes(cell_width, cell_height, cell_rows, cell_cols, probability, boxes_raw)
     boxes_all = copy.deepcopy(boxes_raw)
     boxes_all.update(boxes_rand)
     # print(boxes_all)
     boxes_str = pathsToSVG(boxesToPaths(boxes_all, element_extend=2))
     # print(boxes_str)
     boxes_patch = copy.deepcopy(boxes_rand)
     boxes_patch['sector'] = copy.deepcopy(boxes_raw['sector'])
@@ -457,30 +477,30 @@
     image = cv2.imread(img_path, cv2.IMREAD_UNCHANGED)
     gray = cv2.cvtColor(image, cv2.COLOR_BGRA2GRAY)
     binary = cv2.threshold(gray, 127, 255, cv2.THRESH_BINARY_INV+cv2.THRESH_OTSU)[1]
     cont = cv2.drawContours(np.full_like(binary, 0, np.uint8), cv2.findContours(binary, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE)[0], -1, 255, 10)
     binary = np.stack([binary]*4, axis=2)
     cont = np.stack([cont]*4, axis=2)
     img_str = opencv2base64(image)
-    gry_str = opencv2base64(cont)
+    con_str = opencv2base64(cont)
     bin_str = opencv2base64(binary)
     image_height, image_width = image.shape[:2]
-    image_height, image_width = image_height // 10, image_width // 10
+    image_height, image_width = image_height // 15, image_width // 15
     svg_str = tileWithTri(
-        resolution_width=2048, resolution_height=1024,
-        canvas_width=2048, canvas_height=1024,
-        original_img_str=img_str, derive1_img_str=bin_str, derive2_img_str=gry_str,
-        structure='y-2',
+        resolution_width=1024, resolution_height=1024,
+        canvas_width=1024, canvas_height=1024,
+        original_img_str=img_str, derive1_img_str=bin_str, derive2_img_str=con_str,
+        structure='2-1',
         direction='right',
         location='islet',
         shift='3',
-        probability=0.0,
-        reference_cx=0.8, reference_cy=0.4,
+        probability=0.5,
+        reference_cx=0.5, reference_cy=0.4,
         image_width=image_width, image_height=image_height,
         space_width=image_width//10, space_height=image_width//12,
     )
-    with open('result.svg', 'w') as fp:
+    with open('2-1-0.5.svg', 'w') as fp:
         fp.write(svg_str)
 
 
 if '__main__' == __name__:
     test()
```

