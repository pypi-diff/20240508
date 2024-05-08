# Comparing `tmp/surya_ocr-0.4.0.tar.gz` & `tmp/surya_ocr-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surya_ocr-0.4.0.tar", max compression
+gzip compressed data, was "surya_ocr-0.4.1.tar", max compression
```

## Comparing `surya_ocr-0.4.0.tar` & `surya_ocr-0.4.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35085 2024-04-22 17:16:24.619974 surya_ocr-0.4.0/LICENSE
--rw-r--r--   0        0        0    24927 2024-04-22 17:16:24.619974 surya_ocr-0.4.0/README.md
--rw-r--r--   0        0        0     3084 2024-04-22 17:16:24.619974 surya_ocr-0.4.0/detect_layout.py
--rw-r--r--   0        0        0     3314 2024-04-22 17:16:24.619974 surya_ocr-0.4.0/detect_text.py
--rw-r--r--   0        0        0     6909 2024-04-22 17:16:24.619974 surya_ocr-0.4.0/ocr_app.py
--rw-r--r--   0        0        0     4112 2024-04-22 17:16:24.619974 surya_ocr-0.4.0/ocr_text.py
--rw-r--r--   0        0        0     1326 2024-04-22 17:18:14.529458 surya_ocr-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3720 2024-04-22 17:16:24.623974 surya_ocr-0.4.0/reading_order.py
--rw-r--r--   0        0        0      530 2024-04-22 17:16:24.623974 surya_ocr-0.4.0/run_ocr_app.py
--rw-r--r--   0        0        0      827 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/benchmark/bbox.py
--rw-r--r--   0        0        0     4239 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/benchmark/metrics.py
--rw-r--r--   0        0        0     4971 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/benchmark/tesseract.py
--rw-r--r--   0        0        0      887 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/benchmark/util.py
--rw-r--r--   0        0        0     4714 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/detection.py
--rw-r--r--   0        0        0      603 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/input/langs.py
--rw-r--r--   0        0        0     2268 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/input/load.py
--rw-r--r--   0        0        0     3167 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/input/processing.py
--rw-r--r--   0        0        0     2138 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/languages.py
--rw-r--r--   0        0        0     8558 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/layout.py
--rw-r--r--   0        0        0     6139 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/detection/segformer.py
--rw-r--r--   0        0        0      159 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/ordering/config.py
--rw-r--r--   0        0        0    25734 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/ordering/decoder.py
--rw-r--r--   0        0        0     3670 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/ordering/encoder.py
--rw-r--r--   0        0        0     3902 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/ordering/encoderdecoder.py
--rw-r--r--   0        0        0     1568 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/ordering/model.py
--rw-r--r--   0        0        0     6199 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/ordering/processor.py
--rw-r--r--   0        0        0     1676 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/recognition/config.py
--rw-r--r--   0        0        0    32140 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/recognition/decoder.py
--rw-r--r--   0        0        0     2762 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/recognition/encoder.py
--rw-r--r--   0        0        0     2646 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/recognition/model.py
--rw-r--r--   0        0        0     9296 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/recognition/processor.py
--rw-r--r--   0        0        0     3588 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/model/recognition/tokenizer.py
--rw-r--r--   0        0        0     3972 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/ocr.py
--rw-r--r--   0        0        0     5619 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/ordering.py
--rw-r--r--   0        0        0     6085 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/postprocessing/affinity.py
--rw-r--r--   0        0        0      853 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/postprocessing/fonts.py
--rw-r--r--   0        0        0     7862 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/postprocessing/heatmap.py
--rw-r--r--   0        0        0     3313 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/postprocessing/math/latex.py
--rw-r--r--   0        0        0     3114 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/postprocessing/math/render.py
--rw-r--r--   0        0        0     4382 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/postprocessing/text.py
--rw-r--r--   0        0        0     1253 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/postprocessing/util.py
--rw-r--r--   0        0        0     3833 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/recognition.py
--rw-r--r--   0        0        0     4529 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/schema.py
--rw-r--r--   0        0        0     3505 2024-04-22 17:16:24.767977 surya_ocr-0.4.0/surya/settings.py
--rw-r--r--   0        0        0    26225 1970-01-01 00:00:00.000000 surya_ocr-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35085 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/LICENSE
+-rw-r--r--   0        0        0    24927 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/README.md
+-rw-r--r--   0        0        0     3084 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/detect_layout.py
+-rw-r--r--   0        0        0     3314 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/detect_text.py
+-rw-r--r--   0        0        0     6909 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/ocr_app.py
+-rw-r--r--   0        0        0     4112 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/ocr_text.py
+-rw-r--r--   0        0        0     1326 2024-05-08 19:06:52.710150 surya_ocr-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3720 2024-05-08 19:02:19.480145 surya_ocr-0.4.1/reading_order.py
+-rw-r--r--   0        0        0      530 2024-05-08 19:02:19.480145 surya_ocr-0.4.1/run_ocr_app.py
+-rw-r--r--   0        0        0      827 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/benchmark/bbox.py
+-rw-r--r--   0        0        0     4239 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/benchmark/metrics.py
+-rw-r--r--   0        0        0     4971 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/benchmark/tesseract.py
+-rw-r--r--   0        0        0      887 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/benchmark/util.py
+-rw-r--r--   0        0        0     4802 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/detection.py
+-rw-r--r--   0        0        0      603 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/input/langs.py
+-rw-r--r--   0        0        0     2268 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/input/load.py
+-rw-r--r--   0        0        0     3167 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/input/processing.py
+-rw-r--r--   0        0        0     2138 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/languages.py
+-rw-r--r--   0        0        0     8598 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/layout.py
+-rw-r--r--   0        0        0     6139 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/detection/segformer.py
+-rw-r--r--   0        0        0      159 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/config.py
+-rw-r--r--   0        0        0    25734 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/decoder.py
+-rw-r--r--   0        0        0     3670 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/encoder.py
+-rw-r--r--   0        0        0     3902 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/encoderdecoder.py
+-rw-r--r--   0        0        0     1568 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/model.py
+-rw-r--r--   0        0        0     6199 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/processor.py
+-rw-r--r--   0        0        0     1676 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/config.py
+-rw-r--r--   0        0        0    32140 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/decoder.py
+-rw-r--r--   0        0        0     2762 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/encoder.py
+-rw-r--r--   0        0        0     2646 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/model.py
+-rw-r--r--   0        0        0     9296 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/processor.py
+-rw-r--r--   0        0        0     3588 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/tokenizer.py
+-rw-r--r--   0        0        0     4114 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/ocr.py
+-rw-r--r--   0        0        0     5667 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/ordering.py
+-rw-r--r--   0        0        0     6085 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/affinity.py
+-rw-r--r--   0        0        0      853 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/fonts.py
+-rw-r--r--   0        0        0     7862 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/heatmap.py
+-rw-r--r--   0        0        0     3313 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/math/latex.py
+-rw-r--r--   0        0        0     3114 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/math/render.py
+-rw-r--r--   0        0        0     4382 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/text.py
+-rw-r--r--   0        0        0     1253 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/util.py
+-rw-r--r--   0        0        0     3882 2024-05-08 19:02:19.624146 surya_ocr-0.4.1/surya/recognition.py
+-rw-r--r--   0        0        0     4529 2024-05-08 19:02:19.624146 surya_ocr-0.4.1/surya/schema.py
+-rw-r--r--   0        0        0     3615 2024-05-08 19:02:19.624146 surya_ocr-0.4.1/surya/settings.py
+-rw-r--r--   0        0        0    26225 1970-01-01 00:00:00.000000 surya_ocr-0.4.1/PKG-INFO
```

### Comparing `surya_ocr-0.4.0/LICENSE` & `surya_ocr-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/README.md` & `surya_ocr-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/detect_layout.py` & `surya_ocr-0.4.1/detect_layout.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/detect_text.py` & `surya_ocr-0.4.1/detect_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/ocr_app.py` & `surya_ocr-0.4.1/ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/ocr_text.py` & `surya_ocr-0.4.1/ocr_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/pyproject.toml` & `surya_ocr-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surya-ocr"
-version = "0.4.0"
+version = "0.4.1"
 description = "OCR, layout, reading order, and line detection in 90+ languages"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/surya"
 keywords = ["ocr", "pdf", "text detection", "text recognition"]
 packages = [
```

### Comparing `surya_ocr-0.4.0/reading_order.py` & `surya_ocr-0.4.1/reading_order.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/run_ocr_app.py` & `surya_ocr-0.4.1/run_ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/benchmark/bbox.py` & `surya_ocr-0.4.1/surya/benchmark/bbox.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/benchmark/metrics.py` & `surya_ocr-0.4.1/surya/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/benchmark/tesseract.py` & `surya_ocr-0.4.1/surya/benchmark/tesseract.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/benchmark/util.py` & `surya_ocr-0.4.1/surya/benchmark/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/detection.py` & `surya_ocr-0.4.1/surya/detection.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,17 +19,18 @@
     if batch_size is None:
         batch_size = 6
         if settings.TORCH_DEVICE_MODEL == "cuda":
             batch_size = 24
     return batch_size
 
 
-def batch_detection(images: List, model, processor) -> Tuple[List[List[np.ndarray]], List[Tuple[int, int]]]:
+def batch_detection(images: List, model, processor, batch_size=None) -> Tuple[List[List[np.ndarray]], List[Tuple[int, int]]]:
     assert all([isinstance(image, Image.Image) for image in images])
-    batch_size = get_batch_size()
+    if batch_size is None:
+        batch_size = get_batch_size()
     heatmap_count = model.config.num_labels
 
     images = [image.convert("RGB") for image in images]
     orig_sizes = [image.size for image in images]
     split_index = []
     split_heights = []
     image_splits = []
@@ -105,16 +106,16 @@
         heatmap=heat_img,
         affinity_map=aff_img,
         image_bbox=[0, 0, orig_sizes[0], orig_sizes[1]]
     )
     return result
 
 
