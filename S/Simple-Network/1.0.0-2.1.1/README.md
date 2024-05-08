# Comparing `tmp/Simple-Network-1.0.0.tar.gz` & `tmp/Simple-Network-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Simple-Network-1.0.0.tar", last modified: Thu Apr 11 02:19:13 2024, max compression
+gzip compressed data, was "Simple-Network-2.1.1.tar", last modified: Wed May  8 20:06:37 2024, max compression
```

## Comparing `Simple-Network-1.0.0.tar` & `Simple-Network-2.1.1.tar`

### file list

```diff
@@ -1,21 +1,33 @@
-drwxr-xr-x   0 admin     (1001) root         (0)        0 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/
--rw-r--r--   0 admin     (1001) root         (0)     1065 2024-04-09 17:32:21.000000 Simple-Network-1.0.0/LICENSE
--rw-r--r--   0 admin     (1001) root         (0)    12679 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/PKG-INFO
--rw-r--r--   0 admin     (1001) root         (0)    11615 2024-04-11 01:42:55.000000 Simple-Network-1.0.0/README.md
-drwxr-xr-x   0 admin     (1001) root         (0)        0 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/Simple_Network.egg-info/
--rw-r--r--   0 admin     (1001) root         (0)    12679 2024-04-11 02:19:13.000000 Simple-Network-1.0.0/Simple_Network.egg-info/PKG-INFO
--rw-r--r--   0 admin     (1001) root         (0)      331 2024-04-11 02:19:13.000000 Simple-Network-1.0.0/Simple_Network.egg-info/SOURCES.txt
--rw-r--r--   0 admin     (1001) root         (0)        1 2024-04-11 02:19:13.000000 Simple-Network-1.0.0/Simple_Network.egg-info/dependency_links.txt
--rw-r--r--   0 admin     (1001) root         (0)       28 2024-04-11 02:19:13.000000 Simple-Network-1.0.0/Simple_Network.egg-info/requires.txt
--rw-r--r--   0 admin     (1001) root         (0)        8 2024-04-11 02:19:13.000000 Simple-Network-1.0.0/Simple_Network.egg-info/top_level.txt
--rw-r--r--   0 admin     (1001) root         (0)     1097 2024-04-11 01:14:06.000000 Simple-Network-1.0.0/pyproject.toml
--rw-r--r--   0 admin     (1001) root         (0)       38 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/setup.cfg
--rw-r--r--   0 admin     (1001) root         (0)      668 2024-04-11 01:14:26.000000 Simple-Network-1.0.0/setup.py
-drwxr-xr-x   0 admin     (1001) root         (0)        0 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/simpleN/
--rw-r--r--   0 admin     (1001) root         (0)       97 2024-04-11 02:18:15.000000 Simple-Network-1.0.0/simpleN/__init__.py
--rw-r--r--   0 admin     (1001) root         (0)     8094 2024-04-11 02:12:20.000000 Simple-Network-1.0.0/simpleN/analyze.py
--rw-r--r--   0 admin     (1001) root         (0)    10959 2024-04-11 01:20:00.000000 Simple-Network-1.0.0/simpleN/net.py
--rw-r--r--   0 admin     (1001) root         (0)     3466 2024-04-11 01:20:24.000000 Simple-Network-1.0.0/simpleN/visual.py
-drwxr-xr-x   0 admin     (1001) root         (0)        0 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/tests/
--rw-r--r--   0 admin     (1001) root         (0)     2227 2024-04-11 01:17:15.000000 Simple-Network-1.0.0/tests/test.py
--rw-r--r--   0 admin     (1001) root         (0)     2205 2024-04-11 01:18:27.000000 Simple-Network-1.0.0/tests/test2.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-08 20:06:37.019615 Simple-Network-2.1.1/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-08 20:06:37.015616 Simple-Network-2.1.1/.github/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-08 20:06:37.015616 Simple-Network-2.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 user      (1000) user      (1000)      126 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 user      (1000) user      (1000)     3093 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)     1072 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    13122 2024-05-08 20:06:37.019615 Simple-Network-2.1.1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)    12058 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-08 20:06:37.015616 Simple-Network-2.1.1/Simple_Network.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    13122 2024-05-08 20:06:36.000000 Simple-Network-2.1.1/Simple_Network.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      526 2024-05-08 20:06:36.000000 Simple-Network-2.1.1/Simple_Network.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-08 20:06:36.000000 Simple-Network-2.1.1/Simple_Network.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       13 2024-05-08 20:06:36.000000 Simple-Network-2.1.1/Simple_Network.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2024-05-08 20:06:36.000000 Simple-Network-2.1.1/Simple_Network.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1068 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-05-08 20:06:37.019615 Simple-Network-2.1.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      668 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-08 20:06:37.015616 Simple-Network-2.1.1/simpleN/
+-rw-r--r--   0 user      (1000) user      (1000)      265 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/simpleN/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    16262 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/simpleN/analyze.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-08 20:06:37.019615 Simple-Network-2.1.1/simpleN/link/
+-rw-r--r--   0 user      (1000) user      (1000)      180 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/simpleN/link/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     4998 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/simpleN/link/advance.py
+-rw-r--r--   0 user      (1000) user      (1000)     2614 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/simpleN/link/simple.py
+-rw-r--r--   0 user      (1000) user      (1000)     7028 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/simpleN/link/target.py
+-rw-r--r--   0 user      (1000) user      (1000)     6049 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/simpleN/link/withattrs.py
+-rw-r--r--   0 user      (1000) user      (1000)    18989 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/simpleN/net.py
+-rw-r--r--   0 user      (1000) user      (1000)     4599 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/simpleN/visual.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-08 20:06:37.019615 Simple-Network-2.1.1/tests/
+-rw-r--r--   0 user      (1000) user      (1000)     2227 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/tests/test.py
+-rw-r--r--   0 user      (1000) user      (1000)     2205 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/tests/test2.py
+-rw-r--r--   0 user      (1000) user      (1000)     2249 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/tests/test3.py
+-rw-r--r--   0 user      (1000) user      (1000)     2078 2024-05-08 20:06:16.000000 Simple-Network-2.1.1/tests/test4.py
```

### Comparing `Simple-Network-1.0.0/LICENSE` & `Simple-Network-2.1.1/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 cloner174
+Copyright (c) 2024 Hamed Hajipour
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,9 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
+
```

### Comparing `Simple-Network-1.0.0/PKG-INFO` & `Simple-Network-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Network
-Version: 1.0.0
+Version: 2.1.1
 Summary: A basic tool designed for the construction and visualization of complex, multilayer networks.
 Home-page: https://github.com/cloner174/Simple-Network
 Author: Hamed Hajipour
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Network
 Project-URL: Documentation, https://github.com/cloner174/Simple-Network#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Network
