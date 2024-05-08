# Comparing `tmp/skywatch-0.1.3.tar.gz` & `tmp/skywatch-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skywatch-0.1.3.tar", last modified: Mon May  6 23:46:13 2024, max compression
+gzip compressed data, was "skywatch-0.1.4.tar", last modified: Wed May  8 02:43:44 2024, max compression
```

## Comparing `skywatch-0.1.3.tar` & `skywatch-0.1.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.991994 skywatch-0.1.3/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1070 2024-04-04 01:44:39.000000 skywatch-0.1.3/LICENSE.md
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      485 2024-05-06 23:46:13.991994 skywatch-0.1.3/PKG-INFO
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      743 2024-04-04 04:24:08.000000 skywatch-0.1.3/README.md
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       38 2024-05-06 23:46:13.991994 skywatch-0.1.3/setup.cfg
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      609 2024-05-06 23:46:12.000000 skywatch-0.1.3/setup.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.983994 skywatch-0.1.3/skywatch/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       95 2024-05-06 23:43:15.000000 skywatch-0.1.3/skywatch/__init__.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.983994 skywatch-0.1.3/skywatch/access/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       70 2024-05-06 23:43:54.000000 skywatch-0.1.3/skywatch/access/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    11674 2024-05-06 23:41:52.000000 skywatch-0.1.3/skywatch/access/access.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      810 2024-04-04 01:53:30.000000 skywatch-0.1.3/skywatch/access/base_constraint.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.983994 skywatch-0.1.3/skywatch/access/constraints/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      105 2024-03-26 04:27:30.000000 skywatch-0.1.3/skywatch/access/constraints/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3004 2024-05-06 02:41:19.000000 skywatch-0.1.3/skywatch/access/constraints/az_el_range.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6186 2024-03-26 04:27:30.000000 skywatch-0.1.3/skywatch/access/constraints/line_of_sight.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2189 2024-03-26 04:27:30.000000 skywatch-0.1.3/skywatch/access/constraints/temporal.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.987994 skywatch-0.1.3/skywatch/attitude/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       72 2024-03-26 04:27:30.000000 skywatch-0.1.3/skywatch/attitude/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      677 2024-03-26 04:27:30.000000 skywatch-0.1.3/skywatch/attitude/base_attitude.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.987994 skywatch-0.1.3/skywatch/attitude/builtins/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       77 2024-03-26 04:27:30.000000 skywatch-0.1.3/skywatch/attitude/builtins/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      525 2024-03-26 04:27:30.000000 skywatch-0.1.3/skywatch/attitude/builtins/fixed.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4437 2024-03-28 04:43:15.000000 skywatch-0.1.3/skywatch/attitude/builtins/lvlh.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      640 2024-03-26 04:27:30.000000 skywatch-0.1.3/skywatch/attitude/builtins/slerped.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.987994 skywatch-0.1.3/skywatch/look_angles/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      107 2024-03-26 22:07:28.000000 skywatch-0.1.3/skywatch/look_angles/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      195 2024-03-17 22:41:05.000000 skywatch-0.1.3/skywatch/look_angles/aert.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      680 2024-04-04 02:04:42.000000 skywatch-0.1.3/skywatch/look_angles/base_look_angle.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.987994 skywatch-0.1.3/skywatch/look_angles/builtins/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      102 2024-04-04 02:45:14.000000 skywatch-0.1.3/skywatch/look_angles/builtins/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6306 2024-04-04 02:44:33.000000 skywatch-0.1.3/skywatch/look_angles/builtins/default_look_strategy.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2390 2024-04-04 02:44:16.000000 skywatch-0.1.3/skywatch/look_angles/builtins/local_tangent_enu.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.987994 skywatch-0.1.3/skywatch/skypath/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       29 2024-03-26 04:27:30.000000 skywatch-0.1.3/skywatch/skypath/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5378 2024-04-04 02:42:47.000000 skywatch-0.1.3/skywatch/skypath/creation.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     8338 2024-04-04 02:43:16.000000 skywatch-0.1.3/skywatch/skypath/skypath.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.987994 skywatch-0.1.3/skywatch/time/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       44 2024-05-06 23:44:37.000000 skywatch-0.1.3/skywatch/time/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      640 2024-05-06 23:41:53.000000 skywatch-0.1.3/skywatch/time/interval.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.987994 skywatch-0.1.3/skywatch/utils/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       30 2024-03-17 22:41:05.000000 skywatch-0.1.3/skywatch/utils/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    11347 2024-05-06 23:45:18.000000 skywatch-0.1.3/skywatch/utils/coverage.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4103 2024-04-04 03:45:44.000000 skywatch-0.1.3/skywatch/utils/funcs.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.983994 skywatch-0.1.3/skywatch.egg-info/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      485 2024-05-06 23:46:13.000000 skywatch-0.1.3/skywatch.egg-info/PKG-INFO
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1250 2024-05-06 23:46:13.000000 skywatch-0.1.3/skywatch.egg-info/SOURCES.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2024-05-06 23:46:13.000000 skywatch-0.1.3/skywatch.egg-info/dependency_links.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       41 2024-05-06 23:46:13.000000 skywatch-0.1.3/skywatch.egg-info/requires.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       15 2024-05-06 23:46:13.000000 skywatch-0.1.3/skywatch.egg-info/top_level.txt
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 23:46:13.991994 skywatch-0.1.3/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2024-03-26 04:36:18.000000 skywatch-0.1.3/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1811 2024-04-04 01:37:37.000000 skywatch-0.1.3/tests/geovista_example.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     9876 2024-04-04 02:56:41.000000 skywatch-0.1.3/tests/test_look_angles.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     7334 2024-05-06 02:41:19.000000 skywatch-0.1.3/tests/test_smoke.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1583 2024-03-26 04:27:30.000000 skywatch-0.1.3/tests/utils.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1070 2024-04-04 01:44:39.000000 skywatch-0.1.4/LICENSE.md
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      485 2024-05-08 02:43:44.772999 skywatch-0.1.4/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      743 2024-04-04 04:24:08.000000 skywatch-0.1.4/README.md
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       38 2024-05-08 02:43:44.772999 skywatch-0.1.4/setup.cfg
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      609 2024-05-08 02:43:20.000000 skywatch-0.1.4/setup.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/skywatch/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       95 2024-05-06 23:43:15.000000 skywatch-0.1.4/skywatch/__init__.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/skywatch/access/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       70 2024-05-06 23:43:54.000000 skywatch-0.1.4/skywatch/access/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    11683 2024-05-08 02:42:17.000000 skywatch-0.1.4/skywatch/access/access.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      810 2024-04-04 01:53:30.000000 skywatch-0.1.4/skywatch/access/base_constraint.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/skywatch/access/constraints/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      105 2024-03-26 04:27:30.000000 skywatch-0.1.4/skywatch/access/constraints/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3004 2024-05-06 02:41:19.000000 skywatch-0.1.4/skywatch/access/constraints/az_el_range.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6186 2024-03-26 04:27:30.000000 skywatch-0.1.4/skywatch/access/constraints/line_of_sight.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2189 2024-03-26 04:27:30.000000 skywatch-0.1.4/skywatch/access/constraints/temporal.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/skywatch/attitude/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       72 2024-03-26 04:27:30.000000 skywatch-0.1.4/skywatch/attitude/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      677 2024-03-26 04:27:30.000000 skywatch-0.1.4/skywatch/attitude/base_attitude.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/skywatch/attitude/builtins/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       77 2024-03-26 04:27:30.000000 skywatch-0.1.4/skywatch/attitude/builtins/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      525 2024-03-26 04:27:30.000000 skywatch-0.1.4/skywatch/attitude/builtins/fixed.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4437 2024-03-28 04:43:15.000000 skywatch-0.1.4/skywatch/attitude/builtins/lvlh.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      640 2024-03-26 04:27:30.000000 skywatch-0.1.4/skywatch/attitude/builtins/slerped.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/skywatch/look_angles/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      107 2024-03-26 22:07:28.000000 skywatch-0.1.4/skywatch/look_angles/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      195 2024-03-17 22:41:05.000000 skywatch-0.1.4/skywatch/look_angles/aert.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      680 2024-04-04 02:04:42.000000 skywatch-0.1.4/skywatch/look_angles/base_look_angle.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/skywatch/look_angles/builtins/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      102 2024-04-04 02:45:14.000000 skywatch-0.1.4/skywatch/look_angles/builtins/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6306 2024-04-04 02:44:33.000000 skywatch-0.1.4/skywatch/look_angles/builtins/default_look_strategy.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2390 2024-04-04 02:44:16.000000 skywatch-0.1.4/skywatch/look_angles/builtins/local_tangent_enu.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/skywatch/skypath/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       29 2024-03-26 04:27:30.000000 skywatch-0.1.4/skywatch/skypath/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5378 2024-04-04 02:42:47.000000 skywatch-0.1.4/skywatch/skypath/creation.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     8338 2024-04-04 02:43:16.000000 skywatch-0.1.4/skywatch/skypath/skypath.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/skywatch/time/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       44 2024-05-06 23:44:37.000000 skywatch-0.1.4/skywatch/time/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      640 2024-05-06 23:41:53.000000 skywatch-0.1.4/skywatch/time/interval.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/skywatch/utils/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       30 2024-03-17 22:41:05.000000 skywatch-0.1.4/skywatch/utils/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    11347 2024-05-06 23:45:18.000000 skywatch-0.1.4/skywatch/utils/coverage.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4103 2024-04-04 03:45:44.000000 skywatch-0.1.4/skywatch/utils/funcs.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/skywatch.egg-info/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      485 2024-05-08 02:43:44.000000 skywatch-0.1.4/skywatch.egg-info/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1250 2024-05-08 02:43:44.000000 skywatch-0.1.4/skywatch.egg-info/SOURCES.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2024-05-08 02:43:44.000000 skywatch-0.1.4/skywatch.egg-info/dependency_links.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       41 2024-05-08 02:43:44.000000 skywatch-0.1.4/skywatch.egg-info/requires.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       15 2024-05-08 02:43:44.000000 skywatch-0.1.4/skywatch.egg-info/top_level.txt
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-08 02:43:44.772999 skywatch-0.1.4/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2024-03-26 04:36:18.000000 skywatch-0.1.4/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1811 2024-04-04 01:37:37.000000 skywatch-0.1.4/tests/geovista_example.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     9876 2024-04-04 02:56:41.000000 skywatch-0.1.4/tests/test_look_angles.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     7334 2024-05-06 02:41:19.000000 skywatch-0.1.4/tests/test_smoke.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1583 2024-03-26 04:27:30.000000 skywatch-0.1.4/tests/utils.py
```

### Comparing `skywatch-0.1.3/LICENSE.md` & `skywatch-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/README.md` & `skywatch-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/setup.py` & `skywatch-0.1.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="skywatch",
-    version="0.1.3",
+    version="0.1.4",
     url="https://github.com/nsspencer/SkyWatch",
     author="Nathan Spencer",
     description="Aerospace/astrodynamics analysis library providing high level interfaces for coordinate, attitude, access, and look angle calculations.",
     packages=find_packages(),
     install_requires=["astropy", "numpy", "portion", "scipy", "pymap3d", "tqdm"],
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `skywatch-0.1.3/skywatch/access/access.py` & `skywatch-0.1.4/skywatch/access/access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import List
 
 import astropy.units as u
 import numpy as np
 import portion as P
 from astropy.time import Time
 
+from skywatch.time.interval import Interval
+
 from .base_constraint import BaseAccessConstraint
-from .time_interval import Interval
 
 
 class Access:
     def __init__(self, *constraints) -> None:
         """
         Access is used to calculate times when all provided constraints
         are satisfied.
```

