# Comparing `tmp/imseqvis-0.2.2.tar.gz` & `tmp/imseqvis-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imseqvis-0.2.2.tar", last modified: Sun Jul 30 11:33:54 2023, max compression
+gzip compressed data, was "imseqvis-0.2.3.tar", last modified: Tue May  7 20:23:03 2024, max compression
```

## Comparing `imseqvis-0.2.2.tar` & `imseqvis-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.065924 imseqvis-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.061923 imseqvis-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.061923 imseqvis-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-30 11:33:44.000000 imseqvis-0.2.2/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-30 11:33:44.000000 imseqvis-0.2.2/.github/workflows/publish-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-30 11:33:44.000000 imseqvis-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-30 11:33:44.000000 imseqvis-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-30 11:33:54.065924 imseqvis-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-30 11:33:44.000000 imseqvis-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.061923 imseqvis-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-30 11:33:44.000000 imseqvis-0.2.2/examples/demo_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-30 11:33:44.000000 imseqvis-0.2.2/examples/demo_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)    75232 2023-07-30 11:33:44.000000 imseqvis-0.2.2/examples/screenshot.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.061923 imseqvis-0.2.2/imseqvis/
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-30 11:33:44.000000 imseqvis-0.2.2/imseqvis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-07-30 11:33:44.000000 imseqvis-0.2.2/imseqvis/control_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-07-30 11:33:44.000000 imseqvis-0.2.2/imseqvis/image_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-30 11:33:44.000000 imseqvis-0.2.2/imseqvis/sequence_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 11:33:54.061923 imseqvis-0.2.2/imseqvis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-30 11:33:54.000000 imseqvis-0.2.2/imseqvis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-30 11:33:54.000000 imseqvis-0.2.2/imseqvis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 11:33:54.000000 imseqvis-0.2.2/imseqvis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-30 11:33:54.000000 imseqvis-0.2.2/imseqvis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 11:33:54.000000 imseqvis-0.2.2/imseqvis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-30 11:33:44.000000 imseqvis-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 11:33:54.065924 imseqvis-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:03.646849 imseqvis-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 20:22:52.000000 imseqvis-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-07 20:23:03.646849 imseqvis-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-07 20:22:52.000000 imseqvis-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:03.646849 imseqvis-0.2.3/imseqvis/
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-07 20:22:52.000000 imseqvis-0.2.3/imseqvis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-07 20:22:52.000000 imseqvis-0.2.3/imseqvis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10962 2024-05-07 20:22:52.000000 imseqvis-0.2.3/imseqvis/control_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16818 2024-05-07 20:22:52.000000 imseqvis-0.2.3/imseqvis/image_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-07 20:22:52.000000 imseqvis-0.2.3/imseqvis/sequence_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:03.646849 imseqvis-0.2.3/imseqvis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-07 20:23:03.000000 imseqvis-0.2.3/imseqvis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 20:23:03.000000 imseqvis-0.2.3/imseqvis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:23:03.000000 imseqvis-0.2.3/imseqvis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 20:23:03.000000 imseqvis-0.2.3/imseqvis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 20:23:03.000000 imseqvis-0.2.3/imseqvis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-07 20:22:52.000000 imseqvis-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:23:03.646849 imseqvis-0.2.3/setup.cfg
```

### Comparing `imseqvis-0.2.2/LICENSE` & `imseqvis-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imseqvis-0.2.2/PKG-INFO` & `imseqvis-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imseqvis
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Qt-based image sequence visualizer widget
 Author-email: snototter <snototter@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 snototter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,25 +29,34 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: natsort
+Requires-Dist: numpy
+Requires-Dist: qimage2ndarray
+Requires-Dist: qtpy
+Requires-Dist: vito
 Provides-Extra: pyqt5
+Requires-Dist: PyQt5; extra == "pyqt5"
 Provides-Extra: pyqt6
+Requires-Dist: PyQt6; extra == "pyqt6"
 Provides-Extra: pyside2
