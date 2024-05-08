# Comparing `tmp/icare_nlp-0.0.3.tar.gz` & `tmp/icare_nlp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icare_nlp-0.0.3.tar", last modified: Thu May  2 05:09:39 2024, max compression
+gzip compressed data, was "icare_nlp-0.0.4.tar", last modified: Wed May  8 06:54:50 2024, max compression
```

## Comparing `icare_nlp-0.0.3.tar` & `icare_nlp-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-02 05:09:39.959745 icare_nlp-0.0.3/
--rw-r--r--   0 yi        (1000) yi        (1000)      166 2024-05-02 05:09:39.959745 icare_nlp-0.0.3/PKG-INFO
--rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-05-01 12:45:45.000000 icare_nlp-0.0.3/README.md
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-02 05:09:39.959745 icare_nlp-0.0.3/icare_nlp/
--rw-rw-r--   0 yi        (1000) yi        (1000)       49 2024-05-01 13:47:31.000000 icare_nlp-0.0.3/icare_nlp/__init__.py
--rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-04-29 11:36:21.000000 icare_nlp-0.0.3/icare_nlp/object_desc.py
--rw-rw-r--   0 yi        (1000) yi        (1000)     7319 2024-05-02 05:06:00.000000 icare_nlp-0.0.3/icare_nlp/object_qa.py
--rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-04-29 09:07:45.000000 icare_nlp-0.0.3/icare_nlp/receipt_desc.py
--rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-04-29 09:07:53.000000 icare_nlp-0.0.3/icare_nlp/receipt_qa.py
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-02 05:09:39.959745 icare_nlp-0.0.3/icare_nlp/resources/
--rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-05-02 04:39:47.000000 icare_nlp-0.0.3/icare_nlp/resources/__init__.py
--rw-rw-r--   0 yi        (1000) yi        (1000)   247000 2024-04-30 13:33:50.000000 icare_nlp-0.0.3/icare_nlp/resources/category_emb_tensor.pt
--rw-rw-r--   0 yi        (1000) yi        (1000)    15275 2024-05-02 05:01:02.000000 icare_nlp-0.0.3/icare_nlp/resources/category_tactile_description.json
--rw-rw-r--   0 yi        (1000) yi        (1000)     1491 2024-04-30 12:13:21.000000 icare_nlp-0.0.3/icare_nlp/resources/inv_yolo_obj_class_def.json
--rw-rw-r--   0 yi        (1000) yi        (1000)      261 2024-04-30 12:07:36.000000 icare_nlp-0.0.3/icare_nlp/resources/invert.py
--rw-rw-r--   0 yi        (1000) yi        (1000)    11708 2024-04-30 13:50:11.000000 icare_nlp-0.0.3/icare_nlp/resources/object_types.py
--rw-rw-r--   0 yi        (1000) yi        (1000)     3529 2024-04-30 13:33:44.000000 icare_nlp-0.0.3/icare_nlp/resources/rev_yolo_obj_class_def.json
--rw-rw-r--   0 yi        (1000) yi        (1000)     1491 2024-04-30 13:35:28.000000 icare_nlp-0.0.3/icare_nlp/resources/yolo_obj_class_def.json
--rw-rw-r--   0 yi        (1000) yi        (1000)     2999 2024-05-01 12:31:18.000000 icare_nlp-0.0.3/icare_nlp/utils.py
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-02 05:09:39.959745 icare_nlp-0.0.3/icare_nlp.egg-info/
--rw-r--r--   0 yi        (1000) yi        (1000)      166 2024-05-02 05:09:39.000000 icare_nlp-0.0.3/icare_nlp.egg-info/PKG-INFO
--rw-rw-r--   0 yi        (1000) yi        (1000)      624 2024-05-02 05:09:39.000000 icare_nlp-0.0.3/icare_nlp.egg-info/SOURCES.txt
--rw-rw-r--   0 yi        (1000) yi        (1000)        1 2024-05-02 05:09:39.000000 icare_nlp-0.0.3/icare_nlp.egg-info/dependency_links.txt
--rw-rw-r--   0 yi        (1000) yi        (1000)       10 2024-05-02 05:09:39.000000 icare_nlp-0.0.3/icare_nlp.egg-info/top_level.txt
--rw-rw-r--   0 yi        (1000) yi        (1000)       38 2024-05-02 05:09:39.959745 icare_nlp-0.0.3/setup.cfg
--rw-rw-r--   0 yi        (1000) yi        (1000)      438 2024-05-02 05:09:24.000000 icare_nlp-0.0.3/setup.py
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/
+-rw-r--r--   0 yi        (1000) yi        (1000)      166 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/PKG-INFO
+-rw-rw-r--   0 yi        (1000) yi        (1000)      327 2024-05-02 05:18:30.000000 icare_nlp-0.0.4/README.md
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/icare_nlp/
+-rw-rw-r--   0 yi        (1000) yi        (1000)       49 2024-05-01 13:47:31.000000 icare_nlp-0.0.4/icare_nlp/__init__.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)     2803 2024-05-06 06:31:01.000000 icare_nlp-0.0.4/icare_nlp/object_desc.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)     7433 2024-05-06 06:49:59.000000 icare_nlp-0.0.4/icare_nlp/object_qa.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)      650 2024-05-08 06:52:37.000000 icare_nlp-0.0.4/icare_nlp/receipt_desc.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)      459 2024-05-08 06:52:37.000000 icare_nlp-0.0.4/icare_nlp/receipt_qa.py
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/icare_nlp/resources/
+-rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-05-02 04:39:47.000000 icare_nlp-0.0.4/icare_nlp/resources/__init__.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)   247000 2024-04-30 13:33:50.000000 icare_nlp-0.0.4/icare_nlp/resources/category_emb_tensor.pt
+-rw-rw-r--   0 yi        (1000) yi        (1000)    15275 2024-05-02 05:01:02.000000 icare_nlp-0.0.4/icare_nlp/resources/category_tactile_description.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)     6623 2024-05-06 04:31:11.000000 icare_nlp-0.0.4/icare_nlp/resources/desc_words.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)     1491 2024-04-30 12:13:21.000000 icare_nlp-0.0.4/icare_nlp/resources/inv_yolo_obj_class_def.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)      261 2024-04-30 12:07:36.000000 icare_nlp-0.0.4/icare_nlp/resources/invert.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)    11708 2024-04-30 13:50:11.000000 icare_nlp-0.0.4/icare_nlp/resources/object_types.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)     3529 2024-04-30 13:33:44.000000 icare_nlp-0.0.4/icare_nlp/resources/rev_yolo_obj_class_def.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)     1491 2024-04-30 13:35:28.000000 icare_nlp-0.0.4/icare_nlp/resources/yolo_obj_class_def.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)     2999 2024-05-06 06:31:39.000000 icare_nlp-0.0.4/icare_nlp/utils.py
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/icare_nlp.egg-info/
+-rw-r--r--   0 yi        (1000) yi        (1000)      166 2024-05-08 06:54:50.000000 icare_nlp-0.0.4/icare_nlp.egg-info/PKG-INFO
+-rw-rw-r--   0 yi        (1000) yi        (1000)      660 2024-05-08 06:54:50.000000 icare_nlp-0.0.4/icare_nlp.egg-info/SOURCES.txt
+-rw-rw-r--   0 yi        (1000) yi        (1000)        1 2024-05-08 06:54:50.000000 icare_nlp-0.0.4/icare_nlp.egg-info/dependency_links.txt
+-rw-rw-r--   0 yi        (1000) yi        (1000)       10 2024-05-08 06:54:50.000000 icare_nlp-0.0.4/icare_nlp.egg-info/top_level.txt
+-rw-rw-r--   0 yi        (1000) yi        (1000)       38 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/setup.cfg
+-rw-rw-r--   0 yi        (1000) yi        (1000)      438 2024-05-08 06:53:03.000000 icare_nlp-0.0.4/setup.py
```

### Comparing `icare_nlp-0.0.3/icare_nlp/object_qa.py` & `icare_nlp-0.0.4/icare_nlp/object_qa.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         self.target_obj=''
         # with open("resources/category_tactile_description.json", "r", encoding="utf-8") as f:
         #     self.cate_tac_desc = json.load(f)
         with resources.open_text("icare_nlp.resources", "category_tactile_description.json", encoding="utf-8") as f:
             self.cate_tac_desc = json.load(f)
         with resources.path("icare_nlp.resources", "category_emb_tensor.pt") as path:
             self.category_emb_tensor = torch.load(str(path))
