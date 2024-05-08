# Comparing `tmp/cellmirage-0.1.1.tar.gz` & `tmp/cellmirage-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmirage-0.1.1.tar", max compression
+gzip compressed data, was "cellmirage-0.1.2.tar", max compression
```

## Comparing `cellmirage-0.1.1.tar` & `cellmirage-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1291 2024-01-24 22:34:12.519785 cellmirage-0.1.1/README.md
--rwxr-xr-x   0        0        0       88 2024-01-24 22:29:15.953247 cellmirage-0.1.1/mirage/__init__.py
--rwxr-xr-x   0        0        0        0 2024-01-24 22:29:15.953378 cellmirage-0.1.1/mirage/data/sample0.png
--rwxr-xr-x   0        0        0   518716 2024-01-24 22:29:15.957430 cellmirage-0.1.1/mirage/data/sample1.tiff
--rwxr-xr-x   0        0        0  2009660 2024-01-24 22:29:15.970877 cellmirage-0.1.1/mirage/data/sample2_image.tiff
--rwxr-xr-x   0        0        0  2009660 2024-01-24 22:29:15.978218 cellmirage-0.1.1/mirage/data/sample2_reference.tiff
--rwxr-xr-x   0        0        0      258 2024-01-24 22:29:15.979679 cellmirage-0.1.1/mirage/exceptions.py
--rwxr-xr-x   0        0        0       81 2024-01-24 22:29:15.979828 cellmirage-0.1.1/mirage/pl/__init__.py
--rwxr-xr-x   0        0        0     1000 2024-01-24 22:29:15.979919 cellmirage-0.1.1/mirage/pl/plot_before_after.py
--rwxr-xr-x   0        0        0     1061 2024-01-24 22:29:15.980034 cellmirage-0.1.1/mirage/pl/plot_ssim.py
--rwxr-xr-x   0        0        0      506 2024-01-24 22:29:15.980112 cellmirage-0.1.1/mirage/pl/utils.py
--rwxr-xr-x   0        0        0     1954 2024-01-24 22:29:15.980233 cellmirage-0.1.1/mirage/tests/test_model.py
--rwxr-xr-x   0        0        0     5087 2024-01-24 22:29:15.980328 cellmirage-0.1.1/mirage/tests/utils.py
--rwxr-xr-x   0        0        0    24461 2024-01-24 22:29:15.980551 cellmirage-0.1.1/mirage/tl/MIRAGE.py
--rwxr-xr-x   0        0        0       80 2024-01-24 22:29:15.980632 cellmirage-0.1.1/mirage/tl/__init__.py
--rwxr-xr-x   0        0        0     1354 2024-01-24 22:29:15.980716 cellmirage-0.1.1/mirage/tl/get_data.py
--rwxr-xr-x   0        0        0     1441 2024-01-24 22:29:15.980789 cellmirage-0.1.1/mirage/tl/mesh.py
--rwxr-xr-x   0        0        0      587 2024-01-24 23:10:09.857278 cellmirage-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 cellmirage-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1291 2024-01-24 22:34:12.519785 cellmirage-0.1.2/README.md
+-rwxr-xr-x   0        0        0       88 2024-01-24 22:29:15.953247 cellmirage-0.1.2/mirage/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-01-24 22:29:15.953378 cellmirage-0.1.2/mirage/data/sample0.png
+-rwxr-xr-x   0        0        0   518716 2024-01-24 22:29:15.957430 cellmirage-0.1.2/mirage/data/sample1.tiff
+-rwxr-xr-x   0        0        0  2009660 2024-01-24 22:29:15.970877 cellmirage-0.1.2/mirage/data/sample2_image.tiff
+-rwxr-xr-x   0        0        0  2009660 2024-01-24 22:29:15.978218 cellmirage-0.1.2/mirage/data/sample2_reference.tiff
+-rwxr-xr-x   0        0        0      258 2024-01-24 22:29:15.979679 cellmirage-0.1.2/mirage/exceptions.py
+-rwxr-xr-x   0        0        0       81 2024-01-24 22:29:15.979828 cellmirage-0.1.2/mirage/pl/__init__.py
+-rwxr-xr-x   0        0        0     1000 2024-01-24 22:29:15.979919 cellmirage-0.1.2/mirage/pl/plot_before_after.py
+-rwxr-xr-x   0        0        0     1061 2024-01-24 22:29:15.980034 cellmirage-0.1.2/mirage/pl/plot_ssim.py
+-rwxr-xr-x   0        0        0      506 2024-01-24 22:29:15.980112 cellmirage-0.1.2/mirage/pl/utils.py
+-rwxr-xr-x   0        0        0     1954 2024-01-24 22:29:15.980233 cellmirage-0.1.2/mirage/tests/test_model.py
+-rwxr-xr-x   0        0        0     5087 2024-01-24 22:29:15.980328 cellmirage-0.1.2/mirage/tests/utils.py
+-rwxr-xr-x   0        0        0    24568 2024-05-08 15:38:07.840838 cellmirage-0.1.2/mirage/tl/MIRAGE.py
+-rwxr-xr-x   0        0        0       80 2024-01-24 22:29:15.980632 cellmirage-0.1.2/mirage/tl/__init__.py
+-rwxr-xr-x   0        0        0     1354 2024-01-24 22:29:15.980716 cellmirage-0.1.2/mirage/tl/get_data.py
+-rwxr-xr-x   0        0        0     1441 2024-01-24 22:29:15.980789 cellmirage-0.1.2/mirage/tl/mesh.py
+-rwxr-xr-x   0        0        0      614 2024-05-08 15:40:13.252521 cellmirage-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2178 1970-01-01 00:00:00.000000 cellmirage-0.1.2/PKG-INFO
```

### Comparing `cellmirage-0.1.1/README.md` & `cellmirage-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cellmirage-0.1.1/mirage/data/sample1.tiff` & `cellmirage-0.1.2/mirage/data/sample1.tiff`

 * *Files identical despite different names*

### Comparing `cellmirage-0.1.1/mirage/data/sample2_image.tiff` & `cellmirage-0.1.2/mirage/data/sample2_image.tiff`

 * *Files identical despite different names*

### Comparing `cellmirage-0.1.1/mirage/data/sample2_reference.tiff` & `cellmirage-0.1.2/mirage/data/sample2_reference.tiff`

 * *Files identical despite different names*

### Comparing `cellmirage-0.1.1/mirage/pl/plot_before_after.py` & `cellmirage-0.1.2/mirage/pl/plot_before_after.py`

 * *Files identical despite different names*

### Comparing `cellmirage-0.1.1/mirage/pl/plot_ssim.py` & `cellmirage-0.1.2/mirage/pl/plot_ssim.py`

 * *Files identical despite different names*

### Comparing `cellmirage-0.1.1/mirage/tests/test_model.py` & `cellmirage-0.1.2/mirage/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `cellmirage-0.1.1/mirage/tests/utils.py` & `cellmirage-0.1.2/mirage/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cellmirage-0.1.1/mirage/tl/MIRAGE.py` & `cellmirage-0.1.2/mirage/tl/MIRAGE.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
             f"Images must be 2D or a list of 2D images. Got dimension {references.ndim}."
         assert np.all(references >= 0) and np.all(references <= 1), \
             f"Image values must be between 0 and 1. Got min: {np.min(references)} " \
             f"and max: {np.max(references)}. Transform images to 0-1 using for example: `<img> / 255`"
         assert (bin_mask is None) or (bin_mask.shape == references.shape), \
             f"Mask must be same shape as images. Got {bin_mask.shape} (mask) and " \
             f"{references.shape} (images)."
-        # TODO: CPU cannot support edges of meshes in function gather_nd()
+        # TODO: CPU cannot support edges of meshes in function gather_nd() --> Only sample from "valid" region
         assert tf.config.list_physical_devices("GPU"), \
             f"GPU must be available. Got {tf.config.list_physical_devices('GPU')}." 
         if loss not in ["SSIM"]:
             warnings.warn(f"Loss function {loss} is not test. Recommended to use `SSIM` instead.")
 
         # Initialize
         self.num_layers = num_layers
@@ -301,15 +301,17 @@
         y: Image 2
         """
         square_shape = tf.math.sqrt(tf.cast(x.shape[0], tf.float64))
 
         x = tf.reshape(x, [square_shape, square_shape])
         y = tf.reshape(y, [square_shape, square_shape])
 
-        return tf.reduce_mean(tf.image.ssim(x, y))
+        out = tf.reduce_mean(tf.image.ssim(x, y))
+        out = tf.where(tf.math.is_nan(out), 0., out)
+        return out
 
     @tf.function
     def multi_ssim(self, align_glimpses, ref_glimpses):
         """Deprecated"""
         warnings.warn(f"Deprecated. Use loss `SSIM` instead.", DeprecationWarning)
         align_glimpses = tf.reshape(
             tf.transpose(align_glimpses, [0, 3, 1, 2]),
```

