# Comparing `tmp/bamboost-0.6.1.tar.gz` & `tmp/bamboost-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bamboost-0.6.1.tar", last modified: Fri Apr 26 09:04:25 2024, max compression
+gzip compressed data, was "bamboost-0.6.2.tar", last modified: Tue May  7 23:06:34 2024, max compression
```

## Comparing `bamboost-0.6.1.tar` & `bamboost-0.6.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-26 09:04:25.567148 bamboost-0.6.1/
--rw-r--r--   0 florez    (1000) florez    (1000)     1060 2024-01-29 08:07:36.000000 bamboost-0.6.1/LICENSE
--rw-r--r--   0 florez    (1000) florez    (1000)       62 2024-03-05 17:53:33.000000 bamboost-0.6.1/MANIFEST.in
--rw-r--r--   0 florez    (1000) florez    (1000)    13793 2024-04-26 09:04:25.567148 bamboost-0.6.1/PKG-INFO
--rw-r--r--   0 florez    (1000) florez    (1000)    11755 2024-03-05 17:53:33.000000 bamboost-0.6.1/README.md
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-26 09:04:25.563815 bamboost-0.6.1/bamboost/
--rw-r--r--   0 florez    (1000) florez    (1000)      524 2024-04-26 08:54:30.000000 bamboost-0.6.1/bamboost/__init__.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-26 09:04:25.563815 bamboost-0.6.1/bamboost/accessors/
--rw-r--r--   0 florez    (1000) florez    (1000)       67 2024-04-26 08:33:17.000000 bamboost-0.6.1/bamboost/accessors/__init__.py
--rw-r--r--   0 florez    (1000) florez    (1000)     6210 2024-04-26 08:33:17.000000 bamboost-0.6.1/bamboost/accessors/fielddata.py
--rw-r--r--   0 florez    (1000) florez    (1000)      932 2024-03-05 17:53:33.000000 bamboost-0.6.1/bamboost/accessors/globals.py
--rw-r--r--   0 florez    (1000) florez    (1000)     1570 2024-04-26 08:37:45.000000 bamboost-0.6.1/bamboost/accessors/meshes.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-26 09:04:25.563815 bamboost-0.6.1/bamboost/common/
--rw-r--r--   0 florez    (1000) florez    (1000)      181 2024-04-26 09:02:02.000000 bamboost-0.6.1/bamboost/common/__init__.py
--rw-r--r--   0 florez    (1000) florez    (1000)     3045 2024-04-17 13:09:34.000000 bamboost-0.6.1/bamboost/common/_mock_mpi.py
--rw-r--r--   0 florez    (1000) florez    (1000)     5291 2024-04-17 13:09:34.000000 bamboost-0.6.1/bamboost/common/file_handler.py
--rw-r--r--   0 florez    (1000) florez    (1000)     1474 2024-03-05 17:53:33.000000 bamboost-0.6.1/bamboost/common/git_utility.py
--rw-r--r--   0 florez    (1000) florez    (1000)     8985 2024-04-17 13:09:34.000000 bamboost-0.6.1/bamboost/common/hdf_pointer.py
--rw-r--r--   0 florez    (1000) florez    (1000)     3432 2024-04-26 08:33:17.000000 bamboost-0.6.1/bamboost/common/job.py
--rw-r--r--   0 florez    (1000) florez    (1000)      932 2024-04-26 08:37:45.000000 bamboost-0.6.1/bamboost/common/mpi.py
--rw-r--r--   0 florez    (1000) florez    (1000)     5966 2024-04-26 09:02:24.000000 bamboost-0.6.1/bamboost/common/utilities.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-26 09:04:25.563815 bamboost-0.6.1/bamboost/extensions/
--rw-r--r--   0 florez    (1000) florez    (1000)      529 2024-04-26 08:37:39.000000 bamboost-0.6.1/bamboost/extensions/__init__.py
--rw-r--r--   0 florez    (1000) florez    (1000)     7332 2024-04-26 08:37:39.000000 bamboost-0.6.1/bamboost/extensions/fenics.py
--rw-r--r--   0 florez    (1000) florez    (1000)     2352 2024-04-26 08:37:39.000000 bamboost-0.6.1/bamboost/extensions/slurm.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-26 09:04:25.563815 bamboost-0.6.1/bamboost/html/
--rw-r--r--   0 florez    (1000) florez    (1000)     3741 2024-04-26 09:00:53.000000 bamboost-0.6.1/bamboost/html/hdf5_group.html
--rw-r--r--   0 florez    (1000) florez    (1000)    58161 2024-03-05 17:53:33.000000 bamboost-0.6.1/bamboost/html/icon.png
--rw-r--r--   0 florez    (1000) florez    (1000)    77548 2024-03-05 17:53:33.000000 bamboost-0.6.1/bamboost/html/icon.txt
--rw-r--r--   0 florez    (1000) florez    (1000)     1353 2024-03-05 17:53:33.000000 bamboost-0.6.1/bamboost/html/manager.html
--rw-r--r--   0 florez    (1000) florez    (1000)     3471 2024-03-05 17:53:33.000000 bamboost-0.6.1/bamboost/html/simulation.html
--rw-r--r--   0 florez    (1000) florez    (1000)     5119 2024-04-26 08:33:17.000000 bamboost-0.6.1/bamboost/index.py
--rw-r--r--   0 florez    (1000) florez    (1000)    18120 2024-04-26 08:37:45.000000 bamboost-0.6.1/bamboost/manager.py
--rw-r--r--   0 florez    (1000) florez    (1000)    17062 2024-04-26 08:37:45.000000 bamboost-0.6.1/bamboost/simulation.py
--rw-r--r--   0 florez    (1000) florez    (1000)    11320 2024-04-26 08:55:19.000000 bamboost-0.6.1/bamboost/simulation_writer.py
--rw-r--r--   0 florez    (1000) florez    (1000)     6577 2024-04-26 08:50:59.000000 bamboost-0.6.1/bamboost/xdmf.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-26 09:04:25.567148 bamboost-0.6.1/bamboost.egg-info/
--rw-r--r--   0 florez    (1000) florez    (1000)    13793 2024-04-26 09:04:25.000000 bamboost-0.6.1/bamboost.egg-info/PKG-INFO
--rw-r--r--   0 florez    (1000) florez    (1000)      977 2024-04-26 09:04:25.000000 bamboost-0.6.1/bamboost.egg-info/SOURCES.txt
--rw-r--r--   0 florez    (1000) florez    (1000)        1 2024-04-26 09:04:25.000000 bamboost-0.6.1/bamboost.egg-info/dependency_links.txt
--rw-r--r--   0 florez    (1000) florez    (1000)       89 2024-04-26 09:04:25.000000 bamboost-0.6.1/bamboost.egg-info/requires.txt
--rw-r--r--   0 florez    (1000) florez    (1000)        9 2024-04-26 09:04:25.000000 bamboost-0.6.1/bamboost.egg-info/top_level.txt
--rw-r--r--   0 florez    (1000) florez    (1000)     1019 2024-04-26 08:54:30.000000 bamboost-0.6.1/pyproject.toml
--rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-04-26 09:04:25.567148 bamboost-0.6.1/setup.cfg
--rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-02-02 10:38:32.000000 bamboost-0.6.1/setup.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-04-26 09:04:25.567148 bamboost-0.6.1/tests/
--rw-r--r--   0 florez    (1000) florez    (1000)     1280 2024-04-26 08:33:17.000000 bamboost-0.6.1/tests/test_manager.py
--rw-r--r--   0 florez    (1000) florez    (1000)       64 2024-04-26 08:33:17.000000 bamboost-0.6.1/tests/test_reader.py
--rw-r--r--   0 florez    (1000) florez    (1000)     3324 2024-04-17 13:14:35.000000 bamboost-0.6.1/tests/test_writer.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 23:06:34.346558 bamboost-0.6.2/
+-rw-r--r--   0 florez    (1000) florez    (1000)     1060 2024-01-29 08:07:36.000000 bamboost-0.6.2/LICENSE
+-rw-r--r--   0 florez    (1000) florez    (1000)       62 2024-05-07 23:06:07.000000 bamboost-0.6.2/MANIFEST.in
+-rw-r--r--   0 florez    (1000) florez    (1000)    13793 2024-05-07 23:06:34.346558 bamboost-0.6.2/PKG-INFO
+-rw-r--r--   0 florez    (1000) florez    (1000)    11755 2024-03-05 17:53:33.000000 bamboost-0.6.2/README.md
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 23:06:34.343224 bamboost-0.6.2/bamboost/
+-rw-r--r--   0 florez    (1000) florez    (1000)      524 2024-05-07 23:06:10.000000 bamboost-0.6.2/bamboost/__init__.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 23:06:34.343224 bamboost-0.6.2/bamboost/accessors/
+-rw-r--r--   0 florez    (1000) florez    (1000)       67 2024-05-07 23:06:10.000000 bamboost-0.6.2/bamboost/accessors/__init__.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     6210 2024-05-07 23:06:10.000000 bamboost-0.6.2/bamboost/accessors/fielddata.py
+-rw-r--r--   0 florez    (1000) florez    (1000)      932 2024-03-05 17:53:33.000000 bamboost-0.6.2/bamboost/accessors/globals.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     1570 2024-04-26 08:37:45.000000 bamboost-0.6.2/bamboost/accessors/meshes.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 23:06:34.346558 bamboost-0.6.2/bamboost/common/
+-rw-r--r--   0 florez    (1000) florez    (1000)      181 2024-04-26 09:02:02.000000 bamboost-0.6.2/bamboost/common/__init__.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     3045 2024-04-17 13:09:34.000000 bamboost-0.6.2/bamboost/common/_mock_mpi.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     5291 2024-04-17 13:09:34.000000 bamboost-0.6.2/bamboost/common/file_handler.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     1474 2024-03-05 17:53:33.000000 bamboost-0.6.2/bamboost/common/git_utility.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     8985 2024-04-17 13:09:34.000000 bamboost-0.6.2/bamboost/common/hdf_pointer.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     3432 2024-05-07 23:06:10.000000 bamboost-0.6.2/bamboost/common/job.py
+-rw-r--r--   0 florez    (1000) florez    (1000)      932 2024-05-07 23:06:10.000000 bamboost-0.6.2/bamboost/common/mpi.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     5966 2024-05-07 23:06:10.000000 bamboost-0.6.2/bamboost/common/utilities.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 23:06:34.346558 bamboost-0.6.2/bamboost/extensions/
+-rw-r--r--   0 florez    (1000) florez    (1000)      529 2024-05-07 23:06:10.000000 bamboost-0.6.2/bamboost/extensions/__init__.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     7332 2024-05-02 09:30:47.000000 bamboost-0.6.2/bamboost/extensions/fenics.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     2352 2024-05-02 09:30:47.000000 bamboost-0.6.2/bamboost/extensions/slurm.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 23:06:34.346558 bamboost-0.6.2/bamboost/html/
+-rw-r--r--   0 florez    (1000) florez    (1000)     3741 2024-05-02 09:30:47.000000 bamboost-0.6.2/bamboost/html/hdf5_group.html
+-rw-r--r--   0 florez    (1000) florez    (1000)    58161 2024-03-05 17:53:33.000000 bamboost-0.6.2/bamboost/html/icon.png
+-rw-r--r--   0 florez    (1000) florez    (1000)    77548 2024-03-05 17:53:33.000000 bamboost-0.6.2/bamboost/html/icon.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)     1353 2024-03-05 17:53:33.000000 bamboost-0.6.2/bamboost/html/manager.html
+-rw-r--r--   0 florez    (1000) florez    (1000)     3471 2024-03-05 17:53:33.000000 bamboost-0.6.2/bamboost/html/simulation.html
+-rw-r--r--   0 florez    (1000) florez    (1000)     5119 2024-05-07 23:06:10.000000 bamboost-0.6.2/bamboost/index.py
+-rw-r--r--   0 florez    (1000) florez    (1000)    18120 2024-05-07 23:06:10.000000 bamboost-0.6.2/bamboost/manager.py
+-rw-r--r--   0 florez    (1000) florez    (1000)    17792 2024-05-07 23:06:10.000000 bamboost-0.6.2/bamboost/simulation.py
+-rw-r--r--   0 florez    (1000) florez    (1000)    11320 2024-05-07 23:06:10.000000 bamboost-0.6.2/bamboost/simulation_writer.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     6577 2024-05-02 09:30:47.000000 bamboost-0.6.2/bamboost/xdmf.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 23:06:34.346558 bamboost-0.6.2/bamboost.egg-info/
+-rw-r--r--   0 florez    (1000) florez    (1000)    13793 2024-05-07 23:06:34.000000 bamboost-0.6.2/bamboost.egg-info/PKG-INFO
+-rw-r--r--   0 florez    (1000) florez    (1000)      977 2024-05-07 23:06:34.000000 bamboost-0.6.2/bamboost.egg-info/SOURCES.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)        1 2024-05-07 23:06:34.000000 bamboost-0.6.2/bamboost.egg-info/dependency_links.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)       89 2024-05-07 23:06:34.000000 bamboost-0.6.2/bamboost.egg-info/requires.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)        9 2024-05-07 23:06:34.000000 bamboost-0.6.2/bamboost.egg-info/top_level.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)     1019 2024-05-07 23:06:10.000000 bamboost-0.6.2/pyproject.toml
+-rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-05-07 23:06:34.346558 bamboost-0.6.2/setup.cfg
+-rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-02-02 10:38:32.000000 bamboost-0.6.2/setup.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 23:06:34.346558 bamboost-0.6.2/tests/
+-rw-r--r--   0 florez    (1000) florez    (1000)     1280 2024-05-07 23:06:10.000000 bamboost-0.6.2/tests/test_manager.py
+-rw-r--r--   0 florez    (1000) florez    (1000)      638 2024-05-07 23:06:10.000000 bamboost-0.6.2/tests/test_reader.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     3631 2024-05-07 23:06:10.000000 bamboost-0.6.2/tests/test_writer.py
```

### Comparing `bamboost-0.6.1/LICENSE` & `bamboost-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/PKG-INFO` & `bamboost-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamboost
-Version: 0.6.1
+Version: 0.6.2
 Summary: A light weight database manager using HDF5
 Author-email: Flavio Lorez <florez@ethz.ch>
 License: Copyright (c) 2023 CMBM, ETH Zurich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bamboost Version: 0.6.1 Summary: A light weight