+        self.device=torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
     def classify_query(self, question):
         input_embedding = self.cls_model.encode(question, convert_to_tensor=True)
         similarities1 = util.pytorch_cos_sim(input_embedding, self.embeddings1)
         similarities2 = util.pytorch_cos_sim(input_embedding, self.embeddings2)
         max_similarity1 = torch.max(similarities1)
         max_similarity2 = torch.max(similarities2)
         return 1 if max_similarity1 > max_similarity2 else 2
@@ -73,15 +75,15 @@
         selected_embs = self.category_emb_tensor[obj_index_list]
         short, centric_hand = self.get_short_expression(question)
         short_emb = self.cls_model.encode(short, convert_to_tensor=True)
         if short in self.rev_yolo_cls:
             tmp=self.rev_yolo_cls[short]
             self.target_obj=self.yolo_cls[str(tmp)]
         else:
-            similarities = util.pytorch_cos_sim(short_emb, selected_embs)
+            similarities = util.pytorch_cos_sim(short_emb.to(self.device), selected_embs.to(self.device))
             most_similar_idx = torch.argmax(similarities).item()
             self.target_obj=self.yolo_cls[str(obj_index_list[most_similar_idx])]
 
         for obj in obj_detect:
             if obj["text"] == self.target_obj:
                 target_pos = obj["position"]
                 break
