# Comparing `tmp/wormimtools-0.3.2.tar.gz` & `tmp/wormimtools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wormimtools-0.3.2.tar", last modified: Sun Mar  3 01:13:44 2024, max compression
+gzip compressed data, was "wormimtools-1.0.0.tar", last modified: Tue May  7 22:16:45 2024, max compression
```

## Comparing `wormimtools-0.3.2.tar` & `wormimtools-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:13:44.944470 wormimtools-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-03 01:13:33.000000 wormimtools-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-03-03 01:13:44.944470 wormimtools-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-03-03 01:13:33.000000 wormimtools-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 01:13:44.944470 wormimtools-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-03 01:13:33.000000 wormimtools-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:13:44.944470 wormimtools-0.3.2/wormimtools/
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-03-03 01:13:33.000000 wormimtools-0.3.2/wormimtools/Processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-03-03 01:13:33.000000 wormimtools-0.3.2/wormimtools/Reg_NeuralNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-03 01:13:33.000000 wormimtools-0.3.2/wormimtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-03 01:13:33.000000 wormimtools-0.3.2/wormimtools/con_auto_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:13:44.944470 wormimtools-0.3.2/wormimtools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-03 01:13:33.000000 wormimtools-0.3.2/wormimtools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-03 01:13:33.000000 wormimtools-0.3.2/wormimtools/utils/rme_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-03 01:13:33.000000 wormimtools-0.3.2/wormimtools/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:13:44.944470 wormimtools-0.3.2/wormimtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-03-03 01:13:44.000000 wormimtools-0.3.2/wormimtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-03 01:13:44.000000 wormimtools-0.3.2/wormimtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 01:13:44.000000 wormimtools-0.3.2/wormimtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-03 01:13:44.000000 wormimtools-0.3.2/wormimtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-03 01:13:44.000000 wormimtools-0.3.2/wormimtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:16:45.988557 wormimtools-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-07 22:16:33.000000 wormimtools-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-07 22:16:45.988557 wormimtools-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-07 22:16:33.000000 wormimtools-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:16:45.988557 wormimtools-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-07 22:16:33.000000 wormimtools-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:16:45.984557 wormimtools-1.0.0/wormimtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-07 22:16:33.000000 wormimtools-1.0.0/wormimtools/Processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-05-07 22:16:33.000000 wormimtools-1.0.0/wormimtools/Reg_NeuralNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-07 22:16:33.000000 wormimtools-1.0.0/wormimtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-07 22:16:33.000000 wormimtools-1.0.0/wormimtools/con_auto_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:16:45.988557 wormimtools-1.0.0/wormimtools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 22:16:33.000000 wormimtools-1.0.0/wormimtools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-07 22:16:33.000000 wormimtools-1.0.0/wormimtools/utils/rme_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-07 22:16:33.000000 wormimtools-1.0.0/wormimtools/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:16:45.988557 wormimtools-1.0.0/wormimtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-07 22:16:45.000000 wormimtools-1.0.0/wormimtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 22:16:45.000000 wormimtools-1.0.0/wormimtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:16:45.000000 wormimtools-1.0.0/wormimtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 22:16:45.000000 wormimtools-1.0.0/wormimtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 22:16:45.000000 wormimtools-1.0.0/wormimtools.egg-info/top_level.txt
```

### Comparing `wormimtools-0.3.2/LICENSE` & `wormimtools-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wormimtools-0.3.2/PKG-INFO` & `wormimtools-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wormimtools
-Version: 0.3.2
+Version: 1.0.0
 Summary: A short description of my package
 Home-page: https://github.com/moore-andrew05/imtools
 Author: Andrew Moore
 Author-email: moore.andrew0598@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,21 +23,22 @@
 
 This package can be installed through pip using:  
 
 ```
 pip install wormimtools
 ```
 
