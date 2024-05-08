# Comparing `tmp/mdetsyn-0.0.4.tar.gz` & `tmp/mdetsyn-0.0.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdetsyn-0.0.4.tar", last modified: Wed May  8 08:54:08 2024, max compression
+gzip compressed data, was "mdetsyn-0.0.4.post1.tar", last modified: Wed May  8 10:18:56 2024, max compression
```

## Comparing `mdetsyn-0.0.4.tar` & `mdetsyn-0.0.4.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-08 08:54:08.803715 mdetsyn-0.0.4/
--rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)     2263 2024-05-08 08:54:08.803715 mdetsyn-0.0.4/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     1994 2024-05-08 08:02:23.000000 mdetsyn-0.0.4/README.md
-drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-08 08:54:08.803715 mdetsyn-0.0.4/mdetsyn/
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       46 2024-05-08 08:00:50.000000 mdetsyn-0.0.4/mdetsyn/__init__.py
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     9603 2024-05-08 08:50:45.000000 mdetsyn-0.0.4/mdetsyn/detsyn.py
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     7598 2024-05-08 08:52:37.000000 mdetsyn-0.0.4/mdetsyn/helpers.py
-drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-08 08:54:08.803715 mdetsyn-0.0.4/mdetsyn.egg-info/
--rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)     2263 2024-05-08 08:54:08.000000 mdetsyn-0.0.4/mdetsyn.egg-info/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      246 2024-05-08 08:54:08.000000 mdetsyn-0.0.4/mdetsyn.egg-info/SOURCES.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        1 2024-05-08 08:54:08.000000 mdetsyn-0.0.4/mdetsyn.egg-info/dependency_links.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       21 2024-05-08 08:54:08.000000 mdetsyn-0.0.4/mdetsyn.egg-info/requires.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        8 2024-05-08 08:54:08.000000 mdetsyn-0.0.4/mdetsyn.egg-info/top_level.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       20 2024-05-06 07:47:54.000000 mdetsyn-0.0.4/requirements.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       38 2024-05-08 08:54:08.803715 mdetsyn-0.0.4/setup.cfg
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      696 2024-05-08 08:53:38.000000 mdetsyn-0.0.4/setup.py
+drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-08 10:18:56.656861 mdetsyn-0.0.4.post1/
+-rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)     2269 2024-05-08 10:18:56.656861 mdetsyn-0.0.4.post1/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     1994 2024-05-08 08:02:23.000000 mdetsyn-0.0.4.post1/README.md
+drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-08 10:18:56.656861 mdetsyn-0.0.4.post1/mdetsyn/
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       46 2024-05-08 08:00:50.000000 mdetsyn-0.0.4.post1/mdetsyn/__init__.py
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     9594 2024-05-08 10:17:08.000000 mdetsyn-0.0.4.post1/mdetsyn/detsyn.py
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     7879 2024-05-08 10:16:53.000000 mdetsyn-0.0.4.post1/mdetsyn/helpers.py
+drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-08 10:18:56.656861 mdetsyn-0.0.4.post1/mdetsyn.egg-info/
+-rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)     2269 2024-05-08 10:18:56.000000 mdetsyn-0.0.4.post1/mdetsyn.egg-info/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      246 2024-05-08 10:18:56.000000 mdetsyn-0.0.4.post1/mdetsyn.egg-info/SOURCES.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        1 2024-05-08 10:18:56.000000 mdetsyn-0.0.4.post1/mdetsyn.egg-info/dependency_links.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       21 2024-05-08 10:18:56.000000 mdetsyn-0.0.4.post1/mdetsyn.egg-info/requires.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        8 2024-05-08 10:18:56.000000 mdetsyn-0.0.4.post1/mdetsyn.egg-info/top_level.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       20 2024-05-06 07:47:54.000000 mdetsyn-0.0.4.post1/requirements.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       38 2024-05-08 10:18:56.656861 mdetsyn-0.0.4.post1/setup.cfg
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      702 2024-05-08 10:18:00.000000 mdetsyn-0.0.4.post1/setup.py
```

### Comparing `mdetsyn-0.0.4/PKG-INFO` & `mdetsyn-0.0.4.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdetsyn
-Version: 0.0.4
+Version: 0.0.4.post1
 Summary: Data Synthesis pipeline to generate object detection data
 Author: PD-Mera
 Author-email: phuongdong1772000@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python
 Requires-Dist: pillow
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: mdetsyn Version: 0.0.4 Summary: Data Synthesis
-pipeline to generate object detection data Author: PD-Mera Author-email:
-phuongdong1772000@gmail.com Description-Content-Type: text/markdown Requires-
-Dist: opencv-python Requires-Dist: pillow # Object Detection Data Synthesis
-Data Synthesis pipeline to generate object detection data _[_A_l_t_ _t_e_x_t_]## How to
-run ### Run with pip ``` bash pip install mdetsyn ``` And run in python file
-``` python from mdetsyn import run_synthesis, create_args args = create_args()
-run_synthesis(args) ``` ### Run with command line ``` bash python synthesis.py
---backgrounds ./backgrounds \ --objects ./objects \ --savename ./synthesis \ --
-number 1000 \ --class_mapping ./class_mapping.json \ --class_txt ./classes.txt
-``` ## Sample - Backgrounds folder contain background images (in any folmat)
-``` âââ backgrounds/ âââ background-0.jpg âââ background-
-1.jpg âââ ... ``` - Objects folder contain object images in subfolders
-(the best is `.png` format with `A` channel but any format is still runnable)
-``` âââ objects/ âââ class_1/ â âââ image-0.png â
-âââ image-1.png â âââ ... âââ class_2/ âââ ... ``` -
-Each image in objects folder will be synthesis by `n` times with `n` is user
-input - Output is a synthesis folder contain `images` and `labels` dir same as
-YOLO format - Sample visualization: | Background | Object | Synthesis | | :---:
-| :---: | :---: | | ![](./sample/backgrounds/background-0.jpg) | ![](./sample/
-objects/vanamo/vanamo-0.png) | ![](./sample/synthesis/images/4b09b7ae-3290-
-45d7-afef-82a7c5cef26d.jpg) | ## Support synthesis methods - Random Resize -
-Random Rotate - Random Transparency - Random Perspective Transform - Seamless
+Metadata-Version: 2.1 Name: mdetsyn Version: 0.0.4.post1 Summary: Data
+Synthesis pipeline to generate object detection data Author: PD-Mera Author-
+email: phuongdong1772000@gmail.com Description-Content-Type: text/markdown
+Requires-Dist: opencv-python Requires-Dist: pillow # Object Detection Data
+Synthesis Data Synthesis pipeline to generate object detection data _[_A_l_t
+_t_e_x_t_]## How to run ### Run with pip ``` bash pip install mdetsyn ``` And run in
+python file ``` python from mdetsyn import run_synthesis, create_args args =
+create_args() run_synthesis(args) ``` ### Run with command line ``` bash python
+synthesis.py --backgrounds ./backgrounds \ --objects ./objects \ --savename ./
+synthesis \ --number 1000 \ --class_mapping ./class_mapping.json \ --class_txt
+./classes.txt ``` ## Sample - Backgrounds folder contain background images (in
+any folmat) ``` âââ backgrounds/ âââ background-0.jpg âââ
+background-1.jpg âââ ... ``` - Objects folder contain object images in
+subfolders (the best is `.png` format with `A` channel but any format is still
+runnable) ``` âââ objects/ âââ class_1/ â âââ image-0.png
+â âââ image-1.png â âââ ... âââ class_2/ âââ ...
+``` - Each image in objects folder will be synthesis by `n` times with `n` is
+user input - Output is a synthesis folder contain `images` and `labels` dir
+same as YOLO format - Sample visualization: | Background | Object | Synthesis |
+| :---: | :---: | :---: | | ![](./sample/backgrounds/background-0.jpg) | ![](./
+sample/objects/vanamo/vanamo-0.png) | ![](./sample/synthesis/images/4b09b7ae-
+3290-45d7-afef-82a7c5cef26d.jpg) | ## Support synthesis methods - Random Resize
+- Random Rotate - Random Transparency - Random Perspective Transform - Seamless
 Clone - Grayscale ## Error and TODO - [ ] Sometimes seamless clone does not
 work - [x] Input parameter for each augment - [ ] Add default arguments to
 argparse help
```

