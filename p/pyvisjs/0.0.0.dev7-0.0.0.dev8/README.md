# Comparing `tmp/pyvisjs-0.0.0.dev7.tar.gz` & `tmp/pyvisjs-0.0.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-0.0.0.dev7.tar", last modified: Wed May  1 16:40:09 2024, max compression
+gzip compressed data, was "pyvisjs-0.0.0.dev8.tar", last modified: Wed May  8 18:44:57 2024, max compression
```

## Comparing `pyvisjs-0.0.0.dev7.tar` & `pyvisjs-0.0.0.dev8.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.839229 pyvisjs-0.0.0.dev7/
--rw-rw-rw-   0 root         (0) root         (0)     1355 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     4004 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3384 2024-05-01 16:40:09.838229 pyvisjs-0.0.0.dev7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1454 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.833229 pyvisjs-0.0.0.dev7/examples/
--rw-rw-rw-   0 root         (0) root         (0)      525 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/examples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/examples/readme_usage.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.835229 pyvisjs-0.0.0.dev7/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2014 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)     5161 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/node.py
--rw-rw-rw-   0 root         (0) root         (0)    12282 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.836229 pyvisjs-0.0.0.dev7/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)      923 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)      998 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.838229 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3384 2024-05-01 16:40:09.000000 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      637 2024-05-01 16:40:09.000000 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 16:40:09.000000 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-01 16:40:09.000000 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-01 16:40:09.000000 pyvisjs-0.0.0.dev7/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 16:40:09.839229 pyvisjs-0.0.0.dev7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 16:40:09.838229 pyvisjs-0.0.0.dev7/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     7380 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     2373 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3740 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_options.py
--rw-rw-rw-   0 root         (0) root         (0)     2507 2024-05-01 16:39:54.000000 pyvisjs-0.0.0.dev7/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.489679 pyvisjs-0.0.0.dev8/
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-05-08 18:44:57.489679 pyvisjs-0.0.0.dev8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.484679 pyvisjs-0.0.0.dev8/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     8435 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/examples/bluor.py
+-rw-rw-rw-   0 root         (0) root         (0)      525 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/examples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/examples/readme_usage.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.485679 pyvisjs-0.0.0.dev8/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     5325 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/node.py
+-rw-rw-rw-   0 root         (0) root         (0)    13062 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.487679 pyvisjs-0.0.0.dev8/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3355 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)     5254 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/templates/bs-container.html
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.488679 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-05-08 18:44:57.000000 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      691 2024-05-08 18:44:57.000000 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 18:44:57.000000 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-08 18:44:57.000000 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-08 18:44:57.000000 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 18:44:57.489679 pyvisjs-0.0.0.dev8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.488679 pyvisjs-0.0.0.dev8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     8846 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev7/.gitignore` & `pyvisjs-0.0.0.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/.gitlab-ci.yml` & `pyvisjs-0.0.0.dev8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/CONTRIBUTING.md` & `pyvisjs-0.0.0.dev8/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 for example ```This commit is also related to #17 and fixes #18, #19```
 
 
 ## The terminal part from above in short
 ```
 git clone https://gitlab.com/22kittens/pyvisjs.git
+cd pyvisjs
 git checkout dev
 git checkout -b feature-name
 py -m venv .venv
 .venv\Scripts\activate
 py -m pip install -r requirements.txt
 py -m pip install -e .
 pytest
```

### Comparing `pyvisjs-0.0.0.dev7/LICENSE` & `pyvisjs-0.0.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/PKG-INFO` & `pyvisjs-0.0.0.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev7
+Version: 0.0.0.dev8
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev7/README.md` & `pyvisjs-0.0.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/examples/main.py` & `pyvisjs-0.0.0.dev8/examples/main.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/folder_structure.txt` & `pyvisjs-0.0.0.dev8/folder_structure.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/pyproject.toml` & `pyvisjs-0.0.0.dev8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/pyvisjs/base_dictable.py` & `pyvisjs-0.0.0.dev8/pyvisjs/base_dictable.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,11 +40,11 @@
                     if not attr_value: continue
                     result[attr_name] = process_dict(attr_value)
                 elif has_to_dict(attr_value):
                     obj_dict = attr_value.to_dict()
                     if not obj_dict: continue
                     result[attr_name] = obj_dict
                 else:
-                    if not attr_value: continue
+                    if attr_value is None: continue
                     result[attr_name] = attr_value
                     
         return result
```

### Comparing `pyvisjs-0.0.0.dev7/pyvisjs/edge.py` & `pyvisjs-0.0.0.dev8/pyvisjs/edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/pyvisjs/network.py` & `pyvisjs-0.0.0.dev8/pyvisjs/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,26 +105,29 @@
 
         if not [edge.start for edge in self.edges if edge.start == from_id and edge.end == to_id]:
             self.edges.append(Edge(from_id, to_id, **kwargs))
 
     def to_dict(self):
         return super().to_dict()["_data"]
 
-    def show(self, file_name):
+    def show(self, file_name, enable_highlighting=False):
         self.render_template(open_in_browser=True, output_filename=file_name)
 
-    def render_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html", template_filename="basic.html") -> str:
+    def render_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html", template_filename="basic.html", enable_highlighting=False) -> str:
         network_dict = self.to_dict()
         
         html_output = self.env \
             .get_template(template_filename) \
             .render(
                 width=network_dict["options"].get("width", "100%"),
                 height=network_dict["options"].get("height", "100%"),
-                data=network_dict
+                data=network_dict,
+                pyvisjs={
+                    "enable_highlighting": enable_highlighting,
+                },
             )
 
         if save_to_output or open_in_browser:
             file_path = save_file(output_filename, html_output)
 
         if open_in_browser:
             open_file(file_path)
```

### Comparing `pyvisjs-0.0.0.dev7/pyvisjs/node.py` & `pyvisjs-0.0.0.dev8/pyvisjs/node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/pyvisjs/options.py` & `pyvisjs-0.0.0.dev8/pyvisjs/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,16 +97,36 @@
             """
             self._update_dict_with_locals(self.scaling, locals())
             return self
         
     class Edges(BaseDictable):
         def __init__(self):
             super().__init__()
+
+            self.arrows:str = None
+            self.arrowStrikethrough:bool = None
+
             self.color = {}
             self.smooth = {}
+
+        def set(self, arrows:str=None, arrowStrikethrough:bool=None) -> Self:
+            """
+            Parameters
+            ----------
+            arrows : str, default None
+                Can be any combination with any separating symbol of `'to, from, middle'`
+
+            arrowStrikethrough : bool, default=True
+                When false, the edge stops at the arrow. This can be useful if you have thick lines and you want the arrow to end in a point. Middle arrows are not affected by this.
+
+            """
+            if arrows: self.arrows = arrows
+            if arrowStrikethrough is not None: self.arrowStrikethrough = arrowStrikethrough
+
+            return self
         
         def set_color(self, color:str=None, highlight:str=None, hover:str=None, inherit:str=None, opacity:float=None, dashes:bool=None) -> Self:
             """
             Parameters
             ----------
             color : str, default='#848484'
                 The color of the edge when it is not selected or hovered over (assuming hover is enabled in the interaction module).
@@ -178,15 +198,15 @@
             minVelocity : float, default=0.1
                 Once the minimum velocity is reached for all nodes, we assume the network has been stabilized and the simulation stops.
 
             maxVelocity : float, default=50.0
                 The physics module limits the maximum velocity of the nodes to increase the time to stabilization. This is the maximum value.
 
             """
-            if enabled: self.enabled = enabled
+            if enabled is not None: self.enabled = enabled
             if minVelocity: self.minVelocity = minVelocity
             if maxVelocity: self.maxVelocity = maxVelocity
 
             return self
 
         def set_barnesHutKV(self, key:str, value):
             """