### Comparing `skywatch-0.1.3/skywatch/access/base_constraint.py` & `skywatch-0.1.4/skywatch/access/base_constraint.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/access/constraints/az_el_range.py` & `skywatch-0.1.4/skywatch/access/constraints/az_el_range.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/access/constraints/line_of_sight.py` & `skywatch-0.1.4/skywatch/access/constraints/line_of_sight.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/access/constraints/temporal.py` & `skywatch-0.1.4/skywatch/access/constraints/temporal.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/attitude/base_attitude.py` & `skywatch-0.1.4/skywatch/attitude/base_attitude.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/attitude/builtins/fixed.py` & `skywatch-0.1.4/skywatch/attitude/builtins/fixed.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/attitude/builtins/lvlh.py` & `skywatch-0.1.4/skywatch/attitude/builtins/lvlh.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/attitude/builtins/slerped.py` & `skywatch-0.1.4/skywatch/attitude/builtins/slerped.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/look_angles/base_look_angle.py` & `skywatch-0.1.4/skywatch/look_angles/base_look_angle.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/look_angles/builtins/default_look_strategy.py` & `skywatch-0.1.4/skywatch/look_angles/builtins/default_look_strategy.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/look_angles/builtins/local_tangent_enu.py` & `skywatch-0.1.4/skywatch/look_angles/builtins/local_tangent_enu.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/skypath/creation.py` & `skywatch-0.1.4/skywatch/skypath/creation.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/skypath/skypath.py` & `skywatch-0.1.4/skywatch/skypath/skypath.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/time/interval.py` & `skywatch-0.1.4/skywatch/time/interval.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/utils/coverage.py` & `skywatch-0.1.4/skywatch/utils/coverage.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch/utils/funcs.py` & `skywatch-0.1.4/skywatch/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/skywatch.egg-info/SOURCES.txt` & `skywatch-0.1.4/skywatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/tests/geovista_example.py` & `skywatch-0.1.4/tests/geovista_example.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/tests/test_look_angles.py` & `skywatch-0.1.4/tests/test_look_angles.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/tests/test_smoke.py` & `skywatch-0.1.4/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.3/tests/utils.py` & `skywatch-0.1.4/tests/utils.py`

 * *Files identical despite different names*

