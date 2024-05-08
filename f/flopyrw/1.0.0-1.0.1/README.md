# Comparing `tmp/flopyrw-1.0.0.tar.gz` & `tmp/flopyrw-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flopyrw-1.0.0.tar", last modified: Mon Aug  7 16:33:57 2023, max compression
+gzip compressed data, was "flopyrw-1.0.1.tar", last modified: Wed May  8 09:41:11 2024, max compression
```

## Comparing `flopyrw-1.0.0.tar` & `flopyrw-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leno      (1000) leno      (1000)        0 2023-08-07 16:33:57.881872 flopyrw-1.0.0/
--rw-r--r--   0 leno      (1000) leno      (1000)     1115 2023-05-25 15:16:56.000000 flopyrw-1.0.0/LICENSE.md
--rw-r--r--   0 leno      (1000) leno      (1000)     6295 2023-08-07 16:33:57.881872 flopyrw-1.0.0/PKG-INFO
--rw-r--r--   0 leno      (1000) leno      (1000)     4898 2023-07-04 21:58:58.000000 flopyrw-1.0.0/README.md
-drwxr-xr-x   0 leno      (1000) leno      (1000)        0 2023-08-07 16:33:57.878539 flopyrw-1.0.0/flopyrw/
--rw-r--r--   0 leno      (1000) leno      (1000)       25 2023-05-24 12:22:51.000000 flopyrw-1.0.0/flopyrw/__init__.py
--rw-r--r--   0 leno      (1000) leno      (1000)       72 2023-05-25 13:41:01.000000 flopyrw-1.0.0/flopyrw/version.py
-drwxr-xr-x   0 leno      (1000) leno      (1000)        0 2023-08-07 16:33:57.878539 flopyrw-1.0.0/flopyrw.egg-info/
--rw-r--r--   0 leno      (1000) leno      (1000)     6295 2023-08-07 16:33:57.000000 flopyrw-1.0.0/flopyrw.egg-info/PKG-INFO
--rw-r--r--   0 leno      (1000) leno      (1000)      228 2023-08-07 16:33:57.000000 flopyrw-1.0.0/flopyrw.egg-info/SOURCES.txt
--rw-r--r--   0 leno      (1000) leno      (1000)        1 2023-08-07 16:33:57.000000 flopyrw-1.0.0/flopyrw.egg-info/dependency_links.txt
--rw-r--r--   0 leno      (1000) leno      (1000)       64 2023-08-07 16:33:57.000000 flopyrw-1.0.0/flopyrw.egg-info/requires.txt
--rw-r--r--   0 leno      (1000) leno      (1000)        8 2023-08-07 16:33:57.000000 flopyrw-1.0.0/flopyrw.egg-info/top_level.txt
--rw-r--r--   0 leno      (1000) leno      (1000)      721 2023-06-30 09:18:23.000000 flopyrw-1.0.0/pyproject.toml
--rw-r--r--   0 leno      (1000) leno      (1000)       38 2023-08-07 16:33:57.881872 flopyrw-1.0.0/setup.cfg
+drwxr-xr-x   0 leno      (1000) leno      (1000)        0 2024-05-08 09:41:11.064070 flopyrw-1.0.1/
+-rw-r--r--   0 leno      (1000) leno      (1000)     1115 2023-05-25 15:16:56.000000 flopyrw-1.0.1/LICENSE.md
+-rw-r--r--   0 leno      (1000) leno      (1000)     6496 2024-05-08 09:41:11.064070 flopyrw-1.0.1/PKG-INFO
+-rw-r--r--   0 leno      (1000) leno      (1000)     4900 2023-09-21 14:49:30.000000 flopyrw-1.0.1/README.md
+drwxr-xr-x   0 leno      (1000) leno      (1000)        0 2024-05-08 09:41:11.060736 flopyrw-1.0.1/flopyrw/
+-rw-r--r--   0 leno      (1000) leno      (1000)       25 2023-05-24 12:22:51.000000 flopyrw-1.0.1/flopyrw/__init__.py
+-rw-r--r--   0 leno      (1000) leno      (1000)       72 2024-05-08 09:40:57.000000 flopyrw-1.0.1/flopyrw/version.py
+drwxr-xr-x   0 leno      (1000) leno      (1000)        0 2024-05-08 09:41:11.060736 flopyrw-1.0.1/flopyrw.egg-info/
+-rw-r--r--   0 leno      (1000) leno      (1000)     6496 2024-05-08 09:41:11.000000 flopyrw-1.0.1/flopyrw.egg-info/PKG-INFO
+-rw-r--r--   0 leno      (1000) leno      (1000)      228 2024-05-08 09:41:11.000000 flopyrw-1.0.1/flopyrw.egg-info/SOURCES.txt
+-rw-r--r--   0 leno      (1000) leno      (1000)        1 2024-05-08 09:41:11.000000 flopyrw-1.0.1/flopyrw.egg-info/dependency_links.txt
+-rw-r--r--   0 leno      (1000) leno      (1000)       64 2024-05-08 09:41:11.000000 flopyrw-1.0.1/flopyrw.egg-info/requires.txt
+-rw-r--r--   0 leno      (1000) leno      (1000)        8 2024-05-08 09:41:11.000000 flopyrw-1.0.1/flopyrw.egg-info/top_level.txt
+-rw-r--r--   0 leno      (1000) leno      (1000)      721 2023-06-30 09:18:23.000000 flopyrw-1.0.1/pyproject.toml
+-rw-r--r--   0 leno      (1000) leno      (1000)       38 2024-05-08 09:41:11.064070 flopyrw-1.0.1/setup.cfg
```

### Comparing `flopyrw-1.0.0/LICENSE.md` & `flopyrw-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flopyrw-1.0.0/PKG-INFO` & `flopyrw-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: flopyrw
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python interface based on FloPy to configure input files for MODPATH-RW
 Keywords: MODPATH-RW,hydrogeology,rwpt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.md
