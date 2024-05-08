# Comparing `tmp/grasp_planning-0.4.1.tar.gz` & `tmp/grasp_planning-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.4.1.tar", last modified: Wed May  8 08:45:27 2024, max compression
+gzip compressed data, was "grasp_planning-0.4.2.tar", last modified: Wed May  8 08:46:34 2024, max compression
```

## Comparing `grasp_planning-0.4.1.tar` & `grasp_planning-0.4.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:45:27.709557 grasp_planning-0.4.1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      267 2024-05-08 08:45:27.709557 grasp_planning-0.4.1/PKG-INFO
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:45:27.709557 grasp_planning-0.4.1/grasp_planning/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2024-05-07 16:34:01.000000 grasp_planning-0.4.1/grasp_planning/__init__.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:45:27.709557 grasp_planning-0.4.1/grasp_planning/constraints/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2024-05-03 09:25:11.000000 grasp_planning-0.4.1/grasp_planning/constraints/collision_constraint.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      271 2024-05-07 16:07:10.000000 grasp_planning-0.4.1/grasp_planning/constraints/constraint_template.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      252 2024-05-08 08:42:32.000000 grasp_planning-0.4.1/grasp_planning/constraints/constraints.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1434 2024-05-07 16:34:01.000000 grasp_planning-0.4.1/grasp_planning/constraints/grasp_pos_constraint.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3156 2024-05-07 16:34:01.000000 grasp_planning-0.4.1/grasp_planning/constraints/grasp_rot_constraint.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1037 2024-05-07 16:34:01.000000 grasp_planning-0.4.1/grasp_planning/constraints/manipulation_constraint.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:45:27.709557 grasp_planning-0.4.1/grasp_planning/cost/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       65 2024-05-07 16:34:01.000000 grasp_planning-0.4.1/grasp_planning/cost/costs.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2024-05-02 12:00:02.000000 grasp_planning-0.4.1/grasp_planning/cost/dist_to_home.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1439 2024-04-18 15:29:48.000000 grasp_planning-0.4.1/grasp_planning/cost/squared_acc_cost.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:45:27.709557 grasp_planning-0.4.1/grasp_planning/solver/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5714 2024-05-07 16:34:01.000000 grasp_planning-0.4.1/grasp_planning/solver/gomp_planner.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1736 2024-05-08 08:42:59.000000 grasp_planning-0.4.1/grasp_planning/solver/robot_model.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:45:27.709557 grasp_planning-0.4.1/grasp_planning.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      267 2024-05-08 08:45:27.000000 grasp_planning-0.4.1/grasp_planning.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      718 2024-05-08 08:45:27.000000 grasp_planning-0.4.1/grasp_planning.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-05-08 08:45:27.000000 grasp_planning-0.4.1/grasp_planning.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      100 2024-05-08 08:45:27.000000 grasp_planning-0.4.1/grasp_planning.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2024-05-08 08:45:27.000000 grasp_planning-0.4.1/grasp_planning.egg-info/top_level.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      428 2024-05-08 08:41:47.000000 grasp_planning-0.4.1/pyproject.toml
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2024-05-08 08:45:27.709557 grasp_planning-0.4.1/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      714 2024-05-08 08:45:23.000000 grasp_planning-0.4.1/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      267 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/PKG-INFO
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/grasp_planning/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/__init__.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/grasp_planning/constraints/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2024-05-03 09:25:11.000000 grasp_planning-0.4.2/grasp_planning/constraints/collision_constraint.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      271 2024-05-07 16:07:10.000000 grasp_planning-0.4.2/grasp_planning/constraints/constraint_template.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      252 2024-05-08 08:42:32.000000 grasp_planning-0.4.2/grasp_planning/constraints/constraints.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1434 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/constraints/grasp_pos_constraint.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3156 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/constraints/grasp_rot_constraint.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1037 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/constraints/manipulation_constraint.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/grasp_planning/cost/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       65 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/cost/costs.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2024-05-02 12:00:02.000000 grasp_planning-0.4.2/grasp_planning/cost/dist_to_home.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1439 2024-04-18 15:29:48.000000 grasp_planning-0.4.2/grasp_planning/cost/squared_acc_cost.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/grasp_planning/solver/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5714 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/solver/gomp_planner.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1736 2024-05-08 08:42:59.000000 grasp_planning-0.4.2/grasp_planning/solver/robot_model.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/grasp_planning.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      267 2024-05-08 08:46:34.000000 grasp_planning-0.4.2/grasp_planning.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      718 2024-05-08 08:46:34.000000 grasp_planning-0.4.2/grasp_planning.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-05-08 08:46:34.000000 grasp_planning-0.4.2/grasp_planning.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      100 2024-05-08 08:46:34.000000 grasp_planning-0.4.2/grasp_planning.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2024-05-08 08:46:34.000000 grasp_planning-0.4.2/grasp_planning.egg-info/top_level.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      428 2024-05-08 08:41:47.000000 grasp_planning-0.4.2/pyproject.toml
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      714 2024-05-08 08:46:09.000000 grasp_planning-0.4.2/setup.py
```

### Comparing `grasp_planning-0.4.1/grasp_planning/constraints/grasp_pos_constraint.py` & `grasp_planning-0.4.2/grasp_planning/constraints/grasp_pos_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.4.1/grasp_planning/constraints/grasp_rot_constraint.py` & `grasp_planning-0.4.2/grasp_planning/constraints/grasp_rot_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.4.1/grasp_planning/constraints/manipulation_constraint.py` & `grasp_planning-0.4.2/grasp_planning/constraints/manipulation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.4.1/grasp_planning/cost/squared_acc_cost.py` & `grasp_planning-0.4.2/grasp_planning/cost/squared_acc_cost.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.4.1/grasp_planning/solver/gomp_planner.py` & `grasp_planning-0.4.2/grasp_planning/solver/gomp_planner.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.4.1/grasp_planning/solver/robot_model.py` & `grasp_planning-0.4.2/grasp_planning/solver/robot_model.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.4.1/grasp_planning.egg-info/SOURCES.txt` & `grasp_planning-0.4.2/grasp_planning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.4.1/setup.py` & `grasp_planning-0.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,23 +7,23 @@
  'grasp_planning.cost',
  'grasp_planning.solver']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['casadi>3.5',
+['casadi>3.6',
  'forwardkinematics>=1.1.3',
  'numpy>=1.15.3,<2.0.0',
  'scipy<=1.10.1',
  'spatial-casadi>=1.1.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'grasp_planning',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': '"Grasp and Motion Planning Python Package."',
     'author': 'Tomas Merva',
     'author_email': 'tmerva7@gmail.com',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<3.10',
```

