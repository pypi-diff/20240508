# Comparing `tmp/mdetsyn-0.0.2.tar.gz` & `tmp/mdetsyn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdetsyn-0.0.2.tar", last modified: Mon May  6 09:16:46 2024, max compression
+gzip compressed data, was "mdetsyn-0.0.3.tar", last modified: Wed May  8 08:04:26 2024, max compression
```

## Comparing `mdetsyn-0.0.2.tar` & `mdetsyn-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-06 09:16:46.278164 mdetsyn-0.0.2/
--rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)     1093 2024-05-06 09:16:46.278164 mdetsyn-0.0.2/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      824 2024-05-06 09:01:16.000000 mdetsyn-0.0.2/README.md
-drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-06 09:16:46.278164 mdetsyn-0.0.2/mdetsyn/
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       33 2024-05-06 08:46:15.000000 mdetsyn-0.0.2/mdetsyn/__init__.py
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     7301 2024-05-06 08:50:24.000000 mdetsyn-0.0.2/mdetsyn/detsyn.py
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     7494 2024-05-06 09:15:27.000000 mdetsyn-0.0.2/mdetsyn/helpers.py
-drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-06 09:16:46.278164 mdetsyn-0.0.2/mdetsyn.egg-info/
--rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)     1093 2024-05-06 09:16:46.000000 mdetsyn-0.0.2/mdetsyn.egg-info/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      246 2024-05-06 09:16:46.000000 mdetsyn-0.0.2/mdetsyn.egg-info/SOURCES.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        1 2024-05-06 09:16:46.000000 mdetsyn-0.0.2/mdetsyn.egg-info/dependency_links.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       21 2024-05-06 09:16:46.000000 mdetsyn-0.0.2/mdetsyn.egg-info/requires.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        8 2024-05-06 09:16:46.000000 mdetsyn-0.0.2/mdetsyn.egg-info/top_level.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       20 2024-05-06 07:47:54.000000 mdetsyn-0.0.2/requirements.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       38 2024-05-06 09:16:46.278164 mdetsyn-0.0.2/setup.cfg
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      696 2024-05-06 09:16:01.000000 mdetsyn-0.0.2/setup.py
+drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-08 08:04:26.741350 mdetsyn-0.0.3/
+-rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)     2263 2024-05-08 08:04:26.741350 mdetsyn-0.0.3/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     1994 2024-05-08 08:02:23.000000 mdetsyn-0.0.3/README.md
+drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-08 08:04:26.737350 mdetsyn-0.0.3/mdetsyn/
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       46 2024-05-08 08:00:50.000000 mdetsyn-0.0.3/mdetsyn/__init__.py
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     9603 2024-05-08 07:58:07.000000 mdetsyn-0.0.3/mdetsyn/detsyn.py
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     7552 2024-05-08 06:59:20.000000 mdetsyn-0.0.3/mdetsyn/helpers.py
+drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-08 08:04:26.741350 mdetsyn-0.0.3/mdetsyn.egg-info/
+-rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)     2263 2024-05-08 08:04:26.000000 mdetsyn-0.0.3/mdetsyn.egg-info/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      246 2024-05-08 08:04:26.000000 mdetsyn-0.0.3/mdetsyn.egg-info/SOURCES.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        1 2024-05-08 08:04:26.000000 mdetsyn-0.0.3/mdetsyn.egg-info/dependency_links.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       21 2024-05-08 08:04:26.000000 mdetsyn-0.0.3/mdetsyn.egg-info/requires.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        8 2024-05-08 08:04:26.000000 mdetsyn-0.0.3/mdetsyn.egg-info/top_level.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       20 2024-05-06 07:47:54.000000 mdetsyn-0.0.3/requirements.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       38 2024-05-08 08:04:26.741350 mdetsyn-0.0.3/setup.cfg
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      696 2024-05-08 08:03:58.000000 mdetsyn-0.0.3/setup.py
```

### Comparing `mdetsyn-0.0.2/mdetsyn/detsyn.py` & `mdetsyn-0.0.3/mdetsyn/detsyn.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,162 +9,184 @@
 from PIL import Image
 
 from .helpers import to_pil, adjust_background_size, \
                     random_resize, random_reduce_transparency, random_rotate, random_perspective_transform, \
                     seamless_clone, \
                     get_iob, bboxes_to_yolo_labels
 
