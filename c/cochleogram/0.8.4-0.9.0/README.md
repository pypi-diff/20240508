# Comparing `tmp/cochleogram-0.8.4.tar.gz` & `tmp/cochleogram-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.8.4.tar", last modified: Mon Apr 15 18:02:43 2024, max compression
+gzip compressed data, was "cochleogram-0.9.0.tar", last modified: Tue May  7 22:05:34 2024, max compression
```

## Comparing `cochleogram-0.8.4.tar` & `cochleogram-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.990105 cochleogram-0.8.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.982105 cochleogram-0.8.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.986105 cochleogram-0.8.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-15 18:02:39.000000 cochleogram-0.8.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-15 18:02:39.000000 cochleogram-0.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-15 18:02:43.990105 cochleogram-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-15 18:02:39.000000 cochleogram-0.8.4/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.986105 cochleogram-0.8.4/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    28716 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.990105 cochleogram-0.8.4/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/main-icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (127)    25893 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18597 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.990105 cochleogram-0.8.4/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 18:02:39.000000 cochleogram-0.8.4/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-15 18:02:39.000000 cochleogram-0.8.4/license
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-15 18:02:39.000000 cochleogram-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-04-15 18:02:39.000000 cochleogram-0.8.4/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:02:43.990105 cochleogram-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.726924 cochleogram-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.718924 cochleogram-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.718924 cochleogram-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-07 22:05:30.000000 cochleogram-0.9.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-07 22:05:30.000000 cochleogram-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-05-07 22:05:34.726924 cochleogram-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-07 22:05:30.000000 cochleogram-0.9.0/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.722924 cochleogram-0.9.0/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28645 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.726924 cochleogram-0.9.0/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/main-icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25893 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16508 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18597 2024-05-07 22:05:30.000000 cochleogram-0.9.0/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:05:34.726924 cochleogram-0.9.0/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 22:05:34.000000 cochleogram-0.9.0/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-07 22:05:30.000000 cochleogram-0.9.0/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-07 22:05:30.000000 cochleogram-0.9.0/license
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-07 22:05:30.000000 cochleogram-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-05-07 22:05:30.000000 cochleogram-0.9.0/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:05:34.726924 cochleogram-0.9.0/setup.cfg
```

### Comparing `cochleogram-0.8.4/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.9.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/.gitignore` & `cochleogram-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/PKG-INFO` & `cochleogram-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.8.4
+Version: 0.9.0
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Requires-Dist: atom
 Requires-Dist: enaml[qt6-pyside]
 Requires-Dist: matplotlib
-Requires-Dist: ndimage-enaml>=0.0.7
+Requires-Dist: ndimage-enaml>=0.0.8
 Requires-Dist: numpy
 Requires-Dist: raster_geometry
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: scikit-image
 Requires-Dist: psiaudio
 Provides-Extra: czi