+Metadata-Version: 2.1 Name: bamboost Version: 0.6.2 Summary: A light weight
 database manager using HDF5 Author-email: Flavio Lorez
 ethz.ch> License: Copyright (c) 2023 CMBM, ETH Zurich Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `bamboost-0.6.1/README.md` & `bamboost-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/__init__.py` & `bamboost-0.6.2/bamboost/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "florez@ethz.ch"
 __copyright__ = ""
 __license__ = "LGPLv3"
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 import logging
 import os
 
 from .manager import Manager
 from .simulation import Simulation
 from .simulation_writer import SimulationWriter
```

### Comparing `bamboost-0.6.1/bamboost/accessors/fielddata.py` & `bamboost-0.6.2/bamboost/accessors/fielddata.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/accessors/globals.py` & `bamboost-0.6.2/bamboost/accessors/globals.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/accessors/meshes.py` & `bamboost-0.6.2/bamboost/accessors/meshes.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/common/_mock_mpi.py` & `bamboost-0.6.2/bamboost/common/_mock_mpi.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/common/file_handler.py` & `bamboost-0.6.2/bamboost/common/file_handler.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/common/git_utility.py` & `bamboost-0.6.2/bamboost/common/git_utility.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/common/hdf_pointer.py` & `bamboost-0.6.2/bamboost/common/hdf_pointer.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/common/job.py` & `bamboost-0.6.2/bamboost/common/job.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/common/mpi.py` & `bamboost-0.6.2/bamboost/common/mpi.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/common/utilities.py` & `bamboost-0.6.2/bamboost/common/utilities.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/extensions/__init__.py` & `bamboost-0.6.2/bamboost/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/extensions/fenics.py` & `bamboost-0.6.2/bamboost/extensions/fenics.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/extensions/slurm.py` & `bamboost-0.6.2/bamboost/extensions/slurm.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/html/hdf5_group.html` & `bamboost-0.6.2/bamboost/html/hdf5_group.html`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/html/icon.png` & `bamboost-0.6.2/bamboost/html/icon.png`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/html/icon.txt` & `bamboost-0.6.2/bamboost/html/icon.txt`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/html/manager.html` & `bamboost-0.6.2/bamboost/html/manager.html`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/html/simulation.html` & `bamboost-0.6.2/bamboost/html/simulation.html`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/index.py` & `bamboost-0.6.2/bamboost/index.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/manager.py` & `bamboost-0.6.2/bamboost/manager.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/simulation.py` & `bamboost-0.6.2/bamboost/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from __future__ import annotations
 
 import logging
 import os
 import pkgutil
 import subprocess