@@ -19,14 +19,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Simple-Network Package
 
+```bash
+        pip install simple-network
+```
 ## Overview
 
 The Simple-Network Package is a powerful tool designed for the construction and visualization of complex, multilayer networks. With an emphasis on ease of use and flexibility, this package allows users to create intricate network structures and render them in stunning 3D using Python. The MultilayerNetwork class is designed to efficiently handle both directed and undirected graphs, support sparse representations for large graphs, and manage attributes for nodes and edges, including the capability to handle inter-layer edges.
 
 ## Core Features of the MultilayerNetwork Class
 
     Initialization and Graph Representation:
@@ -133,30 +136,37 @@
 This package offers comprehensive tools for constructing and visualizing complex multilayer networks in a 3D space. It features two primary components: MultilayerNetwork, for creating the network structure, and Visualize, for rendering the network interactively in 3D.
 
 ## Usage
 **Building a Multilayer Network**
 
 To start building a multilayer network, import the MultilayerNetwork class from the package:
 ```python
-from simpleG import MultilayerNetwork
+from simpleN import MultilayerNetwork
 ```
 *Initialize the network*
 ```
 graph = MultilayerNetwork()
 ```
 *Adding Layers*
 
 ```python
 graph.add_layer(layer_name='Layer_1')
+# Or Simple as :
+graph.add_layer('Layer_1')
+#Both lines above are same as each other!
 ```
 *Adding Nodes*
 
 ```python
 graph.add_node(layer_name='Layer_1', node=1)
 graph.add_node(layer_name='Layer_1', node=4)
+# Or Simple as :
+graph.add_node(1, Layer_1')
+graph.add_node(4, 'Layer_1')
+#Both two ways above are same as each other!
 ```
 *Adding Edges*
 ```python
 graph.add_edge(node1=1, node2=4, layer_name='Layer_1', weight=1)
 ```
 
 *Setting Node and Edge Attributes*
@@ -171,20 +181,20 @@
 To visualize the network in 3D:
 
 ```python
 
 from visualize import Visualize
 
 # Create an instance of Visualize with the network
-visualizer = Visualize(network=graph)
+my_visualizer = Visualize(network=graph)
 
 # Visualize the network
-visualizer.show_graph(edge_visibility_threshold=0.1)
+my_visualizer.show_graph(edge_visibility_threshold=0.1)
 ```
-Alternatively:
+Or Simple as :
 
 ```python
 Visualize(graph).show_graph()
 ```
 ## Examples
 
 For basic usage examples, please refer to the Jupyter Notebook in the Examples folder.