-This can also be performed using pip within a conda environment if you wish to use conda to install other dependencies. 
+This should be performed using pip within a conda environment. It can also be built from source and/or modified using this repository.
 
 To upgrade the package through pip, run:  
 
 ```
 pip install --upgrade wormimtools  
 ```
+
 ## Using `worm-imtools`
 
 It is highly recommended that this is performed using a jupyter notebook.
 
 #### Processing
 
 To process a directory like the one created above, import and instantiate a `Processor` object. The channel_info should be specified as a list of tuples containing your channel names and their indexes (0-based) within the images. You can use up to 4 channels: 
@@ -82,42 +83,46 @@
 stage                           # C. elegans developmental stage 
 rating                          # Rating of quality of worm
 comments                        # Comments given at imaging
 ID                              # UUID
 ```
 It also contains the following data columns for channel i (i = 0,1,2,3):
 
-``` python 
+``` python
 channel{i}_name                 # Channel i name specified in `channel_info`
 channel{i}_arr_vals             # Normalized and interpolated array values
 channel{i}_arr_vals_ni          # Normalized array values
 channel{i}_arr_vals_raw         # Raw array values
 ```
+
 In most cases, the raw array values should be used for downstream analysis. 
 
 
 #### Barcode Plotting
 
 1.  To create barcode plots of the processed arrays, import and instantiate a `BarcodePlotter` object: 
 
 ``` python
 from wormimtools import BarcodePlotter
 
 plotter = BarcodePlotter()
 ```
 
 ##### Single Channel Plotting
+
 ``` python
 data = [["Single Channel"]]    # List of arrays generated by Processor
 
 plotter.plot_barcodes_single(data, save={"save_path"})
 ```
+
 The `save` argument is optional, defaulting to None. 
 
 ##### Dual Channel Plotting
+
 ``` python
 data = [[["Channel 0"], ["Channel 1"]]] # List of lists of len=2 with arrays for 2 channels of an image
 
 plotter.plot_barcodes_dual(data)
 ```
-The `save` argument is the same as single channel plotting. 
 
+The `save` argument is the same as single channel plotting.
```

### Comparing `wormimtools-0.3.2/README.md` & `wormimtools-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 This package can be installed through pip using:  
 
 ```
 pip install wormimtools
 ```
 
-This can also be performed using pip within a conda environment if you wish to use conda to install other dependencies. 
+This should be performed using pip within a conda environment. It can also be built from source and/or modified using this repository.
 
 To upgrade the package through pip, run:  
 
 ```
 pip install --upgrade wormimtools  
 ```
+
 ## Using `worm-imtools`
 
 It is highly recommended that this is performed using a jupyter notebook.
 
 #### Processing
 
 To process a directory like the one created above, import and instantiate a `Processor` object. The channel_info should be specified as a list of tuples containing your channel names and their indexes (0-based) within the images. You can use up to 4 channels: 
@@ -63,42 +64,46 @@
 stage                           # C. elegans developmental stage 
 rating                          # Rating of quality of worm
 comments                        # Comments given at imaging
 ID                              # UUID
 ```
 It also contains the following data columns for channel i (i = 0,1,2,3):
 
-``` python 
+``` python
 channel{i}_name                 # Channel i name specified in `channel_info`
 channel{i}_arr_vals             # Normalized and interpolated array values
 channel{i}_arr_vals_ni          # Normalized array values
 channel{i}_arr_vals_raw         # Raw array values
 ```
+
 In most cases, the raw array values should be used for downstream analysis. 
 
 
 #### Barcode Plotting
 
 1.  To create barcode plots of the processed arrays, import and instantiate a `BarcodePlotter` object: 
 
 ``` python
 from wormimtools import BarcodePlotter
 
 plotter = BarcodePlotter()
 ```
 
 ##### Single Channel Plotting
+
 ``` python
 data = [["Single Channel"]]    # List of arrays generated by Processor
 
 plotter.plot_barcodes_single(data, save={"save_path"})
 ```