+from contextlib import contextmanager
 from typing import Any, Iterable, Tuple
 
 import numpy as np
 import pandas as pd
 from typing_extensions import Self, deprecated
 
 from . import index
@@ -398,20 +399,28 @@
 
     def submit(self) -> None:
         """Submit the job for this simulation."""
         if f"sbatch_{self.uid}.sh" in os.listdir(self.path):
             batch_script = os.path.abspath(
                 os.path.join(self.path, f"sbatch_{self.uid}.sh")
             )
-            subprocess.Popen(["sbatch", f"{batch_script}"])
-        if f"{self.uid}.sh" in os.listdir(self.path):
+            env = os.environ.copy()
+            _ = env.pop("BAMBOOST_NO_MPI", None)
+            subprocess.run(["sbatch", f"{batch_script}"], env=env)
+        elif f"{self.uid}.sh" in os.listdir(self.path):
             bash_script = os.path.abspath(os.path.join(self.path, f"{self.uid}.sh"))
-            subprocess.Popen(["bash", f"{bash_script}"])
+            env = os.environ.copy()
+            _ = env.pop("BAMBOOST_NO_MPI", None)
+            subprocess.run(["bash", f"{bash_script}"], env=env)
+        else:
+            raise FileNotFoundError(
+                f"Could not find a batch script for simulation {self.uid}."
+            )
 
