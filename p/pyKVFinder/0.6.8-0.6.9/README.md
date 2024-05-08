# Comparing `tmp/pyKVFinder-0.6.8.tar.gz` & `tmp/pyKVFinder-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyKVFinder-0.6.8.tar", last modified: Thu Oct 26 16:58:49 2023, max compression
+gzip compressed data, was "pyKVFinder-0.6.9.tar", last modified: Tue Nov 21 21:55:56 2023, max compression
```

## Comparing `pyKVFinder-0.6.8.tar` & `pyKVFinder-0.6.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:58:49.006175 pyKVFinder-0.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:58:48.998175 pyKVFinder-0.6.8/C/
--rw-r--r--   0 runner    (1001) docker     (127)   104503 2023-10-26 16:58:32.000000 pyKVFinder-0.6.8/C/numpy.i
--rw-r--r--   0 runner    (1001) docker     (127)    78654 2023-10-26 16:58:32.000000 pyKVFinder-0.6.8/C/pyKVFinder.c
--rw-r--r--   0 runner    (1001) docker     (127)     7353 2023-10-26 16:58:32.000000 pyKVFinder-0.6.8/C/pyKVFinder.h
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2023-10-26 16:58:32.000000 pyKVFinder-0.6.8/C/pyKVFinder.i
--rw-r--r--   0 runner    (1001) docker     (127)    35140 2023-10-26 16:58:32.000000 pyKVFinder-0.6.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-10-26 16:58:32.000000 pyKVFinder-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    44886 2023-10-26 16:58:49.006175 pyKVFinder-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-10-26 16:58:32.000000 pyKVFinder-0.6.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:58:48.998175 pyKVFinder-0.6.8/pyKVFinder/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10722 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:58:49.002175 pyKVFinder-0.6.8/pyKVFinder/data/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/EisenbergWeiss.toml
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/HessaHeijne.toml
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/KyteDoolittle.toml
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/MoonFleming.toml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/RadzickaWolfenden.toml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/WimleyWhite.toml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/ZhaoLondon.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:58:49.006175 pyKVFinder-0.6.8/pyKVFinder/data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   338350 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
--rw-r--r--   0 runner    (1001) docker     (127)   226706 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/tests/1FMO.pdb
--rw-r--r--   0 runner    (1001) docker     (127)    88538 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/tests/1FMO.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/tests/ADN.pdb
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/tests/ADN.xyz
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/tests/ClO4.pdb
--rw-r--r--   0 runner    (1001) docker     (127)    12640 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/tests/PKI.pdb
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/tests/custom-box.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/tests/residues-box.toml
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/data/vdw.dat
--rw-r--r--   0 runner    (1001) docker     (127)   107710 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    71034 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    63360 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyKVFinder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:58:49.002175 pyKVFinder-0.6.8/pyKVFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44886 2023-10-26 16:58:48.000000 pyKVFinder-0.6.8/pyKVFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-10-26 16:58:48.000000 pyKVFinder-0.6.8/pyKVFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 16:58:48.000000 pyKVFinder-0.6.8/pyKVFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-26 16:58:48.000000 pyKVFinder-0.6.8/pyKVFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-10-26 16:58:48.000000 pyKVFinder-0.6.8/pyKVFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-26 16:58:48.000000 pyKVFinder-0.6.8/pyKVFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-26 16:58:49.006175 pyKVFinder-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-10-26 16:58:33.000000 pyKVFinder-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 21:55:56.889206 pyKVFinder-0.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 21:55:56.881205 pyKVFinder-0.6.9/C/
+-rw-r--r--   0 runner    (1001) docker     (127)   104503 2023-11-21 21:55:46.000000 pyKVFinder-0.6.9/C/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (127)    78654 2023-11-21 21:55:46.000000 pyKVFinder-0.6.9/C/pyKVFinder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7353 2023-11-21 21:55:46.000000 pyKVFinder-0.6.9/C/pyKVFinder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2023-11-21 21:55:46.000000 pyKVFinder-0.6.9/C/pyKVFinder.i
+-rw-r--r--   0 runner    (1001) docker     (127)    35140 2023-11-21 21:55:46.000000 pyKVFinder-0.6.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2023-11-21 21:55:46.000000 pyKVFinder-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    44886 2023-11-21 21:55:56.889206 pyKVFinder-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-11-21 21:55:46.000000 pyKVFinder-0.6.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 21:55:56.885206 pyKVFinder-0.6.9/pyKVFinder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 21:55:56.885206 pyKVFinder-0.6.9/pyKVFinder/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/EisenbergWeiss.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/HessaHeijne.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/KyteDoolittle.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/MoonFleming.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/RadzickaWolfenden.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/WimleyWhite.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/ZhaoLondon.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 21:55:56.889206 pyKVFinder-0.6.9/pyKVFinder/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   338350 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)   226706 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/tests/1FMO.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)    88538 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/tests/1FMO.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/tests/ADN.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/tests/ADN.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/tests/ClO4.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)    12640 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/tests/PKI.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/tests/custom-box.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/tests/residues-box.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/data/vdw.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   107710 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71034 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63360 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyKVFinder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 21:55:56.889206 pyKVFinder-0.6.9/pyKVFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44886 2023-11-21 21:55:56.000000 pyKVFinder-0.6.9/pyKVFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2023-11-21 21:55:56.000000 pyKVFinder-0.6.9/pyKVFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 21:55:56.000000 pyKVFinder-0.6.9/pyKVFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-21 21:55:56.000000 pyKVFinder-0.6.9/pyKVFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-11-21 21:55:56.000000 pyKVFinder-0.6.9/pyKVFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-21 21:55:56.000000 pyKVFinder-0.6.9/pyKVFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 21:55:56.889206 pyKVFinder-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2023-11-21 21:55:47.000000 pyKVFinder-0.6.9/setup.py
```

### Comparing `pyKVFinder-0.6.8/C/numpy.i` & `pyKVFinder-0.6.9/C/numpy.i`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/C/pyKVFinder.c` & `pyKVFinder-0.6.9/C/pyKVFinder.c`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/C/pyKVFinder.h` & `pyKVFinder-0.6.9/C/pyKVFinder.h`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/C/pyKVFinder.i` & `pyKVFinder-0.6.9/C/pyKVFinder.i`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/LICENSE.txt` & `pyKVFinder-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/PKG-INFO` & `pyKVFinder-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python package to detect and characterize cavities in biomolecular structures
 Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Leandro Oliveira Bortot, José Geraldo de Carvalho Pereira, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -693,21 +693,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: toml==0.10.2