+
 The `save` argument is optional, defaulting to None. 
 
 ##### Dual Channel Plotting
+
 ``` python
 data = [[["Channel 0"], ["Channel 1"]]] # List of lists of len=2 with arrays for 2 channels of an image
 
 plotter.plot_barcodes_dual(data)
 ```
-The `save` argument is the same as single channel plotting. 
 
+The `save` argument is the same as single channel plotting.
```

### Comparing `wormimtools-0.3.2/setup.py` & `wormimtools-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wormimtools',
-    version='0.3.2',
+    version='1.0.0',
     packages=find_packages(),
     install_requires=["numpy", "scipy", "matplotlib", "pandas", "scikit-image"],
     author='Andrew Moore',
     author_email='moore.andrew0598@gmail.com',
     description='A short description of my package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `wormimtools-0.3.2/wormimtools/Processing.py` & `wormimtools-1.0.0/wormimtools/Processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 import pandas as pd
 from .utils.rme_parser import rme_parser
 from .utils.utils import interp1d, normalize
 import uuid
 import re
 
 class Processor:
-    def __init__(self, path, channel_info, group_number=1, max_value=65535, final_len=3500):
+    def __init__(self, path, channel_info, group_number=1, max_value=65535, final_len=3500, _trim_edge = False):
         """
         Processes a directory containing images and a README generated by "con_auto_dir.py".
 
         :param path: Absolute path to directory containing images and README.txt (can use relative path if in same directory)
         :param channel_info: List of tuples containing channel names and index of  channels as they appear in image, max length 4 \\
         Example: [("channel_name_1", 0), ("channel_name_2", 1)]
         :param group_number: Number of group to be processed if multiple groups appear in README.txt. Not index based, first group is 1.
         :param max_value: Maximum value of pixels in images. Default is 65535. Used to normalize images, can be any value.
         :param final_len: Length of final 1D arrays. Default is 3500. Used to interpolate images, can be any value.
         """
 
         if path[-1] != "/":
             path += "/"
 
+        self.trim_edge = _trim_edge
         self.channel_info = channel_info
         self.metadata = rme_parser(path + "README.txt")
         self.header = self.metadata.header
         self.dbdata = self.metadata.infos[group_number-1]
         self._max_value = max_value
         self._final_len = final_len
         self.Raw_Arrays = self._gen_raw_arrays(path)