-        print(f"Simulation {self.uid} submitted!")
+        log.info(f"Simulation {self.uid} submitted!")
 
         with self._file("a") as file:
             file.attrs.update({"submitted": True})
 
     @with_file_open("a")
     def change_note(self, note) -> None:
         self._file.attrs["notes"] = note
@@ -509,7 +518,22 @@
 
     @with_file_open()
     def show_h5tree(self) -> None:
         """Print the tree inside the h5 file."""
         # print('\U00002B57 ' + os.path.basename(self.h5file))
         print("\U0001F43C " + os.path.basename(self.h5file))
         utilities.h5_tree(self._file.file_object)
+
+    @contextmanager
+    def enter_path(self):
+        """A context manager for changing the working directory to this simulations' path.
+
+        >>> with sim.working_directory():
+        >>>     ...
+        """
+
+        current_dir = os.getcwd()
+        try:
+            os.chdir(self.path)
+            yield
+        finally:
+            os.chdir(current_dir)
```

### Comparing `bamboost-0.6.1/bamboost/simulation_writer.py` & `bamboost-0.6.2/bamboost/simulation_writer.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost/xdmf.py` & `bamboost-0.6.2/bamboost/xdmf.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/bamboost.egg-info/PKG-INFO` & `bamboost-0.6.2/bamboost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamboost
-Version: 0.6.1
+Version: 0.6.2
 Summary: A light weight database manager using HDF5
 Author-email: Flavio Lorez <florez@ethz.ch>
 License: Copyright (c) 2023 CMBM, ETH Zurich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bamboost Version: 0.6.1 Summary: A light weight