```

### Comparing `cochleogram-0.8.4/cochleogram/config.py` & `cochleogram-0.9.0/cochleogram/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 CELLS = ('IHC', 'OHC1', 'OHC2', 'OHC3', 'Extra')
 
 
 CHANNEL_CONFIG = {
-    'CtBP2': { 'display_color': 'red'},
-    'MyosinVIIa': {'display_color': 'blue'},
-    'GluR2': {'display_color': 'green'},
-    'GlueR2': {'display_color': 'green'},
-    'PMT': {'display_color': 'white'},
-    'DAPI': {'display_color': 'white'},
+    'CtBP2': { 'display_color': '#FF0000'},
+    'MyosinVIIa': {'display_color': '#0000FF'},
+    'GluR2': {'display_color': '#00FF00'},
+    'GlueR2': {'display_color': '#00FF00'},
+    'PMT': {'display_color': '#FFFFFF'},
+    'DAPI': {'display_color': '#FFFFFF', 'visible': False},
 
     # Channels are tagged as unknown if there's difficulty parsing the channel
     # information from the file.
-    'Unknown 1': {'display_color': 'red'},
-    'Unknown 2': {'display_color': 'green'},
-    'Unknown 3': {'display_color': 'blue'},
+    'Unknown 1': {'display_color': '#FF0000'},
+    'Unknown 2': {'display_color': '#00FF00'},
+    'Unknown 3': {'display_color': '#0000FF'},
+    'Unknown 4': {'display_color': '#FFFFFF'},
 }
 
 
 TOOL_KEY_MAP = {
     's': 'spiral',
     'e': 'exclude',
     'c': 'cells',
```

### Comparing `cochleogram-0.8.4/cochleogram/gui.enaml` & `cochleogram-0.9.0/cochleogram/gui.enaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 log = logging.getLogger(__name__)
 
 from importlib import resources
 from pathlib import Path
 import re
+import urllib.request
 
 from enaml.application import deferred_call
 from enaml.core.api import Conditional, Looper
 from enaml.icon import Icon, IconImage
 from enaml.image import Image
 from enaml.layout.api import align, hbox, InsertTab, RemoveItem, spacer, TabLayout, vbox
 from enaml.stdlib.fields import FloatField
@@ -67,15 +68,15 @@
     return open_cochlea_dataset(window, readers.CZICochleaReader, 'dir')
 
 
 def load_cochlea_dataset(path, window, reader_class=None):
     path = Path(path)
     if reader_class is None:
         if path.is_dir():
-            reader_class = readers.ProcessedCochleaReader
+            reader_class = readers.CZICochleaReader
         elif path.suffix.lower() == '.lif':
             reader_class = readers.LIFCochleaReader
         else:
             raise ValueError(f'Unrecognized format for {path}')
 
     # First, make sure we can load the data
     reader = reader_class(path)
@@ -229,22 +230,14 @@
             try:
                 presenter.action_clear_cells()
             except Exception as e:
                 log.exception(e)
                 information(self, 'Error', str(e))
 
 
-def guess_cells_channel(cells, channel_names):
-    if cells == 'IHC' and 'CtBP2' in channel_names:
-        return 'CtBP2'
-    if 'MyosinVIIa' in channel_names:
-        return 'MyosinVIIa'
-    return channel_names[0]
-
-
 enamldef ActionGuessCells(HGroup):
     attr presenter
     attr is_copy = False
 
     constraints = [
         guess_width.width == 50,
         guess_spacing.width == 50,
@@ -255,78 +248,67 @@
     share_layout = True
     trailing_spacer = spacer(0)
     enabled << (presenter.current_spiral_artist is not None) \
         and presenter.current_spiral_artist.has_spline
     Label:
         text = 'Find cells within'
     FloatField: guess_width:
-        value = 2.5
+        value := presenter.guess_width
     Label:
         text = 'μm of spline with a spacing of'
     FloatField: guess_spacing:
-        value = 5.0
+        value := presenter.guess_spacing
     Label:
         text = 'μm using'
     ObjectCombo: guess_channel:
         items = presenter.obj.channel_names
-        selected << guess_cells_channel(presenter.cells, presenter.obj.channel_names)
+        selected := presenter.guess_channel
 
     PushButton:
-        text = 'update'
+        text = 'Count'
         clicked ::
             button = question(self, 'Confirm action', f'Are you sure you want to overwrite the existing cells?')
             if button is not None and button.text == 'Yes':
                 try:
-                    n = presenter.action_guess_cells(guess_width.value,
-                                                     guess_spacing.value,
-                                                     guess_channel.selected)
+                    n = presenter.action_guess_cells()
                     information(self, 'Info', f'Found {n} cells')
                 except Exception as e:
                     log.exception(e)
                     information(self, 'Error', str(e))
 
 
-P_FREQ = re.compile(r'.*?(\d+p\d+)_kHz.*')
-
-def get_tile_di_title(unsaved_changes, name):
+def get_tile_di_title(unsaved_changes, obj):
     pre = '*' if unsaved_changes else ''
-    if (m := P_FREQ.match(name)) is not None:
-        freq = m.group(1).replace('p', '.')
-        title = f'{pre}{freq} kHz - {name}'
-    else:
-        title = f'{pre}{name}'
-    return title
+    if obj.frequency is not None:
+        return f'{pre}{obj.frequency} kHz - {obj.name}'
+    return f'{pre}{obj.name}'
 
 
 enamldef TileDockItem(DockItem): dock_item:
 
-    title << get_tile_di_title(presenter.unsaved_changes, presenter.obj.name)
+    title << get_tile_di_title(presenter.unsaved_changes, presenter.obj)
 
     attr presenter
     closable = False
 
     initialized ::
         bind_focus(container.children, canvas.set_focus)
         deferred_call(canvas.set_focus)
 
     Container: container:
         constraints = [
             vbox(
                 dc,
-                hbox(tool_label, mode_buttons, spacer, load_analysis, save_analysis),
-                hbox(action_label, action_clear_spiral, action_clear_cells,
-                     spacer, spacing=0),
-                hbox(action_guess_cells, spacer, spacing=0),
+                hbox(tool_label, mode_buttons, action_clear_spiral, action_clear_cells, spacer, spacing=0),
+                hbox(action_guess_cells, spacer, load_analysis, save_analysis, spacing=0),
                 canvas,
             ),
-            align('v_center', tool_label, mode_buttons),
-            align('v_center', action_label, action_clear_spiral, action_clear_cells),
-            align('left', tool_label, dc.children[0], action_label),
-            align('left', dc.children[1], mode_buttons,
-                  action_clear_spiral, action_guess_cells),
+            align('v_center', tool_label, mode_buttons, action_clear_spiral, action_clear_cells),
+            align('left', tool_label, dc.children[0]),
+            align('left', dc.children[1], mode_buttons),
         ]
 
         DisplayConfig: dc:
             presenter << dock_item.presenter
 
         PushButton: load_analysis:
             text = 'Load'
@@ -365,18 +347,15 @@
                     enabled << not (presenter.cells == 'Extra' and loop_item != 'cells')
                     group = tool_group
                     checkable = True
                     checked << loop_item == presenter.tool
                     toggled ::
                         if self.checked:
                             presenter.tool = loop_item
-                    tool_tip = "Press s to select spiral tool, c to select cell tool"
-
-        Label: action_label:
-            text = 'Actions'
+                    tool_tip = "Press shift+s to select spiral tool, shift+c to select cell tool"
 
         PBActionClearSpiral: action_clear_spiral:
             presenter << dock_item.presenter
 
         PBActionClearCells: action_clear_cells:
             presenter << dock_item.presenter
 
@@ -729,19 +708,19 @@
                             cb = lambda x, pp=pp: setattr(pp, 'progress', x)
                             deferred_call(util.czi_to_ims, path, reprocess=True, cb=cb)
 
             Action:
                 separator = True
 
             Action:
-                text = 'Save analysis\tCtrl+S'
+                text = 'Save analysis'
                 triggered ::
                     save_state(window, window.presenters)
             Action:
-                text = 'Load analysis\tCtrl+L'
+                text = 'Load analysis'
                 triggered ::
                     load_state(window, window.presenters)
 
             Action:
                 separator = True
 
             Action:
@@ -773,17 +752,31 @@
             button = question(window, 'Question', 'There are unsaved changes. Are you sure you want to exit?')
             if button is None or button.text == 'No':
                 change['value'].ignore()
 
     Container:
         DockArea: workspace:
             name = 'dock_area'
-
+            features = Feature.DropEnabled
             layout = TabLayout('help')
 
+            drag_enter => (event):
+                if event.mime_data().has_format('text/uri-list'):
+                    event.accept_proposed_action()
+
+            drop => (event):
+                text = event.mime_data().data('text/uri-list').decode('utf-8')
+                filenames = []
+                for t in text.strip().split('\n'):
+                    t = urllib.parse.unquote(t).strip()
+                    fragments = urllib.parse.urlsplit(t)
+                    path = Path(urllib.request.url2pathname(fragments.path))
+                    filenames.append(path)
+                load_dataset(filenames[0], window)
+
             DockItem:
                 name = 'help'
                 title = 'Help'
                 closable = False
 
                 Container:
                     Html:
```

### Comparing `cochleogram-0.8.4/cochleogram/icons/cells.png` & `cochleogram-0.9.0/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/cochleogram/icons/exclude.png` & `cochleogram-0.9.0/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/cochleogram/icons/main-icon.ico` & `cochleogram-0.9.0/cochleogram/icons/main-icon.ico`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/cochleogram/icons/main-icon.png` & `cochleogram-0.9.0/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/cochleogram/icons/make_icons.py` & `cochleogram-0.9.0/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/cochleogram/icons/spiral.png` & `cochleogram-0.9.0/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/cochleogram/icons/tile.png` & `cochleogram-0.9.0/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/cochleogram/instructions.html` & `cochleogram-0.9.0/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/cochleogram/main.py` & `cochleogram-0.9.0/cochleogram/main.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/cochleogram/model.py` & `cochleogram-0.9.0/cochleogram/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from scipy import ndimage
 from scipy import signal
 from skimage.registration import phase_cross_correlation
 from skimage.color import rgb2gray
 
 from raster_geometry import sphere
 
-from ndimage_enaml.model import ChannelConfig, NDImage, NDImageCollection
+from ndimage_enaml.model import NDImage, NDImageCollection
 
 from cochleogram import util
 from cochleogram.config import CELLS, CHANNEL_CONFIG
 
 
 class Points(Atom):
 
@@ -271,14 +271,17 @@
         self.updated = True
 
 
 class Tile(NDImage):
 
     source = Str()
 
+    def _default_channel_defaults(self):
+        return CHANNEL_CONFIG
+
     def __init__(self, info, image, source):
         super().__init__(info, image)
         self.source = source
 
 
 class CellAnalysis(NDImageCollection):
 
@@ -485,18 +488,20 @@
 
         return info
 
 
 class TileAnalysis(CellAnalysis):
 
     name = Str()
+    frequency = Value()
 
-    def __init__(self, tile, name):
+    def __init__(self, tile, name, frequency=None):
         super().__init__(tiles=[tile])
         self.name = name
+        self.frequency = frequency
 
 
 class TileAnalysisCollection:
 
     def __init__(self, tiles):
         self.tiles = tiles
```

### Comparing `cochleogram-0.8.4/cochleogram/plot.py` & `cochleogram-0.9.0/cochleogram/plot.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/cochleogram/presenter.py` & `cochleogram-0.9.0/cochleogram/presenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,18 +33,19 @@
 from matplotlib import patches as mpatches
 from matplotlib import path as mpath
 from matplotlib import transforms as T
 
 import numpy as np
 from scipy import interpolate
 
+from ndimage_enaml.model import ChannelConfig
 from ndimage_enaml.presenter import NDImageCollectionPresenter, StatePersistenceMixin
 
 from cochleogram.config import CELLS, CELL_COLORS, CELL_KEY_MAP, TOOL_KEY_MAP
-from cochleogram.model import ChannelConfig, Piece, Points, Tile
+from cochleogram.model import Piece, Points, Tile
 from cochleogram.readers import BaseReader
 from cochleogram.util import get_region, make_plot_path, shortest_path
 
 
 class PointPlot(Atom):
 
     #: Artist that plots the nodes the user specified
@@ -331,14 +332,15 @@
         self.rectangle = mp.patches.Rectangle((0, 0), 0, 0, ec='red', fc='None', zorder=5000, transform=self.transform)
         self.rectangle.set_alpha(0)
         self.axes.add_patch(self.rectangle)
         self.z_slice_max = self.tile.image.shape[2] - 1
         self.z_slice = self.tile.image.shape[2] // 2
         self.shift = self.tile.info["voxel_size"][0] * 5
         self.channel_config = {c: ChannelConfig(name=c) for c in tile.channel_names}
+
         for config in self.channel_config.values():
             config.observe('visible', self.request_redraw)
             config.observe('min_value', self.request_redraw)
             config.observe('max_value', self.request_redraw)
         tile.observe('extent', self.request_redraw)
 
     def _observe_highlight(self, event):
@@ -412,20 +414,44 @@
 
     #: Label of cell being marked
     cells = Str()
 
     #: List of available cells
     available_cells = Tuple()
 
+    #: Width along line to search for cells
+    guess_width = Float(2.5)
+
+    #: Minimum spacing of cells identified
+    guess_spacing = Float(5.0)
+
+    #: Channel to use for searching for cells
+    guess_channel = Str()
+
     def _default_available_cells(self):
         return CELLS
 
     def _default_cells(self):
         return self.available_cells[0]
 
+    def _default_guess_channel(self):
+        return self._guess_channel()
+
+    def _guess_channel(self):
+        if self.cells == 'IHC' and 'CtBP2' in self.obj.channel_names:
+            return 'CtBP2'
+        elif 'MyosinVIIa' in self.obj.channel_names:
+            return 'MyosinVIIa'
+        else:
+            return self.obj.channel_names[0]
+
+    def _observe_cells(self, event):
+        # Select reasonable default for guessing cells.
+        self.guess_channel = self._guess_channel()
+
     #: Active tool
     tool = Str()
 
     #: List of available tools
     available_tools = Tuple()
 
     def _default_tool(self):
@@ -486,17 +512,17 @@
             self.current_cells_artist = self.point_artists[self.cells, 'cells']
             self.current_spiral_artist.exclude_active = True
             if self.tool in ('spiral', 'exclude'):
                 self.current_spiral_artist.active = True
             else:
                 self.current_cells_artist.active = True
 
-    def action_guess_cells(self, width, spacing, channel):
+    def action_guess_cells(self):
         z_slice = self.current_artist.z_slice if self.current_artist.display_mode == 'slice' else None
-        n = self.obj.guess_cells(self.cells, width, spacing, channel, z_slice)
+        n = self.obj.guess_cells(self.cells, self.guess_width, self.guess_spacing, self.guess_channel, z_slice)
         self.set_interaction_mode(None, 'cells')
         return n
 
     def action_clear_cells(self):
         self.obj.clear_cells(self.cells)
         self.set_interaction_mode(None, 'cells')
 
@@ -542,14 +568,19 @@
         key = event.key.lower()
         if (t := TOOL_KEY_MAP.get(key, None)) is not None:
             deferred_call(self.set_interaction_mode, None, t)
             return True
         if (c := CELL_KEY_MAP.get(key, None)) is not None:
             deferred_call(self.set_interaction_mode, c, None)
             return True
+        if key == 'ctrl+s':
+            self.save_state()
+            return True
+        if key == 'ctrl+c':
+            self.action_guess_cells()
         return False
 
     def get_state(self):
         artist_states = {k: a.get_state() for k, a in self.ndimage_artists.items()}
         point_artist_states = {':'.join(k): a.get_state() for k, a in self.point_artists.items()}
         return {
             "cells": self.cells,
```

### Comparing `cochleogram-0.8.4/cochleogram/readers.py` & `cochleogram-0.9.0/cochleogram/readers.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 import re
 
 import numpy as np
 
 from . import model
 from . import util
 
+P_FREQ = re.compile(r'.*?(\d+p\d+)_kHz.*')
+
+
+def extract_frequency(name):
+    if (m := P_FREQ.match(name)) is not None:
+        return float(m.group(1).replace('p', '.'))
+    return None
+
 
 class BaseReader:
     '''
     Base class of all readers. Provides state persistence for analysis. Actual
     loading of data and generation of filenames for saving state persistence
     data should be handled by subclasses.
     '''
@@ -238,39 +246,41 @@
         from readlif.reader import LifFile
         super().__init__(path, pattern)
         self.fh = LifFile(path)
 
     def load_tile(self, tile_name):
         info, img = util.load_lif(self.path, tile_name)
         tile = model.Tile(info, img, source=tile_name)
-        return model.TileAnalysis(tile, name=tile_name)
+        freq = extract_frequency(tile_name)
+        return model.TileAnalysis(tile, name=tile_name, frequency=freq)
 
     def list_tiles(self):
         tile_names = {}
         for img in self.fh.get_iter_image():
             try:
                 tile_name = self.pattern.match(img.name).group(1)
                 tile_names[img.name] = tile_name
             except Exception as e:
                 pass
-        return tile_names
+        return sorted(tile_names, key=extract_frequency)
 
     def save_path(self):
         return self.path.parent / self.path.stem
 
 
 class CZITileReader(TileReader):
 
     def load_tile(self, tile_name):
         filename = self.path / f'{tile_name}.czi'
         info, img = util.load_czi(filename)
         tile = model.Tile(info, img, source=tile_name)
-        return model.TileAnalysis(tile, name=tile_name)
+        freq = extract_frequency(tile_name)
+        return model.TileAnalysis(tile, name=tile_name, frequency=freq)
 
     def list_tiles(self):
         tile_names = {}
         for img in self.path.glob('*.czi'):
             tile_names[img.stem] = img.stem
-        return tile_names
+        return sorted(tile_names, key=extract_frequency)
 
     def save_path(self):
         return self.path
```

### Comparing `cochleogram-0.8.4/cochleogram/util.py` & `cochleogram-0.9.0/cochleogram/util.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.9.0/cochleogram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.8.4
+Version: 0.9.0
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Requires-Dist: atom
 Requires-Dist: enaml[qt6-pyside]
 Requires-Dist: matplotlib
-Requires-Dist: ndimage-enaml>=0.0.7
+Requires-Dist: ndimage-enaml>=0.0.8
 Requires-Dist: numpy
 Requires-Dist: raster_geometry
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: scikit-image
 Requires-Dist: psiaudio
 Provides-Extra: czi
```

### Comparing `cochleogram-0.8.4/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.9.0/cochleogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/license` & `cochleogram-0.9.0/license`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.4/pyproject.toml` & `cochleogram-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 maintainers = [
     {name = "Brad Buran", email="buran@ohsu.edu"},
 ]
 dependencies = [
     "atom",
     "enaml[qt6-pyside]",
     "matplotlib",
-	"ndimage-enaml >= 0.0.7",
+	"ndimage-enaml >= 0.0.8",
     "numpy",
     "raster_geometry",
     "pandas",
     "scipy",
     "scikit-image",
     "psiaudio",
 ]
```

### Comparing `cochleogram-0.8.4/readme.rst` & `cochleogram-0.9.0/readme.rst`

 * *Files identical despite different names*

