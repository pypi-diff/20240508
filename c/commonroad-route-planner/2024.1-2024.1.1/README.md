# Comparing `tmp/commonroad_route_planner-2024.1.tar.gz` & `tmp/commonroad_route_planner-2024.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonroad_route_planner-2024.1.tar", max compression
+gzip compressed data, was "commonroad_route_planner-2024.1.1.tar", max compression
```

## Comparing `commonroad_route_planner-2024.1.tar` & `commonroad_route_planner-2024.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1582 2024-03-11 09:43:01.345238 commonroad_route_planner-2024.1/LICENSE.txt
--rw-r--r--   0        0        0     1959 2024-03-12 14:35:33.012194 commonroad_route_planner-2024.1/README.md
--rw-r--r--   0        0        0        0 2024-03-12 15:16:43.096955 commonroad_route_planner-2024.1/commonroad_route_planner/__init__.py
--rw-r--r--   0        0        0        0 2024-03-12 15:16:43.100955 commonroad_route_planner-2024.1/commonroad_route_planner/frenet_tools/__init__.py
--rw-r--r--   0        0        0     7735 2024-03-12 14:09:56.790750 commonroad_route_planner-2024.1/commonroad_route_planner/frenet_tools/route_extendor.py
--rw-r--r--   0        0        0     7440 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1/commonroad_route_planner/frenet_tools/route_slice.py
--rw-r--r--   0        0        0        0 2024-03-12 15:16:43.100955 commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/__init__.py
--rw-r--r--   0        0        0     1577 2024-03-12 14:09:56.790750 commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/change_instruction.py
--rw-r--r--   0        0        0     3975 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/change_position.py
--rw-r--r--   0        0        0    12678 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/lane_change_handler.py
--rw-r--r--   0        0        0        0 2024-03-12 15:16:43.100955 commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/lane_change_methods/__init__.py
--rw-r--r--   0        0        0     3099 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/lane_change_methods/method_interface.py
--rw-r--r--   0        0        0     2566 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/lane_change_methods/polynomial_change.py
--rw-r--r--   0        0        0     8728 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1/commonroad_route_planner/map_matching.py
--rw-r--r--   0        0        0        0 2024-03-12 15:16:43.100955 commonroad_route_planner-2024.1/commonroad_route_planner/planners/__init__.py
--rw-r--r--   0        0        0     1111 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1/commonroad_route_planner/planners/base_route_planner.py
--rw-r--r--   0        0        0     7959 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1/commonroad_route_planner/planners/networkx.py
--rw-r--r--   0        0        0     4141 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1/commonroad_route_planner/planners/no_goal_found_planner.py
--rw-r--r--   0        0        0     2877 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1/commonroad_route_planner/route.py
--rw-r--r--   0        0        0     1205 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1/commonroad_route_planner/route_candidate_holder.py
--rw-r--r--   0        0        0        0 2024-03-12 15:16:43.100955 commonroad_route_planner-2024.1/commonroad_route_planner/route_generation_strategies/__init__.py
--rw-r--r--   0        0        0     1104 2024-03-12 10:06:16.420238 commonroad_route_planner-2024.1/commonroad_route_planner/route_generation_strategies/base_generation_strategy.py
--rw-r--r--   0        0        0    11887 2024-03-12 13:30:57.085067 commonroad_route_planner-2024.1/commonroad_route_planner/route_generation_strategies/default_generation_strategy.py
--rw-r--r--   0        0        0    11031 2024-03-12 13:30:57.085067 commonroad_route_planner-2024.1/commonroad_route_planner/route_generator.py
--rw-r--r--   0        0        0    13605 2024-03-12 13:49:15.893663 commonroad_route_planner-2024.1/commonroad_route_planner/route_planner.py
--rw-r--r--   0        0        0        0 2024-03-12 15:16:43.100955 commonroad_route_planner-2024.1/commonroad_route_planner/route_sections/__init__.py
--rw-r--r--   0        0        0     3448 2024-03-12 14:09:56.790750 commonroad_route_planner-2024.1/commonroad_route_planner/route_sections/lanelet_section.py
--rw-r--r--   0        0        0        0 2024-03-12 15:16:43.100955 commonroad_route_planner-2024.1/commonroad_route_planner/utility/__init__.py
--rw-r--r--   0        0        0      241 2023-10-24 16:01:39.313676 commonroad_route_planner-2024.1/commonroad_route_planner/utility/exceptions.py
--rw-r--r--   0        0        0      772 2024-03-12 13:30:57.085067 commonroad_route_planner-2024.1/commonroad_route_planner/utility/overtake_init_state.py
--rw-r--r--   0        0        0        0 2024-03-12 15:16:43.100955 commonroad_route_planner-2024.1/commonroad_route_planner/utility/polyline_operations/__init__.py
--rw-r--r--   0        0        0     5336 2024-03-12 14:09:56.790750 commonroad_route_planner-2024.1/commonroad_route_planner/utility/polyline_operations/polyline_operations.py
--rw-r--r--   0        0        0     5928 2024-03-12 13:30:57.085067 commonroad_route_planner-2024.1/commonroad_route_planner/utility/route_util.py
--rw-r--r--   0        0        0     8400 2024-03-12 13:30:57.085067 commonroad_route_planner-2024.1/commonroad_route_planner/utility/visualization.py
--rw-r--r--   0        0        0     1496 2024-03-12 14:09:56.790750 commonroad_route_planner-2024.1/pyproject.toml
--rw-r--r--   0        0        0     3053 1970-01-01 00:00:00.000000 commonroad_route_planner-2024.1/PKG-INFO
+-rw-r--r--   0        0        0     1582 2024-03-11 09:43:01.345238 commonroad_route_planner-2024.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1959 2024-03-12 14:35:33.012194 commonroad_route_planner-2024.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-22 13:49:01.358648 commonroad_route_planner-2024.1.1/commonroad_route_planner/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 13:49:01.358648 commonroad_route_planner-2024.1.1/commonroad_route_planner/frenet_tools/__init__.py
+-rw-r--r--   0        0        0     7735 2024-03-12 14:09:56.790750 commonroad_route_planner-2024.1.1/commonroad_route_planner/frenet_tools/route_extendor.py
+-rw-r--r--   0        0        0     7440 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1.1/commonroad_route_planner/frenet_tools/route_slice.py
+-rw-r--r--   0        0        0        0 2024-03-22 13:49:01.358648 commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/__init__.py
+-rw-r--r--   0        0        0     1577 2024-03-12 14:09:56.790750 commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/change_instruction.py
+-rw-r--r--   0        0        0     3975 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/change_position.py
+-rw-r--r--   0        0        0    12678 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/lane_change_handler.py
+-rw-r--r--   0        0        0        0 2024-03-22 13:49:01.358648 commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/lane_change_methods/__init__.py
+-rw-r--r--   0        0        0     3099 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/lane_change_methods/method_interface.py
+-rw-r--r--   0        0        0     2566 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/lane_change_methods/polynomial_change.py
+-rw-r--r--   0        0        0     8728 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1.1/commonroad_route_planner/map_matching.py
+-rw-r--r--   0        0        0        0 2024-03-22 13:49:01.358648 commonroad_route_planner-2024.1.1/commonroad_route_planner/planners/__init__.py
+-rw-r--r--   0        0        0     1111 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1.1/commonroad_route_planner/planners/base_route_planner.py
+-rw-r--r--   0        0        0     7959 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1.1/commonroad_route_planner/planners/networkx.py
+-rw-r--r--   0        0        0     4141 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1.1/commonroad_route_planner/planners/no_goal_found_planner.py
+-rw-r--r--   0        0        0     2877 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1.1/commonroad_route_planner/route.py
+-rw-r--r--   0        0        0     1205 2024-03-12 13:30:57.081067 commonroad_route_planner-2024.1.1/commonroad_route_planner/route_candidate_holder.py
+-rw-r--r--   0        0        0        0 2024-03-22 13:49:01.358648 commonroad_route_planner-2024.1.1/commonroad_route_planner/route_generation_strategies/__init__.py
+-rw-r--r--   0        0        0     1104 2024-03-12 10:06:16.420238 commonroad_route_planner-2024.1.1/commonroad_route_planner/route_generation_strategies/base_generation_strategy.py
+-rw-r--r--   0        0        0    11887 2024-03-12 13:30:57.085067 commonroad_route_planner-2024.1.1/commonroad_route_planner/route_generation_strategies/default_generation_strategy.py
+-rw-r--r--   0        0        0    11031 2024-03-12 13:30:57.085067 commonroad_route_planner-2024.1.1/commonroad_route_planner/route_generator.py
+-rw-r--r--   0        0        0    13607 2024-03-22 13:24:22.309018 commonroad_route_planner-2024.1.1/commonroad_route_planner/route_planner.py
+-rw-r--r--   0        0        0        0 2024-03-22 13:49:01.358648 commonroad_route_planner-2024.1.1/commonroad_route_planner/route_sections/__init__.py
+-rw-r--r--   0        0        0     3448 2024-03-12 14:09:56.790750 commonroad_route_planner-2024.1.1/commonroad_route_planner/route_sections/lanelet_section.py
+-rw-r--r--   0        0        0        0 2024-03-22 13:49:01.358648 commonroad_route_planner-2024.1.1/commonroad_route_planner/utility/__init__.py
+-rw-r--r--   0        0        0      241 2023-10-24 16:01:39.313676 commonroad_route_planner-2024.1.1/commonroad_route_planner/utility/exceptions.py
+-rw-r--r--   0        0        0      772 2024-03-12 13:30:57.085067 commonroad_route_planner-2024.1.1/commonroad_route_planner/utility/overtake_init_state.py
+-rw-r--r--   0        0        0        0 2024-03-22 13:49:01.358648 commonroad_route_planner-2024.1.1/commonroad_route_planner/utility/polyline_operations/__init__.py
+-rw-r--r--   0        0        0     5336 2024-03-12 14:09:56.790750 commonroad_route_planner-2024.1.1/commonroad_route_planner/utility/polyline_operations/polyline_operations.py
+-rw-r--r--   0        0        0     5928 2024-03-12 13:30:57.085067 commonroad_route_planner-2024.1.1/commonroad_route_planner/utility/route_util.py
+-rw-r--r--   0        0        0     8400 2024-03-12 13:30:57.085067 commonroad_route_planner-2024.1.1/commonroad_route_planner/utility/visualization.py
+-rw-r--r--   0        0        0     1499 2024-03-22 13:24:22.313018 commonroad_route_planner-2024.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3047 1970-01-01 00:00:00.000000 commonroad_route_planner-2024.1.1/PKG-INFO
```

### Comparing `commonroad_route_planner-2024.1/LICENSE.txt` & `commonroad_route_planner-2024.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/README.md` & `commonroad_route_planner-2024.1.1/README.md`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/frenet_tools/route_extendor.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/frenet_tools/route_extendor.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/frenet_tools/route_slice.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/frenet_tools/route_slice.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/change_instruction.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/change_instruction.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/change_position.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/change_position.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/lane_change_handler.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/lane_change_handler.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/lane_change_methods/method_interface.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/lane_change_methods/method_interface.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/lane_changing/lane_change_methods/polynomial_change.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/lane_changing/lane_change_methods/polynomial_change.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/map_matching.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/map_matching.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/planners/base_route_planner.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/planners/base_route_planner.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/planners/networkx.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/planners/networkx.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/planners/no_goal_found_planner.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/planners/no_goal_found_planner.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/route.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/route.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/route_candidate_holder.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/route_candidate_holder.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/route_generation_strategies/base_generation_strategy.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/route_generation_strategies/base_generation_strategy.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/route_generation_strategies/default_generation_strategy.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/route_generation_strategies/default_generation_strategy.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/route_generator.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/route_generator.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/route_planner.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/route_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __author__ = (
     "Tobias Mascetta, Daniel Tar, Peter Kocsis, Edmond Irani Liu, Luis Gressenbuch"
 )
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = [""]
-__version__ = "2024.1"
+__version__ = "2024.1.1"
 __maintainer__ = "Tobias Mascetta"
 __email__ = "tobias.mascetta@tum.de"
 __status__ = "Release"
 
 
 import logging
```

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/route_sections/lanelet_section.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/route_sections/lanelet_section.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/utility/overtake_init_state.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/utility/overtake_init_state.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/utility/polyline_operations/polyline_operations.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/utility/polyline_operations/polyline_operations.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/utility/route_util.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/utility/route_util.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/commonroad_route_planner/utility/visualization.py` & `commonroad_route_planner-2024.1.1/commonroad_route_planner/utility/visualization.py`

 * *Files identical despite different names*

### Comparing `commonroad_route_planner-2024.1/pyproject.toml` & `commonroad_route_planner-2024.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "commonroad-route-planner"
-version = "2024.1"
+version = "2024.1.1"
 description = "Route and reference path planning tool for CommonRoad scenarios"
 authors = ["Tobias Mascetta <commonroad@lists.lrz.de>"]
 license = "BSD"
 readme = "README.md"
 
 homepage = "https://commonroad.in.tum.de"
 keywords= ["autonomous", "automated", "vehicles", "driving", "motion", "planning", "prediction"]