-def batch_text_detection(images: List, model, processor) -> List[TextDetectionResult]:
-    preds, orig_sizes = batch_detection(images, model, processor)
+def batch_text_detection(images: List, model, processor, batch_size=None) -> List[TextDetectionResult]:
+    preds, orig_sizes = batch_detection(images, model, processor, batch_size=batch_size)
     results = []
     if len(images) == 1: # Ensures we don't parallelize with streamlit
         for i in range(len(images)):
             result = parallel_get_lines(preds[i], orig_sizes[i])
             results.append(result)
     else:
         with ProcessPoolExecutor(max_workers=settings.DETECTOR_POSTPROCESSING_CPU_WORKERS) as executor:
```

### Comparing `surya_ocr-0.4.0/surya/input/langs.py` & `surya_ocr-0.4.1/surya/input/langs.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/input/load.py` & `surya_ocr-0.4.1/surya/input/load.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/input/processing.py` & `surya_ocr-0.4.1/surya/input/processing.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/languages.py` & `surya_ocr-0.4.1/surya/languages.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/layout.py` & `surya_ocr-0.4.1/surya/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,16 +177,16 @@
         heatmaps=heatmaps,
         image_bbox=[0, 0, orig_size[0], orig_size[1]]
     )
 
     return result
 
 
