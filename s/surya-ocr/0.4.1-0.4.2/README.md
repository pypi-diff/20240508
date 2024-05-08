# Comparing `tmp/surya_ocr-0.4.1.tar.gz` & `tmp/surya_ocr-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surya_ocr-0.4.1.tar", max compression
+gzip compressed data, was "surya_ocr-0.4.2.tar", max compression
```

## Comparing `surya_ocr-0.4.1.tar` & `surya_ocr-0.4.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35085 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/LICENSE
--rw-r--r--   0        0        0    24927 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/README.md
--rw-r--r--   0        0        0     3084 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/detect_layout.py
--rw-r--r--   0        0        0     3314 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/detect_text.py
--rw-r--r--   0        0        0     6909 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/ocr_app.py
--rw-r--r--   0        0        0     4112 2024-05-08 19:02:19.476145 surya_ocr-0.4.1/ocr_text.py
--rw-r--r--   0        0        0     1326 2024-05-08 19:06:52.710150 surya_ocr-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3720 2024-05-08 19:02:19.480145 surya_ocr-0.4.1/reading_order.py
--rw-r--r--   0        0        0      530 2024-05-08 19:02:19.480145 surya_ocr-0.4.1/run_ocr_app.py
--rw-r--r--   0        0        0      827 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/benchmark/bbox.py
--rw-r--r--   0        0        0     4239 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/benchmark/metrics.py
--rw-r--r--   0        0        0     4971 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/benchmark/tesseract.py
--rw-r--r--   0        0        0      887 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/benchmark/util.py
--rw-r--r--   0        0        0     4802 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/detection.py
--rw-r--r--   0        0        0      603 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/input/langs.py
--rw-r--r--   0        0        0     2268 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/input/load.py
--rw-r--r--   0        0        0     3167 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/input/processing.py
--rw-r--r--   0        0        0     2138 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/languages.py
--rw-r--r--   0        0        0     8598 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/layout.py
--rw-r--r--   0        0        0     6139 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/detection/segformer.py
--rw-r--r--   0        0        0      159 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/config.py
--rw-r--r--   0        0        0    25734 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/decoder.py
--rw-r--r--   0        0        0     3670 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/encoder.py
--rw-r--r--   0        0        0     3902 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/encoderdecoder.py
--rw-r--r--   0        0        0     1568 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/model.py
--rw-r--r--   0        0        0     6199 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/ordering/processor.py
--rw-r--r--   0        0        0     1676 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/config.py
--rw-r--r--   0        0        0    32140 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/decoder.py
--rw-r--r--   0        0        0     2762 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/encoder.py
--rw-r--r--   0        0        0     2646 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/model.py
--rw-r--r--   0        0        0     9296 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/processor.py
--rw-r--r--   0        0        0     3588 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/model/recognition/tokenizer.py
--rw-r--r--   0        0        0     4114 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/ocr.py
--rw-r--r--   0        0        0     5667 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/ordering.py
--rw-r--r--   0        0        0     6085 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/affinity.py
--rw-r--r--   0        0        0      853 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/fonts.py
--rw-r--r--   0        0        0     7862 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/heatmap.py
--rw-r--r--   0        0        0     3313 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/math/latex.py
--rw-r--r--   0        0        0     3114 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/math/render.py
--rw-r--r--   0        0        0     4382 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/text.py
--rw-r--r--   0        0        0     1253 2024-05-08 19:02:19.620146 surya_ocr-0.4.1/surya/postprocessing/util.py
--rw-r--r--   0        0        0     3882 2024-05-08 19:02:19.624146 surya_ocr-0.4.1/surya/recognition.py
--rw-r--r--   0        0        0     4529 2024-05-08 19:02:19.624146 surya_ocr-0.4.1/surya/schema.py
--rw-r--r--   0        0        0     3615 2024-05-08 19:02:19.624146 surya_ocr-0.4.1/surya/settings.py
--rw-r--r--   0        0        0    26225 1970-01-01 00:00:00.000000 surya_ocr-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35085 2024-05-08 19:31:12.118507 surya_ocr-0.4.2/LICENSE
+-rw-r--r--   0        0        0    24927 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/README.md
+-rw-r--r--   0        0        0     3084 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/detect_layout.py
+-rw-r--r--   0        0        0     3314 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/detect_text.py
+-rw-r--r--   0        0        0     6909 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/ocr_app.py
+-rw-r--r--   0        0        0     4112 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/ocr_text.py
+-rw-r--r--   0        0        0     1326 2024-05-08 19:33:06.349772 surya_ocr-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3720 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/reading_order.py
+-rw-r--r--   0        0        0      530 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/run_ocr_app.py
+-rw-r--r--   0        0        0      827 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/benchmark/bbox.py
+-rw-r--r--   0        0        0     4239 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/benchmark/metrics.py
+-rw-r--r--   0        0        0     4971 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/benchmark/tesseract.py
+-rw-r--r--   0        0        0      887 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/benchmark/util.py
+-rw-r--r--   0        0        0     4802 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/detection.py
+-rw-r--r--   0        0        0      603 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/input/langs.py
+-rw-r--r--   0        0        0     2268 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/input/load.py
+-rw-r--r--   0        0        0     3167 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/input/processing.py
+-rw-r--r--   0        0        0     2138 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/languages.py
+-rw-r--r--   0        0        0     8598 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/layout.py
+-rw-r--r--   0        0        0     6139 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/detection/segformer.py
+-rw-r--r--   0        0        0      159 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/config.py
+-rw-r--r--   0        0        0    25734 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/decoder.py
+-rw-r--r--   0        0        0     3670 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/encoder.py
+-rw-r--r--   0        0        0     3902 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/encoderdecoder.py
+-rw-r--r--   0        0        0     1568 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/model.py
+-rw-r--r--   0        0        0     6199 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/processor.py
+-rw-r--r--   0        0        0     1676 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/config.py
+-rw-r--r--   0        0        0    32140 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/decoder.py
+-rw-r--r--   0        0        0     2762 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/encoder.py
+-rw-r--r--   0        0        0     2646 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/model.py
+-rw-r--r--   0        0        0     9296 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/processor.py
+-rw-r--r--   0        0        0     3588 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/tokenizer.py
+-rw-r--r--   0        0        0     4154 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/ocr.py
+-rw-r--r--   0        0        0     5667 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/ordering.py
+-rw-r--r--   0        0        0     6085 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/affinity.py
+-rw-r--r--   0        0        0      853 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/fonts.py
+-rw-r--r--   0        0        0     7862 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/heatmap.py
+-rw-r--r--   0        0        0     3313 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/math/latex.py
+-rw-r--r--   0        0        0     3114 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/math/render.py
+-rw-r--r--   0        0        0     4382 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/text.py
+-rw-r--r--   0        0        0     1253 2024-05-08 19:31:12.270506 surya_ocr-0.4.2/surya/postprocessing/util.py
+-rw-r--r--   0        0        0     3882 2024-05-08 19:31:12.270506 surya_ocr-0.4.2/surya/recognition.py
+-rw-r--r--   0        0        0     4529 2024-05-08 19:31:12.270506 surya_ocr-0.4.2/surya/schema.py
+-rw-r--r--   0        0        0     3615 2024-05-08 19:31:12.270506 surya_ocr-0.4.2/surya/settings.py
+-rw-r--r--   0        0        0    26225 1970-01-01 00:00:00.000000 surya_ocr-0.4.2/PKG-INFO
```

### Comparing `surya_ocr-0.4.1/LICENSE` & `surya_ocr-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/README.md` & `surya_ocr-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/detect_layout.py` & `surya_ocr-0.4.2/detect_layout.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/detect_text.py` & `surya_ocr-0.4.2/detect_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/ocr_app.py` & `surya_ocr-0.4.2/ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/ocr_text.py` & `surya_ocr-0.4.2/ocr_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/pyproject.toml` & `surya_ocr-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surya-ocr"
-version = "0.4.1"
+version = "0.4.2"
 description = "OCR, layout, reading order, and line detection in 90+ languages"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/surya"
 keywords = ["ocr", "pdf", "text detection", "text recognition"]
 packages = [
```

### Comparing `surya_ocr-0.4.1/reading_order.py` & `surya_ocr-0.4.2/reading_order.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/run_ocr_app.py` & `surya_ocr-0.4.2/run_ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/benchmark/bbox.py` & `surya_ocr-0.4.2/surya/benchmark/bbox.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/benchmark/metrics.py` & `surya_ocr-0.4.2/surya/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/benchmark/tesseract.py` & `surya_ocr-0.4.2/surya/benchmark/tesseract.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/benchmark/util.py` & `surya_ocr-0.4.2/surya/benchmark/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/detection.py` & `surya_ocr-0.4.2/surya/detection.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/input/langs.py` & `surya_ocr-0.4.2/surya/input/langs.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/input/load.py` & `surya_ocr-0.4.2/surya/input/load.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/input/processing.py` & `surya_ocr-0.4.2/surya/input/processing.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/languages.py` & `surya_ocr-0.4.2/surya/languages.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/layout.py` & `surya_ocr-0.4.2/surya/layout.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/detection/segformer.py` & `surya_ocr-0.4.2/surya/model/detection/segformer.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/ordering/decoder.py` & `surya_ocr-0.4.2/surya/model/ordering/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/ordering/encoder.py` & `surya_ocr-0.4.2/surya/model/ordering/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/ordering/encoderdecoder.py` & `surya_ocr-0.4.2/surya/model/ordering/encoderdecoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/ordering/model.py` & `surya_ocr-0.4.2/surya/model/ordering/model.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/ordering/processor.py` & `surya_ocr-0.4.2/surya/model/ordering/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/recognition/config.py` & `surya_ocr-0.4.2/surya/model/recognition/config.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/recognition/decoder.py` & `surya_ocr-0.4.2/surya/model/recognition/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/recognition/encoder.py` & `surya_ocr-0.4.2/surya/model/recognition/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/recognition/model.py` & `surya_ocr-0.4.2/surya/model/recognition/model.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/recognition/processor.py` & `surya_ocr-0.4.2/surya/model/recognition/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/model/recognition/tokenizer.py` & `surya_ocr-0.4.2/surya/model/recognition/tokenizer.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/ocr.py` & `surya_ocr-0.4.2/surya/ocr.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from surya.detection import batch_text_detection
 from surya.input.processing import slice_polys_from_image, slice_bboxes_from_image
 from surya.postprocessing.text import truncate_repetitions, sort_text_lines
 from surya.recognition import batch_recognition
 from surya.schema import TextLine, OCRResult
 
 
-def run_recognition(images: List[Image.Image], langs: List[List[str]], rec_model, rec_processor, bboxes: List[List[List[int]]] = None, polygons: List[List[List[List[int]]]] = None) -> List[OCRResult]:
+def run_recognition(images: List[Image.Image], langs: List[List[str]], rec_model, rec_processor, bboxes: List[List[List[int]]] = None, polygons: List[List[List[List[int]]]] = None, batch_size=None) -> List[OCRResult]:
     # Polygons need to be in corner format - [[x1, y1], [x2, y2], [x3, y3], [x4, y4]], bboxes in [x1, y1, x2, y2] format
     assert bboxes is not None or polygons is not None
     assert len(images) == len(langs), "You need to pass in one list of languages for each image"
     slice_map = []
     all_slices = []
     all_langs = []
     for idx, (image, lang) in enumerate(zip(images, langs)):
@@ -24,15 +24,15 @@
             slices = slice_polys_from_image(image, polygons[idx])
         else:
             slices = slice_bboxes_from_image(image, bboxes[idx])
         slice_map.append(len(slices))
         all_slices.extend(slices)
         all_langs.extend([lang] * len(slices))
 
-    rec_predictions, _ = batch_recognition(all_slices, all_langs, rec_model, rec_processor)
+    rec_predictions, _ = batch_recognition(all_slices, all_langs, rec_model, rec_processor, batch_size=batch_size)
 
     predictions_by_image = []
     slice_start = 0
     for idx, (image, lang) in enumerate(zip(images, langs)):
         slice_end = slice_start + slice_map[idx]
         image_lines = rec_predictions[slice_start:slice_end]
         slice_start = slice_end
```

### Comparing `surya_ocr-0.4.1/surya/ordering.py` & `surya_ocr-0.4.2/surya/ordering.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/postprocessing/affinity.py` & `surya_ocr-0.4.2/surya/postprocessing/affinity.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/postprocessing/fonts.py` & `surya_ocr-0.4.2/surya/postprocessing/fonts.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/postprocessing/heatmap.py` & `surya_ocr-0.4.2/surya/postprocessing/heatmap.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/postprocessing/math/latex.py` & `surya_ocr-0.4.2/surya/postprocessing/math/latex.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/postprocessing/math/render.py` & `surya_ocr-0.4.2/surya/postprocessing/math/render.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/postprocessing/text.py` & `surya_ocr-0.4.2/surya/postprocessing/text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/postprocessing/util.py` & `surya_ocr-0.4.2/surya/postprocessing/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/recognition.py` & `surya_ocr-0.4.2/surya/recognition.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/schema.py` & `surya_ocr-0.4.2/surya/schema.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/surya/settings.py` & `surya_ocr-0.4.2/surya/settings.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.1/PKG-INFO` & `surya_ocr-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surya-ocr
-Version: 0.4.1
+Version: 0.4.2
 Summary: OCR, layout, reading order, and line detection in 90+ languages
 Home-page: https://github.com/VikParuchuri/surya
 License: GPL-3.0-or-later
 Keywords: ocr,pdf,text detection,text recognition
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
```