@@ -42,15 +43,15 @@
         """
         image_names = [i for i in os.listdir(path) if not i.startswith(".") and not i.endswith(".txt")]
         image_names = sorted(image_names, key = lambda x: int(re.findall(r'[\d]+', x)[0]))
         Raw_Images = []
 
 
         for _, name in enumerate(image_names):
-            img = io.imread(path+name)
+            img = io.imread(os.path.join(path, name))
             img_shape = img.shape
 
             min_index = np.argmin(img_shape)
 
             if len(img_shape) == 2:         # Case of image with a single channel
                 Raw_Images.append(img)
             elif min_index == 0:            # If statements to catch cases where image channel is in different dimension than expected
@@ -77,22 +78,23 @@
 
         for _, channels in enumerate(Raw_data):
             img_arrs_ni = []
             img_arrs_raw = []
             img_arrs = []
 
             for image in channels:
-                arr = image.max(axis=0)                             # Collapse 2d image into vector based on max value in each column
+                arr = np.array(image).astype(np.uint16)
+                if self.trim_edge:
+                    arr = arr[1:, 1:]
+                arr = np.max(arr, axis=0)                         # Collapse 2d image into vector based on max value in each column
                 img_arrs_raw.append(np.copy(arr))                   # Append raw arrays
-                arr = normalize(arr, self._max_value)                      # Normalize to values between 0 and 1.
-                # arr = arr / np.max(arr)               
+                arr = normalize(arr, self._max_value)               # Normalize to values between 0 and 1.          
                 img_arrs_ni.append(np.copy(arr))                    # Append uninterpolated arrays
 
-                arr_int = interp1d(arr, self._final_len)      # Interpolate the vector into uniform length.
-
+                arr_int = interp1d(arr, self._final_len)            # Interpolate the vector into uniform length.
                 img_arrs.append(np.copy(arr_int))
 
             flatdata.append(np.copy(img_arrs))
             flatdata_ni.append(np.copy(img_arrs_ni))   
             flatdata_raw.append(np.copy(img_arrs_raw))
             
         return flatdata_ni, np.asarray(flatdata), flatdata_raw
```

### Comparing `wormimtools-0.3.2/wormimtools/Reg_NeuralNet.py` & `wormimtools-1.0.0/wormimtools/Reg_NeuralNet.py`

 * *Files identical despite different names*

### Comparing `wormimtools-0.3.2/wormimtools/con_auto_dir.py` & `wormimtools-1.0.0/wormimtools/con_auto_dir.py`

 * *Files identical despite different names*

### Comparing `wormimtools-0.3.2/wormimtools/utils/rme_parser.py` & `wormimtools-1.0.0/wormimtools/utils/rme_parser.py`

 * *Files identical despite different names*

### Comparing `wormimtools-0.3.2/wormimtools/utils/utils.py` & `wormimtools-1.0.0/wormimtools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `wormimtools-0.3.2/wormimtools.egg-info/PKG-INFO` & `wormimtools-1.0.0/wormimtools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wormimtools
-Version: 0.3.2
+Version: 1.0.0
 Summary: A short description of my package
 Home-page: https://github.com/moore-andrew05/imtools
 Author: Andrew Moore
 Author-email: moore.andrew0598@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,21 +23,22 @@
 
 This package can be installed through pip using:  
 
 ```
 pip install wormimtools
 ```
 
-This can also be performed using pip within a conda environment if you wish to use conda to install other dependencies. 
+This should be performed using pip within a conda environment. It can also be built from source and/or modified using this repository.
 
 To upgrade the package through pip, run:  
 
 ```
 pip install --upgrade wormimtools  
 ```
+
 ## Using `worm-imtools`
 
 It is highly recommended that this is performed using a jupyter notebook.
 
 #### Processing
 
 To process a directory like the one created above, import and instantiate a `Processor` object. The channel_info should be specified as a list of tuples containing your channel names and their indexes (0-based) within the images. You can use up to 4 channels: 
@@ -82,42 +83,46 @@
 stage                           # C. elegans developmental stage 
 rating                          # Rating of quality of worm
 comments                        # Comments given at imaging
 ID                              # UUID
 ```
 It also contains the following data columns for channel i (i = 0,1,2,3):
 
-``` python 
+``` python
 channel{i}_name                 # Channel i name specified in `channel_info`
 channel{i}_arr_vals             # Normalized and interpolated array values
 channel{i}_arr_vals_ni          # Normalized array values
 channel{i}_arr_vals_raw         # Raw array values
 ```
+
 In most cases, the raw array values should be used for downstream analysis. 
 
 
 #### Barcode Plotting
 
 1.  To create barcode plots of the processed arrays, import and instantiate a `BarcodePlotter` object: 
 
 ``` python
 from wormimtools import BarcodePlotter
 
 plotter = BarcodePlotter()
 ```
 
 ##### Single Channel Plotting
+
 ``` python
 data = [["Single Channel"]]    # List of arrays generated by Processor
 
 plotter.plot_barcodes_single(data, save={"save_path"})
 ```
+
 The `save` argument is optional, defaulting to None. 
 
 ##### Dual Channel Plotting
+
 ``` python
 data = [[["Channel 0"], ["Channel 1"]]] # List of lists of len=2 with arrays for 2 channels of an image
 
 plotter.plot_barcodes_dual(data)
 ```
-The `save` argument is the same as single channel plotting. 
 
+The `save` argument is the same as single channel plotting.
```