-MAX_OVERLAP_IOB = 0.2
-MAX_OVERLAP_RETRY = 10
+def create_args():
+    parser = argparse.ArgumentParser(description='Object Detection Data Synthesis')
+    parser_base = parser.add_argument_group('Specify base arguments')
+    parser_base.add_argument('--backgrounds', default='./backgrounds', type=str, help='Path to background images directory')
+    parser_base.add_argument('--objects', default='./objects', type=str, help='Path to objects images directory')
+    parser_base.add_argument('--savename', default='./synthesis', type=str, help='Path to save synthesis images directory')
+    parser_base.add_argument('--number', default=1, type=int, help='Number of generate labels for each class')
+    parser_base.add_argument('--class_mapping', default=None, type=str, help='Path to class mapping file')
+    parser_base.add_argument('--class_txt', default=None, type=str, help='Path to classes.txt file')
+    parser_base.add_argument('--min_background_size', default=640, type=int, help='Min image size of result')
+    parser_base.add_argument('--min_object_per_image', default=1, type=int, help='Min Number of generate labels for each image')
+    parser_base.add_argument('--max_object_per_image', default=5, type=int, help='Max Number of generate labels for each image')
+
+    parser_aug = parser.add_argument_group('Specify augmentation arguments')
+    parser_aug.add_argument('--resize_min_ratio', default=0.2, type=float, help='Min object size ratio')
+    parser_aug.add_argument('--resize_max_ratio', default=0.4, type=float, help='Max object size ratio')
+
+    parser_aug.add_argument('--rotate_max_degree', default=180, type=float, help='Max rotate degree')
+    parser_aug.add_argument('--rotate_prob', default=1, type=float, help='Probability of using rotate')
+
+    parser_aug.add_argument('--transparency_min_ratio', default=0.7, type=float, help='Min transparency size ratio')
+    parser_aug.add_argument('--transparency_max_ratio', default=1.0, type=float, help='Max transparency size ratio')
+    parser_aug.add_argument('--transparency_prob', default=1, type=float, help='Probability of using transparency')
+
+    parser_aug.add_argument('--perspective_min_value', default=3, type=float, help='Min value of x (Split image to x part, lower mean more perspective)')
+    parser_aug.add_argument('--perspective_max_value', default=10, type=float, help='Max value of x (Split image to x part, higher mean less perspective)')
+    parser_aug.add_argument('--perspective_prob', default=1, type=float, help='Probability of using perspective')
+    
+    parser_aug.add_argument('--seamless_clone_prob', default=0.1, type=float, help='Probability of using seamless clone')
+    parser_aug.add_argument('--grayscale_prob', default=0.15, type=float, help='Probability of using grayscale image')
+
+    parser_other = parser.add_argument_group('Other arguments')
+    parser_other.add_argument('--max_overlap_iob', default=0.2, type=float, help='max ratio of intersaction over box')
+    parser_other.add_argument('--max_overlap_retry', default=10, type=int, help='Max creates objects retry time')
+    
+    args = parser.parse_args()
+    return args
 
-def paste_list_object_to_background(list_object_path, 
-                               background_image, 
-                               object_min_ratio = 0.2,
-                               object_max_ratio = 0.4):
+def paste_list_object_to_background(list_object_path, background_image, args):
     list_object_image = [Image.open(object_path).convert("RGBA") for object_path in list_object_path]
     
     bboxes = []
     for object_image, object_path in zip(list_object_image, list_object_path):
         class_name = object_path.split("/")[-2]
 
         object_image_pil = to_pil(object_image)
         background_image_pil = to_pil(background_image)
 
         background_w, background_h = background_image_pil.size
 
-        min_object_size = int(min(background_h, background_w) * object_min_ratio)
-        max_object_size = int(min(background_h, background_w) * object_max_ratio)
+        min_object_size = int(min(background_h, background_w) * args.resize_min_ratio)
+        max_object_size = int(min(background_h, background_w) * args.resize_max_ratio)
         object_image_pil = random_resize(object_image_pil, start_size = min_object_size, stop_size = max_object_size)
-        object_image_pil = random_rotate(object_image_pil, degree = (-20, 20))
-        object_image_pil = random_reduce_transparency(object_image_pil, rate=(0.7, 1.0))
-        object_image_pil = random_perspective_transform(object_image_pil)
+
+        if random.random() < args.rotate_prob:
+            object_image_pil = random_rotate(object_image_pil, degree = (-args.rotate_max_degree, args.rotate_max_degree))
+        if random.random() < args.transparency_prob:
+            object_image_pil = random_reduce_transparency(object_image_pil, rate=(args.transparency_min_ratio, args.transparency_max_ratio))
+        if random.random() < args.perspective_prob:
+            object_image_pil = random_perspective_transform(object_image_pil, transform_range=(args.perspective_min_value, args.perspective_max_value))
         
         object_w, object_h = object_image_pil.size
 