-def batch_layout_detection(images: List, model, processor, detection_results: Optional[List[TextDetectionResult]] = None) -> List[LayoutResult]:
-    preds, orig_sizes = batch_detection(images, model, processor)
+def batch_layout_detection(images: List, model, processor, detection_results: Optional[List[TextDetectionResult]] = None, batch_size=None) -> List[LayoutResult]:
+    preds, orig_sizes = batch_detection(images, model, processor, batch_size=batch_size)
     id2label = model.config.id2label
 
     results = []
     if len(images) == 1: # Ensures we don't parallelize with streamlit
         for i in range(len(images)):
             result = parallel_get_regions(preds[i], orig_sizes[i], id2label, detection_results[i] if detection_results else None)
             results.append(result)
```

### Comparing `surya_ocr-0.4.0/surya/model/detection/segformer.py` & `surya_ocr-0.4.1/surya/model/detection/segformer.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/model/ordering/decoder.py` & `surya_ocr-0.4.1/surya/model/ordering/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/model/ordering/encoder.py` & `surya_ocr-0.4.1/surya/model/ordering/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/model/ordering/encoderdecoder.py` & `surya_ocr-0.4.1/surya/model/ordering/encoderdecoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/model/ordering/model.py` & `surya_ocr-0.4.1/surya/model/ordering/model.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/model/ordering/processor.py` & `surya_ocr-0.4.1/surya/model/ordering/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/model/recognition/config.py` & `surya_ocr-0.4.1/surya/model/recognition/config.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/model/recognition/decoder.py` & `surya_ocr-0.4.1/surya/model/recognition/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/model/recognition/encoder.py` & `surya_ocr-0.4.1/surya/model/recognition/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/model/recognition/model.py` & `surya_ocr-0.4.1/surya/model/recognition/model.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/model/recognition/processor.py` & `surya_ocr-0.4.1/surya/model/recognition/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/model/recognition/tokenizer.py` & `surya_ocr-0.4.1/surya/model/recognition/tokenizer.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/ocr.py` & `surya_ocr-0.4.1/surya/ocr.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from surya.recognition import batch_recognition
 from surya.schema import TextLine, OCRResult
 
 
 def run_recognition(images: List[Image.Image], langs: List[List[str]], rec_model, rec_processor, bboxes: List[List[List[int]]] = None, polygons: List[List[List[List[int]]]] = None) -> List[OCRResult]:
     # Polygons need to be in corner format - [[x1, y1], [x2, y2], [x3, y3], [x4, y4]], bboxes in [x1, y1, x2, y2] format
     assert bboxes is not None or polygons is not None