```

### Comparing `pyvisjs-0.0.0.dev7/pyvisjs/utils.py` & `pyvisjs-0.0.0.dev8/pyvisjs/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import subprocess
 import os
 
 
 def open_file(url):
     """
-    :param url: web url or a file path on your computer
+    Parameters
+    ---------
+    url : str
+        Web url or a file path on your computer
     >>> open_file("https://stackoverflow.com")
     >>> open_file("\\\\pyvisjs\\\\templates\\\\basic.html")  
     """
 
     try: # should work on Windows
         os.startfile(url)
     except AttributeError:
@@ -27,11 +30,11 @@
         relative_path = os.path.join(os.getcwd(), file_path)
         output_dir, file_name = os.path.split(relative_path)
 
     os.makedirs(output_dir, exist_ok=True)
 
     file_path = os.path.join(output_dir, file_name)
 
-    with open(file_path, "w") as f:
+    with open(file_path, "w", encoding="utf-8") as f:
         f.write(file_content)
 
     return file_path
```

### Comparing `pyvisjs-0.0.0.dev7/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-0.0.0.dev8/pyvisjs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev7
+Version: 0.0.0.dev8
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev7/pyvisjs.egg-info/SOURCES.txt` & `pyvisjs-0.0.0.dev8/pyvisjs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .gitlab-ci.yml
 CONTRIBUTING.md
 LICENSE
 README.md
 folder_structure.txt
 pyproject.toml
 requirements.txt
+examples/bluor.py
 examples/main.py
 examples/readme_usage.py
 pyvisjs/__init__.py
 pyvisjs/_version.py
 pyvisjs/base_dictable.py
 pyvisjs/edge.py
 pyvisjs/network.py
@@ -18,14 +19,15 @@
 pyvisjs/utils.py
 pyvisjs.egg-info/PKG-INFO
 pyvisjs.egg-info/SOURCES.txt
 pyvisjs.egg-info/dependency_links.txt
 pyvisjs.egg-info/requires.txt
 pyvisjs.egg-info/top_level.txt
 pyvisjs/templates/basic.html
+pyvisjs/templates/bs-container.html
 tests/__init__.py
 tests/test_base_dictable.py
 tests/test_edge.py
 tests/test_network.py
 tests/test_node.py
 tests/test_options.py
 tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev7/tests/test_base_dictable.py` & `pyvisjs-0.0.0.dev8/tests/test_base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/tests/test_edge.py` & `pyvisjs-0.0.0.dev8/tests/test_edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/tests/test_network.py` & `pyvisjs-0.0.0.dev8/tests/test_network.py`

 * *Files 13% similar despite different names*

```diff
@@ -153,14 +153,58 @@
     n.add_edge(1, 2) # both nodes exist
     n.add_edge(2, 3) # one node missing
     n.add_edge(2, 3) # duplicate edge
     
     # assert
     assert n.to_dict() == NETWORK_DICT
 
+@patch('pyvisjs.network.Environment')
+def test_network_render_template_passing_render_default_params(mock_Environment):
+    # init
+    WIDTH="100%"
+    HEIGHT="100%"
+    DATA={"nodes": [], "edges": [], "options": {}}
+    PYVISJS={
+        "enable_highlighting": False,
+    }
+    
+    # mock
+    mock_render = mock_Environment.return_value.get_template.return_value.render
+
+    # call
+    network = Network("Test Network")
+    html_output = network.render_template() # <--------------------
+
+    # assert
+    mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
+
+@patch('pyvisjs.network.Environment')
+def test_network_render_template_passing_render_params(mock_Environment):
+    # init
+    WIDTH="100%"
+    HEIGHT="100%"
+    DATA={"nodes": [], "edges": [], "options": {}}
+    TEMPLATE_FILENAME="another_template.html"
+    ENABLE_HIGHLIGHTING=True
+    PYVISJS={
+        "enable_highlighting": ENABLE_HIGHLIGHTING,
+    }
+    
+    # mock
+    mock_get_template = mock_Environment.return_value.get_template
+    mock_render = mock_get_template.return_value.render
+
+    # call
+    network = Network("Test Network")
+    html_output = network.render_template(template_filename=TEMPLATE_FILENAME, enable_highlighting=ENABLE_HIGHLIGHTING) # <--------------------
+
+    # assert
+    mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
+    mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
+
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
 @patch('pyvisjs.network.Environment')
 def test_network_render_template_with_all_default_values(mock_Environment, mock_save_file, mock_open_file):
     # init
     RENDER_RESULT = "<html>template</html>"
     DEFAULT_TEMPLATE_FILENAME = "basic.html"