-        for _ in range(MAX_OVERLAP_RETRY):
+        for _ in range(args.max_overlap_retry):
             x_start = random.randrange(0, background_w - object_w)
             y_start = random.randrange(0, background_h - object_h)
 
             current_bbox = {"label": class_name, 
                             "x1": x_start, 
                             "y1": y_start, 
                             "x2": x_start + object_image_pil.size[0], 
                             "y2": y_start + object_image_pil.size[1],
                             "bg_w": background_w,
                             "bg_h": background_h,}
             iob = 0
             for bbox in bboxes:
                 iob = get_iob(current_bbox, bbox)
-                if iob > MAX_OVERLAP_IOB:
+                if iob > args.max_overlap_iob:
                     break
 
-            if iob > MAX_OVERLAP_IOB:
+            if iob > args.max_overlap_iob:
                 continue
 
             break
                 
-        if random.random() > 0.9:
+        if random.random() < args.seamless_clone_prob:
             x_center = int(x_start + object_image_pil.size[0] / 2.0)
             y_center = int(y_start + object_image_pil.size[1] / 2.0)
             background_image = seamless_clone(background_image, object_image_pil, x_center, y_center)     
         else:
             background_image.paste(object_image_pil, (x_start, y_start), object_image_pil)
+
         bboxes.append(current_bbox)
+
+        if random.random() < args.grayscale_prob:
+            background_image = background_image.convert("L").convert("RGB")
+
     return background_image, bboxes
 
 
-def run_synthesis(backgrounds_dir: str, 
-                  objects_dir: str, 
-                  synthetic_save_dir: str, 
-                  synthetic_number: int, 
-                  class_mapping_path: Union[None, str] = None, 
-                  class_txt_path: Union[None, str] = None):
+def run_synthesis(args: argparse.Namespace):
     """
-        backgrounds_dir: path to background image folder (contain background images)
-        objects_dir: path to objects image folder (contain each object images in seperate subfolder)
-        synthetic_save_dir: path to save synthetic data in YOLO format (images, labels)
-        synthetic_number: Number of each labels image to generate
-        class_mapping_path: path to json file contain class mapping
-        class_txt_path: path to txt file contain classnames
+        backgrounds: path to background image folder (contain background images)
+        objects: path to objects image folder (contain each object images in seperate subfolder)
+        savename: path to save synthetic data in YOLO format (images, labels)
+        number: Number of each labels image to generate
+        class_mapping: path to json file contain class mapping
+        class_txt: path to txt file contain classnames
     """
-    os.makedirs(synthetic_save_dir, exist_ok=True)
-    save_images_dir = os.path.join(synthetic_save_dir, "images")
-    save_labels_dir = os.path.join(synthetic_save_dir, "labels")
+    os.makedirs(args.backgrounds, exist_ok=True)
+    save_images_dir = os.path.join(args.savename, "images")
+    save_labels_dir = os.path.join(args.savename, "labels")
     os.makedirs(save_images_dir, exist_ok=True)
     os.makedirs(save_labels_dir, exist_ok=True)
     
-    list_object_path = glob.glob(f"{objects_dir}/*/*")
-    list_background_path = glob.glob(f"{backgrounds_dir}/*")
+    list_object_path = glob.glob(f"{args.objects}/*/*")
+    list_background_path = glob.glob(f"{args.backgrounds}/*")
 
-    list_object_path = list_object_path * synthetic_number
+    list_object_path = list_object_path * args.number
     random.shuffle(list_object_path)
 
-    if class_mapping_path is not None:
+    if args.class_mapping is not None:
         try:
-            with open(class_mapping_path, 'r') as f:
+            with open(args.class_mapping, 'r') as f:
                 class_mapping_dict = json.load(f)
         except:
-            with open(class_mapping_path, 'w') as f:
+            with open(args.class_mapping, 'w') as f:
                 f.write(R"{}")
                 class_mapping_dict = {}
 
     all_length = len(list_object_path)
     process_length = 0
     while len(list_object_path) > 0:
