# Comparing `tmp/imseqvis-0.2.3.tar.gz` & `tmp/imseqvis-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imseqvis-0.2.3.tar", last modified: Tue May  7 20:23:03 2024, max compression
+gzip compressed data, was "imseqvis-0.2.4.tar", last modified: Wed May  8 06:45:51 2024, max compression
```

## Comparing `imseqvis-0.2.3.tar` & `imseqvis-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:03.646849 imseqvis-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 20:22:52.000000 imseqvis-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-07 20:23:03.646849 imseqvis-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-07 20:22:52.000000 imseqvis-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:03.646849 imseqvis-0.2.3/imseqvis/
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-07 20:22:52.000000 imseqvis-0.2.3/imseqvis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-07 20:22:52.000000 imseqvis-0.2.3/imseqvis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10962 2024-05-07 20:22:52.000000 imseqvis-0.2.3/imseqvis/control_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    16818 2024-05-07 20:22:52.000000 imseqvis-0.2.3/imseqvis/image_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-07 20:22:52.000000 imseqvis-0.2.3/imseqvis/sequence_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:03.646849 imseqvis-0.2.3/imseqvis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-07 20:23:03.000000 imseqvis-0.2.3/imseqvis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 20:23:03.000000 imseqvis-0.2.3/imseqvis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:23:03.000000 imseqvis-0.2.3/imseqvis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 20:23:03.000000 imseqvis-0.2.3/imseqvis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 20:23:03.000000 imseqvis-0.2.3/imseqvis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-07 20:22:52.000000 imseqvis-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:23:03.646849 imseqvis-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:45:51.379168 imseqvis-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 06:45:44.000000 imseqvis-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-08 06:45:51.379168 imseqvis-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-08 06:45:44.000000 imseqvis-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:45:51.375168 imseqvis-0.2.4/imseqvis/
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-08 06:45:44.000000 imseqvis-0.2.4/imseqvis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-08 06:45:44.000000 imseqvis-0.2.4/imseqvis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10962 2024-05-08 06:45:44.000000 imseqvis-0.2.4/imseqvis/control_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16993 2024-05-08 06:45:44.000000 imseqvis-0.2.4/imseqvis/image_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-08 06:45:44.000000 imseqvis-0.2.4/imseqvis/sequence_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:45:51.379168 imseqvis-0.2.4/imseqvis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-08 06:45:51.000000 imseqvis-0.2.4/imseqvis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 06:45:51.000000 imseqvis-0.2.4/imseqvis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:45:51.000000 imseqvis-0.2.4/imseqvis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-08 06:45:51.000000 imseqvis-0.2.4/imseqvis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 06:45:51.000000 imseqvis-0.2.4/imseqvis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-08 06:45:44.000000 imseqvis-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 06:45:51.379168 imseqvis-0.2.4/setup.cfg
```

### Comparing `imseqvis-0.2.3/LICENSE` & `imseqvis-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imseqvis-0.2.3/PKG-INFO` & `imseqvis-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imseqvis
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Qt-based image sequence visualizer widget
 Author-email: snototter <snototter@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 snototter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,69 +57,75 @@
 ![Screenshot Sequence Viewer](https://github.com/snototter/imseqvis/blob/main/examples/screenshot.jpg?raw=true "SequenceViewer widget")
 
 ### Installation
 It is highly recommended to set up a separate virtual environment with an up-to-date `pip`:
 ```bash
 python3 -m venv venv
 source venv/bin/activate
-python -m pip install -U pip
+python3 -m pip install -U pip
 ```
 
 Then, simply install `imseqvis` via:
 ```bash
-python -m pip install imseqvis
+python3 -m pip install imseqvis
 ```
 
 If you want to try the latest alpha, i.e. the latest `main` branch packaged and
 published to [TestPyPI](https://test.pypi.org/), you can instead install it via:
 ```bash
-python -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple "imseqvis[pyside2]"
+python3 -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple "imseqvis[pyside2]"
 ```
 
 ### Qt Backend
 `imseqvis` requires a [Qt](https://www.qt.io/) backend. In Python, you need to
 either install [PyQt](https://www.riverbankcomputing.com/software/pyqt/download)
 or [PySide](https://doc.qt.io/qtforpython-6/).  
 The default installation **will not install** any of these backends, you have
 to select one on your own.
 
 Optionally, you can install `imseqvis` with a specific backend. Currently,
 `pyqt5`, `pyqt6`, `pyside2`, and `pyside6` are supported:
 ```bash
 # PyQt5
-python -m pip install "imseqvis[pyqt5]"
+python3 -m pip install "imseqvis[pyqt5]"
 
 # OR PyQt6
-python -m pip install "imseqvis[pyqt6]"
+python3 -m pip install "imseqvis[pyqt6]"
 
 # OR PySide2
-python -m pip install "imseqvis[pyside2]"
+python3 -m pip install "imseqvis[pyside2]"
 
 # OR PySide6
-python -m pip install "imseqvis[pyside6]"
+python3 -m pip install "imseqvis[pyside6]"
 ```
 
 ### Usage as Standalone Application
 To quickly visualize all images within a folder or sequence (and nothing else),
 you can use the provided wrappers to start a standalone GUI application:
+```bash
+python3 -m imseqvis path/to/image-folder
+```
+
+Or start the viewer from within your code, either specifically for a folder
+or iterable image sequence (*i.e.* a random access container of NumPy [ndarrays](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html)):
 ```python
 import imseqvis
 # Show all images in the given folder.
-imseqvis.show_folder('path/to/images')
+imseqvis.show_folder('path/to/image-folder')
 
 # Show all images in a random access container. For an exemplary data source
 # refer to `imseqvis.sequence_viewer.ImageSequence`.
 sequence = [...]
 imseqvis.show_sequence(sequence)
 ```
 
 Alternatively, you could simply use the provided `show` functionality:
 ```python
 import imseqvis
-imseqvis.show('path/to/images')
+imseqvis.show('path/to/image-folder')
 
 sequence = [...]
 imseqvis.show(sequence)
 ```
 
 ### Usage as Widget
 To integrate the viewer into your own application, use the `ImageSequenceViewer`
```

### Comparing `imseqvis-0.2.3/README.md` & `imseqvis-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,69 +7,75 @@
 ![Screenshot Sequence Viewer](https://github.com/snototter/imseqvis/blob/main/examples/screenshot.jpg?raw=true "SequenceViewer widget")
 
 ### Installation
 It is highly recommended to set up a separate virtual environment with an up-to-date `pip`:
 ```bash
 python3 -m venv venv
 source venv/bin/activate
-python -m pip install -U pip
+python3 -m pip install -U pip
 ```
 
 Then, simply install `imseqvis` via:
 ```bash
-python -m pip install imseqvis
+python3 -m pip install imseqvis
 ```
 
 If you want to try the latest alpha, i.e. the latest `main` branch packaged and
 published to [TestPyPI](https://test.pypi.org/), you can instead install it via:
 ```bash
-python -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple "imseqvis[pyside2]"
+python3 -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple "imseqvis[pyside2]"
 ```
 
 ### Qt Backend
 `imseqvis` requires a [Qt](https://www.qt.io/) backend. In Python, you need to
 either install [PyQt](https://www.riverbankcomputing.com/software/pyqt/download)
 or [PySide](https://doc.qt.io/qtforpython-6/).  
 The default installation **will not install** any of these backends, you have
 to select one on your own.
 
 Optionally, you can install `imseqvis` with a specific backend. Currently,
 `pyqt5`, `pyqt6`, `pyside2`, and `pyside6` are supported:
 ```bash
 # PyQt5
-python -m pip install "imseqvis[pyqt5]"
+python3 -m pip install "imseqvis[pyqt5]"
 
 # OR PyQt6
-python -m pip install "imseqvis[pyqt6]"
+python3 -m pip install "imseqvis[pyqt6]"
 
 # OR PySide2
-python -m pip install "imseqvis[pyside2]"
+python3 -m pip install "imseqvis[pyside2]"
 
 # OR PySide6
-python -m pip install "imseqvis[pyside6]"
+python3 -m pip install "imseqvis[pyside6]"
 ```
 
 ### Usage as Standalone Application
 To quickly visualize all images within a folder or sequence (and nothing else),
 you can use the provided wrappers to start a standalone GUI application:
+```bash
+python3 -m imseqvis path/to/image-folder
+```
+
+Or start the viewer from within your code, either specifically for a folder
+or iterable image sequence (*i.e.* a random access container of NumPy [ndarrays](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html)):
 ```python
 import imseqvis
 # Show all images in the given folder.
-imseqvis.show_folder('path/to/images')
+imseqvis.show_folder('path/to/image-folder')
 
 # Show all images in a random access container. For an exemplary data source
 # refer to `imseqvis.sequence_viewer.ImageSequence`.
 sequence = [...]
 imseqvis.show_sequence(sequence)
 ```
 
 Alternatively, you could simply use the provided `show` functionality:
 ```python
 import imseqvis
-imseqvis.show('path/to/images')
+imseqvis.show('path/to/image-folder')
 
 sequence = [...]
 imseqvis.show(sequence)
 ```
 
 ### Usage as Widget
 To integrate the viewer into your own application, use the `ImageSequenceViewer`
```

### Comparing `imseqvis-0.2.3/imseqvis/__init__.py` & `imseqvis-0.2.4/imseqvis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Union
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 
 def show_sequence(
         image_sequence,
         window_title: str = "Image Sequence Viewer",
         **kwargs) -> int:
     """
@@ -18,15 +18,15 @@
       window_title: The title of the application window.
       kwargs: Additional arguments passed to the SequenceViewer.
 
     Returns:
       The application's exit code.
     """
     from qtpy.QtWidgets import QApplication, QShortcut
-    from qtpy.QtGui import QKeySequence
+    from qtpy.QtGui import QKeySequence, QGuiApplication
     import sys
     from .sequence_viewer import SequenceViewer
 
     app = QApplication(sys.argv)
     viewer = SequenceViewer(image_sequence=image_sequence, **kwargs)
 
     # Add keyboard shortcuts for zooming.
@@ -46,15 +46,15 @@
     shortcut_jump = QShortcut(QKeySequence('Ctrl+J'), viewer)
     shortcut_jump.activated.connect(viewer.focusOnManualInput)
 
     # Run the application.
     viewer.setWindowTitle(window_title)
     viewer.show()
     viewer.resize(
-        QApplication.desktop().availableGeometry(viewer).size() * 0.7)
+        QGuiApplication.primaryScreen().availableGeometry().size() * 0.7)
     return app.exec()
 
 
 def show_folder(
         folder: Path,
         window_title: str = "Image Folder Viewer",
         **kwargs) -> int:
```

### Comparing `imseqvis-0.2.3/imseqvis/__main__.py` & `imseqvis-0.2.4/imseqvis/__main__.py`

 * *Files identical despite different names*

### Comparing `imseqvis-0.2.3/imseqvis/control_widget.py` & `imseqvis-0.2.4/imseqvis/control_widget.py`

 * *Files identical despite different names*

### Comparing `imseqvis-0.2.3/imseqvis/image_viewer.py` & `imseqvis-0.2.4/imseqvis/image_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,16 +156,16 @@
             new_pos.setX(max(pr.left(), min(pr.right(), new_pos.x())))
             new_pos.setY(max(pr.top(), min(pr.bottom(), new_pos.y())))
         self._prev_drag_pos = new_pos
         # The magic scale factor ensures that dragging is a bit more subtle
         # than scrolling with the mouse wheel. On my gnome-based system, a
         # factor of 6 means that the dragged image follows exactly the
         # mouse pointer...
-        dx and self.scrollRequest.emit(dx * 6, Qt.Horizontal)
-        dy and self.scrollRequest.emit(dy * 6, Qt.Vertical)
+        dx and self.scrollRequest.emit(dx * 6, Qt.Horizontal.value)
+        dy and self.scrollRequest.emit(dy * 6, Qt.Vertical.value)
 
     def mousePressEvent(self, event: QMouseEvent) -> None:
         """Event handler for mouse press events."""
         if event.button() == Qt.RightButton:
             # Viewer can be panned via the right button.
             self._prev_drag_pos = self.mapToParent(event.pos())
             QApplication.setOverrideCursor(Qt.ClosedHandCursor)
@@ -194,16 +194,16 @@
                 dy *= 10
             if dy:
                 self.zoomRequest.emit(dy)
         else:
             if modifiers & Qt.ShiftModifier:
                 dx *= 10
                 dy *= 10
-            dx and self.scrollRequest.emit(dx, Qt.Horizontal)
-            dy and self.scrollRequest.emit(dy, Qt.Vertical)
+            dx and self.scrollRequest.emit(dx, Qt.Horizontal.value)
+            dy and self.scrollRequest.emit(dy, Qt.Vertical.value)
         event.accept()
 
     def dragEnterEvent(self, event):
         """Event handler to support drag&drop of files/folders."""
         if isMimeDataLocalPath(event.mimeData()):
             event.accept()
         else:
@@ -333,17 +333,17 @@
         self._canvas.mouseClickedRight.connect(self.mouseClickedRight)
         self._canvas.imageScaleChanged.connect(self.imageScaleChanged)
         self._canvas.imageScaleChanged.connect(lambda _scale: self.viewChanged.emit())
         self._canvas.pathDropped.connect(self.pathDropped)
 
         self.setWidget(self._canvas)
         self.setWidgetResizable(True)
-        self._scoll_bars = {
-            Qt.Vertical: self.verticalScrollBar(),
-            Qt.Horizontal: self.horizontalScrollBar()
+        self._scroll_bars = {
+            Qt.Vertical.value: self.verticalScrollBar(),
+            Qt.Horizontal.value: self.horizontalScrollBar()
         }
         # Observe the valueChanged signal so we know whether the user dragged
         # a scroll bar or used the keyboard (e.g. arrow keys) to adjust the
         # bar's position.
         self.verticalScrollBar().valueChanged.connect(
             lambda new_value: self.scrollAbsolute(new_value, Qt.Vertical))
         self.horizontalScrollBar().valueChanged.connect(
@@ -375,23 +375,27 @@
         self.scrollRelative(
             delta_widget.y()*120/self.verticalScrollBar().singleStep(),
             Qt.Vertical)
 
     @Slot(int, int)
     def scrollRelative(self, delta, orientation):
         """Slot for scrollRequest signal of image canvas."""
+        if orientation not in self._scroll_bars:
+            return
         steps = -delta / 120
-        bar = self._scoll_bars[orientation]
+        bar = self._scroll_bars[orientation]
         value = bar.value() + bar.singleStep() * steps
         self.scrollAbsolute(value, orientation)
 
     @Slot(int, int)
     def scrollAbsolute(self, value, orientation):
         """Sets the scrollbar to the given value."""
-        bar = self._scoll_bars[orientation]
+        if orientation not in self._scroll_bars:
+            return
+        bar = self._scroll_bars[orientation]
         # Ensure that value is an integer to prevent TypeError within bar.setValue()
         value = int(value)
         if value < bar.minimum():
             value = bar.minimum()
         if value > bar.maximum():
             value = bar.maximum()
         bar.setValue(value)
```

### Comparing `imseqvis-0.2.3/imseqvis/sequence_viewer.py` & `imseqvis-0.2.4/imseqvis/sequence_viewer.py`

 * *Files identical despite different names*

### Comparing `imseqvis-0.2.3/imseqvis.egg-info/PKG-INFO` & `imseqvis-0.2.4/imseqvis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imseqvis
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Qt-based image sequence visualizer widget
 Author-email: snototter <snototter@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 snototter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,69 +57,75 @@
 ![Screenshot Sequence Viewer](https://github.com/snototter/imseqvis/blob/main/examples/screenshot.jpg?raw=true "SequenceViewer widget")
 
 ### Installation
 It is highly recommended to set up a separate virtual environment with an up-to-date `pip`:
 ```bash
 python3 -m venv venv
 source venv/bin/activate
-python -m pip install -U pip
+python3 -m pip install -U pip
 ```
 
 Then, simply install `imseqvis` via:
 ```bash
-python -m pip install imseqvis
+python3 -m pip install imseqvis
 ```
 
 If you want to try the latest alpha, i.e. the latest `main` branch packaged and
 published to [TestPyPI](https://test.pypi.org/), you can instead install it via:
 ```bash
-python -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple "imseqvis[pyside2]"
+python3 -m pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple "imseqvis[pyside2]"
 ```
 
 ### Qt Backend
 `imseqvis` requires a [Qt](https://www.qt.io/) backend. In Python, you need to
 either install [PyQt](https://www.riverbankcomputing.com/software/pyqt/download)
 or [PySide](https://doc.qt.io/qtforpython-6/).  
 The default installation **will not install** any of these backends, you have
 to select one on your own.
 
 Optionally, you can install `imseqvis` with a specific backend. Currently,
 `pyqt5`, `pyqt6`, `pyside2`, and `pyside6` are supported:
 ```bash
 # PyQt5
-python -m pip install "imseqvis[pyqt5]"
+python3 -m pip install "imseqvis[pyqt5]"
 
 # OR PyQt6
-python -m pip install "imseqvis[pyqt6]"
+python3 -m pip install "imseqvis[pyqt6]"
 
 # OR PySide2
-python -m pip install "imseqvis[pyside2]"
+python3 -m pip install "imseqvis[pyside2]"
 
 # OR PySide6
-python -m pip install "imseqvis[pyside6]"
+python3 -m pip install "imseqvis[pyside6]"
 ```
 
 ### Usage as Standalone Application
 To quickly visualize all images within a folder or sequence (and nothing else),
 you can use the provided wrappers to start a standalone GUI application:
+```bash
+python3 -m imseqvis path/to/image-folder
+```
+
+Or start the viewer from within your code, either specifically for a folder
+or iterable image sequence (*i.e.* a random access container of NumPy [ndarrays](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html)):
 ```python
 import imseqvis
 # Show all images in the given folder.
-imseqvis.show_folder('path/to/images')
+imseqvis.show_folder('path/to/image-folder')
 
 # Show all images in a random access container. For an exemplary data source
 # refer to `imseqvis.sequence_viewer.ImageSequence`.
 sequence = [...]
 imseqvis.show_sequence(sequence)
 ```
 
 Alternatively, you could simply use the provided `show` functionality:
 ```python
 import imseqvis
-imseqvis.show('path/to/images')
+imseqvis.show('path/to/image-folder')
 
 sequence = [...]
 imseqvis.show(sequence)
 ```
 
 ### Usage as Widget
 To integrate the viewer into your own application, use the `ImageSequenceViewer`
```

### Comparing `imseqvis-0.2.3/pyproject.toml` & `imseqvis-0.2.4/pyproject.toml`

 * *Files identical despite different names*

