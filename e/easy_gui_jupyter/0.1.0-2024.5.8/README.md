# Comparing `tmp/easy_gui_jupyter-0.1.0.tar.gz` & `tmp/easy_gui_jupyter-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gui_jupyter-0.1.0.tar", max compression
+gzip compressed data, was "easy_gui_jupyter-2024.5.8.tar", max compression
```

## Comparing `easy_gui_jupyter-0.1.0.tar` & `easy_gui_jupyter-2024.5.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1104 2024-05-08 10:31:35.279760 easy_gui_jupyter-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2674 2024-05-08 10:29:30.553206 easy_gui_jupyter-0.1.0/README.md
--rw-r--r--   0        0        0       38 2024-05-08 09:01:49.062606 easy_gui_jupyter-0.1.0/easy_gui_jupyter/__init__.py
--rw-r--r--   0        0        0     9278 2024-05-08 10:22:59.623339 easy_gui_jupyter-0.1.0/easy_gui_jupyter/easy_gui_jupyter.py
--rw-r--r--   0        0        0      803 2024-05-08 10:35:16.354427 easy_gui_jupyter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3270 1970-01-01 00:00:00.000000 easy_gui_jupyter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1104 2024-05-08 10:31:35.279760 easy_gui_jupyter-2024.5.8/LICENSE.txt
+-rw-r--r--   0        0        0     2674 2024-05-08 10:29:30.553206 easy_gui_jupyter-2024.5.8/README.md
+-rw-r--r--   0        0        0       52 2024-05-08 11:08:51.866358 easy_gui_jupyter-2024.5.8/easy_gui_jupyter/__init__.py
+-rw-r--r--   0        0        0     9311 2024-05-08 11:08:51.867208 easy_gui_jupyter-2024.5.8/easy_gui_jupyter/easy_gui_jupyter.py
+-rw-r--r--   0        0        0      840 2024-05-08 14:12:51.366763 easy_gui_jupyter-2024.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3312 1970-01-01 00:00:00.000000 easy_gui_jupyter-2024.5.8/PKG-INFO
```

### Comparing `easy_gui_jupyter-0.1.0/LICENSE.txt` & `easy_gui_jupyter-2024.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easy_gui_jupyter-0.1.0/README.md` & `easy_gui_jupyter-2024.5.8/README.md`

 * *Files identical despite different names*

### Comparing `easy_gui_jupyter-0.1.0/easy_gui_jupyter/easy_gui_jupyter.py` & `easy_gui_jupyter-2024.5.8/easy_gui_jupyter/easy_gui_jupyter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 """
 A module to help simplify the create of GUIs in Jupyter notebooks using ipywidgets.
 """
 
 import os
 import yaml
-import platform
 from ipyfilechooser import FileChooser
 
-
-# import cache if python >= 3.9, otherwise import lru_cache
-if platform.python_version_tuple() >= ("3", "9"):
-    from functools import cache
-else:
-    from functools import lru_cache as cache
-
 import ipywidgets as widgets
 from IPython.display import display, clear_output
 
 
 class EasyGUI:
     """
     A class to simplify the creation of GUIs in Jupyter notebooks using ipywidgets.
@@ -91,110 +83,132 @@
     def add_label(self, *args, **kwargs):
         """
         Add a label widget to the container.
         :param args: args for the widget
         :param kwargs: kwargs for the widget
         """
         self._nLabels += 1
-        self._widgets[f"label_{self._nLabels}"] = widgets.Label(*args, **kwargs, layout=self._layout, style=self._style)
+        self._widgets[f"label_{self._nLabels}"] = widgets.Label(
+            *args, **kwargs, layout=self._layout, style=self._style
+        )
 
     def add_button(self, tag, *args, **kwargs):
         """
         Add a button widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
         :param kwargs: kwargs for the widget
         """
-        self._widgets[tag] = widgets.Button(*args, **kwargs, layout=self._layout, style=self._style)
+        self._widgets[tag] = widgets.Button(
+            *args, **kwargs, layout=self._layout, style=self._style
+        )
 
     def add_text(self, tag, *args, **kwargs):
         """
         Add a text widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
         :param kwargs: kwargs for the widget
 
         Example:
             >>> gui = EasyGUI()
             >>> gui.add_text("text", value="Hello, world!")
         """
-        self._widgets[tag] = widgets.Text(*args, **kwargs, layout=self._layout, style=self._style)
+        self._widgets[tag] = widgets.Text(
+            *args, **kwargs, layout=self._layout, style=self._style
+        )
 
     def add_int_slider(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a integer slider widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
         :param remember_value: remember the last value
         :param kwargs: kwargs for the widget
         """