+Metadata-Version: 2.1 Name: bamboost Version: 0.6.2 Summary: A light weight
 database manager using HDF5 Author-email: Flavio Lorez
 ethz.ch> License: Copyright (c) 2023 CMBM, ETH Zurich Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `bamboost-0.6.1/bamboost.egg-info/SOURCES.txt` & `bamboost-0.6.2/bamboost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/pyproject.toml` & `bamboost-0.6.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bamboost"
-version = "0.6.1"
+version = "0.6.2"
 description = "A light weight database manager using HDF5"
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [{ name = "Flavio Lorez", email = "florez@ethz.ch" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `bamboost-0.6.1/tests/test_manager.py` & `bamboost-0.6.2/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `bamboost-0.6.1/tests/test_writer.py` & `bamboost-0.6.2/tests/test_writer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-from test_manager import temp_manager
+import os
+
 import numpy as np
 import pytest
+from test_manager import temp_manager
 
 
-@pytest.mark.parametrize("dtype,array", [['<f4', np.array([1, 2], dtype=int)],
-                                         ["int32", np.array([1, 2])],
-                                         ])
+@pytest.mark.parametrize(
+    "dtype,array",
+    [
+        ["<f4", np.array([1, 2], dtype=int)],
+        ["int32", np.array([1, 2])],
+    ],
+)
 def test_field_dtype_forced(temp_manager, dtype, array):
     sim = temp_manager.create_simulation()
     uid = sim.uid
     sim.add_field("test", array, dtype=dtype)
 
     sim.finish_step()
     sim.add_field("test", 2 * array, dtype=dtype)
@@ -17,17 +23,21 @@
     sim.finish_sim()
 
     sim = temp_manager.sim(uid)
 
     assert sim.data["test"].dtype == dtype
 
 
-@pytest.mark.parametrize("dtype,value", [['<f4', 1],
-                                         ["int32", 1],
-                                         ])
+@pytest.mark.parametrize(
+    "dtype,value",
+    [
+        ["<f4", 1],
+        ["int32", 1],
+    ],
+)
 def test_global_field_dtype_forced(temp_manager, dtype, value):
     sim = temp_manager.create_simulation()
     uid = sim.uid
     sim.add_global_field("test", value, dtype=dtype)
 
     sim.finish_step()
     sim.add_global_field("test", 2 * value, dtype=dtype)
@@ -35,17 +45,21 @@
     sim.finish_sim()
 
     sim = temp_manager.sim(uid)
 
     assert sim.globals["test"].dtype == dtype
 
 
-@pytest.mark.parametrize("array", [np.array([1., 2.]),
-                                   np.array([1, 2], dtype="int"),
-                                   ])
+@pytest.mark.parametrize(
+    "array",
+    [
+        np.array([1.0, 2.0]),
+        np.array([1, 2], dtype="int"),
+    ],
+)
 def test_field_dtype_inferred(temp_manager, array):
     sim = temp_manager.create_simulation()
     uid = sim.uid
     sim.add_field("test", array)
 
     sim.finish_step()
     sim.add_field("test", 2 * array)
@@ -54,15 +68,21 @@
 
     sim = temp_manager.sim(uid)
 
     # The dtypes are equivalent (although they may have another string representation)
     assert np.dtype(sim.data["test"].dtype) == array.dtype
 
 
-@pytest.mark.parametrize("val", [1., 1, ])
+@pytest.mark.parametrize(
+    "val",
+    [
+        1.0,
+        1,
+    ],
+)
 def test_global_field_dtype_inferred(temp_manager, val):
     sim = temp_manager.create_simulation()
     uid = sim.uid
     sim.add_global_field("test", val)
 
     sim.finish_step()
     sim.add_global_field("test", 2 * val)
@@ -71,17 +91,21 @@
 
     sim = temp_manager.sim(uid)
 
     # The dtypes are equivalent (although they may have another string representation)
     assert np.dtype(sim.globals["test"].dtype) == np.array([val]).dtype
 
 
-@pytest.mark.parametrize("array", [np.array([1., 2.]),
-                                   np.array([1, 2], dtype="int"),
-                                   ])
+@pytest.mark.parametrize(
+    "array",
+    [
+        np.array([1.0, 2.0]),
+        np.array([1, 2], dtype="int"),
+    ],
+)
 def test_userdata_dtype_inferred(temp_manager, array):
     sim = temp_manager.create_simulation()
     uid = sim.uid
     sim.userdata.add_dataset("test", array)
 
     sim.finish_step()
     sim.userdata.add_dataset("test", 2 * array)
@@ -90,23 +114,45 @@
 
     sim = temp_manager.sim(uid)
 
     # The dtypes are equivalent (although they may have another string representation)
     assert np.dtype(sim.userdata["test"].dtype) == array.dtype
 
 
-@pytest.mark.parametrize("dtype,array", [['<f4', np.array([1, 2], dtype=int)],
-                                         ["int32", np.array([1, 2])],
-                                         ])
+@pytest.mark.parametrize(
+    "dtype,array",
+    [
+        ["<f4", np.array([1, 2], dtype=int)],
+        ["int32", np.array([1, 2])],
+    ],
+)
 def test_userdata_dtype_forced(temp_manager, dtype, array):
     sim = temp_manager.create_simulation()
     uid = sim.uid
     sim.userdata.add_dataset("test", array, dtype=dtype)
 
     sim.finish_step()
     sim.userdata.add_dataset("test", 2 * array, dtype=dtype)
 
     sim.finish_sim()
 
     sim = temp_manager.sim(uid)
 
     assert sim.userdata["test"].dtype == dtype
+
+
+def test_enter_path(temp_manager):
+    sim = temp_manager.create_simulation()
+    sim.finish_sim()
+    path = sim.path
+    uid = sim.uid
+    original_path = os.getcwd()
+    with sim.enter_path():
+        assert os.getcwd() == path
+    assert os.getcwd() == original_path
+
+    # check that we return in the right path even when throwing an error
+    try:
+        with sim.enter_path():
+            raise ValueError()
+    except ValueError:
+        assert os.getcwd() == original_path
```