+    assert len(images) == len(langs), "You need to pass in one list of languages for each image"
     slice_map = []
     all_slices = []
     all_langs = []
     for idx, (image, lang) in enumerate(zip(images, langs)):
         if polygons is not None:
             slices = slice_polys_from_image(image, polygons[idx])
         else:
@@ -55,30 +56,30 @@
             image_bbox=[0, 0, image.size[0], image.size[1]]
         )
         predictions_by_image.append(pred)
 
     return predictions_by_image
 
 
-def run_ocr(images: List[Image.Image], langs: List[List[str]], det_model, det_processor, rec_model, rec_processor) -> List[OCRResult]:
+def run_ocr(images: List[Image.Image], langs: List[List[str]], det_model, det_processor, rec_model, rec_processor, batch_size=None) -> List[OCRResult]:
     det_predictions = batch_text_detection(images, det_model, det_processor)
-    if det_model.device == "cuda":
+    if det_model.device.type == "cuda":
         torch.cuda.empty_cache() # Empty cache from first model run
 
     slice_map = []
     all_slices = []
     all_langs = []
     for idx, (image, det_pred, lang) in enumerate(zip(images, det_predictions, langs)):
         polygons = [p.polygon for p in det_pred.bboxes]
         slices = slice_polys_from_image(image, polygons)
         slice_map.append(len(slices))
         all_slices.extend(slices)
         all_langs.extend([lang] * len(slices))
 
-    rec_predictions, confidence_scores = batch_recognition(all_slices, all_langs, rec_model, rec_processor)
+    rec_predictions, confidence_scores = batch_recognition(all_slices, all_langs, rec_model, rec_processor, batch_size=batch_size)
 
     predictions_by_image = []
     slice_start = 0
     for idx, (image, det_pred, lang) in enumerate(zip(images, det_predictions, langs)):
         slice_end = slice_start + slice_map[idx]
         image_lines = rec_predictions[slice_start:slice_end]
         line_confidences = confidence_scores[slice_start:slice_end]
```

### Comparing `surya_ocr-0.4.0/surya/ordering.py` & `surya_ocr-0.4.1/surya/ordering.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 
     for rank_value, (original_index, value) in enumerate(enumerated_and_sorted):
         rank[original_index] = rank_value
 
     return rank
 
 
-def batch_ordering(images: List, bboxes: List[List[List[float]]], model, processor) -> List[OrderResult]:
+def batch_ordering(images: List, bboxes: List[List[List[float]]], model, processor, batch_size=None) -> List[OrderResult]:
     assert all([isinstance(image, Image.Image) for image in images])
     assert len(images) == len(bboxes)