@@ -220,17 +230,17 @@
 
 The Visualize class enables interactive 3D visualization of networks using Plotly.
 
 *Methods:*
 
     show_graph(edge_visibility_threshold=0.1): Renders the network in 3D. Edges below the specified visibility threshold are not displayed.
 
-## Contributing
+## Mistakes and Corrections
 
-We welcome contributions to the MultilayerNetwork Package. Please refer to GitHub contributing guidelines for more information on how to participate in the development.
+To err is human, and nobody likes a perfect person! If you come across any mistakes or if you have questions, feel free to raise an issue or submit a pull request. Your contributions to improving the content are highly appreciated. Please refer to GitHub contributing guidelines for more information on how to participate in the development.
 
 ## License
 
 This project is licensed under the MIT License. For more details, see the LICENSE file in the project repository.
 
 ## Contact
```

### Comparing `Simple-Network-1.0.0/README.md` & `Simple-Network-2.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Simple-Network Package
 
+```bash
+        pip install simple-network
+```
 ## Overview
 
 The Simple-Network Package is a powerful tool designed for the construction and visualization of complex, multilayer networks. With an emphasis on ease of use and flexibility, this package allows users to create intricate network structures and render them in stunning 3D using Python. The MultilayerNetwork class is designed to efficiently handle both directed and undirected graphs, support sparse representations for large graphs, and manage attributes for nodes and edges, including the capability to handle inter-layer edges.
 
 ## Core Features of the MultilayerNetwork Class
 
     Initialization and Graph Representation:
@@ -110,30 +113,37 @@
 This package offers comprehensive tools for constructing and visualizing complex multilayer networks in a 3D space. It features two primary components: MultilayerNetwork, for creating the network structure, and Visualize, for rendering the network interactively in 3D.
 
 ## Usage
 **Building a Multilayer Network**
 
 To start building a multilayer network, import the MultilayerNetwork class from the package:
 ```python
-from simpleG import MultilayerNetwork
+from simpleN import MultilayerNetwork
 ```
 *Initialize the network*
 ```
 graph = MultilayerNetwork()
 ```
 *Adding Layers*
 
 ```python
 graph.add_layer(layer_name='Layer_1')
+# Or Simple as :
+graph.add_layer('Layer_1')
+#Both lines above are same as each other!
 ```
 *Adding Nodes*
 
 ```python
 graph.add_node(layer_name='Layer_1', node=1)
 graph.add_node(layer_name='Layer_1', node=4)
+# Or Simple as :
+graph.add_node(1, Layer_1')
+graph.add_node(4, 'Layer_1')
+#Both two ways above are same as each other!
 ```
 *Adding Edges*
 ```python
 graph.add_edge(node1=1, node2=4, layer_name='Layer_1', weight=1)
 ```
 
 *Setting Node and Edge Attributes*
@@ -148,20 +158,20 @@
 To visualize the network in 3D:
 
 ```python
 
 from visualize import Visualize
 
 # Create an instance of Visualize with the network
-visualizer = Visualize(network=graph)
+my_visualizer = Visualize(network=graph)
 
 # Visualize the network
-visualizer.show_graph(edge_visibility_threshold=0.1)
+my_visualizer.show_graph(edge_visibility_threshold=0.1)
 ```
-Alternatively:
+Or Simple as :
 
 ```python
 Visualize(graph).show_graph()
 ```
 ## Examples
 
 For basic usage examples, please refer to the Jupyter Notebook in the Examples folder.
@@ -197,17 +207,17 @@
 
 The Visualize class enables interactive 3D visualization of networks using Plotly.
 
 *Methods:*
 
     show_graph(edge_visibility_threshold=0.1): Renders the network in 3D. Edges below the specified visibility threshold are not displayed.
 
-## Contributing
+## Mistakes and Corrections
 
-We welcome contributions to the MultilayerNetwork Package. Please refer to GitHub contributing guidelines for more information on how to participate in the development.
+To err is human, and nobody likes a perfect person! If you come across any mistakes or if you have questions, feel free to raise an issue or submit a pull request. Your contributions to improving the content are highly appreciated. Please refer to GitHub contributing guidelines for more information on how to participate in the development.
 
 ## License
 
 This project is licensed under the MIT License. For more details, see the LICENSE file in the project repository.
 
 ## Contact
```

### Comparing `Simple-Network-1.0.0/Simple_Network.egg-info/PKG-INFO` & `Simple-Network-2.1.1/Simple_Network.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Network
-Version: 1.0.0
+Version: 2.1.1
 Summary: A basic tool designed for the construction and visualization of complex, multilayer networks.
 Home-page: https://github.com/cloner174/Simple-Network
 Author: Hamed Hajipour
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Network
 Project-URL: Documentation, https://github.com/cloner174/Simple-Network#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Network
@@ -19,14 +19,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Simple-Network Package
 