-Requires-Dist: numpy==1.26.1
-Requires-Dist: matplotlib==3.7.3
+Requires-Dist: numpy==1.26.2
+Requires-Dist: matplotlib==3.8.2
 Requires-Dist: plotly==5.18.0
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.3; extra == "dev"
 Requires-Dist: pytest-cov==4.1.0; extra == "dev"
-Requires-Dist: black==23.10.1; extra == "dev"
+Requires-Dist: black==23.11.0; extra == "dev"
 Requires-Dist: flake8==6.1.0; extra == "dev"
 
 ##########
 pyKVFinder
 ##########
 
 .. image:: https://img.shields.io/pypi/v/pyKVFinder
```

### Comparing `pyKVFinder-0.6.8/README.rst` & `pyKVFinder-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder/__init__.py` & `pyKVFinder-0.6.9/pyKVFinder/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Python-C parallel KVFinder.
 
 pyKVFinder detects and characterizes cavities in biomolecular structures.
 
 The characterization includes shape, volume, area, depth, hydropathy and
 interface residues and their frequencies.
 
-In addition to the set of function that can be imported on Python scritps,
+In addition to the set of functions that can be imported into Python scripts,
 it contains a command line interface (CLI).
 
 Python package
 --------------
 >>> import pyKVFinder
 
 Command Line Interface