```

### Comparing `pyvisjs-0.0.0.dev7/tests/test_node.py` & `pyvisjs-0.0.0.dev8/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev7/tests/test_options.py` & `pyvisjs-0.0.0.dev8/tests/test_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,16 @@
 def test_options_bluor_use_case():
     # init
     OPTIONS_DICT = {
         "configure": {
             "enabled": False
         },
         "edges": {
+            "arrows": "to",
+            "arrowStrikethrough": False,
             "color": {
                 "inherit": True
             },
             "smooth": {
                 "enabled": True,
                 "type": "dynamic"
             }
@@ -135,15 +137,16 @@
     # call
     options = Options()
     options \
         .set_configure(enabled=False) \
         .set_interaction(dragNodes=True, hideEdgesOnDrag=False, hideNodesOnDrag=False)
     options.edges \
         .set_color(inherit=True) \
-        .set_smooth(type="dynamic", enabled=True)
+        .set_smooth(type="dynamic", enabled=True) \
+        .set(arrows="to", arrowStrikethrough=False)
     options.physics \
         .set(enabled=True) \
         .set_barnesHut(avoidOverlap=0, centralGravity=0.3, damping=1, gravitationalConstant=-2750, springConstant=0, springLength=250) \
         .set_stabilization(enabled=True, fit=True, iterations=1000, onlyDynamicEdges=False, updateInterval=50)
     
     # assert
     assert options.to_dict() == OPTIONS_DICT
```

### Comparing `pyvisjs-0.0.0.dev7/tests/test_utils.py` & `pyvisjs-0.0.0.dev8/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     # call
     file_result = save_file("output.html", "<html>hello</html>") # <------------------
 
     # assert
     mock_getcwd.assert_called_once()
     mock_makedirs.assert_called_once_with(DIR_PATH, exist_ok=True)
-    mock_open.assert_called_once_with(FULL_PATH, "w")
+    mock_open.assert_called_once_with(FULL_PATH, "w", encoding="utf-8")
     mock_write.assert_called_once_with("<html>hello</html>")
     assert file_result == FULL_PATH
 
 
 @patch("os.makedirs")
 @patch("builtins.open")
 @patch("os.getcwd")
@@ -42,15 +42,15 @@
 
     # call
     file_result = save_file(REL_PATH, "<html>hello</html>") # <------------------
 
     # assert
     mock_getcwd.assert_called_once()
     mock_makedirs.assert_called_once_with(DIR_PATH, exist_ok=True)
-    mock_open.assert_called_once_with(FULL_PATH, "w")
+    mock_open.assert_called_once_with(FULL_PATH, "w", encoding="utf-8")
     mock_write.assert_called_once_with("<html>hello</html>")
     assert file_result == FULL_PATH
 
 
 @patch("os.makedirs")
 @patch("builtins.open")
 @patch("os.getcwd")
@@ -68,10 +68,10 @@
 
     # call
     file_result = save_file(FULL_PATH, "<html>hello</html>") # <------------------
 
     # assert
     mock_getcwd.assert_not_called()
     mock_makedirs.assert_called_once_with(DIR_PATH, exist_ok=True)
-    mock_open.assert_called_once_with(FULL_PATH, "w")
+    mock_open.assert_called_once_with(FULL_PATH, "w", encoding="utf-8")
     mock_write.assert_called_once_with("<html>hello</html>")
     assert file_result == FULL_PATH
```