-        random_number_labels = random.randint(1, 5)
+        assert args.min_object_per_image <= args.max_object_per_image
+        random_number_labels = random.randint(args.min_object_per_image, args.max_object_per_image)
         random_number_labels = random_number_labels if random_number_labels < len(list_object_path) else len(list_object_path)
         list_process_object_path = []
         for _ in range(random_number_labels):
             list_process_object_path.append(list_object_path.pop())
             process_length += 1
 
         print(f"Processing {process_length}/{all_length}")
 
         background_path = random.choice(list_background_path)
         background_image_pil = Image.open(background_path).convert("RGB")
-        background_image_pil = adjust_background_size(background_image_pil, 640)
+        background_image_pil = adjust_background_size(background_image_pil, args.min_background_size)
 
-        background_image, bboxes = paste_list_object_to_background(list_process_object_path, background_image_pil)
+        background_image, bboxes = paste_list_object_to_background(list_process_object_path, background_image_pil, args)
 
         # print(bboxes)
         save_name = str(uuid.uuid4())
         save_image_path = os.path.join(save_images_dir, f"{save_name}.jpg")
         save_label_path = os.path.join(save_labels_dir, f"{save_name}.txt")
         save_label_str, class_mapping_dict = bboxes_to_yolo_labels(bboxes, class_mapping_dict)
 
         background_image.save(save_image_path)
         with open(save_label_path, "w") as f:
             f.write(save_label_str)
 
-    if class_mapping_path is not None:
-        with open(class_mapping_path, 'w') as f:
+    if args.class_mapping is not None:
+        with open(args.class_mapping, 'w') as f:
             json.dump(class_mapping_dict, f)
 
-    if class_txt_path is not None and class_txt_path.endswith(".txt"):
-        with open(class_txt_path, 'w') as f:
+    if args.class_txt is not None:
+        with open(args.class_txt, 'w') as f:
             swap_dict = {}
             for key in class_mapping_dict.keys():
                 swap_dict[class_mapping_dict[key]] = key
 
             for i in range(len(swap_dict.keys())):
                 f.write(swap_dict[i])
                 f.write("\n")
-
+    
 
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser(description='Object Detection Data Synthesis')
-    parser.add_argument('--backgrounds', default='./backgrounds', type=str, help='Path to background images directory')
-    parser.add_argument('--objects', default='./objects', type=str, help='Path to objects images directory')
-    parser.add_argument('--savename', default='./synthesis', type=str, help='Path to save synthesis images directory')
-    parser.add_argument('--number', default=1, type=int, help='Number of generate labels for each class')
-    parser.add_argument('--class_mapping', default=None, type=str, help='Path to class mapping file')
-    parser.add_argument('--class_txt', default=None, type=str, help='Path to classes.txt file')
-
-
-    args = parser.parse_args()
-
-    run_synthesis(args.backgrounds,
-                  args.objects,
-                  args.savename,
-                  args.number,
-                  args.class_mapping,
-                  args.class_txt)
+    args = create_args()
+    run_synthesis(args)
```

### Comparing `mdetsyn-0.0.2/mdetsyn/helpers.py` & `mdetsyn-0.0.3/mdetsyn/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,19 +79,19 @@
     angle = random.randint(degree[0], degree[1])
     rotated_image = image.rotate(angle, expand=True)
 
     image_pil = to_pil(rotated_image)
 
     return image_pil
 
-def random_perspective_transform(image):
+def random_perspective_transform(image, transform_range=(3, 10)):
     image = to_cv2(image)
     
     h, w, _ = image.shape
-    split_number = random.randint(3, 10)
+    split_number = random.randint(transform_range[0], transform_range[1])
 
     new_x1 = random.randint(0, int(w / split_number))
     new_y1 = random.randint(0, int(h / split_number))
 
     new_x2 = random.randint(int(w / split_number) * (split_number - 1), w)
     new_y2 = random.randint(0, int(h / split_number))
```

### Comparing `mdetsyn-0.0.2/setup.py` & `mdetsyn-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def get_requirements_txt(requirements_path):
     with open(requirements_path, 'r') as file:
         requirements = [line.rstrip('\n') for line in file.readlines()]
     return requirements
 
 setup( 
     name='mdetsyn', 
-    version='0.0.2', 
+    version='0.0.3', 
     description='Data Synthesis pipeline to generate object detection data', 
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     author='PD-Mera', 
     author_email='phuongdong1772000@gmail.com', 
     packages=find_packages(), 
     data_files=["requirements.txt"],
```

