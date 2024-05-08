# Comparing `tmp/frccontrol-2024.19.tar.gz` & `tmp/frccontrol-2024.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frccontrol-2024.19.tar", last modified: Sat Jan  6 08:20:53 2024, max compression
+gzip compressed data, was "frccontrol-2024.20.tar", last modified: Wed May  8 18:48:48 2024, max compression
```

## Comparing `frccontrol-2024.19.tar` & `frccontrol-2024.20.tar`

### file list

```diff
@@ -1,39 +1,30 @@
-drwxr-xr-x   0 tav       (1000) users      (984)        0 2024-01-06 08:20:53.843121 frccontrol-2024.19/
--rw-r--r--   0 tav       (1000) users      (984)       66 2023-06-27 21:44:56.000000 frccontrol-2024.19/.gitignore
--rw-r--r--   0 tav       (1000) users      (984)    21157 2023-03-18 04:18:42.000000 frccontrol-2024.19/.pylintrc
--rw-r--r--   0 tav       (1000) users      (984)     1457 2023-06-27 21:44:56.000000 frccontrol-2024.19/LICENSE.txt
--rw-r--r--   0 tav       (1000) users      (984)     1151 2024-01-06 08:20:53.843121 frccontrol-2024.19/PKG-INFO
--rw-r--r--   0 tav       (1000) users      (984)      383 2022-11-10 21:45:34.000000 frccontrol-2024.19/README.rst
-drwxr-xr-x   0 tav       (1000) users      (984)        0 2024-01-06 08:20:53.843121 frccontrol-2024.19/examples/
--rwxr-xr-x   0 tav       (1000) users      (984)     3875 2023-03-28 17:13:57.000000 frccontrol-2024.19/examples/differential_drive.py
--rwxr-xr-x   0 tav       (1000) users      (984)    10415 2023-04-24 20:42:51.000000 frccontrol-2024.19/examples/double_jointed_arm.py
--rwxr-xr-x   0 tav       (1000) users      (984)     2979 2023-03-28 17:14:28.000000 frccontrol-2024.19/examples/elevator.py
--rwxr-xr-x   0 tav       (1000) users      (984)     2905 2023-03-28 17:14:37.000000 frccontrol-2024.19/examples/flywheel.py
--rwxr-xr-x   0 tav       (1000) users      (984)     2989 2023-03-28 17:14:47.000000 frccontrol-2024.19/examples/single_jointed_arm.py
-drwxr-xr-x   0 tav       (1000) users      (984)        0 2024-01-06 08:20:53.843121 frccontrol-2024.19/frccontrol/
--rw-r--r--   0 tav       (1000) users      (984)      427 2023-04-24 20:42:51.000000 frccontrol-2024.19/frccontrol/__init__.py
--rw-r--r--   0 tav       (1000) users      (984)     1865 2023-03-17 22:26:57.000000 frccontrol-2024.19/frccontrol/ctrlutil.py
--rw-r--r--   0 tav       (1000) users      (984)     2240 2023-03-19 21:39:39.000000 frccontrol-2024.19/frccontrol/discretization.py
--rw-r--r--   0 tav       (1000) users      (984)     4252 2023-03-26 17:19:21.000000 frccontrol-2024.19/frccontrol/extended_kalman_filter.py
--rw-r--r--   0 tav       (1000) users      (984)     2587 2023-03-17 22:26:57.000000 frccontrol-2024.19/frccontrol/kalman_filter.py
--rw-r--r--   0 tav       (1000) users      (984)     1484 2023-03-17 22:26:57.000000 frccontrol-2024.19/frccontrol/linear_plant_inversion_feedforward.py
--rw-r--r--   0 tav       (1000) users      (984)     2797 2023-03-17 22:26:57.000000 frccontrol-2024.19/frccontrol/linear_quadratic_regulator.py
--rw-r--r--   0 tav       (1000) users      (984)     6150 2023-03-26 01:10:05.000000 frccontrol-2024.19/frccontrol/models.py
--rw-r--r--   0 tav       (1000) users      (984)     3980 2023-03-26 22:28:18.000000 frccontrol-2024.19/frccontrol/numerical_integration.py
--rw-r--r--   0 tav       (1000) users      (984)     1518 2023-03-15 05:59:43.000000 frccontrol-2024.19/frccontrol/numerical_jacobian.py
--rw-r--r--   0 tav       (1000) users      (984)     3193 2023-03-28 17:13:23.000000 frccontrol-2024.19/frccontrol/plotutil.py
--rw-r--r--   0 tav       (1000) users      (984)     4462 2023-03-15 06:00:03.000000 frccontrol-2024.19/frccontrol/profiles.py
-drwxr-xr-x   0 tav       (1000) users      (984)        0 2024-01-06 08:20:53.843121 frccontrol-2024.19/frccontrol/test/
--rw-r--r--   0 tav       (1000) users      (984)        0 2022-10-01 04:59:40.000000 frccontrol-2024.19/frccontrol/test/__init__.py
--rw-r--r--   0 tav       (1000) users      (984)      654 2022-10-01 05:01:04.000000 frccontrol-2024.19/frccontrol/test/test_numerical_jacobian.py
--rw-r--r--   0 tav       (1000) users      (984)     8039 2023-04-24 20:42:51.000000 frccontrol-2024.19/frccontrol/trajectory.py
--rw-r--r--   0 tav       (1000) users      (984)      789 2023-06-27 23:01:49.000000 frccontrol-2024.19/frccontrol/version.py
-drwxr-xr-x   0 tav       (1000) users      (984)        0 2024-01-06 08:20:53.843121 frccontrol-2024.19/frccontrol.egg-info/
--rw-r--r--   0 tav       (1000) users      (984)     1151 2024-01-06 08:20:53.000000 frccontrol-2024.19/frccontrol.egg-info/PKG-INFO
--rw-r--r--   0 tav       (1000) users      (984)      868 2024-01-06 08:20:53.000000 frccontrol-2024.19/frccontrol.egg-info/SOURCES.txt
--rw-r--r--   0 tav       (1000) users      (984)        1 2024-01-06 08:20:53.000000 frccontrol-2024.19/frccontrol.egg-info/dependency_links.txt
--rw-r--r--   0 tav       (1000) users      (984)       23 2024-01-06 08:20:53.000000 frccontrol-2024.19/frccontrol.egg-info/requires.txt
--rw-r--r--   0 tav       (1000) users      (984)       11 2024-01-06 08:20:53.000000 frccontrol-2024.19/frccontrol.egg-info/top_level.txt
--rwxr-xr-x   0 tav       (1000) users      (984)      636 2023-06-27 22:12:58.000000 frccontrol-2024.19/publish-frccontrol.sh
--rw-r--r--   0 tav       (1000) users      (984)     1086 2024-01-06 08:17:19.000000 frccontrol-2024.19/pyproject.toml
--rw-r--r--   0 tav       (1000) users      (984)       38 2024-01-06 08:20:53.843121 frccontrol-2024.19/setup.cfg
+drwxr-xr-x   0 tav       (1000) users      (984)        0 2024-05-08 18:48:48.593825 frccontrol-2024.20/
+-rw-r--r--   0 tav       (1000) users      (984)     1457 2023-06-27 21:44:56.000000 frccontrol-2024.20/LICENSE.txt
+-rw-r--r--   0 tav       (1000) users      (984)     1151 2024-05-08 18:48:48.593825 frccontrol-2024.20/PKG-INFO
+-rw-r--r--   0 tav       (1000) users      (984)      383 2022-11-10 21:45:34.000000 frccontrol-2024.20/README.rst
+drwxr-xr-x   0 tav       (1000) users      (984)        0 2024-05-08 18:48:48.593825 frccontrol-2024.20/frccontrol/
+-rw-r--r--   0 tav       (1000) users      (984)      427 2023-04-24 20:42:51.000000 frccontrol-2024.20/frccontrol/__init__.py
+-rw-r--r--   0 tav       (1000) users      (984)     1865 2023-03-17 22:26:57.000000 frccontrol-2024.20/frccontrol/ctrlutil.py
+-rw-r--r--   0 tav       (1000) users      (984)     2240 2023-03-19 21:39:39.000000 frccontrol-2024.20/frccontrol/discretization.py
+-rw-r--r--   0 tav       (1000) users      (984)     4252 2023-03-26 17:19:21.000000 frccontrol-2024.20/frccontrol/extended_kalman_filter.py
+-rw-r--r--   0 tav       (1000) users      (984)     2587 2023-03-17 22:26:57.000000 frccontrol-2024.20/frccontrol/kalman_filter.py
+-rw-r--r--   0 tav       (1000) users      (984)     1484 2023-03-17 22:26:57.000000 frccontrol-2024.20/frccontrol/linear_plant_inversion_feedforward.py
+-rw-r--r--   0 tav       (1000) users      (984)     2797 2023-03-17 22:26:57.000000 frccontrol-2024.20/frccontrol/linear_quadratic_regulator.py
+-rw-r--r--   0 tav       (1000) users      (984)     6150 2023-03-26 01:10:05.000000 frccontrol-2024.20/frccontrol/models.py
+-rw-r--r--   0 tav       (1000) users      (984)     3980 2023-03-26 22:28:18.000000 frccontrol-2024.20/frccontrol/numerical_integration.py
+-rw-r--r--   0 tav       (1000) users      (984)     1518 2023-03-15 05:59:43.000000 frccontrol-2024.20/frccontrol/numerical_jacobian.py
+-rw-r--r--   0 tav       (1000) users      (984)     3193 2023-03-28 17:13:23.000000 frccontrol-2024.20/frccontrol/plotutil.py
+-rw-r--r--   0 tav       (1000) users      (984)     4462 2023-03-15 06:00:03.000000 frccontrol-2024.20/frccontrol/profiles.py
+drwxr-xr-x   0 tav       (1000) users      (984)        0 2024-05-08 18:48:48.593825 frccontrol-2024.20/frccontrol/test/
+-rw-r--r--   0 tav       (1000) users      (984)        0 2022-10-01 04:59:40.000000 frccontrol-2024.20/frccontrol/test/__init__.py
+-rw-r--r--   0 tav       (1000) users      (984)      654 2022-10-01 05:01:04.000000 frccontrol-2024.20/frccontrol/test/test_numerical_jacobian.py
+-rw-r--r--   0 tav       (1000) users      (984)     8039 2023-04-24 20:42:51.000000 frccontrol-2024.20/frccontrol/trajectory.py
+-rw-r--r--   0 tav       (1000) users      (984)      789 2023-06-27 23:01:49.000000 frccontrol-2024.20/frccontrol/version.py
+drwxr-xr-x   0 tav       (1000) users      (984)        0 2024-05-08 18:48:48.593825 frccontrol-2024.20/frccontrol.egg-info/
+-rw-r--r--   0 tav       (1000) users      (984)     1151 2024-05-08 18:48:48.000000 frccontrol-2024.20/frccontrol.egg-info/PKG-INFO
+-rw-r--r--   0 tav       (1000) users      (984)      690 2024-05-08 18:48:48.000000 frccontrol-2024.20/frccontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 tav       (1000) users      (984)        1 2024-05-08 18:48:48.000000 frccontrol-2024.20/frccontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 tav       (1000) users      (984)       23 2024-05-08 18:48:48.000000 frccontrol-2024.20/frccontrol.egg-info/requires.txt
+-rw-r--r--   0 tav       (1000) users      (984)       11 2024-05-08 18:48:48.000000 frccontrol-2024.20/frccontrol.egg-info/top_level.txt
+-rw-r--r--   0 tav       (1000) users      (984)     1086 2024-01-06 08:17:19.000000 frccontrol-2024.20/pyproject.toml
+-rw-r--r--   0 tav       (1000) users      (984)       38 2024-05-08 18:48:48.593825 frccontrol-2024.20/setup.cfg
```

### Comparing `frccontrol-2024.19/LICENSE.txt` & `frccontrol-2024.20/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/PKG-INFO` & `frccontrol-2024.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frccontrol
-Version: 2024.19
+Version: 2024.20
 Summary: Provides SciPy wrappers for easing development of state-space models for the FIRST Robotics Competition
 Author-email: Tyler Veness <calcmogul@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/calcmogul/frccontrol
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `frccontrol-2024.19/frccontrol/ctrlutil.py` & `frccontrol-2024.20/frccontrol/ctrlutil.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/discretization.py` & `frccontrol-2024.20/frccontrol/discretization.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/extended_kalman_filter.py` & `frccontrol-2024.20/frccontrol/extended_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/kalman_filter.py` & `frccontrol-2024.20/frccontrol/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/linear_plant_inversion_feedforward.py` & `frccontrol-2024.20/frccontrol/linear_plant_inversion_feedforward.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/linear_quadratic_regulator.py` & `frccontrol-2024.20/frccontrol/linear_quadratic_regulator.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/models.py` & `frccontrol-2024.20/frccontrol/models.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/numerical_integration.py` & `frccontrol-2024.20/frccontrol/numerical_integration.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/numerical_jacobian.py` & `frccontrol-2024.20/frccontrol/numerical_jacobian.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/plotutil.py` & `frccontrol-2024.20/frccontrol/plotutil.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/profiles.py` & `frccontrol-2024.20/frccontrol/profiles.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/test/test_numerical_jacobian.py` & `frccontrol-2024.20/frccontrol/test/test_numerical_jacobian.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/trajectory.py` & `frccontrol-2024.20/frccontrol/trajectory.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol/version.py` & `frccontrol-2024.20/frccontrol/version.py`

 * *Files identical despite different names*

### Comparing `frccontrol-2024.19/frccontrol.egg-info/PKG-INFO` & `frccontrol-2024.20/frccontrol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frccontrol
-Version: 2024.19
+Version: 2024.20
 Summary: Provides SciPy wrappers for easing development of state-space models for the FIRST Robotics Competition
 Author-email: Tyler Veness <calcmogul@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/calcmogul/frccontrol
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `frccontrol-2024.19/frccontrol.egg-info/SOURCES.txt` & `frccontrol-2024.20/frccontrol.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-.gitignore
-.pylintrc
 LICENSE.txt
 README.rst
-publish-frccontrol.sh
 pyproject.toml
-examples/differential_drive.py
-examples/double_jointed_arm.py
-examples/elevator.py
-examples/flywheel.py
-examples/single_jointed_arm.py
 frccontrol/__init__.py
 frccontrol/ctrlutil.py
 frccontrol/discretization.py
 frccontrol/extended_kalman_filter.py
 frccontrol/kalman_filter.py
 frccontrol/linear_plant_inversion_feedforward.py
 frccontrol/linear_quadratic_regulator.py
```

### Comparing `frccontrol-2024.19/pyproject.toml` & `frccontrol-2024.20/pyproject.toml`

 * *Files identical despite different names*

