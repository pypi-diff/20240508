# Comparing `tmp/FlowVisor-0.1.0.tar.gz` & `tmp/FlowVisor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.1.0.tar", last modified: Thu Apr 25 10:37:12 2024, max compression
+gzip compressed data, was "FlowVisor-0.1.2.tar", last modified: Thu Apr 25 13:22:21 2024, max compression
```

## Comparing `FlowVisor-0.1.0.tar` & `FlowVisor-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     2800 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      471 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       99 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       52 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-04-25 10:37:12.000000 FlowVisor-0.1.0/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.0/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     2800 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     2119 2024-04-23 15:17:49.000000 FlowVisor-0.1.0/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-04-25 10:31:59.000000 FlowVisor-0.1.0/flowvisor/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/flowvisor/cli/
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.0/flowvisor/cli/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 10:17:04.000000 FlowVisor-0.1.0/flowvisor/cli/add_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2080 2024-04-25 10:34:16.000000 FlowVisor-0.1.0/flowvisor/cli/remove_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    11506 2024-04-25 09:23:49.000000 FlowVisor-0.1.0/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      838 2024-04-25 09:21:07.000000 FlowVisor-0.1.0/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     7439 2024-04-25 09:18:55.000000 FlowVisor-0.1.0/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2644 2024-04-23 20:23:57.000000 FlowVisor-0.1.0/flowvisor/time_tracker.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      299 2024-04-23 18:54:33.000000 FlowVisor-0.1.0/flowvisor/timer.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     1386 2024-04-25 09:19:05.000000 FlowVisor-0.1.0/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-04-25 10:37:12.300068 FlowVisor-0.1.0/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1533 2024-04-25 10:19:31.000000 FlowVisor-0.1.0/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 13:22:21.813190 FlowVisor-0.1.2/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 13:22:21.813190 FlowVisor-0.1.2/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-04-25 13:22:21.000000 FlowVisor-0.1.2/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      497 2024-04-25 13:22:21.000000 FlowVisor-0.1.2/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-04-25 13:22:21.000000 FlowVisor-0.1.2/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-04-25 13:22:21.000000 FlowVisor-0.1.2/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       52 2024-04-25 13:22:21.000000 FlowVisor-0.1.2/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-04-25 13:22:21.000000 FlowVisor-0.1.2/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.2/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-04-25 13:22:21.813190 FlowVisor-0.1.2/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.2/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 13:22:21.813190 FlowVisor-0.1.2/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      180 2024-04-25 12:58:27.000000 FlowVisor-0.1.2/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-25 13:22:21.813190 FlowVisor-0.1.2/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.2/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.2/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.2/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.2/flowvisor/cli/vis_file.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    12115 2024-04-25 12:48:55.000000 FlowVisor-0.1.2/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      881 2024-04-25 12:51:47.000000 FlowVisor-0.1.2/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8042 2024-04-25 13:20:09.000000 FlowVisor-0.1.2/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.2/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      299 2024-04-23 18:54:33.000000 FlowVisor-0.1.2/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2088 2024-04-25 12:36:32.000000 FlowVisor-0.1.2/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-04-25 13:22:21.813190 FlowVisor-0.1.2/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.2/setup.py
```

### Comparing `FlowVisor-0.1.0/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.1.2/FlowVisor.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.0
+Version: 0.1.2
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
@@ -40,20 +40,25 @@
    <a href="https://github.com/cophilot/FlowVisor/commits/master">
        <img src="https://img.shields.io/github/last-commit/cophilot/FlowVisor" alt="last commit" />
    </a>
 </div>
 
 ---
 
