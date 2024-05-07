# Comparing `tmp/ndimage-enaml-0.0.7.tar.gz` & `tmp/ndimage_enaml-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndimage-enaml-0.0.7.tar", last modified: Tue Feb 27 21:24:36 2024, max compression
+gzip compressed data, was "ndimage_enaml-0.0.8.tar", last modified: Tue May  7 22:03:59 2024, max compression
```

## Comparing `ndimage-enaml-0.0.7.tar` & `ndimage_enaml-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:24:36.768663 ndimage-enaml-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:24:36.764662 ndimage-enaml-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:24:36.768663 ndimage-enaml-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-27 21:24:28.000000 ndimage-enaml-0.0.7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-02-27 21:24:28.000000 ndimage-enaml-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-27 21:24:36.768663 ndimage-enaml-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-02-27 21:24:28.000000 ndimage-enaml-0.0.7/license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:24:36.768663 ndimage-enaml-0.0.7/ndimage_enaml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 21:24:28.000000 ndimage-enaml-0.0.7/ndimage_enaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-02-27 21:24:28.000000 ndimage-enaml-0.0.7/ndimage_enaml/gui.enaml
--rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-02-27 21:24:28.000000 ndimage-enaml-0.0.7/ndimage_enaml/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-02-27 21:24:28.000000 ndimage-enaml-0.0.7/ndimage_enaml/presenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-02-27 21:24:28.000000 ndimage-enaml-0.0.7/ndimage_enaml/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-27 21:24:36.000000 ndimage-enaml-0.0.7/ndimage_enaml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:24:36.768663 ndimage-enaml-0.0.7/ndimage_enaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-27 21:24:36.000000 ndimage-enaml-0.0.7/ndimage_enaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-27 21:24:36.000000 ndimage-enaml-0.0.7/ndimage_enaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 21:24:36.000000 ndimage-enaml-0.0.7/ndimage_enaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-27 21:24:36.000000 ndimage-enaml-0.0.7/ndimage_enaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-27 21:24:36.000000 ndimage-enaml-0.0.7/ndimage_enaml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-27 21:24:28.000000 ndimage-enaml-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-27 21:24:28.000000 ndimage-enaml-0.0.7/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 21:24:36.768663 ndimage-enaml-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:03:59.630823 ndimage_enaml-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:03:59.626823 ndimage_enaml-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:03:59.626823 ndimage_enaml-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-07 22:03:55.000000 ndimage_enaml-0.0.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-07 22:03:55.000000 ndimage_enaml-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 22:03:59.630823 ndimage_enaml-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 22:03:55.000000 ndimage_enaml-0.0.8/license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:03:59.626823 ndimage_enaml-0.0.8/ndimage_enaml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:03:55.000000 ndimage_enaml-0.0.8/ndimage_enaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-07 22:03:55.000000 ndimage_enaml-0.0.8/ndimage_enaml/gui.enaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-07 22:03:55.000000 ndimage_enaml-0.0.8/ndimage_enaml/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-05-07 22:03:55.000000 ndimage_enaml-0.0.8/ndimage_enaml/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-07 22:03:55.000000 ndimage_enaml-0.0.8/ndimage_enaml/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 22:03:59.000000 ndimage_enaml-0.0.8/ndimage_enaml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:03:59.630823 ndimage_enaml-0.0.8/ndimage_enaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 22:03:59.000000 ndimage_enaml-0.0.8/ndimage_enaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-07 22:03:59.000000 ndimage_enaml-0.0.8/ndimage_enaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:03:59.000000 ndimage_enaml-0.0.8/ndimage_enaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 22:03:59.000000 ndimage_enaml-0.0.8/ndimage_enaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-07 22:03:59.000000 ndimage_enaml-0.0.8/ndimage_enaml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 22:03:55.000000 ndimage_enaml-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 22:03:55.000000 ndimage_enaml-0.0.8/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:03:59.630823 ndimage_enaml-0.0.8/setup.cfg
```

### Comparing `ndimage-enaml-0.0.7/.github/workflows/publish-to-pypi.yml` & `ndimage_enaml-0.0.8/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `ndimage-enaml-0.0.7/.gitignore` & `ndimage_enaml-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ndimage-enaml-0.0.7/license` & `ndimage_enaml-0.0.8/license`

 * *Files identical despite different names*

### Comparing `ndimage-enaml-0.0.7/ndimage_enaml/gui.enaml` & `ndimage_enaml-0.0.8/ndimage_enaml/gui.enaml`

 * *Files identical despite different names*