+Requires-Dist: flopy>=3.4.1
+Provides-Extra: test
+Requires-Dist: shapely>=1.8; extra == "test"
+Requires-Dist: pyshp; extra == "test"
+Requires-Dist: modflow-devtools; extra == "test"
+Requires-Dist: pytest; extra == "test"
 
 ## flopyrw
-An extension of [FloPy](https://github.com/modflowpy/flopy) to write input simulation files for [MODPATH-RW](https://gitub.com/upc-ghs/modpath-rw) with Python.
+An extension of [FloPy](https://github.com/modflowpy/flopy) to write input simulation files for [MODPATH-RW](https://github.com/upc-ghs/modpath-rw) with Python.
 
 ### Overview
 Provides classes extended from the `modpath` module in `flopy` adapted to specific structures required by MODPATH-RW. Also introduces new package writers required by the program, consistent with the [Documentation of Input-Output](https://github.com/upc-ghs/modpath-rw/blob/develop/doc/modpath-rw_IO_v100_.pdf). 
 
 
 ### Quickstart
 **Install**
@@ -136,15 +141,15 @@
 pmv.plot_grid(colors='white')
 pmv.contour_array(head, levels=[.2, .4, .6, .8], linewidths=3.)
 pmv.plot_vector(qx, qy, normalize=True, color="white")
 pmv.plot_endpoint( epoint.get_alldata(), zorder=10, s=4, linewidth=0.5, edgecolor='k' )
 ```
 <img src="img/quickstart.png" alt="plot" style="width:30;height:30">
 
-**Note**: In order to run a model via the interface a [MODPATH-RW](https://gitub.com/upc-ghs/modpath-rw) executable is required. 
+**Note**: In order to run a model via the interface a [MODPATH-RW](https://github.com/upc-ghs/modpath-rw) executable is required. 
 
 
 ### Testing
 A suite of [automated tests](autotest/) is available verifying different aspects of the interface and the program. In order to run these tests, some additional dependencies are required, which can be installed with:
 
 ```
 pip install ".[test]"
```

### Comparing `flopyrw-1.0.0/README.md` & `flopyrw-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ## flopyrw
-An extension of [FloPy](https://github.com/modflowpy/flopy) to write input simulation files for [MODPATH-RW](https://gitub.com/upc-ghs/modpath-rw) with Python.
+An extension of [FloPy](https://github.com/modflowpy/flopy) to write input simulation files for [MODPATH-RW](https://github.com/upc-ghs/modpath-rw) with Python.
 
 ### Overview
 Provides classes extended from the `modpath` module in `flopy` adapted to specific structures required by MODPATH-RW. Also introduces new package writers required by the program, consistent with the [Documentation of Input-Output](https://github.com/upc-ghs/modpath-rw/blob/develop/doc/modpath-rw_IO_v100_.pdf). 
 
 
 ### Quickstart
 **Install**
@@ -126,15 +126,15 @@
 pmv.plot_grid(colors='white')
 pmv.contour_array(head, levels=[.2, .4, .6, .8], linewidths=3.)
 pmv.plot_vector(qx, qy, normalize=True, color="white")
 pmv.plot_endpoint( epoint.get_alldata(), zorder=10, s=4, linewidth=0.5, edgecolor='k' )
 ```
 <img src="img/quickstart.png" alt="plot" style="width:30;height:30">
 
-**Note**: In order to run a model via the interface a [MODPATH-RW](https://gitub.com/upc-ghs/modpath-rw) executable is required. 
+**Note**: In order to run a model via the interface a [MODPATH-RW](https://github.com/upc-ghs/modpath-rw) executable is required. 
 
 
 ### Testing
 A suite of [automated tests](autotest/) is available verifying different aspects of the interface and the program. In order to run these tests, some additional dependencies are required, which can be installed with:
 
 ```
 pip install ".[test]"
```

### Comparing `flopyrw-1.0.0/flopyrw.egg-info/PKG-INFO` & `flopyrw-1.0.1/flopyrw.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: flopyrw
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python interface based on FloPy to configure input files for MODPATH-RW
 Keywords: MODPATH-RW,hydrogeology,rwpt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.md
+Requires-Dist: flopy>=3.4.1
+Provides-Extra: test
+Requires-Dist: shapely>=1.8; extra == "test"
+Requires-Dist: pyshp; extra == "test"
+Requires-Dist: modflow-devtools; extra == "test"
+Requires-Dist: pytest; extra == "test"
 
 ## flopyrw
-An extension of [FloPy](https://github.com/modflowpy/flopy) to write input simulation files for [MODPATH-RW](https://gitub.com/upc-ghs/modpath-rw) with Python.
+An extension of [FloPy](https://github.com/modflowpy/flopy) to write input simulation files for [MODPATH-RW](https://github.com/upc-ghs/modpath-rw) with Python.
 
 ### Overview
 Provides classes extended from the `modpath` module in `flopy` adapted to specific structures required by MODPATH-RW. Also introduces new package writers required by the program, consistent with the [Documentation of Input-Output](https://github.com/upc-ghs/modpath-rw/blob/develop/doc/modpath-rw_IO_v100_.pdf). 
 
 
 ### Quickstart
 **Install**
@@ -136,15 +141,15 @@
 pmv.plot_grid(colors='white')
 pmv.contour_array(head, levels=[.2, .4, .6, .8], linewidths=3.)
 pmv.plot_vector(qx, qy, normalize=True, color="white")
 pmv.plot_endpoint( epoint.get_alldata(), zorder=10, s=4, linewidth=0.5, edgecolor='k' )
 ```
 <img src="img/quickstart.png" alt="plot" style="width:30;height:30">
 
-**Note**: In order to run a model via the interface a [MODPATH-RW](https://gitub.com/upc-ghs/modpath-rw) executable is required. 
+**Note**: In order to run a model via the interface a [MODPATH-RW](https://github.com/upc-ghs/modpath-rw) executable is required. 
 
 
 ### Testing
 A suite of [automated tests](autotest/) is available verifying different aspects of the interface and the program. In order to run these tests, some additional dependencies are required, which can be installed with:
 
 ```
 pip install ".[test]"
```

### Comparing `flopyrw-1.0.0/pyproject.toml` & `flopyrw-1.0.1/pyproject.toml`

 * *Files identical despite different names*