-## ![FlowVisor-Example](https://raw.githubusercontent.com/cophilot/FlowVisor/main/assets/example.png)
+![FlowVisor-Example](https://raw.githubusercontent.com/cophilot/FlowVisor/main/assets/example.png)
 
 ---
 
 -   [Installation](#installation)
 -   [Usage](#usage)
+-   [CLI](#cli)
+    -   [add-vis](#add-vis)
+    -   [remove-vis](#remove-vis)
+    -   [vis-file](#vis-file)
+-   [Overhead](#overhead)
 -   [Development](#development)
 -   [Example](#example)
 
 ---
 
 ## Installation
 
@@ -74,21 +79,61 @@
 
 @vis
 def my_other_function():
     my_function()
 
 my_other_function()
 FlowVisor.CONFIG.output_file = "example_graph" # You can add some configureation with the CONFIG object
-FlowVisor.generate_graph() # Generate the graph
-FlowVisor.save_flow("example_flow", "json") # Save the flow as json
+FlowVisor.graph() # Generate the graph
+FlowVisor.export("example_flow", "json") # Save the flow as json
 
 ```
 
 ---
 
+## CLI
+
+### add-vis
+
+Adds the vis decorator to all functions in all python files in a directory.
+
+```bash
+add-vis -p <path-to-dir>
+```
+
+### remove-vis
+
+Removes the vis decorator from all functions in all python files in a directory.
+
+```bash
+remove-vis -p <path-to-dir>
+```
+
+### vis-file
+
+Generate a graph from a exported flow file.
+
+```bash
+vis-file -f <path-to-flow-file>
+```
+
+---
+
+## Overhead
+
+The overhead of the FlowVisor is tried to be kept as low as possible. The overhead is mainly caused by the decorator. Therefore the time for running the logic of the Flowvisor is excluded from the profiling.
+
+You can even descrease the overhead by the `advanced_ovhead_reduction`:
+
+```python
+FlowVisor.enable_advanced_overhead_reduction()
+```
+
+---
+
 ## Development
 
 ```bash
 git clone https://github.com/cophilot/FlowVisor
 cd FlowVisor
 pip install -r requirements.txt
 ```
@@ -96,14 +141,15 @@
 ---
 
 ## Example
 
 Run the example:
 
 ```python
+pip install -r requirements.txt
 python example.py
 ```
 
 ---
 
 <!-- ## Bugs
```

### Comparing `FlowVisor-0.1.0/LICENSE` & `FlowVisor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.0/PKG-INFO` & `FlowVisor-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.0
+Version: 0.1.2
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
@@ -40,20 +40,25 @@
    <a href="https://github.com/cophilot/FlowVisor/commits/master">
        <img src="https://img.shields.io/github/last-commit/cophilot/FlowVisor" alt="last commit" />
    </a>
 </div>
 
 ---
 
-## ![FlowVisor-Example](https://raw.githubusercontent.com/cophilot/FlowVisor/main/assets/example.png)
+![FlowVisor-Example](https://raw.githubusercontent.com/cophilot/FlowVisor/main/assets/example.png)
 
 ---
 
 -   [Installation](#installation)
 -   [Usage](#usage)
+-   [CLI](#cli)
+    -   [add-vis](#add-vis)
+    -   [remove-vis](#remove-vis)
+    -   [vis-file](#vis-file)
+-   [Overhead](#overhead)
 -   [Development](#development)
 -   [Example](#example)
 
 ---
 
 ## Installation
 
@@ -74,21 +79,61 @@
 
 @vis
 def my_other_function():
     my_function()
 
 my_other_function()
 FlowVisor.CONFIG.output_file = "example_graph" # You can add some configureation with the CONFIG object
-FlowVisor.generate_graph() # Generate the graph
-FlowVisor.save_flow("example_flow", "json") # Save the flow as json
+FlowVisor.graph() # Generate the graph
+FlowVisor.export("example_flow", "json") # Save the flow as json
 
 ```
 
 ---
 
+## CLI
+
+### add-vis
+
+Adds the vis decorator to all functions in all python files in a directory.
+
+```bash
+add-vis -p <path-to-dir>
+```
+
+### remove-vis
+
+Removes the vis decorator from all functions in all python files in a directory.
+
+```bash
+remove-vis -p <path-to-dir>
+```
+
+### vis-file
+
+Generate a graph from a exported flow file.
+
+```bash
+vis-file -f <path-to-flow-file>
+```
+
+---
+
+## Overhead
+
+The overhead of the FlowVisor is tried to be kept as low as possible. The overhead is mainly caused by the decorator. Therefore the time for running the logic of the Flowvisor is excluded from the profiling.
+
+You can even descrease the overhead by the `advanced_ovhead_reduction`:
+
+```python
+FlowVisor.enable_advanced_overhead_reduction()
+```
+
+---
+
 ## Development
 
 ```bash
 git clone https://github.com/cophilot/FlowVisor
 cd FlowVisor
 pip install -r requirements.txt
 ```
@@ -96,14 +141,15 @@
 ---
 
 ## Example
 
 Run the example:
 
 ```python
+pip install -r requirements.txt
 python example.py
 ```
 
 ---
 
 <!-- ## Bugs
```

### Comparing `FlowVisor-0.1.0/README.md` & `FlowVisor-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -21,20 +21,25 @@
    <a href="https://github.com/cophilot/FlowVisor/commits/master">
        <img src="https://img.shields.io/github/last-commit/cophilot/FlowVisor" alt="last commit" />
    </a>
 </div>
 
 ---
 
-## ![FlowVisor-Example](https://raw.githubusercontent.com/cophilot/FlowVisor/main/assets/example.png)
+![FlowVisor-Example](https://raw.githubusercontent.com/cophilot/FlowVisor/main/assets/example.png)
 
 ---
 
 -   [Installation](#installation)
 -   [Usage](#usage)
+-   [CLI](#cli)
+    -   [add-vis](#add-vis)
+    -   [remove-vis](#remove-vis)
+    -   [vis-file](#vis-file)
+-   [Overhead](#overhead)
 -   [Development](#development)
 -   [Example](#example)
 
 ---
 
 ## Installation
 
@@ -55,21 +60,61 @@
 
 @vis
 def my_other_function():
     my_function()
 
 my_other_function()
 FlowVisor.CONFIG.output_file = "example_graph" # You can add some configureation with the CONFIG object
-FlowVisor.generate_graph() # Generate the graph
-FlowVisor.save_flow("example_flow", "json") # Save the flow as json
+FlowVisor.graph() # Generate the graph
+FlowVisor.export("example_flow", "json") # Save the flow as json
 
 ```
 
 ---
 
+## CLI
+
+### add-vis
+
+Adds the vis decorator to all functions in all python files in a directory.
+
+```bash
+add-vis -p <path-to-dir>
+```
+
+### remove-vis
+
+Removes the vis decorator from all functions in all python files in a directory.
+
+```bash
+remove-vis -p <path-to-dir>
+```
+
+### vis-file
+
+Generate a graph from a exported flow file.
+
+```bash
+vis-file -f <path-to-flow-file>
+```
+
+---
+
+## Overhead
+
+The overhead of the FlowVisor is tried to be kept as low as possible. The overhead is mainly caused by the decorator. Therefore the time for running the logic of the Flowvisor is excluded from the profiling.
+
+You can even descrease the overhead by the `advanced_ovhead_reduction`:
+
+```python
+FlowVisor.enable_advanced_overhead_reduction()
+```
+
+---
+
 ## Development
 
 ```bash
 git clone https://github.com/cophilot/FlowVisor
 cd FlowVisor
 pip install -r requirements.txt
 ```
@@ -77,14 +122,15 @@
 ---
 
 ## Example
 
 Run the example:
 
 ```python
+pip install -r requirements.txt
 python example.py
 ```
 
 ---
 
 <!-- ## Bugs
```

### Comparing `FlowVisor-0.1.0/flowvisor/cli/add_vis.py` & `FlowVisor-0.1.2/flowvisor/cli/add_vis.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 IMPORT_STATEMENT = "from flowvisor import vis"
 DECORATOR = "@vis"
 
 def add_decorator(dir_path="."):
     for root, dirs, files in os.walk(dir_path):
         if ignore_dir(os.path.basename(root)):
             continue
-                
+
         for file in files:
             if not file.endswith(".py"):
                 continue
             handle_file(root, file)
+    print("Done")
 
 def handle_file(root, file):
     # read contents of the file
     file_path = os.path.join(root, file)
     with open(file_path, "r") as f:
         lines = f.readlines()
     
@@ -75,15 +76,16 @@
         return True
     return False
 
 def is_function(line):
     return line.strip().startswith("def ") and line.strip().endswith(":")
 
 def main():
-
+    print("This script will add the vis decorator to all python files in the provided directory.")
+    print("Visit https://github.com/cophilot/FlowVisor#cli for more information.")
     # check if the path is provided as an argument
     args = sys.argv
     for index, arg in enumerate(args):
         if arg == "-path" or arg == "-p":
             dir_path = args[index + 1]
             if os.path.exists(dir_path):
                 add_decorator(dir_path)
```

### Comparing `FlowVisor-0.1.0/flowvisor/cli/remove_vis.py` & `FlowVisor-0.1.2/flowvisor/cli/remove_vis.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 IMPORT_STATEMENT = "from flowvisor import vis"
 DECORATOR = "@vis"
 
 def remove_decorator(dir_path="."):
     for root, dirs, files in os.walk(dir_path):
         if ignore_dir(os.path.basename(root)):
             continue
-                
+
         for file in files:
             if not file.endswith(".py"):
                 continue
             handle_file(root, file)
+    print("Done")
 
 def handle_file(root, file):
     # read contents of the file
     file_path = os.path.join(root, file)
     with open(file_path, "r") as f:
         lines = f.readlines()
 
@@ -27,15 +28,15 @@
             continue
         if line.strip() == IMPORT_STATEMENT:
             continue
         new_content.append(line)
 
     with open(file_path, "w") as f:
         f.writelines(new_content)
-    print(f"Removed vis to {file_path}")
+    print(f"Removed vis from {file_path}")
 
 def ignore_dir(dir_name):
     if dir_name.endswith("__pycache__"):
         return True
     if dir_name.endswith("venv"):
         return True
     if dir_name.endswith(".git"):
@@ -46,15 +47,16 @@
         return True
     return False
 
 def is_function(line):
     return line.strip().startswith("def ") and line.strip().endswith(":")
 
 def main():
-
+    print("This script will remove the vis decorator from all python files in the provided directory.")
+    print("Visit https://github.com/cophilot/FlowVisor#cli for more information.")
     # check if the path is provided as an argument
     args = sys.argv
     for index, arg in enumerate(args):
         if arg == "-path" or arg == "-p":
             dir_path = args[index + 1]
             if os.path.exists(dir_path):
                 remove_decorator(dir_path)
```

### Comparing `FlowVisor-0.1.0/flowvisor/flowvisor.py` & `FlowVisor-0.1.2/flowvisor/flowvisor.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,32 +17,34 @@
 
 def vis(func):
     """
     Decorator that visualizes the function.
     """
     def wrapper(*args, **kwargs):
         TimeTracker.stop()
-        if FlowVisor.CONFIG.reduce_overhead:
+
+        reduce_overhead = FlowVisor.CONFIG.reduce_overhead
+        if reduce_overhead:
             TimeTracker.apply(advanced=FlowVisor.get_advanced_overhead_reduction())
             timer_id = TimeTracker.register_new_timer()
 
         FlowVisor.function_called(func)
 
-        start = TimeTracker.start()
+        start = TimeTracker.start(reduce_overhead)
         result = func(*args, **kwargs)
         end = TimeTracker.stop()
 
         duration = end - start
-        if FlowVisor.CONFIG.reduce_overhead:
+        if reduce_overhead:
             TimeTracker.apply(advanced=FlowVisor.get_advanced_overhead_reduction())
             duration = TimeTracker.get_time_and_remove_timer(timer_id)
 
         FlowVisor.function_returned(func, duration)
-        
-        TimeTracker.start()
+
+        TimeTracker.start(reduce_overhead)
         return result
     return wrapper
 
 class FlowVisor:
     """
     The FlowVisor class is responsible for managing the flow of the functions 
     and generating the graph.
@@ -119,19 +121,17 @@
 
         try:
             with Diagram(FlowVisor.CONFIG.graph_title,
                          show=FlowVisor.CONFIG.show_graph,
                          filename=FlowVisor.CONFIG.output_file,
                          direction="LR"):
 
-                FunctionNode.make_node_image_cache()
+                blank_image = FunctionNode.make_node_image_cache()
 
-                if FlowVisor.CONFIG.add_timestamp:
-                    timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-                    Custom(str(timestamp), "", width="0.001", height="0.001")
+                FlowVisor.draw_meta_data(blank_image)
 
                 if FlowVisor.CONFIG.logo != "":
                     Custom("", FlowVisor.CONFIG.logo,
                            width=FlowVisor.CONFIG.get_node_scale(),
                            height=FlowVisor.CONFIG.get_node_scale())
 
                 # Draw nodes
@@ -142,20 +142,36 @@
                         FlowVisor.draw_function_node(n, highest_time)
 
         finally:
             # Make sure to clear the cache always
             FunctionNode.clear_node_image_cache()
 
     @staticmethod
+    def draw_meta_data(blank_image):
+        """
+        Draws some metadata on the graph.
+        """
+        with Cluster("Metadata", graph_attr={"bgcolor": "#FFFFFF"}):
+            if FlowVisor.CONFIG.add_system_info:
+                sys_info = utils.get_sys_info()
+                text = ""
+                for key, value in sys_info.items():
+                    text += f"{key}: {value}\n"
+                Custom(text, blank_image, width="6", height="1")
+            if FlowVisor.CONFIG.add_timestamp:
+                timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+                Custom(str(timestamp), blank_image, width="3", height="0.2")
+
+    @staticmethod
     def draw_nodes_with_cluster(nodes: List[FunctionNode], highest_time: float):
         """
         Draws the nodes with cluster.
         """
         sorted_nodes = FlowVisor.get_node_sorted_by_filename(nodes)
-        total_times = [sum([n.time for n in row]) for row in sorted_nodes]
+        total_times = [sum([n.get_time_without_children() for n in row]) for row in sorted_nodes]
         highest_time_file_time = max(total_times)
         for index, row in enumerate(sorted_nodes):
             cluster_title = f"{row[0].file_name} ({utils.get_time_as_string(total_times[index])})"
             bg_color = utils.value_to_hex_color(total_times[index], highest_time_file_time,
                                                 light_color=[0xFF, 0xFF, 0xFF],
                                                 dark_color=[0xAA, 0xAA, 0xAA])
             font_color = utils.value_to_hex_color(total_times[index], highest_time_file_time,
```

### Comparing `FlowVisor-0.1.0/flowvisor/flowvisor_config.py` & `FlowVisor-0.1.2/flowvisor/flowvisor_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         self.node_scale: float = 2.0
         self.node_show_file: bool = True
         self.node_show_call_count: bool = True
         self.node_show_avg_time: bool = True
         self.static_font_color: str = ""
         self.reduce_overhead: bool = True
         self.add_timestamp: bool = False
+        self.add_system_info: bool = False
         self.advanced_overhead_reduction = None
         self.group_nodes: bool = False
         self.dev_mode: bool = False
 
     def get_node_scale(self):
         """
         Get the node scale as a string
```

### Comparing `FlowVisor-0.1.0/flowvisor/function_node.py` & `FlowVisor-0.1.2/flowvisor/function_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,21 +211,42 @@
         """
         self.children = []
         for child_id in self.children_ids:
             for node in all_nodes:
                 if node.uuid == child_id:
                     self.add_child(node)
 
+    def get_time_without_children(self):
+        """
+        Gets the time without the children.
+        """
+        time = self.time
+        for child in self.children:
+            time -= child.time
+        return time
+
     @staticmethod
     def make_node_image_cache():
         """
         Makes the node image cache.
+        
+        Returns:
+            The file name of the blank image.
         """
         os.makedirs(FunctionNode.NODE_IMAGE_CACHE, exist_ok=True)
 
+        FunctionNode.NODE_IMAGE_CACHE = os.path.abspath(FunctionNode.NODE_IMAGE_CACHE)
+
+        dim = FunctionNode.NODE_IMAGE_SCALE
+        image = Image.new('RGB', (dim, dim), 'white')
+
+        file_name = f"{FunctionNode.NODE_IMAGE_CACHE}/_blank.png"
+        image.save(file_name)
+        return file_name
+
     @staticmethod
     def clear_node_image_cache():
         """
         Clears the node image cache.
         """
         for file in os.listdir(FunctionNode.NODE_IMAGE_CACHE):
             os.remove(f"{FunctionNode.NODE_IMAGE_CACHE}/{file}")
```

### Comparing `FlowVisor-0.1.0/flowvisor/time_tracker.py` & `FlowVisor-0.1.2/flowvisor/time_tracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def stop():
         """
         Stops the time tracker.
         
         Returns:
             The end time.
         """
-
+        # no code here!
         end = time.time()
         TimeTracker.END_TIME = end
         return end
 
     @staticmethod
     def apply(advanced = None):
         """
@@ -35,27 +35,28 @@
             interval_time = interval_time - (advanced * 2)
 
         TimeTracker.add_time_to_all_timers(interval_time)
         TimeTracker.START_TIME = None
         TimeTracker.END_TIME = None
 
     @staticmethod
-    def start():
+    def start(reduce_overhead: bool):
         """
         Starts the time tracker.
         
         Returns:
             The start time.
         """
 
-        if TimeTracker.START_TIME is not None:
+        if reduce_overhead and TimeTracker.START_TIME is not None:
             print("[FlowVisor.INTERNAL] Time tracker is already running.")
             return TimeTracker.START_TIME
 
         TimeTracker.START_TIME = time.time()
+        # no code here!
         return TimeTracker.START_TIME
 
     @staticmethod
     def add_time_to_all_timers(t: float):
         """
         Adds time to all timers.
```

### Comparing `FlowVisor-0.1.0/setup.py` & `FlowVisor-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,13 +41,14 @@
         'Operating System :: Unix',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
     ],
     entry_points={
         'console_scripts': [
             'add-vis=flowvisor.cli.add_vis:main',
-            'remove-vis=flowvisor.cli.remove_vis:main'
+            'remove-vis=flowvisor.cli.remove_vis:main',
+            'vis-file=flowvisor.cli.vis_file:main'
         ]
     }
 )
```