### Comparing `ndimage-enaml-0.0.7/ndimage_enaml/model.py` & `ndimage_enaml-0.0.8/ndimage_enaml/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,11 @@
 import logging
 log = logging.getLogger(__name__)
 
 
-CHANNEL_CONFIG = {
-    'CtBP2': { 'display_color': '#FF0000'},
-    'MyosinVIIa': {'display_color': '#0000FF'},
-    'GluR2': {'display_color': '#00FF00'},
-    'GlueR2': {'display_color': '#00FF00'},
-    'PMT': {'display_color': '#FFFFFF'},
-    'DAPI': {'display_color': '#FFFFFF'},
-
-    # Channels are tagged as unknown if there's difficulty parsing the channel
-    # information from the file.
-    'Unknown 1': {'display_color': '#FF0000'},
-    'Unknown 2': {'display_color': '#00FF00'},
-    'Unknown 3': {'display_color': '#0000FF'},
-    'Unknown 4': {'display_color': '#FFFFFF'},
-}
-
-
 from atom.api import Atom, Bool, Dict, Float, Int, List, Str, Typed
 from enaml.colors import ColorMember
 from matplotlib import transforms as T
 import numpy as np
 from raster_geometry import sphere
 from scipy import ndimage
 from scipy import signal
@@ -52,24 +35,24 @@
             'min_value': self.min_value,
             'max_value': self.max_value,
             'visible': self.visible,
             'display_color': color,
         }
 
 
-def make_channel_config(info):
+def make_channel_config(info, defaults):
     channel_config = {}
     unknown = 0
     for i, c in enumerate(info['channels']):
         name = c['name']
-        if name not in CHANNEL_CONFIG:
-            config = CHANNEL_CONFIG[f'Unknown {unknown+1}'].copy()
+        if name not in defaults:
+            config = defaults[f'Unknown {unknown+1}'].copy()
             unknown += 1
         else:
-            config = CHANNEL_CONFIG[name].copy()
+            config = defaults[name].copy()
         config.update(c)
         config['i'] = i
         channel_config[name] = config
     return channel_config
 
 
 def get_channel_config(channels, channel_config):
@@ -94,29 +77,36 @@
     info = Dict()
     image = Typed(np.ndarray)
     extent = List()
     n_channels = Int()
     source = Str()
     channel_config = Dict()
 
-    def __init__(self, info, image):
+    # This shoudl be a mapping of channel name to a dictionary containing
+    # default values that will be set in ChannelConfig (e.g., display_color,
+    # visible, min_value, max_value, etc.). Any attribute specified by
+    # `ChannelConfig` can be specified here.
+    channel_defaults = Dict()
+
+    def __init__(self, info, image, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.info = info
         self.image = image
         xlb, ylb, zlb = self.info["lower"][:3]
 
         # Images are in XYZC dimension. We need to calculate the upper extent
         # of the image so we can properly plot it.
         xpx, ypx, zpx = self.image.shape[:3]
         xv, yv, zv = self.info['voxel_size'][:3]
         xub = xlb + xpx * xv
         yub = ylb + ypx * yv
         zub = zlb + zpx * zv
         self.extent = [xlb, xub, ylb, yub, zlb, zub]
         self.n_channels = self.image.shape[-1]
-        self.channel_config = make_channel_config(info)
+        self.channel_config = make_channel_config(info, self.channel_defaults)
 
     @property
     def channel_names(self):
         return [c['name'] for c in self.info['channels']]
 
     def contains(self, x, y):
         contains_x = self.extent[0] <= x <= self.extent[1]
@@ -346,8 +336,9 @@
         t_base = self.tiles[0]
         extra_keys = set(t_base.info.keys()) - set(('lower', 'voxel_size', 'rotation'))
         for k in extra_keys:
             for t in self.tiles[1:]:
                 if t_base.info[k] != t.info[k]:
                     raise ValueError(f'Cannot merge tiles. {k} differs.')
             info[k] = t_base.info[k]
-        return NDImage(info, merged_image)
+        return NDImage(info, merged_image,
+                       channel_defaults=self.tiles[0].channel_defaults)
```

### Comparing `ndimage-enaml-0.0.7/ndimage_enaml/presenter.py` & `ndimage_enaml-0.0.8/ndimage_enaml/presenter.py`

 * *Files identical despite different names*

### Comparing `ndimage-enaml-0.0.7/ndimage_enaml/util.py` & `ndimage_enaml-0.0.8/ndimage_enaml/util.py`

 * *Files identical despite different names*

### Comparing `ndimage-enaml-0.0.7/pyproject.toml` & `ndimage_enaml-0.0.8/pyproject.toml`

 * *Files identical despite different names*