+```bash
+        pip install simple-network
+```
 ## Overview
 
 The Simple-Network Package is a powerful tool designed for the construction and visualization of complex, multilayer networks. With an emphasis on ease of use and flexibility, this package allows users to create intricate network structures and render them in stunning 3D using Python. The MultilayerNetwork class is designed to efficiently handle both directed and undirected graphs, support sparse representations for large graphs, and manage attributes for nodes and edges, including the capability to handle inter-layer edges.
 
 ## Core Features of the MultilayerNetwork Class
 
     Initialization and Graph Representation:
@@ -133,30 +136,37 @@
 This package offers comprehensive tools for constructing and visualizing complex multilayer networks in a 3D space. It features two primary components: MultilayerNetwork, for creating the network structure, and Visualize, for rendering the network interactively in 3D.
 
 ## Usage
 **Building a Multilayer Network**
 
 To start building a multilayer network, import the MultilayerNetwork class from the package:
 ```python
-from simpleG import MultilayerNetwork
+from simpleN import MultilayerNetwork
 ```
 *Initialize the network*
 ```
 graph = MultilayerNetwork()
 ```
 *Adding Layers*
 
 ```python
 graph.add_layer(layer_name='Layer_1')
+# Or Simple as :
+graph.add_layer('Layer_1')
+#Both lines above are same as each other!
 ```
 *Adding Nodes*
 
 ```python
 graph.add_node(layer_name='Layer_1', node=1)
 graph.add_node(layer_name='Layer_1', node=4)
+# Or Simple as :
+graph.add_node(1, Layer_1')
+graph.add_node(4, 'Layer_1')
+#Both two ways above are same as each other!
 ```
 *Adding Edges*
 ```python
 graph.add_edge(node1=1, node2=4, layer_name='Layer_1', weight=1)
 ```
 
 *Setting Node and Edge Attributes*
@@ -171,20 +181,20 @@
 To visualize the network in 3D:
 
 ```python
 
 from visualize import Visualize
 
 # Create an instance of Visualize with the network
-visualizer = Visualize(network=graph)
+my_visualizer = Visualize(network=graph)
 
 # Visualize the network
-visualizer.show_graph(edge_visibility_threshold=0.1)
+my_visualizer.show_graph(edge_visibility_threshold=0.1)
 ```
-Alternatively:
+Or Simple as :
 
 ```python
 Visualize(graph).show_graph()
 ```
 ## Examples
 
 For basic usage examples, please refer to the Jupyter Notebook in the Examples folder.
@@ -220,17 +230,17 @@
 
 The Visualize class enables interactive 3D visualization of networks using Plotly.
 
 *Methods:*
 
     show_graph(edge_visibility_threshold=0.1): Renders the network in 3D. Edges below the specified visibility threshold are not displayed.
 
-## Contributing
+## Mistakes and Corrections
 
-We welcome contributions to the MultilayerNetwork Package. Please refer to GitHub contributing guidelines for more information on how to participate in the development.
+To err is human, and nobody likes a perfect person! If you come across any mistakes or if you have questions, feel free to raise an issue or submit a pull request. Your contributions to improving the content are highly appreciated. Please refer to GitHub contributing guidelines for more information on how to participate in the development.
 
 ## License
 
 This project is licensed under the MIT License. For more details, see the LICENSE file in the project repository.
 
 ## Contact
```

### Comparing `Simple-Network-1.0.0/pyproject.toml` & `Simple-Network-2.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple-Network"
-version = "1.0.0"
+version = "2.1.1"
 description = "A basic tool designed for the construction and visualization of complex, multilayer networks."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     { name = "Hamed Hajipour", email = "cloner174.org@gmail.com" },
 ]
 classifiers = [
@@ -19,16 +19,14 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'plotly',
-    'numpy',
-    'scipy',
-    'nbformat'
+    'numpy'
 ]
 [project.urls]
 Homepage = "https://github.com/cloner174/Simple-Network"
 Documentation = "https://github.com/cloner174/Simple-Network#readme"
 Repository = "https://github.com/cloner174/Simple-Network"
 Issues = "https://github.com/cloner174/Simple-Network/issues"
```

### Comparing `Simple-Network-1.0.0/setup.py` & `Simple-Network-2.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Simple-Network',
-    version='1.0.0',
+    version='2.1.1',
     packages=find_packages(),
     author="Hamed Hajipour",
     author_email="cloner174.org@gmail.com",
     description="A basic tool designed for the construction and visualization of complex, multilayer networks.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/cloner174/Simple-Network",
```

### Comparing `Simple-Network-1.0.0/tests/test.py` & `Simple-Network-2.1.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `Simple-Network-1.0.0/tests/test2.py` & `Simple-Network-2.1.1/tests/test2.py`

 * *Files identical despite different names*

