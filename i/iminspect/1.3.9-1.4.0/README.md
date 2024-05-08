# Comparing `tmp/iminspect-1.3.9.tar.gz` & `tmp/iminspect-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iminspect-1.3.9.tar", last modified: Wed Nov 25 13:20:08 2020, max compression
+gzip compressed data, was "iminspect-1.4.0.tar", last modified: Wed May  8 20:22:25 2024, max compression
```

## Comparing `iminspect-1.3.9.tar` & `iminspect-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-25 13:20:08.919321 iminspect-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (116)     8964 2020-11-25 13:20:08.919321 iminspect-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7228 2020-11-25 13:19:58.000000 iminspect-1.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-25 13:20:08.919321 iminspect-1.3.9/iminspect/
--rw-r--r--   0 runner    (1001) docker     (116)      763 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      452 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)    24970 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/imgview.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-25 13:20:08.919321 iminspect-1.3.9/iminspect/iminspect_assets/
--rw-r--r--   0 runner    (1001) docker     (116)     6302 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/iminspect_assets/iminspect.svg
--rw-r--r--   0 runner    (1001) docker     (116)    38882 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/inputs.py
--rw-r--r--   0 runner    (1001) docker     (116)     4942 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/inspection_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    25564 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/inspection_widgets.py
--rw-r--r--   0 runner    (1001) docker     (116)    65043 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-25 13:20:08.919321 iminspect-1.3.9/iminspect/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2518 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2020-11-25 13:19:58.000000 iminspect-1.3.9/iminspect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-25 13:20:08.919321 iminspect-1.3.9/iminspect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8964 2020-11-25 13:20:08.000000 iminspect-1.3.9/iminspect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      476 2020-11-25 13:20:08.000000 iminspect-1.3.9/iminspect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-25 13:20:08.000000 iminspect-1.3.9/iminspect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       39 2020-11-25 13:20:08.000000 iminspect-1.3.9/iminspect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2020-11-25 13:20:08.000000 iminspect-1.3.9/iminspect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-11-25 13:20:08.919321 iminspect-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1350 2020-11-25 13:19:58.000000 iminspect-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:22:25.213922 iminspect-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 20:22:18.000000 iminspect-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10157 2024-05-08 20:22:25.213922 iminspect-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-05-08 20:22:18.000000 iminspect-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:22:25.209922 iminspect-1.4.0/iminspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-08 20:22:18.000000 iminspect-1.4.0/iminspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-08 20:22:18.000000 iminspect-1.4.0/iminspect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25704 2024-05-08 20:22:18.000000 iminspect-1.4.0/iminspect/imgview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41934 2024-05-08 20:22:18.000000 iminspect-1.4.0/iminspect/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-08 20:22:18.000000 iminspect-1.4.0/iminspect/inspection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25453 2024-05-08 20:22:18.000000 iminspect-1.4.0/iminspect/inspection_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65405 2024-05-08 20:22:18.000000 iminspect-1.4.0/iminspect/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:22:25.213922 iminspect-1.4.0/iminspect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10157 2024-05-08 20:22:25.000000 iminspect-1.4.0/iminspect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-08 20:22:25.000000 iminspect-1.4.0/iminspect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:22:25.000000 iminspect-1.4.0/iminspect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 20:22:25.000000 iminspect-1.4.0/iminspect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 20:22:25.000000 iminspect-1.4.0/iminspect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-08 20:22:18.000000 iminspect-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:22:25.213922 iminspect-1.4.0/setup.cfg
```

### Comparing `iminspect-1.3.9/PKG-INFO` & `iminspect-1.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,174 +1,183 @@
-Metadata-Version: 2.1
-Name: iminspect
-Version: 1.3.9
-Summary: Qt-based GUI to visualize image-like data.
-Home-page: https://github.com/snototter/iminspect
-Author: snototter
-Author-email: muspellr@gmail.com
-License: UNKNOWN
-Description: # iminspect
-        [![View on PyPI](https://img.shields.io/pypi/v/iminspect.svg)](https://pypi.org/project/iminspect)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/iminspect.svg)](https://pypi.org/project/iminspect)
-        [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/snototter/iminspect/blob/master/LICENSE?raw=true)
-        
-        A python utility package for image/matrix visualization.
-        
-        Moving from MATLAB to python I was missing fast and easy-to-use inspection tools for image data.
-        Thus, `iminspect` provides a collection of visualization/inspection capabilities along with a simplistic Qt-based GUI.
-        The goal is to enable quick and easy visualization/analysis of:
-        * color images,
-        * monochrome images (i.e. any type of 2D matrices),
-        * label images (i.e. categorical data),
-        * binary masks,
-        * depth maps, and
-        * optical flow data.
-        
-        
-        ## Example usage (within a Python script):
-        ```python
-        from iminspect.inspector import inspect, DataType
-        import numpy as np
-        
-        # Show random noise image:
-        inspect(np.random.rand(4096,4096) - 0.5)
-        
-        # Show as class labels:
-        inspect((np.random.rand(16,16) * 1e2 % 5).astype(np.int16), data_type=DataType.CATEGORICAL)
-        
-        # Show two images next to each other, e.g. useful to analyse RGB and
-        # corresponding depth, or RGB and corresponding optical flow:
-        inspect((data_color, data_depth))
-        # or specify the data types manually:
-        inspect((rgb, flow), data_type=(DataType.COLOR, DataType.FLOW)))
-        ```
-        
-        Example: visualizing categorical data (i.e. labels)<br/>
-        ![Screenshot categorical data](https://github.com/snototter/iminspect/blob/master/screenshots/categorical.jpg?raw=true "iminspect GUI")
-        
-        Example: visualizing a mask image<br/>
-        ![Screenshot binary data](https://github.com/snototter/iminspect/blob/master/screenshots/mask.jpg?raw=true "iminspect GUI")
-        
-        Example: visualizing RGB image and optical flow<br/>
-        ![Screenshot optical flow](https://github.com/snototter/iminspect/blob/master/screenshots/rgb-flow.jpg?raw=true "iminspect GUI")
-        
-        
-        ## Example usage (standalone):
-        The `iminspect` package can be run as a standalone application, so you could create a launcher, add it to your system's binary/executable path, etc.
-        1. Set up a virtual environment (in this example, I'll use a separate `util-iminspect` folder to install the `iminspect` package):
-            ```bash
-            cd desired/installation/path
-            python3 -m venv util-iminspect
-            source util-iminspect/bin/activate
-            pip install -U pip
-            pip install iminspect
-            ```
-        2. Run `iminspect` standalone via:
-            ```bash
-            desired/installation/path/util-iminspect/bin/python3 -m iminspect
-            ```
-        
-        
-        ## Custom input widgets:
-        The `iminspect.inputs` subpackage provides common user input widgets, e.g. to select a rectangular region-of-interest, enter an IP address, etc. See the `examples/inputs_demo.py` application on how to use it. Exemplary screenshot:<br/>
-        ![Screenshot inputs demo](https://github.com/snototter/iminspect/blob/master/screenshots/input-widgets.jpg?raw=true "Common input widgets")
-        
-        
-        ## Dependencies
-        * `numpy`, for matrix manipulation
-        * `PyQt5`, for the graphical user interface - if there's a `PyQt5`-related install error, you need to upgrade `pip` via `pip install --upgrade pip`.
-        * `qimage2ndarray`, to convert numpy ndarrays to Qt images
-        * `vito`, a lightweight vision tool package
-        
-        
-        ## UI Documentation
-        * To inspect a data point/pixel, just move the mouse above it.
-        * Zooming:
-          * `Ctrl+Wheel` to zoom in/out.
-          * `Ctrl+Shift+Wheel` to speed up zooming.
-          * `Ctrl+{+|-}` to zoom in/out.
-          * `Ctrl+Shift+{+|-}` to zoom in/out faster.
-          * `Ctrl+F` to zoom such that the image fills the available canvas.
-          * `Ctrl+1` to scale to original size.
-        * Scrolling:
-          * `Wheel` scrolls up/down.
-          * `Shift+Wheel` speeds up scrolling.
-          * `Ctrl+{Up|Down|Left|Right}` to scroll using keyboard.
-          * `Ctrl+Shift+{Up|Down|Left|Right}` to scroll faster/further. 
-          * Press and move left/right button to drag the image if zoomed in.
-        * Keyboard shortcuts:
-          * `Ctrl+Q` and `Ctrl+W` close the inspection GUI.
-          * `Ctrl+O` shows a dialog to open another file.
-          * `Ctrl+S` shows a dialog to save either the (raw) input or its current visualization.
-          * `Ctrl+T` toggle tool tip display when moving the mouse over the data.
-          * `Ctrl+R` reloads the current data such that the user can select a different visualization/data type.
-        
-        
-        ## Changelog
-        * `1.3.9`
-          * Handle non-finite values: Info/caution message shows in the data summary label, non-finite values are ignored in computing the data statistics.
-          * Option (Shortcut and toolbar button) to reload the currently inspected data with a different visualization/data type.
-          * Added application icon.
-        * `1.3.8`
-          * Added support for opening files via dropping them from external image viewer applications. Tested with common Linux viewers (`eog` and `geeqie`).
-        * `1.3.7`
-          * Support opening files by dropping them into the viewer.
-          * Added `__main__` to run module (open the inspector) via `python -m iminspect`
-        * `1.3.6`
-          * Inspector handles 1D inputs.
-          * Minor tweaks to the `inputs` subpackage.
-        * `1.3.5`
-          * Bug fix - rounding issues during initialization of custom slider widgets (which use floats).
-        * `1.3.4`
-          * Minor tweaks to the `inputs` subpackage.
-        * `1.3.3`
-          * Add functionality to open the inspector without data (in case you want to load from disk).
-        * `1.3.2`
-          * Added color picker widget to `inputs`.
-          * Support multiple file selection dialog.
-        * `1.3.1`
-          * Minor extensions to user `inputs` subpackage.
-        * `1.3.0`
-          * Added a range slider to adjust visualization limits on the fly.
-          * Image viewer (canvas) now supports dragging.
-          * Support toggling the tool tip display.
-          * Support adding custom labels for categorical data.
-          * Fix running `inputs.py` as standalone demo (relative import confusion).
-        * `1.2.0`
-          * Support multi-channel input data (with more than 4 channels).
-          * Support analysing multiple images at once, e.g. color images and corresponding optical flow.
-          * Major refactoring under the hood.
-        * `1.1.0`
-          * Support saving visualization and raw input data to disk.
-          * Added shorthand wrapper to `inspect()` call.
-          * UI improvements/layout changes.
-          * Fixed typos such as `DataType.CATEGORICAL`.
-          * Added support for partially transparent images (i.e. RGBA).
-        * `1.0.0`
-          * Major code refactoring: use data type enum instead of various flags (this breaks previous inspect() calls).
-          * Optical flow support.
-          * Load another file from disk (via `Ctrl+O`).
-          * Usability improvements, e.g. restore display settings when opening similar data type, handle file loading errors, etc.
-        * `0.2.0`
-          * Major refactoring: moved image utils and colorizing code to separate [vito](https://github.com/snototter/vito) package.
-          * Usability improvements: keyboard shortcuts for zooming, scaling and scrolling.
-        * `0.1.2`
-          * Added tests for non-GUI functionality.
-          * Integrate github runners for test/build/deploy.
-          * Fix definition for colormap gray.
-        * `0.1.1`
-          * Additional features:
-            * ImageCanvas supports ROI selection (useful for custom input widgets).
-          * Refactoring:
-            * Clean up imports.
-            * Make pylint/flake8 happier.
-          * Fixes:
-            * Adjust scrollbars when zooming multiple linked ImageCanvas.
-        * `0.1.0` - Initial public release.
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+# iminspect
+[![View on PyPI](https://img.shields.io/pypi/v/iminspect.svg)](https://pypi.org/project/iminspect)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/iminspect.svg)](https://pypi.org/project/iminspect)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/snototter/iminspect/blob/master/LICENSE?raw=true)
+
+A python utility package for image/matrix visualization.
+
+![Application logo](https://github.com/snototter/iminspect/blob/master/screenshots/logo.png?raw=true "Application logo")
+
+Moving from MATLAB to python I was missing fast and easy-to-use inspection tools for image data.
+Thus, `iminspect` provides a collection of visualization/inspection capabilities along with a simplistic Qt-based GUI.
+The goal is to enable quick and easy visualization/analysis of:
+* color images,
+* monochrome images (i.e. any type of 2D matrices),
+* label images (i.e. categorical data),
+* binary masks,
+* depth maps, and
+* optical flow data.
+
+
+## Qt Backend
+`iminspect` requires a [Qt](https://www.qt.io/) backend. In Python, you need to
+either install [PyQt](https://www.riverbankcomputing.com/software/pyqt/download)
+or [PySide](https://doc.qt.io/qtforpython-6/).  
+The default installation **will not install** any of these backends, you have
+to select one on your own.
+
+Optionally, you can install `iminspect` with a specific backend. Currently,
+`pyqt5`, `pyqt6`, `pyside2`, and `pyside6` are supported:
+```bash
+# PyQt5
+python3 -m pip install "iminspect[pyqt5]"
+
+# OR PyQt6
+python3 -m pip install "iminspect[pyqt6]"
+
+# OR PySide2
+python3 -m pip install "iminspect[pyside2]"
+
+# OR PySide6
+python3 -m pip install "iminspect[pyside6]"
+```
+
+## Example usage (within a Python script):
+```python
+from iminspect.inspector import inspect, DataType
+import numpy as np
+
+# Show random noise image:
+inspect(np.random.rand(4096,4096) - 0.5)
+
+# Show as class labels:
+inspect((np.random.rand(16,16) * 1e2 % 5).astype(np.int16), data_type=DataType.CATEGORICAL)
+
+# Show two images next to each other, e.g. useful to analyse RGB and
+# corresponding depth, or RGB and corresponding optical flow:
+inspect((data_color, data_depth))
+# or specify the data types manually:
+inspect((rgb, flow), data_type=(DataType.COLOR, DataType.FLOW)))
+```
+
+Example: visualizing categorical data (i.e. labels)<br/>
+![Screenshot categorical data](https://github.com/snototter/iminspect/blob/master/screenshots/categorical.jpg?raw=true "iminspect GUI")
+
+Example: visualizing a mask image<br/>
+![Screenshot binary data](https://github.com/snototter/iminspect/blob/master/screenshots/mask.jpg?raw=true "iminspect GUI")
+
+Example: visualizing RGB image and optical flow<br/>
+![Screenshot optical flow](https://github.com/snototter/iminspect/blob/master/screenshots/rgb-flow.jpg?raw=true "iminspect GUI")
+
+
+## Example usage (standalone):
+The `iminspect` package can be run as a standalone application, so you could create a launcher, add it to your system's binary/executable path, etc.
+You can either do this manually via the following steps or try the `standalone/install-...` scripts.
+
+1. Set up a virtual environment (in this example, I'll use a separate `util-iminspect` folder to install the `iminspect` package):
+    ```bash
+    cd desired/installation/path
+    python3 -m venv util-iminspect
+    source util-iminspect/bin/activate
+    pip install -U pip
+    pip install iminspect
+    ```
+2. Run `iminspect` standalone via:
+    ```bash
+    desired/installation/path/util-iminspect/bin/python3 -m iminspect
+    ```
+
+
+## Custom input widgets:
+The `iminspect.inputs` subpackage provides common user input widgets, e.g. to select a rectangular region-of-interest, enter an IP address, etc. See the `examples/inputs_demo.py` application on how to use it. Exemplary screenshot:<br/>
+![Screenshot inputs demo](https://github.com/snototter/iminspect/blob/master/screenshots/input-widgets.jpg?raw=true "Common input widgets")
+
+
+## UI Documentation
+* To inspect a data point/pixel, just move the mouse above it.
+* Zooming:
+  * `Ctrl+Wheel` to zoom in/out.
+  * `Ctrl+Shift+Wheel` to speed up zooming.
+  * `Ctrl+{+|-}` to zoom in/out.
+  * `Ctrl+Shift+{+|-}` to zoom in/out faster.
+  * `Ctrl+F` to zoom such that the image fills the available canvas.
+  * `Ctrl+1` to scale to original size.
+* Scrolling:
+  * `Wheel` scrolls up/down.
+  * `Shift+Wheel` speeds up scrolling.
+  * `Ctrl+{Up|Down|Left|Right}` to scroll using keyboard.
+  * `Ctrl+Shift+{Up|Down|Left|Right}` to scroll faster/further. 
+  * Press and move left/right button to drag the image if zoomed in.
+* Keyboard shortcuts:
+  * `Ctrl+Q` and `Ctrl+W` close the inspection GUI.
+  * `Ctrl+O` shows a dialog to open another file.
+  * `Ctrl+S` shows a dialog to save either the (raw) input or its current visualization.
+  * `Ctrl+T` toggle tool tip display when moving the mouse over the data.
+  * `Ctrl+R` reloads the current data such that the user can select a different visualization/data type.
+
+
+## Changelog
+* `1.3.10`
+  * Added utility scripts for [standalone installation](https://github.com/snototter/iminspect/blob/master/standalone/install-standalone-ubuntu-18.04.sh) (on Ubuntu).
+  * Clarified standalone usage example.
+  * Minor tweaks to the `inputs` subpackage.
+* `1.3.9`
+  * Handle non-finite values: Info/caution message shows in the data summary label, non-finite values are ignored in computing the data statistics.
+  * Option (Shortcut and toolbar button) to reload the currently inspected data with a different visualization/data type.
+  * Added application icon.
+* `1.3.8`
+  * Added support for opening files via dropping them from external image viewer applications. Tested with common Linux viewers (`eog` and `geeqie`).
+* `1.3.7`
+  * Support opening files by dropping them into the viewer.
+  * Added `__main__` to run module (open the inspector) via `python -m iminspect`
+* `1.3.6`
+  * Inspector handles 1D inputs.
+  * Minor tweaks to the `inputs` subpackage.
+* `1.3.5`
+  * Bug fix - rounding issues during initialization of custom slider widgets (which use floats).
+* `1.3.4`
+  * Minor tweaks to the `inputs` subpackage.
+* `1.3.3`
+  * Add functionality to open the inspector without data (in case you want to load from disk).
+* `1.3.2`
+  * Added color picker widget to `inputs`.
+  * Support multiple file selection dialog.
+* `1.3.1`
+  * Minor extensions to user `inputs` subpackage.
+* `1.3.0`
+  * Added a range slider to adjust visualization limits on the fly.
+  * Image viewer (canvas) now supports dragging.
+  * Support toggling the tool tip display.
+  * Support adding custom labels for categorical data.
+  * Fix running `inputs.py` as standalone demo (relative import confusion).
+* `1.2.0`
+  * Support multi-channel input data (with more than 4 channels).
+  * Support analysing multiple images at once, e.g. color images and corresponding optical flow.
+  * Major refactoring under the hood.
+* `1.1.0`
+  * Support saving visualization and raw input data to disk.
+  * Added shorthand wrapper to `inspect()` call.
+  * UI improvements/layout changes.
+  * Fixed typos such as `DataType.CATEGORICAL`.
+  * Added support for partially transparent images (i.e. RGBA).
+* `1.0.0`
+  * Major code refactoring: use data type enum instead of various flags (this breaks previous inspect() calls).
+  * Optical flow support.
+  * Load another file from disk (via `Ctrl+O`).
+  * Usability improvements, e.g. restore display settings when opening similar data type, handle file loading errors, etc.
+* `0.2.0`
+  * Major refactoring: moved image utils and colorizing code to separate [vito](https://github.com/snototter/vito) package.
+  * Usability improvements: keyboard shortcuts for zooming, scaling and scrolling.
+* `0.1.2`
+  * Added tests for non-GUI functionality.
+  * Integrate github runners for test/build/deploy.
+  * Fix definition for colormap gray.
+* `0.1.1`
+  * Additional features:
+    * ImageCanvas supports ROI selection (useful for custom input widgets).
+  * Refactoring:
+    * Clean up imports.
+    * Make pylint/flake8 happier.
+  * Fixes:
+    * Adjust scrollbars when zooming multiple linked ImageCanvas.
+* `0.1.0` - Initial public release.
+
```

### Comparing `iminspect-1.3.9/README.md` & `iminspect-1.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,97 @@
+Metadata-Version: 2.1
+Name: iminspect
+Version: 1.4.0
+Summary: Qt-based GUI to visualize image-like data
+Author-email: snototter <snototter@users.noreply.github.com>
+License: MIT License
+        
+        Copyright (c) 2019 snototter
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://github.com/snototter/iminspect
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: qimage2ndarray
+Requires-Dist: qtpy
+Requires-Dist: vito
+Provides-Extra: pyqt5
+Requires-Dist: PyQt5; extra == "pyqt5"
+Provides-Extra: pyqt6
+Requires-Dist: PyQt6; extra == "pyqt6"
+Provides-Extra: pyside2
+Requires-Dist: PySide2; extra == "pyside2"
+Provides-Extra: pyside6
+Requires-Dist: PySide6; extra == "pyside6"
+
 # iminspect
 [![View on PyPI](https://img.shields.io/pypi/v/iminspect.svg)](https://pypi.org/project/iminspect)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/iminspect.svg)](https://pypi.org/project/iminspect)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/snototter/iminspect/blob/master/LICENSE?raw=true)
 
 A python utility package for image/matrix visualization.
 
+![Application logo](https://github.com/snototter/iminspect/blob/master/screenshots/logo.png?raw=true "Application logo")
+
 Moving from MATLAB to python I was missing fast and easy-to-use inspection tools for image data.
 Thus, `iminspect` provides a collection of visualization/inspection capabilities along with a simplistic Qt-based GUI.
 The goal is to enable quick and easy visualization/analysis of:
 * color images,
 * monochrome images (i.e. any type of 2D matrices),
 * label images (i.e. categorical data),
 * binary masks,
 * depth maps, and
 * optical flow data.
 
 
+## Qt Backend
+`iminspect` requires a [Qt](https://www.qt.io/) backend. In Python, you need to
+either install [PyQt](https://www.riverbankcomputing.com/software/pyqt/download)
+or [PySide](https://doc.qt.io/qtforpython-6/).  
+The default installation **will not install** any of these backends, you have
+to select one on your own.
+
+Optionally, you can install `iminspect` with a specific backend. Currently,
+`pyqt5`, `pyqt6`, `pyside2`, and `pyside6` are supported:
+```bash
+# PyQt5
+python3 -m pip install "iminspect[pyqt5]"
+
+# OR PyQt6
+python3 -m pip install "iminspect[pyqt6]"
+
+# OR PySide2
+python3 -m pip install "iminspect[pyside2]"
+
+# OR PySide6
+python3 -m pip install "iminspect[pyside6]"
+```
+
 ## Example usage (within a Python script):
 ```python
 from iminspect.inspector import inspect, DataType
 import numpy as np
 
 # Show random noise image:
 inspect(np.random.rand(4096,4096) - 0.5)
@@ -42,14 +114,16 @@
 
 Example: visualizing RGB image and optical flow<br/>
 ![Screenshot optical flow](https://github.com/snototter/iminspect/blob/master/screenshots/rgb-flow.jpg?raw=true "iminspect GUI")
 
 
 ## Example usage (standalone):
 The `iminspect` package can be run as a standalone application, so you could create a launcher, add it to your system's binary/executable path, etc.
+You can either do this manually via the following steps or try the `standalone/install-...` scripts.
+
 1. Set up a virtual environment (in this example, I'll use a separate `util-iminspect` folder to install the `iminspect` package):
     ```bash
     cd desired/installation/path
     python3 -m venv util-iminspect
     source util-iminspect/bin/activate
     pip install -U pip
     pip install iminspect
@@ -61,21 +135,14 @@
 
 
 ## Custom input widgets:
 The `iminspect.inputs` subpackage provides common user input widgets, e.g. to select a rectangular region-of-interest, enter an IP address, etc. See the `examples/inputs_demo.py` application on how to use it. Exemplary screenshot:<br/>
 ![Screenshot inputs demo](https://github.com/snototter/iminspect/blob/master/screenshots/input-widgets.jpg?raw=true "Common input widgets")
 
 
-## Dependencies
-* `numpy`, for matrix manipulation
-* `PyQt5`, for the graphical user interface - if there's a `PyQt5`-related install error, you need to upgrade `pip` via `pip install --upgrade pip`.
-* `qimage2ndarray`, to convert numpy ndarrays to Qt images
-* `vito`, a lightweight vision tool package
-
-
 ## UI Documentation
 * To inspect a data point/pixel, just move the mouse above it.
 * Zooming:
   * `Ctrl+Wheel` to zoom in/out.
   * `Ctrl+Shift+Wheel` to speed up zooming.
   * `Ctrl+{+|-}` to zoom in/out.
   * `Ctrl+Shift+{+|-}` to zoom in/out faster.
@@ -92,14 +159,18 @@
   * `Ctrl+O` shows a dialog to open another file.
   * `Ctrl+S` shows a dialog to save either the (raw) input or its current visualization.
   * `Ctrl+T` toggle tool tip display when moving the mouse over the data.
   * `Ctrl+R` reloads the current data such that the user can select a different visualization/data type.
 
 
 ## Changelog
+* `1.3.10`
+  * Added utility scripts for [standalone installation](https://github.com/snototter/iminspect/blob/master/standalone/install-standalone-ubuntu-18.04.sh) (on Ubuntu).
+  * Clarified standalone usage example.
+  * Minor tweaks to the `inputs` subpackage.
 * `1.3.9`
   * Handle non-finite values: Info/caution message shows in the data summary label, non-finite values are ignored in computing the data statistics.
   * Option (Shortcut and toolbar button) to reload the currently inspected data with a different visualization/data type.
   * Added application icon.
 * `1.3.8`
   * Added support for opening files via dropping them from external image viewer applications. Tested with common Linux viewers (`eog` and `geeqie`).
 * `1.3.7`
```

### Comparing `iminspect-1.3.9/iminspect/__init__.py` & `iminspect-1.4.0/iminspect/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #!/usr/bin/env python
 # coding=utf-8
 """
 Python Qt5 utils to easily visualize image data for faster development.
 """
 
-__all__ = ['imgview', 'inputs', 'inspection_utils', 'inspection_widgets', 'inspector']
-__author__ = 'snototter'
 
-# Load version
-import os
-with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'version.py')) as vf:
-    exec(vf.read())
+__version__ = '1.4.0'
+
+
+__all__ = ['imgview', 'inputs', 'inspection_utils', 'inspection_widgets', 'inspector']
 
 
 def show(data, **kwargs):
     """Just a "symlink" to iminspector.inspector.inspect() for convenience/out
     of laziness. Refer to inspector.inspect() for the actual documentation.
 
     How to save a few characters using this wrapper:
```

### Comparing `iminspect-1.3.9/iminspect/imgview.py` & `iminspect-1.4.0/iminspect/imgview.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # coding=utf-8
 """
 A Qt-based image viewer which supports zooming and scrolling.
 """
 
 import os
 from enum import Enum
-from PyQt5.QtWidgets import QMainWindow, QApplication, QWidget, QScrollArea,\
+from qtpy.QtWidgets import QMainWindow, QApplication, QWidget, QScrollArea,\
     QHBoxLayout, QVBoxLayout, QDialog
-from PyQt5.QtCore import pyqtSignal, pyqtSlot, Qt, QSize, QPointF, QPoint, QRect
-from PyQt5.QtGui import QPainter, QPixmap, QCursor, QBrush, QColor, QPen, QPalette
+from qtpy.QtCore import Signal, Slot, Qt, QSize, QPointF, QPoint, QRect
+from qtpy.QtGui import QPainter, QPixmap, QCursor, QBrush, QColor, QPen, QPalette
 
 from . import inspection_utils
 
 
 class ImageLabel(QWidget):
     """Widget to display an image, always resized to the widgets dimensions."""
     def __init__(self, pixmap=None, parent=None):
@@ -78,25 +78,31 @@
     raise ValueError('Unsupported QMimeData for dropped file!')
 
 
 
 class ImageCanvas(QWidget):
     """Widget to display a zoomable/scrollable image."""
     # User wants to zoom in/out by amount (mouse wheel delta)
-    zoomRequest = pyqtSignal(int)
-    # User wants to scroll (Qt.Horizontal or Qt.Vertical, mouse wheel delta)
-    scrollRequest = pyqtSignal(int, int)
+    zoomRequest = Signal(int)
+    # User wants to scroll (mouse wheel delta, ORIENTATION_HORIZONTAL or
+    # ORIENTATION_VERTICAL).
+    scrollRequest = Signal(int, int)
     # Mouse moved to this pixel position
-    mouseMoved = pyqtSignal(QPointF)
+    mouseMoved = Signal(QPointF)
     # User selected a rectangle (ImageCanvas must be created with rect_selectable=True)
-    rectSelected = pyqtSignal(tuple)
+    rectSelected = Signal(tuple)
     # Scaling factor of displayed image changed
-    imgScaleChanged = pyqtSignal(float)
+    imgScaleChanged = Signal(float)
     # File has been dropped onto canvas
-    filenameDropped = pyqtSignal(str)
+    filenameDropped = Signal(str)
+
+    # Qt5/6 compatibility - can't use the Qt.Orientation flag as dictionary
+    # keys in Qt6, and Qt5 doesn't provide the ".value" attribute.
+    ORIENTATION_HORIZONTAL = 1
+    ORIENTATION_VERTICAL = 2
 
     def __init__(
             self, parent=None, rect_selectable=False,
             overlay_rect_color=QColor(200, 0, 0, 255), overlay_rect_fill_opacity=0,
             overlay_brush_color=QColor(128, 128, 200, 180)):
         super(ImageCanvas, self).__init__(parent)
         self._scale = 1.0
@@ -160,16 +166,16 @@
             pr = self.parent().rect()
             new_pos.setX(max(pr.left(), min(pr.right(), new_pos.x())))
             new_pos.setY(max(pr.top(), min(pr.bottom(), new_pos.y())))
         self._prev_drag_pos = new_pos
         # The magic scale factor ensures that dragging is a bit more subtle
         # than scrolling with the mouse wheel. On my system, a factor of 6
         # means that the dragged image follows exactly the mouse pointer...
-        dx and self.scrollRequest.emit(dx * 6, Qt.Horizontal)
-        dy and self.scrollRequest.emit(dy * 6, Qt.Vertical)
+        dx and self.scrollRequest.emit(dx * 6, ImageCanvas.ORIENTATION_HORIZONTAL)
+        dy and self.scrollRequest.emit(dy * 6, ImageCanvas.ORIENTATION_VERTICAL)
 
     def mousePressEvent(self, event):
         if Qt.LeftButton == event.button():
             # If this viewer can draw a rectangle => left button starts drawing
             # the rect. Otherwise, left button starts dragging:
             if self._is_rect_selectable:
                 self._prev_pos = self.transformPos(event.pos())
@@ -323,38 +329,38 @@
                 dy *= 10
             if dy:
                 self.zoomRequest.emit(dy)
         else:
             if modifiers & Qt.ShiftModifier:
                 dx *= 10
                 dy *= 10
-            dx and self.scrollRequest.emit(dx, Qt.Horizontal)
-            dy and self.scrollRequest.emit(dy, Qt.Vertical)
+            dx and self.scrollRequest.emit(dx, ImageCanvas.ORIENTATION_HORIZONTAL)
+            dy and self.scrollRequest.emit(dy, ImageCanvas.ORIENTATION_VERTICAL)
         event.accept()
 
 
 class ImageViewerType(Enum):
     """Enumeration for image viewers."""
     VIEW_ONLY = 1       # Just show the image
     RECT_SELECTION = 2  # Let user select a rectangle
 
 
 class ImageViewer(QScrollArea):
     """A widget to view image data (given as numpy ndarray)."""
 
     # Mouse moved to this pixel position
-    mouseMoved = pyqtSignal(QPointF)
+    mouseMoved = Signal(QPointF)
     # User selected a rectangle (ImageCanvas must be created with rect_selectable=True)
-    rectSelected = pyqtSignal(tuple)
+    rectSelected = Signal(tuple)
     # Scaling factor of displayed image changed
-    imgScaleChanged = pyqtSignal(float)
+    imgScaleChanged = Signal(float)
     # The view changed due to the user scrolling or zooming
-    viewChanged = pyqtSignal()
+    viewChanged = Signal()
     # File has been dropped onto canvas
-    filenameDropped = pyqtSignal(str)
+    filenameDropped = Signal(str)
 
     def __init__(self, parent=None, viewer_type=ImageViewerType.VIEW_ONLY, **kwargs):
         super(ImageViewer, self).__init__(parent)
         self._img_np = None
         self._img_scale = 1.0
         self._min_img_scale = None
         self._canvas = None
@@ -371,15 +377,15 @@
         return self._canvas.pixmap()
 
     def pixelFromGlobal(self, global_pos):
         """Map a global position, e.g. QCursor.pos(), to the corresponding
         pixel location."""
         return self._canvas.pixelAtWidgetPos(self._canvas.mapFromGlobal(global_pos))
 
-    @pyqtSlot(tuple)
+    @Slot(tuple)
     def _emitRectSelected(self, rect):
         self.rectSelected.emit(rect)
 
     def setRectangle(self, rect):
         self._canvas.setRectangle(rect)
 
     def _prepareLayout(self, **kwargs):
@@ -395,46 +401,46 @@
         self._canvas.mouseMoved.connect(self.mouseMoved)
         self._canvas.imgScaleChanged.connect(self.imgScaleChanged)
         self._canvas.imgScaleChanged.connect(lambda _: self.viewChanged.emit())
         self._canvas.filenameDropped.connect(self.filenameDropped)
 
         self.setWidget(self._canvas)
         self.setWidgetResizable(True)
-        self._scoll_bars = {
-            Qt.Vertical: self.verticalScrollBar(),
-            Qt.Horizontal: self.horizontalScrollBar()
+        self._scroll_bars = {
+            ImageCanvas.ORIENTATION_HORIZONTAL: self.horizontalScrollBar(),
+            ImageCanvas.ORIENTATION_VERTICAL: self.verticalScrollBar()
         }
         # Observe the valueChanged signal so we know whether the user dragged
         # a scroll bar or used the keyboard (e.g. arrow keys) to adjust the
         # bar's position.
         self.verticalScrollBar().valueChanged.connect(
-            lambda new_value: self.scrollAbsolute(new_value, Qt.Vertical, notify_linked=True))
+            lambda new_value: self.scrollAbsolute(new_value, ImageCanvas.ORIENTATION_VERTICAL, notify_linked=True))
         self.horizontalScrollBar().valueChanged.connect(
-            lambda new_value: self.scrollAbsolute(new_value, Qt.Horizontal, notify_linked=True))
+            lambda new_value: self.scrollAbsolute(new_value, ImageCanvas.ORIENTATION_HORIZONTAL, notify_linked=True))
 
     def currentDisplaySettings(self):
         """Query the current zoom/scroll settings, so you can restore them.
         For example, if you want to show the same region of interest for another
         image.
         """
         settings = {'zoom': self._img_scale}
-        for orientation in [Qt.Horizontal, Qt.Vertical]:
-            bar = self._scoll_bars[orientation]
+        for orientation in [ImageCanvas.ORIENTATION_HORIZONTAL, ImageCanvas.ORIENTATION_VERTICAL]:
+            bar = self._scroll_bars[orientation]
             settings[orientation] = (bar.minimum(), bar.value(), bar.maximum())
         return settings
 
     def restoreDisplaySettings(self, settings):
         self._img_scale = settings['zoom']
         self.paintCanvas()
         # Potential issue: scrollbars may only appear during repainting the
         # widget. Then, setting their value won't work. Best and least
         # complicated way I found so far: force Qt to process the event loop
         # after adjusting the bar's range (and before setting the new value).
-        for orientation in [Qt.Horizontal, Qt.Vertical]:
-            bar = self._scoll_bars[orientation]
+        for orientation in [ImageCanvas.ORIENTATION_HORIZONTAL, ImageCanvas.ORIENTATION_VERTICAL]:
+            bar = self._scroll_bars[orientation]
             bmin, bval, bmax = settings[orientation]
             if bval != 0:
                 bar.setMinimum(bmin)
                 bar.setMaximum(bmax)
                 QApplication.instance().processEvents()
                 bar.setValue(bval)
 
@@ -454,15 +460,15 @@
         if others:
             self._linked_viewers.extend(others)
 
     def clearLinkedViewers(self):
         """Clears the list of linked viewers."""
         self._linked_viewers = list()
 
-    @pyqtSlot(int)
+    @Slot(int)
     def zoom(self, delta, notify_linked=True):
         """Scale the displayed image. Zoom in if delta > 0.
         Usually to be called with mouse wheel delta values, thus
         the actual zoom steps are computed as delta/120.
         """
         # Currently, we adjust the scroll bar position such that the cursor stays
         # at the same pixel. This works well if both scroll bars are visible, otherwise,
@@ -478,31 +484,38 @@
             # Adjust the scroll bar positions to keep cursor at the same pixel
             px_pos_curr = self._canvas.pixelAtWidgetPos(
                 self._canvas.mapFromGlobal(cursor_pos))
             delta_widget = self._canvas.pixelToWidgetPos(px_pos_curr) \
                 - self._canvas.pixelToWidgetPos(px_pos_prev)
             self.scrollRelative(
                 delta_widget.x()*120/self.horizontalScrollBar().singleStep(),
-                Qt.Horizontal, notify_linked=True)
+                ImageCanvas.ORIENTATION_HORIZONTAL, notify_linked=True)
             self.scrollRelative(
                 delta_widget.y()*120/self.verticalScrollBar().singleStep(),
-                Qt.Vertical, notify_linked=True)
+                ImageCanvas.ORIENTATION_VERTICAL, notify_linked=True)
 
-    @pyqtSlot(int, int)
+    @Slot(int, int)
     def scrollRelative(self, delta, orientation, notify_linked=True):
         """Slot for scrollRequest signal of image canvas."""
+        if orientation not in self._scroll_bars:
+            return
         steps = -delta / 120
-        bar = self._scoll_bars[orientation]
+        bar = self._scroll_bars[orientation]
         value = bar.value() + bar.singleStep() * steps
         self.scrollAbsolute(value, orientation, notify_linked=notify_linked)
 
-    @pyqtSlot(int, int)
+    @Slot(int, int)
     def scrollAbsolute(self, value, orientation, notify_linked=True):
         """Sets the scrollbar to the given value."""
-        bar = self._scoll_bars[orientation]
+        if orientation not in self._scroll_bars:
+            return
+        # Cast to int to prevent TypeError encountered in qt versions available
+        # with Ubuntu 22.04 and 24.04
+        value = int(value)
+        bar = self._scroll_bars[orientation]
         if value < bar.minimum():
             value = bar.minimum()
         if value > bar.maximum():
             value = bar.maximum()
         bar.setValue(value)
         self.viewChanged.emit()
         if notify_linked:
@@ -554,15 +567,15 @@
         self._img_scale = max(self._min_img_scale, self._img_scale)
         self._canvas.setScale(self._img_scale)
         self._canvas.adjustSize()
         self._canvas.update()
 
 
 class RectSelectionDialog(QDialog):
-    rectSelected = pyqtSignal(object)
+    rectSelected = Signal(object)
 
     def __init__(self, parent=None):
         super(RectSelectionDialog, self).__init__()
         layout = QVBoxLayout()
         self._img_viewer = ImageViewer(viewer_type=ImageViewerType.RECT_SELECTION)
         self._img_viewer.rectSelected.connect(self._emitRectSelected)
         layout.addWidget(self._img_viewer)
```

### Comparing `iminspect-1.3.9/iminspect/inputs.py` & `iminspect-1.4.0/iminspect/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
 # TODO implement set_value for remaining widgets (currently only needed for
 # checkboxes and dropdowns)
 
 import os
 import sys
 from enum import Enum
-from PyQt5.QtWidgets import QMainWindow, QApplication, QWidget, \
+from qtpy.QtWidgets import QMainWindow, QApplication, QWidget, \
     QHBoxLayout, QVBoxLayout, QPushButton, QLabel, QFrame, \
     QSlider, QCheckBox, QFileDialog, QComboBox, QLineEdit, QSizePolicy, \
     QColorDialog
-from PyQt5.QtCore import pyqtSignal, pyqtSlot, Qt, QSize, QRegExp, QEvent, QRect, QRectF, QFileInfo
-from PyQt5.QtGui import QRegExpValidator, QFontDatabase, QColor, QBrush, QPen, QPainter
+from qtpy.QtCore import Signal, Slot, Qt, QSize, QRegExp, QEvent, QRect, QRectF, QFileInfo
+from qtpy.QtGui import QRegExpValidator, QFontDatabase, QColor, QBrush, QPen, QPainter
 from vito import imutils
 
 from . import imgview
 
 
 def format_int(v, digits=None):
     if digits is None:
@@ -61,15 +61,15 @@
         super(VLine, self).__init__(parent)
         self.setFrameShape(QFrame.VLine)
         self.setFrameShadow(QFrame.Sunken)
 
 
 class InputWidget(QWidget):
     """Base class which defines the value-changed signal to be emitted."""
-    value_changed = pyqtSignal(object)
+    value_changed = Signal(object)
 
     def __init__(self, parent=None):
         super(InputWidget, self).__init__(parent)
 
     def _emit_value_change(self):
         self.value_changed.emit(self.get_input())
 
@@ -111,15 +111,15 @@
 class ColorIndicator(QWidget):
     """
     Draws a right aligned rectangle of dimension
     H x (width_factor * H) with the currently set color.
     H = widget.height() - 2*padding.
     If width_factor is negative, W = widget.width() - 2*padding.
     """
-    clicked = pyqtSignal()
+    clicked = Signal()
 
     def __init__(self, padding=0, width_factor=4, parent=None):
         super(ColorIndicator, self).__init__(parent)
         self._color = None
         self._padding = padding
         self._width_factor = width_factor
         self.setMinimumWidth(30)
@@ -179,15 +179,15 @@
         layout = QHBoxLayout()
         layout.addWidget(lbl)
         layout.addWidget(self._color_indicator)
         layout.addStretch()
         layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(layout)
 
-    @pyqtSlot()
+    @Slot()
     def __choose(self):
         opt = QColorDialog.DontUseNativeDialog
         if self._with_alpha:
             opt = opt | QColorDialog.ShowAlphaChannel
         c = QColorDialog.getColor(
             initial=self.qcolor(),
             parent=self,
@@ -222,19 +222,19 @@
     # Height of the slider's bar (i.e. the "line" behind the handles)
     SLIDER_BAR_HEIGHT = 4
 
     # The slider's handles will be drawn as squares with this side length
     HANDLE_SIDE_LENGTH = 13
 
     # Min/max has changed:
-    rangeChanged = pyqtSignal(int, int)
+    rangeChanged = Signal(int, int)
     # Lower/left value has changed
-    lowerValueChanged = pyqtSignal(int)
+    lowerValueChanged = Signal(int)
     # Upper/right value has changed
-    upperValueChanged = pyqtSignal(int)
+    upperValueChanged = Signal(int)
 
     def __init__(self, min_value=0, max_value=100,
             parent=None):
         super(RangeSlider, self).__init__()
         self._minimum = min_value
         self._maximum = max_value
         self._interval = max_value - min_value
@@ -444,45 +444,112 @@
             RangeSlider.HANDLE_SIDE_LENGTH)
 
 
 class RangeSliderSelectionWidget(InputWidget):
     def __init__(
             self, label, min_value=0, max_value=100,
             initial_lower_value=None, initial_upper_value=None,
-            value_format_fx=format_int,
+            value_format_fx=format_int, allow_text_input=False,
             min_label_width=None, parent=None):
         super(RangeSliderSelectionWidget, self).__init__(parent)
         layout = QHBoxLayout()
         lbl = QLabel(label, parent=self)
         if min_label_width is not None:
             lbl.setMinimumWidth(min_label_width)
         layout.addWidget(lbl)
 
-        self._lbl_lower = QLabel(' ', parent=self)
+        if allow_text_input:
+            self._lbl_lower = QLineEdit()
+            # self._lbl_lower.setMinimumWidth(50)
+            # self._lbl_lower.setMaximumWidth(50)
+            # self._lbl_lower.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Preferred)
+        else:
+            self._lbl_lower = QLabel(' ', parent=self)
         self._lbl_lower.setAlignment(Qt.AlignRight | Qt.AlignVCenter)
         layout.addWidget(self._lbl_lower)
 
         self._slider = RangeSlider(min_value=min_value, max_value=max_value, parent=self)
         if initial_lower_value is not None:
             self._slider.setLowerValue(initial_lower_value)
         if initial_upper_value is not None:
             self._slider.setUpperValue(initial_upper_value)
         self._slider.lowerValueChanged.connect(self.__slider_changed)
         self._slider.upperValueChanged.connect(self.__slider_changed)
         self._slider.rangeChanged.connect(lambda a, b: self.__slider_changed)
+        self._slider.setMinimumWidth(150)
         layout.addWidget(self._slider)
-
-        self._lbl_upper = QLabel(' ', parent=self)
+        
+        if allow_text_input:
+            self._lbl_upper = QLineEdit()
+            # self._lbl_upper.setMinimumWidth(50)
+            # self._lbl_upper.setMaximumWidth(50)
+        else:
+            self._lbl_upper = QLabel(' ', parent=self)
         layout.addWidget(self._lbl_upper)
         self.set_value_format_fx(value_format_fx)
 
         layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(layout)
         self.__slider_changed()
 
+        if allow_text_input:
+            self._lbl_lower.textEdited.connect(self.__min_value_text_edited)
+            self._lbl_upper.textEdited.connect(self.__max_value_text_edited)
+            self._lbl_lower.editingFinished.connect(self.__set_from_text_box)
+            self._lbl_upper.editingFinished.connect(self.__set_from_text_box)
+    
+    @Slot()
+    def __set_from_text_box(self):
+        slider_value = self.get_input()
+        # Check if min is a valid number
+        try:
+            min_value = float(self._lbl_lower.text())
+        except:
+            min_value = slider_value[0]
+        # Check if max is a valid number
+        try:
+            max_value = float(self._lbl_upper.text())
+        except:
+            max_value = slider_value[1]
+        # Check if both are within the range
+        valid_range = self._slider.range()
+        min_value = max(valid_range[0], min(valid_range[1], min_value))
+        max_value = min(valid_range[1], max(valid_range[0], max_value))
+        if min_value > max_value:
+            self.set_value((max_value, min_value))
+        else:
+            self.set_value((min_value, max_value))
+        self.__slider_changed()
+
+    @Slot()
+    def __min_value_text_edited(self):
+        slider_value = self.get_input()
+        try:
+            min_value = float(self._lbl_lower.text())
+        except:
+            min_value = None
+        if min_value is None or min_value > slider_value[1] or min_value < self._slider.range()[0]:
+            print('Ignoring invalid input')
+            print(min_value)
+            print(self._slider.range())
+            return
+        self.set_value((min_value, slider_value[1]))
+    
+    @Slot()
+    def __max_value_text_edited(self):
+        slider_value = self.get_input()
+        try:
+            max_value = float(self._lbl_upper.text())
+        except:
+            max_value = None
+        if max_value is None or max_value < slider_value[0] or max_value > self._slider.range()[1]:
+            print('Ignoring invalid input')
+            return
+        self.set_value((slider_value[0], max_value))
+
     def set_value_format_fx(self, fx):
         self.__value_format_fx = fx
         if self.__value_format_fx is not None:
             # Set label text to the extremal values, so we can fix the width,
             # e.g. "False" vs "True"
             self._lbl_upper.setText(self.__value_format_fx(self._slider.minimum()))
             max_width = self._lbl_upper.sizeHint().width()
@@ -959,14 +1026,20 @@
 
         self._slider_range = RangeSliderSelectionWidget('Range slider:', 0, 100,
             initial_lower_value=23, initial_upper_value=42,
             value_format_fx=lambda v: format_int(v, 4), min_label_width=150)
         main_layout.addWidget(self._slider_range)
         main_layout.addWidget(HLine())
 
+        self._slider_range_textbox = RangeSliderSelectionWidget('Range slider w/ textbox:', 0, 100,
+            initial_lower_value=23, initial_upper_value=42, allow_text_input=True,
+            value_format_fx=lambda v: format_int(v, 4), min_label_width=150)
+        main_layout.addWidget(self._slider_range_textbox)
+        main_layout.addWidget(HLine())
+
         self._cb = CheckBoxWidget('Toggle me:', is_checked=True, min_label_width=150)
         main_layout.addWidget(self._cb)
         main_layout.addWidget(HLine())
 
         self._roi = RoiSelectWidget('Region of interest:', roi=(10, 20, 50, 30), min_label_width=150,
             box_labels=['Left:', 'Top:', 'Width:', 'Height:'], support_image_selection=True)
         main_layout.addWidget(self._roi)
@@ -982,14 +1055,15 @@
         self._file_widget_save.value_changed.connect(self._val_changed)
         self._ip_widget.value_changed.connect(self._val_changed)
         self._size_widget.value_changed.connect(self._val_changed)
         self._dropdown.value_changed.connect(self._val_changed)
         self._slider.value_changed.connect(self._val_changed)
         self._sliderf.value_changed.connect(self._val_changed)
         self._slider_range.value_changed.connect(self._val_changed)
+        self._slider_range_textbox.value_changed.connect(self._val_changed)
         self._cb.value_changed.connect(self._val_changed)
         self._roi.value_changed.connect(self._val_changed)
 
         self._main_widget.setLayout(main_layout)
         self.setCentralWidget(self._main_widget)
         self.resize(QSize(640, 480))
 
@@ -998,15 +1072,15 @@
         print('Some value changed: ', sender.get_input())
 
     def _query(self):
         print('Query all widgets:')
         for w in [self._folder_widget, self._file_widget_open,
                 self._file_widget_save, self._ip_widget, self._size_widget,
                 self._dropdown, self._slider, self._sliderf, self._slider_range,
-                self._cb, self._roi]:
+                self._slider_range_textbox, self._cb, self._roi]:
             print('Input "{}"'.format(w.get_input()))
         print('\n')
 
 
 def run_demo():
     print('########################################################\n')
     print('Demonstration of custom (labelled) input widgets.\n')
```

### Comparing `iminspect-1.3.9/iminspect/inspection_utils.py` & `iminspect-1.4.0/iminspect/inspection_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 import os
 import math
 import qimage2ndarray
-
-# from PyQt5.QtWidgets import QMainWindow, QApplication, QWidget, \
-#     QHBoxLayout, QVBoxLayout, QGridLayout, QPushButton, QLabel, QFrame, QToolTip, \
-#     QShortcut, QDialog, QMessageBox, QToolButton, QScrollArea
-from PyQt5.QtCore import Qt
-from PyQt5.QtGui import QPainter, QFont, QColor, QPixmap, QImage, QPen
+from qtpy.QtCore import Qt
+from qtpy.QtGui import QPainter, QFont, QColor, QPixmap, QImage, QPen
+from typing import Tuple
 
 
 # Utils to format a data point (depending on the range)
 def fmtf(v):
     return '{:f}'.format(v)
 
 
@@ -84,19 +81,18 @@
         qp.drawText(qimage.rect(), Qt.AlignCenter, "Error!\nCannot display a\n{:d}-channel image.".format(img_np.shape[2]))
         qp.end()
     if qimage.isNull():
         raise ValueError('Invalid image received, cannot convert it to QImage')
     return QPixmap.fromImage(qimage)
 
 
-def emptyInspectionImage():
+def emptyInspectionImage(img_size: Tuple[int, int] = (640, 320)):
     """Returns a dummy image to be displayed if the inspector is
     called with invalid (None) data."""
-    img_width = 640
-    img_height = 320
+    img_width, img_height = img_size
     qimage = QImage(img_width, img_height, QImage.Format_RGB32)
     qimage.fill(Qt.white)
     qp = QPainter()
     qp.begin(qimage)
     qp.setRenderHint(QPainter.HighQualityAntialiasing)
     qp.setPen(QPen(QColor(200, 0, 0)))
     font = QFont()
```

### Comparing `iminspect-1.3.9/iminspect/inspection_widgets.py` & `iminspect-1.4.0/iminspect/inspection_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 #!/usr/bin/env python
 # coding=utf-8
 """Inspect matrix/image data"""
 
 import math
 import numpy as np
-from PyQt5.QtWidgets import QWidget, QDialog, QHBoxLayout, QVBoxLayout, QPushButton, QLabel, QToolButton
-from PyQt5.QtCore import Qt, QSize, QRect, QPoint, QPointF, pyqtSignal, pyqtSlot
-from PyQt5.QtGui import QPainter, QFont, QFontMetrics, QBrush, QColor, QIcon, QPen
-
+from qtpy.QtWidgets import QWidget, QDialog, QHBoxLayout, QVBoxLayout, QPushButton, QLabel, QToolButton
+from qtpy.QtCore import Qt, QSize, QRect, QPoint, QPointF, Signal, Slot
+from qtpy.QtGui import QPainter, QFont, QFontMetrics, QBrush, QColor, QIcon, QPen
 from vito import flowutils
 
-from . import imgview
-from . import inputs
-from . import inspection_utils
-from . import inspector
+from . import imgview, inputs, inspection_utils, inspector
 
 
 class ColorBar(QWidget):
     """Draws a vertical color bar."""
     def __init__(self):
         super(ColorBar, self).__init__()
         self._bar_width = 30
@@ -271,15 +267,15 @@
             self._type_widget.set_value(current_data_type)
 
     def open(self):
         super(OpenInspectionFileDialog, self).open()
         if self._filename is None:
             self._file_widget.open_dialog()
 
-    @pyqtSlot(object)
+    @Slot(object)
     def __fileSelected(self, filename):
         self._filename = filename
         if self._filename is not None and self._filename.lower().endswith('.flo'):
             self._type_widget.set_value(inspector.DataType.FLOW)
             self._type_widget.setEnabled(False)
         elif self._filename is not None and self._filename.lower().endswith('.npy'):
             self._type_widget.set_value(inspector.DataType.MULTICHANNEL)
@@ -289,19 +285,19 @@
             if self._type_widget.get_input()[0] == inspector.DataType.FLOW:
                 self._type_widget.set_value(inspector.DataType.COLOR)
             self._type_widget.setEnabled(True)
         self._btn_confirm.setEnabled(self._filename is not None)
         if self._filename is None:
             self.__onCancel()
 
-    @pyqtSlot()
+    @Slot()
     def __onCancel(self):
         self.reject()
 
-    @pyqtSlot()
+    @Slot()
     def __onConfirm(self):
         type_tuple = self._type_widget.get_input()
         if type_tuple is None:
             self._data_type = None
         else:
             self._data_type = type_tuple[0]
         self._confirmed = True
@@ -388,32 +384,32 @@
             hlayout.addLayout(layout)
             self.setLayout(hlayout)
 
     def open(self):
         super(SaveInspectionFileDialog, self).open()
         self._file_widget.open_dialog()
 
-    @pyqtSlot(object)
+    @Slot(object)
     def __updateThumbnail(self, selection):
         if selection is None or self._thumbnails is None:
             return
         self._thumbnail_viewer.setPixmap(self._thumbnails[selection[0]])
 
-    @pyqtSlot(object)
+    @Slot(object)
     def __fileSelected(self, filename):
         self._filename = filename
         self._btn_confirm.setEnabled(self._filename is not None)
         if self._filename is None:
             self.__onCancel()
 
-    @pyqtSlot()
+    @Slot()
     def __onCancel(self):
         self.reject()
 
-    @pyqtSlot()
+    @Slot()
     def __onConfirm(self):
         tpl = self._save_as_widget.get_input()
         if tpl is None:
             self._save_as = None
         else:
             self._save_as = tpl[0]
         self._confirmed = True
@@ -480,19 +476,19 @@
         # Pre-set data type
         if current_data_type is not None:
             self._type_widget.set_value(current_data_type)
 
     def open(self):
         super(ChangeDataTypeDialog, self).open()
 
-    @pyqtSlot()
+    @Slot()
     def __onCancel(self):
         self.reject()
 
-    @pyqtSlot()
+    @Slot()
     def __onConfirm(self):
         type_tuple = self._type_widget.get_input()
         if type_tuple is None:
             self._data_type = None
         else:
             self._data_type = type_tuple[0]
         self._confirmed = True
@@ -504,17 +500,17 @@
         return None
 
 
 class ToolbarFileIOWidget(QWidget):
     """
     Provides buttons to issue open/save file requests.
     """
-    fileOpenRequest = pyqtSignal()
-    fileSaveRequest = pyqtSignal()
-    visualizationChangeRequest = pyqtSignal()
+    fileOpenRequest = Signal()
+    fileSaveRequest = Signal()
+    visualizationChangeRequest = Signal()
 
     def __init__(self, vertical=False, icon_size=QSize(20, 20), parent=None):
         """
         Shows two clickable icons to open a file and save the currently
         inspected data to disk.
         Buttons can be arranged horizontally or vertially, set the "vertical"
         flag accordingly.
@@ -566,17 +562,17 @@
 class ToolbarZoomWidget(QWidget):
     """
     Provides two clickable icons allowing the user to request the standard
     scalings "zoom-best-fit" (fit image to the currently available canvas
     size) and "zoom-original" (show image at 100% zoom).
     """
     # Signal if zoom-best-fit is clicked
-    zoomBestFitRequest = pyqtSignal()
+    zoomBestFitRequest = Signal()
     # Signal if zoom-original is clicked
-    zoomOriginalSizeRequest = pyqtSignal()
+    zoomOriginalSizeRequest = Signal()
 
     def __init__(self, central_widget, parent=None):
         super(ToolbarZoomWidget, self).__init__(parent)
         self._show_label = True
         layout = QHBoxLayout()
         self._scale_label = QLabel('Scale:')
         layout.addWidget(self._scale_label)
@@ -593,15 +589,15 @@
         btn_original.setToolTip('Zoom to original size (Ctrl+1)')
         btn_original.clicked.connect(self.zoomOriginalSizeRequest)
         layout.addWidget(btn_original)
         # Important: remove margins!
         layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(layout)
 
-    @pyqtSlot(float)
+    @Slot(float)
     def setScale(self, scale):
         if not self._show_label:
             return
         if scale < 0.01:
             self._scale_label.setText('Scale < 1 %')
         else:
             self._scale_label.setText('Scale {:d} %'.format(int(scale*100)))
```

### Comparing `iminspect-1.3.9/iminspect/inspector.py` & `iminspect-1.4.0/iminspect/inspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #!/usr/bin/env python
 # coding=utf-8
 """Inspect matrix/image data"""
+from typing import Tuple, Union
 
 # TODO Ideas and potential usability improvements:
 # * Load multiple files via drag & drop from file browser/external image viewer
 #   => requires layout reset; potential issue: variable number of inspection
 #      widgets (what's the expected behavior if there are already multple widgets
 #      open for inspection?)
 #
-# * Add input boxes to range slider for manually typing the upper/lower limits
+# * Add input boxes to range slider for manually typing the upper/lower limits.
+#   This would require forwarding the editFinished signal to the inspector - because
+#   we convert the RangeSlider steps (e.g. 0..100) to the data range (e.g. -0.5..+0.5).
 #
 # * Usability Improvement:
 #   Thumbnail in "Open File"/"Reload Visualization" dialogs could be larger.
 #
 # * GUI issue:
 #   Initial window resize won't scale to the exact specified size.
 #   QApplication().instance().processEvents() doesn't help either. The widgets
@@ -49,30 +52,24 @@
 #   to minor zooming/scrolling issues.
 #   Currently, I prefer not to deal with such unexpected user behavior, as
 #   this increases the code complexity unnecessarily.
 
 import numpy as np
 import os
 from enum import Enum
-from PyQt5.QtWidgets import QMainWindow, QApplication, QWidget, \
+from qtpy.QtWidgets import QMainWindow, QApplication, QWidget, \
     QHBoxLayout, QVBoxLayout, QGridLayout, QLabel, QFrame, QToolTip, \
     QShortcut, QMessageBox, QScrollArea, QSizePolicy
-from PyQt5.QtCore import Qt, QSize, QPoint, pyqtSignal, pyqtSlot
-from PyQt5.QtGui import QCursor, QFont, QKeySequence, QResizeEvent, QIcon
+from qtpy.QtCore import Qt, QSize, QPoint, Signal, Slot
+from qtpy.QtGui import QCursor, QFont, QKeySequence, QResizeEvent, QIcon
 from PIL import UnidentifiedImageError
 
-from vito import imutils
-from vito import colormaps
-from vito import imvis
-from vito import flowutils
-
-from . import imgview
-from . import inputs
-from . import inspection_widgets
-from . import inspection_utils
+from vito import imutils, colormaps, imvis, flowutils
+
+from . import imgview, inputs, inspection_widgets, inspection_utils
 
 
 class DataType(Enum):
     # Standard 3- or 4-channel input
     COLOR = 0
     # Single-channel data, arbitrary type
     MONOCHROME = 1
@@ -209,26 +206,26 @@
     VIS_RAW = -1
     # Ensure that grayscale is the second option
     VIS_COLORMAPS = ['Grayscale'] + [cmn for cmn in colormaps.colormap_names if cmn.lower() != 'grayscale']
 
     # Emitted whenever the user changes the image scale (float).
     # The integer parameter will hold the "inspector_id" as set
     # upon __init__().
-    imgScaleChanged = pyqtSignal(int, float)
+    imgScaleChanged = Signal(int, float)
 
     # Notify observers that a new image has been loaded
-    fileOpened = pyqtSignal(int)
+    fileOpened = Signal(int)
 
     # Emitted whenever the user moves the mouse across the image
     # Yields the "inspector_id" and corresponding (image) pixel position
     # as QPointF or None.
     # If the position is None, this indicates that the user simply changed
     # the visualization mode (e.g. switching from grayscale to raw data)
     # and thus, the currently displayed tooltip (if any) must be updated.
-    showTooltipRequest = pyqtSignal(int, object)
+    showTooltipRequest = Signal(int, object)
 
     def __init__(
             self,
             inspector_id, data, data_type,
             display_settings=None,
             categorical_labels=None):
         super(InspectionWidget, self).__init__()
@@ -400,36 +397,36 @@
 
     def zoomImage(self, delta):
         self._img_viewer.zoom(delta)
 
     def scrollImage(self, delta, orientation):
         self._img_viewer.scroll(delta, orientation)
 
-    @pyqtSlot()
+    @Slot()
     def showFileSaveDialog(self):
         thumbnails = {
             inspection_widgets.SaveInspectionFileDialog.SAVE_VISUALIZATION: self._img_viewer.imagePixmap(),
             inspection_widgets.SaveInspectionFileDialog.SAVE_RAW: inspection_utils.pixmapFromNumPy(self._data)
         }
         self._save_file_dialog = inspection_widgets.SaveInspectionFileDialog(
             self._data_type, thumbnails=thumbnails, parent=self)
         self._save_file_dialog.finished.connect(self.__onSaveFinished)
         self._save_file_dialog.open()
 
-    @pyqtSlot()
+    @Slot()
     def showFileOpenDialog(self):
         # self._open_file_dialog = OpenInspectionFileDialog(self._data_type, parent=self)
         self._open_file_dialog = inspection_widgets.OpenInspectionFileDialog(
             data_type=self._data_type,
             thumbnail=self._img_viewer.imagePixmap(),
             parent=self)
         self._open_file_dialog.finished.connect(self.__onOpenFinished)
         self._open_file_dialog.open()
 
-    @pyqtSlot()
+    @Slot()
     def __onSaveFinished(self):
         res = self._save_file_dialog.getSelection()
         if res is None or any([r is None for r in res]):
             return
         filename, save_type = res
         if save_type == inspection_widgets.SaveInspectionFileDialog.SAVE_VISUALIZATION:
             filename = inspection_utils.FilenameUtils.ensureImageExtension(filename)
@@ -476,15 +473,15 @@
             msg.setText('Error saving {:s}'.format(
                 'current visualization' if save_type == inspection_widgets.SaveInspectionFileDialog.SAVE_VISUALIZATION
                 else 'raw input data'))
             msg.setInformativeText('Logged exception:\n{:s}'.format(str(e)))
             msg.setWindowTitle('Error')
             msg.exec()
 
-    @pyqtSlot(str)
+    @Slot(str)
     def __openDroppedFilename(self, filename):
         if filename is None:
             return
         # 1) Guess datatype
         try:
             dtype = DataType.fromFilename(filename)
         except ValueError:
@@ -499,15 +496,15 @@
             data_type=dtype,
             thumbnail=None if self._data is None else self._img_viewer.imagePixmap(),
             filename_suggestion=filename,
             parent=self)
         self._open_file_dialog.finished.connect(self.__onOpenFinished)
         self._open_file_dialog.open()
 
-    @pyqtSlot()
+    @Slot()
     def __onOpenFinished(self):
         res = self._open_file_dialog.getSelection()
         if res is None or any([r is None for r in res]):
             return
         try:
             filename, data_type = res
             if data_type == DataType.FLOW:
@@ -527,22 +524,22 @@
             msg.setIcon(QMessageBox.Critical)
             msg.setText('Error loading file as type "{:s}"'.format(
                 DataType.toStr(data_type)))
             msg.setInformativeText('Logged exception:\n{:s}'.format(str(e)))
             msg.setWindowTitle('Error')
             msg.exec()
 
-    @pyqtSlot()
+    @Slot()
     def showVisualizationChangeDialog(self):
         self._reload_visualization_dialog = inspection_widgets.ChangeDataTypeDialog(
             self._data_type, self._img_viewer.imagePixmap(), parent=self)
         self._reload_visualization_dialog.finished.connect(self.__onReloadDialogFinished)
         self._reload_visualization_dialog.open()
 
-    @pyqtSlot()
+    @Slot()
     def __onReloadDialogFinished(self):
         new_data_type = self._reload_visualization_dialog.getSelection()
         if new_data_type is None:
             return
         if new_data_type == self._data_type:
             print('The same data type has been selected. Reload request will be ignored.')
             return
@@ -760,15 +757,15 @@
         self._visualization_dropdown.value_changed.connect(self.__updateDisplay)
         self._visualization_dropdown.value_changed.connect(lambda: self.showTooltipRequest.emit(self._inspector_id, None))
         self._visualization_dropdown.setToolTip('Select raw vs. colorized')
         input_layout.addWidget(self._visualization_dropdown)
 
         self._visualization_range_slider = inputs.RangeSliderSelectionWidget('Shown limits:',
             min_value=0, max_value=255,
-            value_format_fx=None)
+            value_format_fx=None, allow_text_input=False)
         self._visualization_range_slider.value_changed.connect(self.__updateDisplay)
         self._visualization_range_slider.value_changed.connect(lambda: self.showTooltipRequest.emit(self._inspector_id, None))
         self._visualization_range_slider.setToolTip('Adjust visualization limits')
         input_layout.addWidget(self._visualization_range_slider)
 
         # Image viewer and colorbar
         img_layout = QHBoxLayout()
@@ -828,15 +825,15 @@
         # widgets. Now, we can set a size constraint for inputs and the
         # data information label.
         min_input_height = self._input_widget.layout().minimumSize().height()
         self._data_label_scroll_area.setMaximumHeight(min_input_height)
         self._input_widget.setMaximumHeight(min_input_height)
         return super(InspectionWidget, self).resizeEvent(event)
 
-    @pyqtSlot()
+    @Slot()
     def __updateDisplay(self):
         # Select which layer to show:
         if self._is_single_channel:
             self._visualized_data = self._data
             is_single_channel = True
         else:
             layer_selection = self._layer_dropdown.get_input()[0]
@@ -962,42 +959,45 @@
         self._save_file_dialog = None
         # Create the central widget (layout will be adjusted within
         # inspectData()
         self._main_widget = QWidget()
         self.setCentralWidget(self._main_widget)
         # Set icon
         self.setWindowIcon(QIcon(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'iminspect_assets', 'iminspect.svg')))
-        #convert iminspect-16.png iminspect-32.png iminspect-64.png iminspect-128.png iminspect-256.png -colors 256 iminspect.ico
         # Set up keyboard shortcuts
         self.__addShortcuts()
         # Add a zoom widget (scale original, fit window, ...) to the status bar
         self._zoom_widget = inspection_widgets.ToolbarZoomWidget(self.centralWidget())
         self._zoom_widget.zoomBestFitRequest.connect(self.scaleImagesFit)
         self._zoom_widget.zoomOriginalSizeRequest.connect(self.scaleImagesOriginal)
         self.statusBar().addPermanentWidget(self._zoom_widget)
         # Finally, show the given data
         self._inspectors = list()
         self.inspectData(data, data_type,
             max_num_widgets_per_row=max_num_widgets_per_row,
             display_settings=display_settings,
             force_linked_viewers=force_linked_viewers,
             categorical_labels=categorical_labels)
+        if initial_window_size is not None:
+            self.resize(initial_window_size)
 
     def inspectData(
             self, data, data_type,
             max_num_widgets_per_row=3, display_settings=None,
             force_linked_viewers=False,
             categorical_labels=None):
         """
         Loads the given data and resets the widget's layout.
         See inspector.inspect() for documentation of the parameters.
         """
         if data is None:
-            #raise ValueError('Input data cannot be None')
-            data = inspection_utils.emptyInspectionImage()
+            sz = (640, 320)
+            if self._initial_window_size is not None:
+                sz = (self._initial_window_size.width(), self._initial_window_size.height())
+            data = inspection_utils.emptyInspectionImage(sz)
 
         if inspection_utils.isArrayLike(data):
             # Check if all images have the same width/height.
             matching_input_shape = True
             # Place inspection widgets in a grid layout.
             layout = QGridLayout()
             # Create inspection widgets:
@@ -1074,22 +1074,24 @@
         Re-applies the display settings previously obtained via
         currentDisplaySettings() where applicable. This means that if the
         data type changed in between, type-specific UI settings/attributes
         will not be restored.
         """
         if settings is None:
             return
-        self.resize(settings['win-size'])
+        if 'win-size' in settings:
+            self.resize(settings['win-size'])
         # Note that restoring the position doesn't always work (issues with
         # windows that are placed partially outside the screen)
-        self.move(settings['win-pos'])
+        if 'win-pos' in settings:
+            self.move(settings['win-pos'])
         # Restore each viewer-specific display only if the number of viewers
         # stayed the same:
         num_inspectors = len(self._inspectors)
-        if num_inspectors == settings['num-inspectors']:
+        if 'num-inspectors' in settings and num_inspectors == settings['num-inspectors']:
             for idx in range(num_inspectors):
                 self._inspectors[idx].restoreDisplaySettings(settings['inspection-widgets'][idx])
         self.update()
 
     def __linkInspectors(self):
         """Link zoom/scroll behavior of multiple inspection widgets, if possible/requested."""
         for insp in self._inspectors:
@@ -1144,43 +1146,43 @@
         # Scale to original size
         shortcut_scale_original = QShortcut(QKeySequence('Ctrl+1'), self)
         shortcut_scale_original.activated.connect(self.scaleImagesOriginal)
         # Toggle tool tip display
         shortcut_toggle_tooltip = QShortcut(QKeySequence('Ctrl+T'), self)
         shortcut_toggle_tooltip.activated.connect(self.toggleTooltipDisplay)
 
-    @pyqtSlot(int)
+    @Slot(int)
     def scrollImages(self, delta, orientation):
         for insp in self._inspectors:
             insp.scrollImage(delta, orientation)
 
-    @pyqtSlot(int)
+    @Slot(int)
     def zoomImages(self, delta):
         for insp in self._inspectors:
             insp.zoomImage(delta)
 
-    @pyqtSlot()
+    @Slot()
     def scaleImagesOriginal(self):
         for insp in self._inspectors:
             insp.setImageScaleAbsolute(1.0)
 
-    @pyqtSlot()
+    @Slot()
     def scaleImagesFit(self):
         for insp in self._inspectors:
             insp.setImageScaleFit()
 
-    @pyqtSlot()
+    @Slot()
     def toggleTooltipDisplay(self):
         self._display_tooltip = not self._display_tooltip
         if self._display_tooltip:
             self.showPixelValue(self.__getActiveInspector(), None)
         else:
             QToolTip.hideText()
 
-    @pyqtSlot(int)
+    @Slot(int)
     def __fileHasBeenOpened(self, inspector_id):
         self.__updateWindowTitle()
         # Update handles for linked inspectors (since image viewers may have
         # been replaced by new objects)
         self.__linkInspectors()
         # Send a dummy resize event to ensure that the "image information label"
         # and input widgets of each InspectionWidget are properly resized.
@@ -1228,15 +1230,15 @@
                 sc = '< 1'
             else:
                 sc = '{:d}'.format(int(query['scale']*100))
             s += '<tr><td>Scale:</td><td> ' + sc + '%</td></tr>'
         s += '</table>'
         return s
 
-    @pyqtSlot(int, object)
+    @Slot(int, object)
     def showPixelValue(self, inspector_id, image_pos):
         """Invoked whenever the mouse position changed."""
         if image_pos is None:
             # Position will be None if the user scrolls/zooms via keyboard
             # shortcuts. Thus, update info for positoin under cursor:
             if not self._inspectors[inspector_id].underMouse():
                 return
@@ -1259,96 +1261,108 @@
         inspection widget.
         """
         for inspector_id in range(len(self._inspectors)):
             if self._inspectors[inspector_id].underMouse():
                 return inspector_id
         return 0
 
-    @pyqtSlot()
+    @Slot()
     def __onOpenShortcut(self):
         inspector_id = self.__getActiveInspector()
         self._inspectors[inspector_id].showFileOpenDialog()
 
-    @pyqtSlot()
+    @Slot()
     def __onSaveShortcut(self):
         inspector_id = self.__getActiveInspector()
         self._inspectors[inspector_id].showFileSaveDialog()
     
-    @pyqtSlot()
+    @Slot()
     def __onReloadShortcut(self):
         inspector_id = self.__getActiveInspector()
         self._inspectors[inspector_id].showVisualizationChangeDialog()
 
 
 def inspect(
-        data,
-        data_type=None,
-        flip_channels=False,
-        label=None,
-        display_settings=None,
-        initial_window_size=(1280, 720),
-        max_num_widgets_per_row=3,
-        force_linked_viewers=False,
-        categorical_labels=None):
-    """Opens a GUI to visualize the given image data.
-
-    data:           numpy ndarray to be visualized. If you want to inspect
-                    several images at once, data may be a tuple of numpy darray.
-
-    data_type:      A DataType enumeration or None. If your input "data" is a
-                    tuple, data_type must be None or a tuple of DataType.
-                    Specifying this is necessary/useful if you want to inspect
-                    a label image: there's no (easy) way of automatically
-                    distinguish a monochrome image from a label image if your
-                    input "data" is uint8.
-                    If None, the "Inspector" will try to guess the data type from
-                    the input data.shape and data.dtype, see DataType.fromData().
-
-    flip_channels:  this qt window works with RGB images, so flip_channels must
-                    be set True if your data is BGR.
-
-    label:          optionally specify a window title.
-
-    display_settings: a dictionary of display settings in case you want to
-                    restore the previous settings. The current settings are
-                    returned by this function.
-
-    initial_window_size: Resize the window.
-
-    max_num_widgets_per_row:  int, if the input "data" is a tuple/list of
-                    multiple images, the GUI will show a grid of
-                    floor(N/num_per_row) x num_per_row inspection widgets.
-
-    force_linked_viewers: bool, if you inspect multiple images at once ("data"
-                    is a tuple), the image viewers will only be linked (i.e.
-                    scroll/zoom simultaneously) if they have the same width
-                    and height. If your input sizes differ, you can set this
-                    flag to force linked viewers.
-
-    categorical_labels: if data_type is CATEGORICAL, you can provide custom
-                    labels to be displayed on the colorbar (as a dictionary,
-                    mapping data values to label strings). If the input data
-                    is a tuple/list, this should be provided as:
-                    * a tuple/list of such dictionaries (if different for each
-                      inputs or not all inputs are categorical), or
-                    * a single dictionary if all inputs show the same labels.
+        data: Union[np.ndarray, Tuple[np.ndarray, ...]],
+        data_type: DataType = None,
+        flip_channels: bool =False,
+        label: str = None,
+        display_settings: dict = None,
+        initial_window_size: Tuple[int, int] = None,
+        max_num_widgets_per_row: int = 3,
+        force_linked_viewers: bool = False,
+        categorical_labels: Union[dict, Tuple[dict, ...]] = None):
+    """
+    Opens a GUI to visualize the given image data.
 
-    returns: the window's exit code and a dictionary of currently used display
-             settings.
+    Args:
+      data: numpy ndarray to be visualized. If you want to inspect
+        several images at once, data may be a tuple of numpy darray.
+
+      data_type: A DataType enumeration or None. If your input "data" is a
+        tuple, data_type must be None or a tuple of DataType.
+        Specifying this is necessary/useful if you want to inspect
+        a label image: there's no (easy) way of automatically
+        distinguish a monochrome image from a label image if your
+        input "data" is uint8.
+        If None, the "Inspector" will try to guess the data type from
+        the input data.shape and data.dtype, see DataType.fromData().
+
+      flip_channels: This qt window works with RGB images, so flip_channels must
+        be set True if your data is BGR.
+
+      label: Optionally specify a window title.
+
+      display_settings: A dictionary of display settings in case you want to
+        restore the previous settings. The current settings are
+        returned by this function.
+
+      initial_window_size: Optionally resize the window to the given (width,
+        height) window size.
+
+      max_num_widgets_per_row: If the input "data" is a tuple/list of
+        multiple images, the GUI will show a grid of
+        floor(N/num_per_row) x num_per_row inspection widgets.
+
+      force_linked_viewers: If you inspect multiple images at once ("data"
+        is a tuple), the image viewers will only be linked (i.e.
+        scroll/zoom simultaneously) if they have the same width
+        and height. If your input sizes differ, you can set this
+        flag to force linked viewers.
+
+      categorical_labels: if data_type is CATEGORICAL, you can provide custom
+        labels to be displayed on the colorbar (as a dictionary,
+        mapping data values to label strings). If the input data
+        is a tuple/list, this should be provided as:
+        * a tuple/list of such dictionaries (if different for each
+          inputs or not all inputs are categorical), or
+        * a single dictionary if all inputs show the same labels.
+
+    Returns:
+      The window's exit code and a dictionary of currently used display
+        settings.
     """
     if flip_channels:
         data = imutils.flip_layers(data)
     # If window title is not provided, make one (indicating the data type).
     app_label = Inspector.makeWindowTitle(label, data, data_type)
 
     app = QApplication([app_label])
-    main_widget = Inspector(data, data_type=data_type,
+
+    if initial_window_size is None:
+        from qtpy.QtGui import QGuiApplication
+        initial_window_size = QGuiApplication.primaryScreen().availableGeometry().size() * 0.7
+    else:
+        initial_window_size = QSize(initial_window_size[0], initial_window_size[1])
+
+    main_widget = Inspector(
+        data=data,
+        data_type=data_type,
         display_settings=display_settings,
-        initial_window_size=None if initial_window_size is None else
-            QSize(initial_window_size[0], initial_window_size[1]),
+        initial_window_size=initial_window_size,
         window_title=label,
         max_num_widgets_per_row=max_num_widgets_per_row,
         force_linked_viewers=force_linked_viewers,
         categorical_labels=categorical_labels)
     main_widget.show()
     rc = app.exec_()
     # Query the viewer settings (in case the user wants to restore them for the
```