-    batch_size = get_batch_size()
+    if batch_size is None:
+        batch_size = get_batch_size()
 
     images = [image.convert("RGB") for image in images]
 
     output_order = []
     for i in tqdm(range(0, len(images), batch_size), desc="Finding reading order"):
         batch_bboxes = deepcopy(bboxes[i:i+batch_size])
         batch_images = images[i:i+batch_size]
```

### Comparing `surya_ocr-0.4.0/surya/postprocessing/affinity.py` & `surya_ocr-0.4.1/surya/postprocessing/affinity.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/postprocessing/fonts.py` & `surya_ocr-0.4.1/surya/postprocessing/fonts.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/postprocessing/heatmap.py` & `surya_ocr-0.4.1/surya/postprocessing/heatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         # make clock-wise order
         startidx = box.sum(axis=1).argmin()
         box = np.roll(box, 4-startidx, 0)
         box = np.array(box)
 
         mask = np.zeros_like(linemap).astype(np.uint8)
         cv2.fillPoly(mask, [np.int32(box)], 255)
-        mask = mask.astype(np.float16) / 255
+        mask = mask.astype(np.float32) / 255
 
         roi = np.where(mask == 1, linemap, 0)
         confidence = np.mean(roi[roi != 0])
 
         if confidence > max_confidence:
             max_confidence = confidence
```

### Comparing `surya_ocr-0.4.0/surya/postprocessing/math/latex.py` & `surya_ocr-0.4.1/surya/postprocessing/math/latex.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/postprocessing/math/render.py` & `surya_ocr-0.4.1/surya/postprocessing/math/render.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/postprocessing/text.py` & `surya_ocr-0.4.1/surya/postprocessing/text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/postprocessing/util.py` & `surya_ocr-0.4.1/surya/postprocessing/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/recognition.py` & `surya_ocr-0.4.1/surya/recognition.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,20 @@
         if settings.TORCH_DEVICE_MODEL == "mps":
             batch_size = 64 # 12GB RAM max
         if settings.TORCH_DEVICE_MODEL == "cuda":
             batch_size = 256
     return batch_size
 
 
-def batch_recognition(images: List, languages: List[List[str]], model, processor):
+def batch_recognition(images: List, languages: List[List[str]], model, processor, batch_size=None):
     assert all([isinstance(image, Image.Image) for image in images])
     assert len(images) == len(languages)
-    batch_size = get_batch_size()
+
+    if batch_size is None:
+        batch_size = get_batch_size()
 
     images = [image.convert("RGB") for image in images]
 
     output_text = []
     confidences = []
     for i in tqdm(range(0, len(images), batch_size), desc="Recognizing Text"):
         batch_langs = languages[i:i+batch_size]
```

### Comparing `surya_ocr-0.4.0/surya/schema.py` & `surya_ocr-0.4.1/surya/schema.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.0/surya/settings.py` & `surya_ocr-0.4.1/surya/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,20 +30,24 @@
             return "mps"
 
         return "cpu"
 
     @computed_field
     def TORCH_DEVICE_DETECTION(self) -> str:
         if self.TORCH_DEVICE is not None:
+            # Does not work with mps
+            if "mps" in self.TORCH_DEVICE:
+                return "cpu"
+
             return self.TORCH_DEVICE
 
-        # Does not work with mps
         if torch.cuda.is_available():
             return "cuda"
 
+        # Does not work with mps
         return "cpu"
 
     # Text detection
     DETECTOR_BATCH_SIZE: Optional[int] = None # Defaults to 2 for CPU, 32 otherwise
     DETECTOR_MODEL_CHECKPOINT: str = "vikp/surya_det2"
     DETECTOR_MATH_MODEL_CHECKPOINT: str = "vikp/surya_det_math"
     DETECTOR_BENCH_DATASET_NAME: str = "vikp/doclaynet_bench"
```

### Comparing `surya_ocr-0.4.0/PKG-INFO` & `surya_ocr-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surya-ocr
-Version: 0.4.0
+Version: 0.4.1
 Summary: OCR, layout, reading order, and line detection in 90+ languages
 Home-page: https://github.com/VikParuchuri/surya
 License: GPL-3.0-or-later
 Keywords: ocr,pdf,text detection,text recognition
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
```