@@ -21,15 +21,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 commonroad-io = ">=2022.2"
 networkx = ">=2.4"
 numpy = ">=1.17.4"
 shapely = ">=1.6.4.post2"
 matplotlib = ">=3.1.2"
-commonroad-drivability-checker = "^2023.1"
+commonroad-drivability-checker = ">=2023.1"
 
 # tutorial
 [tool.poetry.group.tutorial]
 optional = true
 
 [tool.poetry.group.tutorial.dependencies]
 jupyter = "^1.0.0"
```

### Comparing `commonroad_route_planner-2024.1/PKG-INFO` & `commonroad_route_planner-2024.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonroad-route-planner
-Version: 2024.1
+Version: 2024.1.1
 Summary: Route and reference path planning tool for CommonRoad scenarios
 Home-page: https://commonroad.in.tum.de
 License: BSD
 Keywords: autonomous,automated,vehicles,driving,motion,planning,prediction
 Author: Tobias Mascetta
 Author-email: commonroad@lists.lrz.de
 Requires-Python: >=3.8,<4.0
@@ -13,15 +13,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: commonroad-drivability-checker (>=2023.1,<2024.0)
+Requires-Dist: commonroad-drivability-checker (>=2023.1)
 Requires-Dist: commonroad-io (>=2022.2)
 Requires-Dist: matplotlib (>=3.1.2)
 Requires-Dist: networkx (>=2.4)
 Requires-Dist: numpy (>=1.17.4)
 Requires-Dist: shapely (>=1.6.4.post2)
 Description-Content-Type: text/markdown
```