@@ -27,13 +27,13 @@
 --------
 * GitHub repository: https://github.com/LBC-LNBio/pyKVFinder
 
 * Documentation: https://lbc-lnbio.github.io/pyKVFinder
 """
 
 __name__ = "pyKVFinder"
-__version__ = "0.6.8"
+__version__ = "0.6.9"
 license = "GNU GPL-3.0 License"
 
 from .utils import *
 from .grid import *
 from .main import *
```

### Comparing `pyKVFinder-0.6.8/pyKVFinder/argparser.py` & `pyKVFinder-0.6.9/pyKVFinder/argparser.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb` & `pyKVFinder-0.6.9/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder/data/tests/1FMO.pdb` & `pyKVFinder-0.6.9/pyKVFinder/data/tests/1FMO.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder/data/tests/1FMO.xyz` & `pyKVFinder-0.6.9/pyKVFinder/data/tests/1FMO.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder/data/tests/ADN.pdb` & `pyKVFinder-0.6.9/pyKVFinder/data/tests/ADN.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder/data/tests/ADN.xyz` & `pyKVFinder-0.6.9/pyKVFinder/data/tests/ADN.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder/data/tests/PKI.pdb` & `pyKVFinder-0.6.9/pyKVFinder/data/tests/PKI.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder/data/vdw.dat` & `pyKVFinder-0.6.9/pyKVFinder/data/vdw.dat`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder/grid.py` & `pyKVFinder-0.6.9/pyKVFinder/grid.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder/main.py` & `pyKVFinder-0.6.9/pyKVFinder/main.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder/utils.py` & `pyKVFinder-0.6.9/pyKVFinder/utils.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyKVFinder.egg-info/PKG-INFO` & `pyKVFinder-0.6.9/pyKVFinder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python package to detect and characterize cavities in biomolecular structures
 Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Leandro Oliveira Bortot, José Geraldo de Carvalho Pereira, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -693,21 +693,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: toml==0.10.2
-Requires-Dist: numpy==1.26.1
-Requires-Dist: matplotlib==3.7.3
+Requires-Dist: numpy==1.26.2
+Requires-Dist: matplotlib==3.8.2
 Requires-Dist: plotly==5.18.0
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.3; extra == "dev"
 Requires-Dist: pytest-cov==4.1.0; extra == "dev"
-Requires-Dist: black==23.10.1; extra == "dev"
+Requires-Dist: black==23.11.0; extra == "dev"
 Requires-Dist: flake8==6.1.0; extra == "dev"
 
 ##########
 pyKVFinder
 ##########
 
 .. image:: https://img.shields.io/pypi/v/pyKVFinder
```

### Comparing `pyKVFinder-0.6.8/pyKVFinder.egg-info/SOURCES.txt` & `pyKVFinder-0.6.9/pyKVFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.8/pyproject.toml` & `pyKVFinder-0.6.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -42,22 +42,22 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "toml==0.10.2",
-    "numpy==1.26.1",
-    "matplotlib==3.7.3",
+    "numpy==1.26.2",
+    "matplotlib==3.8.2",
     "plotly==5.18.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["pytest==7.4.3", "pytest-cov==4.1.0", "black==23.10.1", "flake8==6.1.0"]
+dev = ["pytest==7.4.3", "pytest-cov==4.1.0", "black==23.11.0", "flake8==6.1.0"]
 
 [project.urls]
 homepage = "https://github.com/LBC-LNBio/pyKVFinder/"
 documentation = "https://lbc-lnbio.github.io/pyKVFinder/"
 issues = "https://github.com/LBC-LNBio/pyKVFinder/issues"
 
 [project.scripts]
```

### Comparing `pyKVFinder-0.6.8/setup.py` & `pyKVFinder-0.6.9/setup.py`

 * *Files identical despite different names*