### Comparing `mdetsyn-0.0.4/README.md` & `mdetsyn-0.0.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `mdetsyn-0.0.4/mdetsyn/detsyn.py` & `mdetsyn-0.0.4.post1/mdetsyn/detsyn.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,21 +63,20 @@
 
         background_w, background_h = background_image_pil.size
 
         min_object_size = int(min(background_h, background_w) * args.resize_min_ratio)
         max_object_size = int(min(background_h, background_w) * args.resize_max_ratio)
         object_image_pil = random_resize(object_image_pil, start_size = min_object_size, stop_size = max_object_size)
 
+        if random.random() < args.perspective_prob:
+            object_image_pil = random_perspective_transform(object_image_pil, transform_range=(args.perspective_min_value, args.perspective_max_value))
         if random.random() < args.rotate_prob:
             object_image_pil = random_rotate(object_image_pil, degree = (-args.rotate_max_degree, args.rotate_max_degree))
         if random.random() < args.transparency_prob:
             object_image_pil = random_reduce_transparency(object_image_pil, rate=(args.transparency_min_ratio, args.transparency_max_ratio))
-        if random.random() < args.perspective_prob:
-            object_image_pil = random_perspective_transform(object_image_pil, transform_range=(args.perspective_min_value, args.perspective_max_value))
-        
         object_w, object_h = object_image_pil.size
 
         for _ in range(args.max_overlap_retry):
             x_start = random.randrange(0, background_w - object_w)
             y_start = random.randrange(0, background_h - object_h)
 
             current_bbox = {"label": class_name,
```

### Comparing `mdetsyn-0.0.4/mdetsyn/helpers.py` & `mdetsyn-0.0.4.post1/mdetsyn/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,19 +49,16 @@
     image_cv2 = to_cv2(image)
 
     h, w, c = image_cv2.shape
     long_edge = max(h, w)
     min_size = random.randrange(start_size, stop_size)
     new_h = int(h / long_edge * min_size)
     new_w = int(w / long_edge * min_size)
-
     resized_image = cv2.resize(image_cv2, (new_w, new_h))
-
     resized_image = to_pil(resized_image)
-
     return resized_image
 
 def random_reduce_transparency(image, rate = (0.5, 1.0)):
     image_cv2 = to_cv2(image)
 
     rate_ = random.uniform(rate[0], rate[1])
 
@@ -105,15 +102,19 @@
                        [0, h], [w, h]])
     
     pts2 = np.float32([[new_x1, new_y1], [new_x2, new_y2],
                        [new_x3, new_y3], [new_x4, new_y4]])
     
     matrix = cv2.getPerspectiveTransform(pts1, pts2)
     warped_image = cv2.warpPerspective(image, matrix, (w, h))
