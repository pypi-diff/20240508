# Comparing `tmp/cnmf-1.5.1.tar.gz` & `tmp/cnmf-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmf-1.5.1.tar", last modified: Wed May  8 02:08:07 2024, max compression
+gzip compressed data, was "cnmf-1.5.2.tar", last modified: Wed May  8 02:21:37 2024, max compression
```

## Comparing `cnmf-1.5.1.tar` & `cnmf-1.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:08:07.585057 cnmf-1.5.1/
--rw-r--r--   0 dkotliar   (503) staff       (20)     1070 2024-05-08 01:55:03.000000 cnmf-1.5.1/LICENSE
--rw-r--r--   0 dkotliar   (503) staff       (20)     9225 2024-05-08 02:08:07.584457 cnmf-1.5.1/PKG-INFO
--rw-r--r--   0 dkotliar   (503) staff       (20)     8519 2024-05-08 01:55:03.000000 cnmf-1.5.1/README.md
--rw-r--r--   0 dkotliar   (503) staff       (20)      103 2024-05-08 01:55:03.000000 cnmf-1.5.1/pyproject.toml
--rw-r--r--   0 dkotliar   (503) staff       (20)       38 2024-05-08 02:08:07.585225 cnmf-1.5.1/setup.cfg
--rw-r--r--   0 dkotliar   (503) staff       (20)     1333 2024-05-08 02:05:15.000000 cnmf-1.5.1/setup.py
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:08:07.572333 cnmf-1.5.1/src/
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:08:07.578814 cnmf-1.5.1/src/cnmf/
--rw-r--r--   0 dkotliar   (503) staff       (20)      131 2024-05-08 02:03:33.000000 cnmf-1.5.1/src/cnmf/__init__.py
--rwxr-xr-x   0 dkotliar   (503) staff       (20)    52529 2024-05-08 01:55:03.000000 cnmf-1.5.1/src/cnmf/cnmf.py
--rw-r--r--   0 dkotliar   (503) staff       (20)    20172 2024-05-08 01:55:03.000000 cnmf-1.5.1/src/cnmf/preprocess.py
--rw-r--r--   0 dkotliar   (503) staff       (20)       22 2024-05-08 02:03:15.000000 cnmf-1.5.1/src/cnmf/version.py
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:08:07.583459 cnmf-1.5.1/src/cnmf.egg-info/
--rw-r--r--   0 dkotliar   (503) staff       (20)     9225 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/PKG-INFO
--rw-r--r--   0 dkotliar   (503) staff       (20)      316 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/SOURCES.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)        1 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/dependency_links.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)       35 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/entry_points.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)       98 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/requires.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)        5 2024-05-08 02:08:07.000000 cnmf-1.5.1/src/cnmf.egg-info/top_level.txt
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:21:37.517779 cnmf-1.5.2/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1070 2024-05-08 02:12:41.000000 cnmf-1.5.2/LICENSE
+-rw-r--r--   0 dkotliar   (503) staff       (20)     8977 2024-05-08 02:21:37.517320 cnmf-1.5.2/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)     8519 2024-05-08 02:12:41.000000 cnmf-1.5.2/README.md
+-rw-r--r--   0 dkotliar   (503) staff       (20)      103 2024-05-08 02:12:41.000000 cnmf-1.5.2/pyproject.toml
+-rw-r--r--   0 dkotliar   (503) staff       (20)       38 2024-05-08 02:21:37.517919 cnmf-1.5.2/setup.cfg
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1333 2024-05-08 02:12:41.000000 cnmf-1.5.2/setup.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:21:37.510509 cnmf-1.5.2/src/
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:21:37.513951 cnmf-1.5.2/src/cnmf/
+-rw-r--r--   0 dkotliar   (503) staff       (20)      131 2024-05-08 02:12:41.000000 cnmf-1.5.2/src/cnmf/__init__.py
+-rwxr-xr-x   0 dkotliar   (503) staff       (20)    52658 2024-05-08 02:18:48.000000 cnmf-1.5.2/src/cnmf/cnmf.py
+-rw-r--r--   0 dkotliar   (503) staff       (20)    20172 2024-05-08 02:12:41.000000 cnmf-1.5.2/src/cnmf/preprocess.py
+-rw-r--r--   0 dkotliar   (503) staff       (20)       22 2024-05-08 02:20:54.000000 cnmf-1.5.2/src/cnmf/version.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 02:21:37.516679 cnmf-1.5.2/src/cnmf.egg-info/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     8977 2024-05-08 02:21:37.000000 cnmf-1.5.2/src/cnmf.egg-info/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)      316 2024-05-08 02:21:37.000000 cnmf-1.5.2/src/cnmf.egg-info/SOURCES.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        1 2024-05-08 02:21:37.000000 cnmf-1.5.2/src/cnmf.egg-info/dependency_links.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       35 2024-05-08 02:21:37.000000 cnmf-1.5.2/src/cnmf.egg-info/entry_points.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       98 2024-05-08 02:21:37.000000 cnmf-1.5.2/src/cnmf.egg-info/requires.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        5 2024-05-08 02:21:37.000000 cnmf-1.5.2/src/cnmf.egg-info/top_level.txt
```

### Comparing `cnmf-1.5.1/LICENSE` & `cnmf-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmf-1.5.1/PKG-INFO` & `cnmf-1.5.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: cnmf
-Version: 1.5.1
-Summary: Consensus NMF for scRNA-Seq data
-Home-page: https://github.com/dylkot/cNMF
-Author: Dylan Kotliar
-Author-email: dylkot@gmail.com
-Project-URL: Bug Tracker, https://github.com/dylkot/cNMF/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: scikit-learn>=1.0
-Requires-Dist: anndata>=0.9
-Requires-Dist: scanpy
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: fastcluster
-Requires-Dist: matplotlib
-Requires-Dist: palettable
-Requires-Dist: scipy
-Requires-Dist: pyyaml
-
 # Consensus NMF (cNMF)
 
 <img src="https://storage.googleapis.com/sabeti-public/dkotliar/elife-cNMF-fig1.jpg" style="height: 800px;" />
 
 cNMF is a pipeline for inferring gene expression programs from scRNA-Seq. It takes a count matrix (N cells X G genes) as input and produces a (K x G) matrix of gene expression programs (GEPs) and a (N x K) matrix specifying the usage of each program for each cell in the data. Read more about the method in the [publication](https://elifesciences.org/articles/43803) and check out examples on [simulated data](Tutorials/analyze_simulated_example_data.ipynb) and [PBMCs](Tutorials/analyze_pbmc_example_data.ipynb).
 
 # Installation
```

### Comparing `cnmf-1.5.1/README.md` & `cnmf-1.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: cnmf
+Version: 1.5.2
+Summary: Consensus NMF for scRNA-Seq data
+Home-page: https://github.com/dylkot/cNMF
+Author: Dylan Kotliar
+Author-email: dylkot@gmail.com
+Project-URL: Bug Tracker, https://github.com/dylkot/cNMF/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Consensus NMF (cNMF)
 
 <img src="https://storage.googleapis.com/sabeti-public/dkotliar/elife-cNMF-fig1.jpg" style="height: 800px;" />
 
 cNMF is a pipeline for inferring gene expression programs from scRNA-Seq. It takes a count matrix (N cells X G genes) as input and produces a (K x G) matrix of gene expression programs (GEPs) and a (N x K) matrix specifying the usage of each program for each cell in the data. Read more about the method in the [publication](https://elifesciences.org/articles/43803) and check out examples on [simulated data](Tutorials/analyze_simulated_example_data.ipynb) and [PBMCs](Tutorials/analyze_pbmc_example_data.ipynb).
 
 # Installation
```

### Comparing `cnmf-1.5.1/setup.py` & `cnmf-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `cnmf-1.5.1/src/cnmf/cnmf.py` & `cnmf-1.5.2/src/cnmf/cnmf.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from fastcluster import linkage
 from scipy.cluster.hierarchy import leaves_list
 
 import matplotlib.pyplot as plt
 
 import scanpy as sc
 
+from .version import __version__
+
 from multiprocessing import Pool 
 
 
 def save_df_to_npz(obj, filename):
     np.savez_compressed(filename, data=obj.values, index=obj.index.values, columns=obj.columns.values)
 
 def save_df_to_text(obj, filename):
@@ -1086,15 +1088,15 @@
 
         python cnmf.py consensus  --name test --output-dir $output_dir
 
     """
 
     import sys, argparse
     parser = argparse.ArgumentParser()
-
+    parser.add_argument('-v', '--version', action='version', version=f'%(prog)s {__version__}')
     parser.add_argument('command', type=str, choices=['prepare', 'factorize', 'combine', 'consensus', 'k_selection_plot'])
     parser.add_argument('--name', type=str, help='[all] Name for analysis. All output will be placed in [output-dir]/[name]/...', nargs='?', default='cNMF')
     parser.add_argument('--output-dir', type=str, help='[all] Output directory. All output will be placed in [output-dir]/[name]/...', nargs='?', default='.')
     parser.add_argument('-c', '--counts', type=str, help='[prepare] Input (cell x gene) counts matrix as df.npz or tab delimited text file')
     parser.add_argument('-k', '--components', type=int, help='[prepare] Numper of components (k) for matrix factorization. Several can be specified with "-k 8 9 10"', nargs='+')
     parser.add_argument('-n', '--n-iter', type=int, help='[prepare] Number of factorization replicates', default=100)
     parser.add_argument('--total-workers', type=int, help='[all] Total number of workers to distribute jobs to', default=1)
```

### Comparing `cnmf-1.5.1/src/cnmf/preprocess.py` & `cnmf-1.5.2/src/cnmf/preprocess.py`

 * *Files identical despite different names*

### Comparing `cnmf-1.5.1/src/cnmf.egg-info/PKG-INFO` & `cnmf-1.5.2/src/cnmf.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 Metadata-Version: 2.1
 Name: cnmf
-Version: 1.5.1
+Version: 1.5.2
 Summary: Consensus NMF for scRNA-Seq data
 Home-page: https://github.com/dylkot/cNMF
 Author: Dylan Kotliar
 Author-email: dylkot@gmail.com
 Project-URL: Bug Tracker, https://github.com/dylkot/cNMF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: scikit-learn>=1.0
-Requires-Dist: anndata>=0.9
-Requires-Dist: scanpy
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: fastcluster
-Requires-Dist: matplotlib
-Requires-Dist: palettable
-Requires-Dist: scipy
-Requires-Dist: pyyaml
 
 # Consensus NMF (cNMF)
 
 <img src="https://storage.googleapis.com/sabeti-public/dkotliar/elife-cNMF-fig1.jpg" style="height: 800px;" />
 
 cNMF is a pipeline for inferring gene expression programs from scRNA-Seq. It takes a count matrix (N cells X G genes) as input and produces a (K x G) matrix of gene expression programs (GEPs) and a (N x K) matrix specifying the usage of each program for each cell in the data. Read more about the method in the [publication](https://elifesciences.org/articles/43803) and check out examples on [simulated data](Tutorials/analyze_simulated_example_data.ipynb) and [PBMCs](Tutorials/analyze_pbmc_example_data.ipynb).
```