+Requires-Dist: PySide2; extra == "pyside2"
 Provides-Extra: pyside6
-License-File: LICENSE
+Requires-Dist: PySide6; extra == "pyside6"
 
 # Image & Sequence Visualization
 [![View on PyPI](https://img.shields.io/pypi/v/imseqvis.svg)](https://pypi.org/project/imseqvis)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/snototter/imseqvis/blob/main/LICENSE?raw=true)
 
-This package provides GUI widgets to show images and playback image sequences.
+This package provides GUI widgets to show images and play back image sequences.
 
 ![Screenshot Sequence Viewer](https://github.com/snototter/imseqvis/blob/main/examples/screenshot.jpg?raw=true "SequenceViewer widget")
 
 ### Installation
 It is highly recommended to set up a separate virtual environment with an up-to-date `pip`:
 ```bash
 python3 -m venv venv
```

### Comparing `imseqvis-0.2.2/README.md` & `imseqvis-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Image & Sequence Visualization
 [![View on PyPI](https://img.shields.io/pypi/v/imseqvis.svg)](https://pypi.org/project/imseqvis)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/snototter/imseqvis/blob/main/LICENSE?raw=true)
 
-This package provides GUI widgets to show images and playback image sequences.
+This package provides GUI widgets to show images and play back image sequences.
 
 ![Screenshot Sequence Viewer](https://github.com/snototter/imseqvis/blob/main/examples/screenshot.jpg?raw=true "SequenceViewer widget")
 
 ### Installation
 It is highly recommended to set up a separate virtual environment with an up-to-date `pip`:
 ```bash
 python3 -m venv venv
```

### Comparing `imseqvis-0.2.2/imseqvis/__init__.py` & `imseqvis-0.2.3/imseqvis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from pathlib import Path
 from typing import Union
 
+__version__ = "0.2.3"
+
 
 def show_sequence(
         image_sequence,
         window_title: str = "Image Sequence Viewer",
         **kwargs) -> int:
     """
     Runs the ImageSequenceViewer for the given image sequence.
@@ -64,15 +66,15 @@
       window_title: The title of the application window.
       kwargs: Additional arguments passed to the SequenceViewer.
 
     Returns:
       The application's exit code.
     """
     from .sequence_viewer import ImageFolder
-    return show_sequence(ImageFolder(folder))
+    return show_sequence(ImageFolder(folder), window_title, **kwargs)
 
 
 def show(
         data_source: Union[Path, str, object],
         window_title: str = "Image Sequence Viewer",
         **kwargs) -> int:
     """
```

### Comparing `imseqvis-0.2.2/imseqvis/control_widget.py` & `imseqvis-0.2.3/imseqvis/control_widget.py`

 * *Files identical despite different names*

### Comparing `imseqvis-0.2.2/imseqvis/image_viewer.py` & `imseqvis-0.2.3/imseqvis/image_viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import qimage2ndarray
 from pathlib import Path
 
 from qtpy.QtWidgets import QWidget, QScrollArea, QApplication
 from qtpy.QtCore import Qt, QPointF, Signal, Slot, QRect, QMimeData
 from qtpy.QtGui import (
     QPixmap, QImage, QFont, QPainter, QPen, QColor, QBrush, QPalette,
-    QMouseEvent)
+    QMouseEvent, QCursor)
 
 
 def pixmapFromNumpy(img_np: np.array) -> QPixmap:
     """
     Converts the given NumPy array image into a QPixmap.
 
     Args:
@@ -355,29 +355,45 @@
 
     @Slot(int)
     def zoom(self, delta: int):
         """Scale the displayed image. Zoom in if delta > 0.
         Usually to be called with mouse wheel delta values, thus
         the actual zoom steps are computed as delta/120.
         """
+        cursor_pos = QCursor().pos()
+        px_pos_prev = self._canvas.pixelAtWidgetPos(
+            self._canvas.mapFromGlobal(cursor_pos))
         self._img_scale += 0.05 * delta / 120
         self.paintCanvas()
+        # Adjust the scroll bar positions to keep cursor at the same pixel
+        px_pos_curr = self._canvas.pixelAtWidgetPos(
+            self._canvas.mapFromGlobal(cursor_pos))
+        delta_widget = self._canvas.pixelToWidgetPos(px_pos_curr) \
+            - self._canvas.pixelToWidgetPos(px_pos_prev)
+        self.scrollRelative(
+            delta_widget.x()*120/self.horizontalScrollBar().singleStep(),
+            Qt.Horizontal)
+        self.scrollRelative(
+            delta_widget.y()*120/self.verticalScrollBar().singleStep(),
+            Qt.Vertical)
 
     @Slot(int, int)
     def scrollRelative(self, delta, orientation):
         """Slot for scrollRequest signal of image canvas."""
         steps = -delta / 120
         bar = self._scoll_bars[orientation]
         value = bar.value() + bar.singleStep() * steps
         self.scrollAbsolute(value, orientation)
 
     @Slot(int, int)
     def scrollAbsolute(self, value, orientation):
         """Sets the scrollbar to the given value."""
         bar = self._scoll_bars[orientation]
+        # Ensure that value is an integer to prevent TypeError within bar.setValue()
+        value = int(value)
         if value < bar.minimum():
             value = bar.minimum()
         if value > bar.maximum():
             value = bar.maximum()
         bar.setValue(value)
         self.viewChanged.emit()
```

### Comparing `imseqvis-0.2.2/imseqvis/sequence_viewer.py` & `imseqvis-0.2.3/imseqvis/sequence_viewer.py`

 * *Files identical despite different names*

### Comparing `imseqvis-0.2.2/imseqvis.egg-info/PKG-INFO` & `imseqvis-0.2.3/imseqvis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imseqvis
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Qt-based image sequence visualizer widget
 Author-email: snototter <snototter@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 snototter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,25 +29,34 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: natsort
+Requires-Dist: numpy
+Requires-Dist: qimage2ndarray
+Requires-Dist: qtpy
+Requires-Dist: vito
 Provides-Extra: pyqt5
+Requires-Dist: PyQt5; extra == "pyqt5"
 Provides-Extra: pyqt6
+Requires-Dist: PyQt6; extra == "pyqt6"
 Provides-Extra: pyside2
+Requires-Dist: PySide2; extra == "pyside2"
 Provides-Extra: pyside6
-License-File: LICENSE
+Requires-Dist: PySide6; extra == "pyside6"
 
 # Image & Sequence Visualization
 [![View on PyPI](https://img.shields.io/pypi/v/imseqvis.svg)](https://pypi.org/project/imseqvis)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/snototter/imseqvis/blob/main/LICENSE?raw=true)
 
-This package provides GUI widgets to show images and playback image sequences.
+This package provides GUI widgets to show images and play back image sequences.
 
 ![Screenshot Sequence Viewer](https://github.com/snototter/imseqvis/blob/main/examples/screenshot.jpg?raw=true "SequenceViewer widget")
 
 ### Installation
 It is highly recommended to set up a separate virtual environment with an up-to-date `pip`:
 ```bash
 python3 -m venv venv
```

### Comparing `imseqvis-0.2.2/pyproject.toml` & `imseqvis-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imseqvis"
+dynamic = ["version"]
 
 description = "A Qt-based image sequence visualizer widget"
 readme = "README.md"
 
-version = "0.2.2"
 license = {file = "LICENSE"}
 
 authors = [
     { name = "snototter", email = "snototter@users.noreply.github.com" }
 ]
 
 requires-python = ">=3.7"
@@ -44,7 +44,10 @@
 pyqt5 = ["PyQt5"]
 pyqt6 = ["PyQt6"]
 pyside2 = ["PySide2"]
 pyside6 = ["PySide6"]
 
 [tool.setuptools]
 packages = ["imseqvis"]
+
+[tool.setuptools.dynamic]
+version = {attr = "imseqvis.__version__"}
```