-
+    new_x_min = min(new_x1, new_x2, new_x3, new_x4)
+    new_x_max = max(new_x1, new_x2, new_x3, new_x4)
+    new_y_min = min(new_y1, new_y2, new_y3, new_y4)
+    new_y_max = max(new_y1, new_y2, new_y3, new_y4)
+    warped_image = warped_image[new_y_min:new_y_max, new_x_min:new_x_max, :]
     warped_image = to_pil(warped_image)
     return warped_image
 
 def seamless_clone(background, content, x_center, y_center):
     background_cv2 = to_cv2(background)
     content_cv2 = to_cv2(content)
     content = content_cv2[:, :, 0:3]
```

### Comparing `mdetsyn-0.0.4/mdetsyn.egg-info/PKG-INFO` & `mdetsyn-0.0.4.post1/mdetsyn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdetsyn
-Version: 0.0.4
+Version: 0.0.4.post1
 Summary: Data Synthesis pipeline to generate object detection data
 Author: PD-Mera
 Author-email: phuongdong1772000@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python
 Requires-Dist: pillow
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: mdetsyn Version: 0.0.4 Summary: Data Synthesis
-pipeline to generate object detection data Author: PD-Mera Author-email:
-phuongdong1772000@gmail.com Description-Content-Type: text/markdown Requires-
-Dist: opencv-python Requires-Dist: pillow # Object Detection Data Synthesis
-Data Synthesis pipeline to generate object detection data _[_A_l_t_ _t_e_x_t_]## How to
-run ### Run with pip ``` bash pip install mdetsyn ``` And run in python file
-``` python from mdetsyn import run_synthesis, create_args args = create_args()
-run_synthesis(args) ``` ### Run with command line ``` bash python synthesis.py
---backgrounds ./backgrounds \ --objects ./objects \ --savename ./synthesis \ --
-number 1000 \ --class_mapping ./class_mapping.json \ --class_txt ./classes.txt
-``` ## Sample - Backgrounds folder contain background images (in any folmat)
-``` âââ backgrounds/ âââ background-0.jpg âââ background-
-1.jpg âââ ... ``` - Objects folder contain object images in subfolders
-(the best is `.png` format with `A` channel but any format is still runnable)
-``` âââ objects/ âââ class_1/ â âââ image-0.png â
-âââ image-1.png â âââ ... âââ class_2/ âââ ... ``` -
-Each image in objects folder will be synthesis by `n` times with `n` is user
-input - Output is a synthesis folder contain `images` and `labels` dir same as
-YOLO format - Sample visualization: | Background | Object | Synthesis | | :---:
-| :---: | :---: | | ![](./sample/backgrounds/background-0.jpg) | ![](./sample/
-objects/vanamo/vanamo-0.png) | ![](./sample/synthesis/images/4b09b7ae-3290-
-45d7-afef-82a7c5cef26d.jpg) | ## Support synthesis methods - Random Resize -
-Random Rotate - Random Transparency - Random Perspective Transform - Seamless
+Metadata-Version: 2.1 Name: mdetsyn Version: 0.0.4.post1 Summary: Data
+Synthesis pipeline to generate object detection data Author: PD-Mera Author-
+email: phuongdong1772000@gmail.com Description-Content-Type: text/markdown
+Requires-Dist: opencv-python Requires-Dist: pillow # Object Detection Data
+Synthesis Data Synthesis pipeline to generate object detection data _[_A_l_t
+_t_e_x_t_]## How to run ### Run with pip ``` bash pip install mdetsyn ``` And run in
+python file ``` python from mdetsyn import run_synthesis, create_args args =
+create_args() run_synthesis(args) ``` ### Run with command line ``` bash python
+synthesis.py --backgrounds ./backgrounds \ --objects ./objects \ --savename ./
+synthesis \ --number 1000 \ --class_mapping ./class_mapping.json \ --class_txt
+./classes.txt ``` ## Sample - Backgrounds folder contain background images (in
+any folmat) ``` âââ backgrounds/ âââ background-0.jpg âââ
+background-1.jpg âââ ... ``` - Objects folder contain object images in
+subfolders (the best is `.png` format with `A` channel but any format is still
+runnable) ``` âââ objects/ âââ class_1/ â âââ image-0.png
+â âââ image-1.png â âââ ... âââ class_2/ âââ ...
+``` - Each image in objects folder will be synthesis by `n` times with `n` is
+user input - Output is a synthesis folder contain `images` and `labels` dir
+same as YOLO format - Sample visualization: | Background | Object | Synthesis |
+| :---: | :---: | :---: | | ![](./sample/backgrounds/background-0.jpg) | ![](./
+sample/objects/vanamo/vanamo-0.png) | ![](./sample/synthesis/images/4b09b7ae-
+3290-45d7-afef-82a7c5cef26d.jpg) | ## Support synthesis methods - Random Resize
+- Random Rotate - Random Transparency - Random Perspective Transform - Seamless
 Clone - Grayscale ## Error and TODO - [ ] Sometimes seamless clone does not
 work - [x] Input parameter for each augment - [ ] Add default arguments to
 argparse help
```

### Comparing `mdetsyn-0.0.4/setup.py` & `mdetsyn-0.0.4.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def get_requirements_txt(requirements_path):
     with open(requirements_path, 'r') as file:
         requirements = [line.rstrip('\n') for line in file.readlines()]
     return requirements
 
 setup( 
     name='mdetsyn', 
-    version='0.0.4', 
+    version='0.0.4.post1', 
     description='Data Synthesis pipeline to generate object detection data', 
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     author='PD-Mera', 
     author_email='phuongdong1772000@gmail.com', 
     packages=find_packages(), 
     data_files=["requirements.txt"],
```