### Comparing `cellmirage-0.1.1/mirage/tl/get_data.py` & `cellmirage-0.1.2/mirage/tl/get_data.py`

 * *Files identical despite different names*

### Comparing `cellmirage-0.1.1/mirage/tl/mesh.py` & `cellmirage-0.1.2/mirage/tl/mesh.py`

 * *Files identical despite different names*

### Comparing `cellmirage-0.1.1/pyproject.toml` & `cellmirage-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "cellmirage"
-version = "0.1.1"
+version = "0.1.2"
 description = "Efficient and scalable image registration (alignment) for multiplexed imaging data"
 authors = ["Doron Haviv <havivd@mskcc.org>"]
 maintainers = ["Tobias Krause <tobiaspk1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "mirage" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.12"
 numpy = "^1.26.3"
 opencv-python = "^4.9.0.80"
 scikit-image = "^0.22.0"
 tensorflow = "^2.8.4"
 tqdm = "^4.66.1"
 urllib3 = "1.26.6"
+matplotlib = "^3.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cellmirage-0.1.1/PKG-INFO` & `cellmirage-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cellmirage
-Version: 0.1.1
+Version: 0.1.2
 Summary: Efficient and scalable image registration (alignment) for multiplexed imaging data
 License: MIT
 Author: Doron Haviv
 Author-email: havivd@mskcc.org
 Maintainer: Tobias Krause
 Maintainer-email: tobiaspk1@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: matplotlib (>=3.6,<4.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: scikit-image (>=0.22.0,<0.23.0)
 Requires-Dist: tensorflow (>=2.8.4,<3.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: urllib3 (==1.26.6)
 Description-Content-Type: text/markdown
```