```

### Comparing `icare_nlp-0.0.3/icare_nlp/resources/category_emb_tensor.pt` & `icare_nlp-0.0.4/icare_nlp/resources/category_emb_tensor.pt`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.3/icare_nlp/resources/category_tactile_description.json` & `icare_nlp-0.0.4/icare_nlp/resources/category_tactile_description.json`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.3/icare_nlp/resources/inv_yolo_obj_class_def.json` & `icare_nlp-0.0.4/icare_nlp/resources/inv_yolo_obj_class_def.json`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.3/icare_nlp/resources/object_types.py` & `icare_nlp-0.0.4/icare_nlp/resources/object_types.py`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.3/icare_nlp/resources/rev_yolo_obj_class_def.json` & `icare_nlp-0.0.4/icare_nlp/resources/rev_yolo_obj_class_def.json`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.3/icare_nlp/resources/yolo_obj_class_def.json` & `icare_nlp-0.0.4/icare_nlp/resources/yolo_obj_class_def.json`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.3/icare_nlp/utils.py` & `icare_nlp-0.0.4/icare_nlp/utils.py`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.3/icare_nlp.egg-info/SOURCES.txt` & `icare_nlp-0.0.4/icare_nlp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 icare_nlp.egg-info/PKG-INFO
 icare_nlp.egg-info/SOURCES.txt
 icare_nlp.egg-info/dependency_links.txt
 icare_nlp.egg-info/top_level.txt
 icare_nlp/resources/__init__.py
 icare_nlp/resources/category_emb_tensor.pt
 icare_nlp/resources/category_tactile_description.json
+icare_nlp/resources/desc_words.json
 icare_nlp/resources/inv_yolo_obj_class_def.json
 icare_nlp/resources/invert.py
 icare_nlp/resources/object_types.py
 icare_nlp/resources/rev_yolo_obj_class_def.json
 icare_nlp/resources/yolo_obj_class_def.json
```

