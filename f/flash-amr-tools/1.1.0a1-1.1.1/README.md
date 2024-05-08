# Comparing `tmp/flash_amr_tools-1.1.0a1.tar.gz` & `tmp/flash_amr_tools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flash_amr_tools-1.1.0a1.tar", last modified: Tue May  7 14:50:48 2024, max compression
+gzip compressed data, was "flash_amr_tools-1.1.1.tar", last modified: Wed May  8 13:17:49 2024, max compression
```

## Comparing `flash_amr_tools-1.1.0a1.tar` & `flash_amr_tools-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     1501 2024-04-30 14:06:17.000000 flash_amr_tools-1.1.0a1/LICENSE
--rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6918 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/PKG-INFO
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     4502 2024-05-07 14:44:30.000000 flash_amr_tools-1.1.0a1/README.md
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/flash_amr_tools/
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       74 2024-05-07 13:59:02.000000 flash_amr_tools-1.1.0a1/flash_amr_tools/__init__.py
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)    20018 2024-05-07 14:23:33.000000 flash_amr_tools-1.1.0a1/flash_amr_tools/amr_tools.py
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     9694 2024-05-07 14:09:54.000000 flash_amr_tools-1.1.0a1/flash_amr_tools/block_tools.py
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     8991 2024-04-30 14:06:32.000000 flash_amr_tools-1.1.0a1/flash_amr_tools/zorder.py
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/
--rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6918 2024-05-07 14:50:48.000000 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/PKG-INFO
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      363 2024-05-07 14:50:48.000000 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)        1 2024-05-07 14:50:48.000000 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       44 2024-05-07 14:50:48.000000 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/requires.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       16 2024-05-07 14:50:48.000000 flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/top_level.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      739 2024-05-07 14:29:00.000000 flash_amr_tools-1.1.0a1/pyproject.toml
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       38 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/setup.cfg
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-07 14:50:48.895331 flash_amr_tools-1.1.0a1/tests/
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     3557 2024-05-07 14:28:24.000000 flash_amr_tools-1.1.0a1/tests/test_amrtools.py
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     1501 2024-04-30 14:06:17.000000 flash_amr_tools-1.1.1/LICENSE
+-rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6916 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/PKG-INFO
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     4502 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/README.md
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/flash_amr_tools/
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       74 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/flash_amr_tools/__init__.py
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)    19965 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/flash_amr_tools/amr_tools.py
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     9694 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/flash_amr_tools/block_tools.py
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     8991 2024-04-30 14:06:32.000000 flash_amr_tools-1.1.1/flash_amr_tools/zorder.py
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/
+-rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6916 2024-05-08 13:17:49.000000 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      363 2024-05-08 13:17:49.000000 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)        1 2024-05-08 13:17:49.000000 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       44 2024-05-08 13:17:49.000000 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/requires.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       16 2024-05-08 13:17:49.000000 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/top_level.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      737 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/pyproject.toml
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       38 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/setup.cfg
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/tests/
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     3557 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/tests/test_amrtools.py
```

### Comparing `flash_amr_tools-1.1.0a1/LICENSE` & `flash_amr_tools-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flash_amr_tools-1.1.0a1/PKG-INFO` & `flash_amr_tools-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash_amr_tools
-Version: 1.1.0a1
+Version: 1.1.1
 Summary: Small tool to create uniform data cubes of FLASH datasets. Port from bitbucket.org/pierrenbg/flash-amr-tools
 Author-email: Keito Watanabe <k.wat8973@gmail.com>, Pierre Nürnberger <nuernb@ph1.uni-koeln.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Keito Watanabe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `flash_amr_tools-1.1.0a1/README.md` & `flash_amr_tools-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flash_amr_tools-1.1.0a1/flash_amr_tools/amr_tools.py` & `flash_amr_tools-1.1.1/flash_amr_tools/amr_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,17 +236,17 @@
     bmax, bmin = brefs
     bnx, bny, bnz = bns
     
     # maximum level, used to create the uniform grid
     max_lvl = bmax - bmin
     
     # computing the coordiante using the lower & upper corners divided by the smallest block size
-    bsize = bsize.min(axis=0)
-    coords = np.round((bbox[:, :, 0] - bbox[0, :, 0]) / bsize)
-    coords = coords.astype(int) * 8
+    bshape = data.shape[1:4]
+    coords = np.round((bbox[:, :, 0] - bbox[0, :, 0]) / bsize.min(axis=0))
+    coords = coords.astype(int) * bshape
     
     # shift refinement level by the maximum within the region of interest
     ref_lvl = bmax - ref_lvl
     
     cube = np.zeros((int(bnx) * 2**(max_lvl+3), int(bny) * 2**(max_lvl+3), int(bnz) * 2**(max_lvl+3)), dtype=data.dtype)
 
     for i in range(len(data)):
@@ -257,15 +257,15 @@
         data_reshape = np.repeat(data[i], diff, axis=0)
         data_reshape = np.repeat(data_reshape, diff, axis=1)
         data_reshape = np.repeat(data_reshape, diff, axis=2)
         
         sub_cube_size = int(2**(ref_lvl[i] + 3))
         cube[x:x+sub_cube_size, y:y+sub_cube_size, z:z+sub_cube_size] = data_reshape.T
         
-    return cube.T
+    return cube
 
 
 def get_reflvl_cube(ref_lvl, bbox, bsize, brefs, bns):
     '''
     Returns the refinement level as a 3-D uniform cube.
 
     - ref_lvl : refinement level for each block, filtered by the block list
@@ -278,16 +278,15 @@
     bmax, bmin = brefs
     bnx, bny, bnz = bns
     
     # maximum level, used to create the uniform grid
     max_lvl = bmax - bmin
 
     # computing the coordiante using the lower & upper corners divided by the smallest block size
-    bsize = bsize.min(axis=0)
-    coords = np.round((bbox[:, :, 0] - bbox[0, :, 0]) / bsize)
+    coords = np.round((bbox[:, :, 0] - bbox[0, :, 0]) / bsize.min(axis=0))
     coords = coords.astype(int) * 8
     
     # shift refinement level by the maximum within the region of interest
     ref_lvl = bmax - ref_lvl
 
     cube = np.zeros((int(bnx) * 2 ** (max_lvl + 3), int(bny) * 2 ** (max_lvl + 3), int(bnz) * 2 ** (max_lvl + 3)), dtype=ref_lvl.dtype)
 
@@ -299,15 +298,15 @@
         data_reshape = np.repeat(ref_lvl[i], diff, axis=0)[..., None]
         data_reshape = np.repeat(data_reshape, diff, axis=1)[..., None]
         data_reshape = np.repeat(data_reshape, diff, axis=2)
 
         sub_cube_size = int(2 ** (ref_lvl[i]+3))
         cube[x:x + sub_cube_size, y:y + sub_cube_size, z:z + sub_cube_size] = data_reshape.T
 
-    return cube.T
+    return cube
 
 
 def get_vector_cube(data_vec, ref_lvl, bbox, bsize, brefs, bns):
     '''
     Wrapper for returning vectorial data as a uniform grid, where the last axis appends the data in each direction.
 
     - data_vec (list): list of length 3, containing each data in each direction.  extracted by h5py & filtered by the block list
@@ -377,34 +376,34 @@
     # maximum level, used to create the uniform grid
     max_lvl = bmax - bmin
 
     # safety features
     assert axis in [0,1,2], f"Axis {axis} is not 0, 1, or 2 (x, y or z)."
 
     # remove axis in which projection occrurs
-    bn_ax = bns.pop(axis)
     ax = [0, 1, 2]
     ax.pop(axis)
 
-    coords = np.round((bbox[:, :, 0] - bbox[0, :, 0]) / bsize.min())
-    coords = coords.astype(int) * 8
+    bshape = data.shape[1:4]
+    coords = np.round((bbox[:, :, 0] - bbox[0, :, 0]) / bsize.min(axis=0))
+    coords = coords.astype(int) * bshape
 
     ref_lvl = bmax - ref_lvl
     sh = data.shape
 
     use_weights = False
     if weights is not None:
-        norm = np.zeros((int(bns[0]) * 2**(max_lvl+3), int(bns[1]) * 2**(max_lvl+3)), dtype=data.dtype)
+        norm = np.zeros((int(bns[ax[0]]) * 2**(max_lvl+3), int(bns[ax[1]]) * 2**(max_lvl+3)), dtype=data.dtype)
 
         # make sure shape of weights is same as data
         assert data.shape == weights.shape, "shape of weights " + weights.shape + " != shape of data " + data.shape + " ."
 
         use_weights = True
 
-    cdens = np.zeros((int(bns[0]) * 2**(max_lvl+3), int(bns[1]) * 2**(max_lvl+3)), dtype=data.dtype)
+    cdens = np.zeros((int(bns[ax[0]]) * 2**(max_lvl+3), int(bns[ax[1]]) * 2**(max_lvl+3)), dtype=data.dtype)
 
     for i in range(len(data)):
         xyz = coords[i].tolist()
 
         xyz.pop(axis)
 
         diff = 2**(ref_lvl[i])
@@ -420,15 +419,15 @@
 
         data_reshape = np.repeat(tmp_data, diff, axis=0)
         data_reshape = np.repeat(data_reshape, diff, axis=1)
 
         cdens[xyz[0]:xyz[0]+sub_cube_size, xyz[1]:xyz[1]+sub_cube_size] += data_reshape
     if use_weights:
         cdens /= norm
-    return cdens.T 
+    return cdens
 
 
 def get_slice(data, pos, axis, ref_lvl, bbox, bsize, brefs, bns):
     '''
     Get the slice of the data at the current position.
 
     - data: data extracted by h5py filtered by the block list
@@ -453,24 +452,21 @@
     # safety features
     assert axis in [0,1,2], f"Axis {axis} is not 0, 1, or 2 (x, y or z)."
 
     # As the data and coordinates are stored in different order
     # we need to derive the axis we have for the data insertion seperately
     ax = [0, 1, 2]
     ax_c = ax.pop(axis)
-    pax = [2, 1, 0]
-    # This is the axis which we slice over
-    pax_c = pax.pop(axis)
     # Remaining axis are left for expansion if necessary
 
     # Derive coordinates from the lower corner of the bounding box
     coords = bbox[:, :, 0] - bbox[0, :, 0]
     # Shift the axis such that 0 in the selected axis is our required slice
     # Normalise to smallest block size
-    coords /= bsize.min()
+    coords /= bsize.min(axis=0)
     # Round values to get next cell position
     coords = np.round(coords)
     # Convert to integer as these are now direct indicies
     coords = coords.astype(int) * bshape
     
     tmp_id = (pos - bbox[:, axis, 0]) / bsize[:, axis] * bshape[axis]
     tmp_id = tmp_id.astype(int)
@@ -486,23 +482,23 @@
         # Get the lower index along the slice axis
         pi = xyz.pop(axis)
 
         # Get factor of block size in relation to smallest block
         diff = 2**(ref_lvl[i])
         
         # Check if our 0 index is within the range of the current block
-        if tmp_id[i] < 0 or tmp_id[i] >= 8:
+        if tmp_id[i] < 0 or tmp_id[i] >= bshape[axis]:
             continue
         
         # Create general slice array
         sel = [slice(None, None, None), slice(None, None, None), slice(None, None, None)]
         sel[ax_c] = slice(tmp_id[i], tmp_id[i]+1, None)
 
         # Increase block size to fit the refinement level
         data_reshape = np.repeat(data[i].T[sel[0], sel[1], sel[2]], diff, axis=ax[0])
         data_reshape = np.repeat(data_reshape, diff, axis=ax[1])
         # Get size of the slice patch
         sub_cube_size = int(2**(ref_lvl[i] + 3))
         # Store in slice array, needs to be transposed to convert from ZYX to XYZ
         sl_ax[xyz[0]:xyz[0]+sub_cube_size, xyz[1]:xyz[1]+sub_cube_size] = np.squeeze(data_reshape)
 
-    return sl_ax.T
+    return sl_ax
```

### Comparing `flash_amr_tools-1.1.0a1/flash_amr_tools/block_tools.py` & `flash_amr_tools-1.1.1/flash_amr_tools/block_tools.py`

 * *Files identical despite different names*

### Comparing `flash_amr_tools-1.1.0a1/flash_amr_tools/zorder.py` & `flash_amr_tools-1.1.1/flash_amr_tools/zorder.py`

 * *Files identical despite different names*

### Comparing `flash_amr_tools-1.1.0a1/flash_amr_tools.egg-info/PKG-INFO` & `flash_amr_tools-1.1.1/flash_amr_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash_amr_tools
-Version: 1.1.0a1
+Version: 1.1.1
 Summary: Small tool to create uniform data cubes of FLASH datasets. Port from bitbucket.org/pierrenbg/flash-amr-tools
 Author-email: Keito Watanabe <k.wat8973@gmail.com>, Pierre Nürnberger <nuernb@ph1.uni-koeln.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Keito Watanabe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `flash_amr_tools-1.1.0a1/tests/test_amrtools.py` & `flash_amr_tools-1.1.1/tests/test_amrtools.py`

 * *Files identical despite different names*