-        if remember_value and tag in self.cfg and kwargs["min"] <= self.cfg[tag] <= kwargs["max"]:
-            kwargs["value"] = self.cfg[tag]
-        self._widgets[tag] = widgets.IntSlider(*args, **kwargs, layout=self._layout, style=self._style)
+        if (
+            remember_value
+            and tag in self.cfg
+            and kwargs["min"] <= self.cfg[tag] <= kwargs["max"]
+        ):
+            kwargs["value"] = self.cfg[tag]
+        self._widgets[tag] = widgets.IntSlider(
+            *args, **kwargs, layout=self._layout, style=self._style
+        )
 
     def add_float_slider(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a float slider widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
         :param remember_value: remember the last value
         :param kwargs: kwargs for the widget
         """
         if remember_value and tag in self.cfg:
             kwargs["value"] = self.cfg[tag]
-        self._widgets[tag] = widgets.FloatSlider(*args, **kwargs, layout=self._layout, style=self._style)
+        self._widgets[tag] = widgets.FloatSlider(
+            *args, **kwargs, layout=self._layout, style=self._style
+        )
 
     def add_checkbox(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a checkbox widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
         :param remember_value: remember the last value
         :param kwargs: kwargs for the widget
         """
         if remember_value and tag in self.cfg:
             kwargs["value"] = self.cfg[tag]
-        self._widgets[tag] = widgets.Checkbox(*args, **kwargs, layout=self._layout, style=self._style)
+        self._widgets[tag] = widgets.Checkbox(
+            *args, **kwargs, layout=self._layout, style=self._style
+        )
 
     def add_int_text(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a integer text widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
         :param remember_value: remember the last value
         :param kwargs: kwargs for the widget
         """
         if remember_value and tag in self.cfg:
             kwargs["value"] = self.cfg[tag]
 
-        self._widgets[tag] = widgets.IntText(*args, **kwargs, layout=self._layout, style=self._style)
+        self._widgets[tag] = widgets.IntText(
+            *args, **kwargs, layout=self._layout, style=self._style
+        )
 
     def add_float_text(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a float text widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
         :param remember_value: remember the last value
         :param kwargs: kwargs for the widget
         """
         if remember_value and tag in self.cfg:
             kwargs["value"] = self.cfg[tag]
-        self._widgets[tag] = widgets.FloatText(*args, **kwargs, layout=self._layout, style=self._style)
+        self._widgets[tag] = widgets.FloatText(
+            *args, **kwargs, layout=self._layout, style=self._style
+        )
 
     def add_dropdown(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a dropdown widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
         :param remember_value: remember the last value
         :param kwargs: kwargs for the widget
         """
         if remember_value and tag in self.cfg and self.cfg[tag] in kwargs["options"]:
             kwargs["value"] = self.cfg[tag]
-        self._widgets[tag] = widgets.Dropdown(*args, **kwargs, layout=self._layout, style=self._style)
+        self._widgets[tag] = widgets.Dropdown(
+            *args, **kwargs, layout=self._layout, style=self._style
+        )
 
     def add_file_upload(self, tag, *args, accept=None, multiple=False, **kwargs):
         """
         Add a file upload widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
         :param accept: file types to accept
@@ -217,15 +231,15 @@
             yaml.dump(self._cfg, f)
 
     def show(self):
         """
         Show the widgets in the container.
         """
         # display the widgets
-        self._main_display.children = (tuple(self._widgets.values()))
+        self._main_display.children = tuple(self._widgets.values())
         clear_output()
         display(self._main_display)
 
     def clear(self):
         """
         Clear the widgets in the container.
         """
```

### Comparing `easy_gui_jupyter-0.1.0/pyproject.toml` & `easy_gui_jupyter-2024.5.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "easy_gui_jupyter"
-version = "0.1.0"
+version = "2024.05.08"
 description = "Simplify the creation of GUI elements in Jupyter notebooks"
 authors = [    
     "Ricardo Henriques <ricardo@henriqueslab.org>", 
     "Bruno Saraiva <bruno.msaraiva2@gmail.com>",
     "António Brito <antmsbrito95@gmail.com>"
     ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 ipython = "^8.24.0"
 ipywidgets = "^8.1.2"
 ipyfilechooser = "^0.6.0"
+pyyaml = "^6.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 ipykernel = "^6.29.4"
+ruff = "^0.4.3"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.2.0"
 pytest-xdist = "^3.6.1"
 nbmake = "^1.5.3"
 gptrepo = "^1.0.3"
 
-
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "--nbmake -n=auto"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `easy_gui_jupyter-0.1.0/PKG-INFO` & `easy_gui_jupyter-2024.5.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: easy_gui_jupyter
-Version: 0.1.0
+Version: 2024.5.8
 Summary: Simplify the creation of GUI elements in Jupyter notebooks
 Author: Ricardo Henriques
 Author-email: ricardo@henriqueslab.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ipyfilechooser (>=0.6.0,<0.7.0)
 Requires-Dist: ipython (>=8.24.0,<9.0.0)
 Requires-Dist: ipywidgets (>=8.1.2,<9.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # Easy GUI Jupyter
 
 Easy GUI Jupyter is a Python library that simplifies the creation of graphical user interfaces (GUIs) in Jupyter notebooks using ipywidgets. It provides a convenient way to add various types of widgets to your Jupyter notebooks, making it easier to interact with your code and visualize results.
 
 ## Features
```

