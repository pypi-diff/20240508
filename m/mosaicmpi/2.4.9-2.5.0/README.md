# Comparing `tmp/mosaicmpi-2.4.9.tar.gz` & `tmp/mosaicmpi-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicmpi-2.4.9.tar", last modified: Wed Apr 24 04:01:02 2024, max compression
+gzip compressed data, was "mosaicmpi-2.5.0.tar", last modified: Wed May  8 16:17:35 2024, max compression
```

## Comparing `mosaicmpi-2.4.9.tar` & `mosaicmpi-2.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 04:01:02.925857 mosaicmpi-2.4.9/
--rw-rw-rw-   0        0        0     1090 2023-08-21 20:09:52.000000 mosaicmpi-2.4.9/LICENSE
--rw-rw-rw-   0        0        0     4517 2024-04-24 04:01:02.924855 mosaicmpi-2.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     3489 2024-04-24 03:56:06.000000 mosaicmpi-2.4.9/README.md
--rw-rw-rw-   0        0        0       86 2023-08-21 03:26:20.000000 mosaicmpi-2.4.9/pyproject.toml
--rw-rw-rw-   0        0        0     1002 2024-04-24 04:01:02.926869 mosaicmpi-2.4.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-24 04:01:02.872254 mosaicmpi-2.4.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 04:01:02.896913 mosaicmpi-2.4.9/src/mosaicmpi/
--rw-rw-rw-   0        0        0      550 2024-01-30 22:56:25.000000 mosaicmpi-2.4.9/src/mosaicmpi/__init__.py
--rw-rw-rw-   0        0        0    17785 2023-11-29 18:30:29.000000 mosaicmpi-2.4.9/src/mosaicmpi/biomart.py
--rw-rw-rw-   0        0        0    69264 2024-02-08 04:04:02.000000 mosaicmpi-2.4.9/src/mosaicmpi/cli.py
--rw-rw-rw-   0        0        0    36516 2024-04-24 03:51:35.000000 mosaicmpi-2.4.9/src/mosaicmpi/cnmf.py
--rw-rw-rw-   0        0        0    16074 2024-01-13 03:13:37.000000 mosaicmpi-2.4.9/src/mosaicmpi/colors.py
--rw-rw-rw-   0        0        0     3126 2023-09-14 15:15:14.000000 mosaicmpi-2.4.9/src/mosaicmpi/config.py
--rw-rw-rw-   0        0        0    58396 2024-03-25 17:20:06.000000 mosaicmpi-2.4.9/src/mosaicmpi/dataset.py
--rw-rw-rw-   0        0        0     3751 2024-02-23 18:15:35.000000 mosaicmpi-2.4.9/src/mosaicmpi/gprofiler.py
--rw-rw-rw-   0        0        0    23345 2024-02-20 17:12:09.000000 mosaicmpi-2.4.9/src/mosaicmpi/integration.py
--rw-rw-rw-   0        0        0     6613 2023-08-21 03:26:20.000000 mosaicmpi-2.4.9/src/mosaicmpi/nancorrmp.py
--rw-rw-rw-   0        0        0    53535 2024-02-02 18:58:00.000000 mosaicmpi-2.4.9/src/mosaicmpi/network.py
--rw-rw-rw-   0        0        0     9186 2023-09-13 17:49:00.000000 mosaicmpi-2.4.9/src/mosaicmpi/orphan.py
--rw-rw-rw-   0        0        0    79357 2024-02-07 22:09:34.000000 mosaicmpi-2.4.9/src/mosaicmpi/plots.py
--rw-rw-rw-   0        0        0     5798 2024-01-19 19:04:03.000000 mosaicmpi-2.4.9/src/mosaicmpi/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 04:01:02.923856 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/
--rw-rw-rw-   0        0        0     4517 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      178 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-24 04:01:02.000000 mosaicmpi-2.4.9/src/mosaicmpi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 16:17:35.384105 mosaicmpi-2.5.0/
+-rw-rw-rw-   0        0        0     1090 2024-05-08 16:00:07.000000 mosaicmpi-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0     4572 2024-05-08 16:17:35.384105 mosaicmpi-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3544 2024-05-08 16:15:02.000000 mosaicmpi-2.5.0/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1002 2024-05-08 16:17:35.387095 mosaicmpi-2.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 16:17:35.168867 mosaicmpi-2.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 16:17:35.341608 mosaicmpi-2.5.0/src/mosaicmpi/
+-rw-rw-rw-   0        0        0      550 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/__init__.py
+-rw-rw-rw-   0        0        0    17785 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/biomart.py
+-rw-rw-rw-   0        0        0    69264 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/cli.py
+-rw-rw-rw-   0        0        0    36516 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/cnmf.py
+-rw-rw-rw-   0        0        0    16074 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/colors.py
+-rw-rw-rw-   0        0        0     3126 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/config.py
+-rw-rw-rw-   0        0        0    62746 2024-05-08 16:15:38.000000 mosaicmpi-2.5.0/src/mosaicmpi/dataset.py
+-rw-rw-rw-   0        0        0     3751 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/gprofiler.py
+-rw-rw-rw-   0        0        0    23345 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/integration.py
+-rw-rw-rw-   0        0        0     6613 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/nancorrmp.py
+-rw-rw-rw-   0        0        0    53535 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/network.py
+-rw-rw-rw-   0        0        0     9186 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/orphan.py
+-rw-rw-rw-   0        0        0    79357 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/plots.py
+-rw-rw-rw-   0        0        0     5798 2024-04-30 19:18:00.000000 mosaicmpi-2.5.0/src/mosaicmpi/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:17:35.383096 mosaicmpi-2.5.0/src/mosaicmpi.egg-info/
+-rw-rw-rw-   0        0        0     4572 2024-05-08 16:17:35.000000 mosaicmpi-2.5.0/src/mosaicmpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2024-05-08 16:17:35.000000 mosaicmpi-2.5.0/src/mosaicmpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 16:17:35.000000 mosaicmpi-2.5.0/src/mosaicmpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-08 16:17:35.000000 mosaicmpi-2.5.0/src/mosaicmpi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      178 2024-05-08 16:17:35.000000 mosaicmpi-2.5.0/src/mosaicmpi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 16:17:35.000000 mosaicmpi-2.5.0/src/mosaicmpi.egg-info/top_level.txt
```

### Comparing `mosaicmpi-2.4.9/LICENSE` & `mosaicmpi-2.5.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Morrissy Lab
+Copyright (c) 2024 Morrissy Lab
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mosaicmpi-2.4.9/PKG-INFO` & `mosaicmpi-2.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicmpi
-Version: 2.4.9
+Version: 2.5.0
 Summary: mosaicMPI: Mosaic Multi-resolution Program Integration
 Home-page: https://github.com/MorrissyLab/mosaicMPI
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/mosaicMPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,54 +30,54 @@
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
 Requires-Dist: fastcluster
 Requires-Dist: tqdm
 
 ![mosaicMPI logo](https://github.com/MorrissyLab/mosaicMPI/blob/main/docs/source/_static/img/logo.png?raw=True)
 
-# mosaicMPI: mosaic multi-resolution program integration
+# mosaicMPI: Mosaic Multi-resolution Program Integration
 
-![version badge](https://img.shields.io/badge/version-2.4.9-blue)
+![version badge](https://img.shields.io/badge/version-2.5.0-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mosaicmpi.svg)](https://pypi.org/project/mosaicmpi/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/mosaicmpi)](https://anaconda.org/conda-forge/mosaicmpi/)
 [![Documentation status](https://readthedocs.org/projects/mosaicmpi/badge/?version=latest&style=flat)](https://mosaicmpi.readthedocs.io)
 [![Downloads](https://static.pepy.tech/badge/mosaicmpi)](https://pepy.tech/project/mosaicmpi)
 [![Stars](https://img.shields.io/github/stars/MorrissyLab/mosaicMPI?logo=GitHub&color=yellow)](https://github.com/MorrissyLab/mosaicMPI/stargazers)
 [![License](https://img.shields.io/pypi/l/mosaicmpi.svg)](https://github.com/MorrissyLab/mosaicMPI/blob/main/LICENSE)
 [![DOI:10.1101/2023.08.18.553919](http://img.shields.io/badge/DOI-10.1101/2023.08.18.553919-B31B1B.svg)](https://doi.org/10.1101/2023.08.18.553919)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Sorana Morrissy](https://github.com/ancasorana)
 
 Contributors: Hyojin Song, Aaron Gillmor, Gurveer Gill, Courtney Hall
 
-**mosaicMPI** is a Python package enabling mosaic integration of bulk, single-cell, and spatial expression data through program-level integration.
-Programs are first discovered using consensus non-negative matrix factorization and then integrated using a flexible network-based approach to
-group similar programs together across resolutions and datasets. Program communities are then interpreted using sample/cell metadata and gene set analyses. Integrative program communities enable metadata transfer across datasets.
+**mosaicMPI** is a Python package for enabling mosaic integration of bulk, single-cell, and spatial expression data through program-level integration. Programs are first discovered using unsupervised deconvolution (consensus non-negative matrix factorization, cNMF) across multiple ranks separately for each dataset. A flexible network-based approach groups similar programs together across resolutions and datasets. Program communities are then interpreted using sample/cell metadata and gene set analyses. Integrative program communities enable metadata transfer across datasets.
 
 ## ⚡Main Features
 
 Here are just a few of the things that mosaicMPI does well:
 
 - Identifies interpretable, non-negative programs at multiple resolutions
 - Mosaic integration does not require subsetting features/genes to
   a shared or overdispersed subset
 - Multi-omics integration without shared sample IDs
-- Ideal for incremental integration (adding datasets one at a time) since
+- Incremental integration (adding datasets one at a time) since
   deconvolution is performed independently on each dataset
-- Integration performs well even when the datasets have mismatched features
-  (eg. Microarray, RNA-Seq, Proteomics) or sparsity (eg single-cell vs bulk RNA-Seq and ATAC-Seq)
+- High performance integration of of datasets with mismatched features
+  (eg. Microarray, RNA-Seq, Proteomics) or sparsity (eg. single-cell vs. bulk)
 - Metadata transfer across datasets
-- Command-line interface for rapid data exploration and python
-  interface for extensibility and flexibility
+
+mosaicMPI is usable via:
+- command-line interface for rapid data exploration and integration
+- python interface for extensibility and flexibility
 
 ## 🔧 Install
 
 ### 🧰 System Requirements
 
-- Compatible with and tested on OS X, Windows and Linux systems
+- Compatible with OS X, Windows and Linux systems
 - Memory usage depends on size and number of datasets
 
 ### ✨ Latest Release
 Install the package with `conda`:
 ```bash
 # create an environment called mosaic and install
 conda create -n mosaic -c conda-forge mosaicmpi
@@ -95,8 +95,8 @@
 
 ## 📖 Documentation
 
 Read the [documentation](https://mosaicmpi.readthedocs.io/).
 
 ## 💭 Getting Help
 
-For errors arising during use of mosaicMPI, create and browse issues in the [GitHub "issues" tab](https://github.com/MorrissyLab/mosaicMPI/issues).
+For questions arising during use of mosaicMPI, create and browse issues in the [GitHub "issues" tab](https://github.com/MorrissyLab/mosaicMPI/issues).
```

### Comparing `mosaicmpi-2.4.9/README.md` & `mosaicmpi-2.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 ![mosaicMPI logo](https://github.com/MorrissyLab/mosaicMPI/blob/main/docs/source/_static/img/logo.png?raw=True)
 
-# mosaicMPI: mosaic multi-resolution program integration
+# mosaicMPI: Mosaic Multi-resolution Program Integration
 
-![version badge](https://img.shields.io/badge/version-2.4.9-blue)
+![version badge](https://img.shields.io/badge/version-2.5.0-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mosaicmpi.svg)](https://pypi.org/project/mosaicmpi/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/mosaicmpi)](https://anaconda.org/conda-forge/mosaicmpi/)
 [![Documentation status](https://readthedocs.org/projects/mosaicmpi/badge/?version=latest&style=flat)](https://mosaicmpi.readthedocs.io)
 [![Downloads](https://static.pepy.tech/badge/mosaicmpi)](https://pepy.tech/project/mosaicmpi)
 [![Stars](https://img.shields.io/github/stars/MorrissyLab/mosaicMPI?logo=GitHub&color=yellow)](https://github.com/MorrissyLab/mosaicMPI/stargazers)
 [![License](https://img.shields.io/pypi/l/mosaicmpi.svg)](https://github.com/MorrissyLab/mosaicMPI/blob/main/LICENSE)
 [![DOI:10.1101/2023.08.18.553919](http://img.shields.io/badge/DOI-10.1101/2023.08.18.553919-B31B1B.svg)](https://doi.org/10.1101/2023.08.18.553919)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Sorana Morrissy](https://github.com/ancasorana)
 
 Contributors: Hyojin Song, Aaron Gillmor, Gurveer Gill, Courtney Hall
 
-**mosaicMPI** is a Python package enabling mosaic integration of bulk, single-cell, and spatial expression data through program-level integration.
-Programs are first discovered using consensus non-negative matrix factorization and then integrated using a flexible network-based approach to
-group similar programs together across resolutions and datasets. Program communities are then interpreted using sample/cell metadata and gene set analyses. Integrative program communities enable metadata transfer across datasets.
+**mosaicMPI** is a Python package for enabling mosaic integration of bulk, single-cell, and spatial expression data through program-level integration. Programs are first discovered using unsupervised deconvolution (consensus non-negative matrix factorization, cNMF) across multiple ranks separately for each dataset. A flexible network-based approach groups similar programs together across resolutions and datasets. Program communities are then interpreted using sample/cell metadata and gene set analyses. Integrative program communities enable metadata transfer across datasets.
 
 ## ⚡Main Features
 
 Here are just a few of the things that mosaicMPI does well:
 
 - Identifies interpretable, non-negative programs at multiple resolutions
 - Mosaic integration does not require subsetting features/genes to
   a shared or overdispersed subset
 - Multi-omics integration without shared sample IDs
-- Ideal for incremental integration (adding datasets one at a time) since
+- Incremental integration (adding datasets one at a time) since
   deconvolution is performed independently on each dataset
-- Integration performs well even when the datasets have mismatched features
-  (eg. Microarray, RNA-Seq, Proteomics) or sparsity (eg single-cell vs bulk RNA-Seq and ATAC-Seq)
+- High performance integration of of datasets with mismatched features
+  (eg. Microarray, RNA-Seq, Proteomics) or sparsity (eg. single-cell vs. bulk)
 - Metadata transfer across datasets
-- Command-line interface for rapid data exploration and python
-  interface for extensibility and flexibility
+
+mosaicMPI is usable via:
+- command-line interface for rapid data exploration and integration
+- python interface for extensibility and flexibility
 
 ## 🔧 Install
 
 ### 🧰 System Requirements
 
-- Compatible with and tested on OS X, Windows and Linux systems
+- Compatible with OS X, Windows and Linux systems
 - Memory usage depends on size and number of datasets
 
 ### ✨ Latest Release
 Install the package with `conda`:
 ```bash
 # create an environment called mosaic and install
 conda create -n mosaic -c conda-forge mosaicmpi
@@ -61,8 +61,8 @@
 
 ## 📖 Documentation
 
 Read the [documentation](https://mosaicmpi.readthedocs.io/).
 
 ## 💭 Getting Help
 
-For errors arising during use of mosaicMPI, create and browse issues in the [GitHub "issues" tab](https://github.com/MorrissyLab/mosaicMPI/issues).
+For questions arising during use of mosaicMPI, create and browse issues in the [GitHub "issues" tab](https://github.com/MorrissyLab/mosaicMPI/issues).
```

### Comparing `mosaicmpi-2.4.9/setup.cfg` & `mosaicmpi-2.5.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f73 6169 636d 7069 0d0a 7665   = mosaicmpi..ve
-00000020: 7273 696f 6e20 3d20 322e 342e 390d 0a61  rsion = 2.4.9..a
+00000020: 7273 696f 6e20 3d20 322e 352e 300d 0a61  rsion = 2.5.0..a
 00000030: 7574 686f 7220 3d20 5465 6420 5665 7268  uthor = Ted Verh
 00000040: 6579 0d0a 6175 7468 6f72 5f65 6d61 696c  ey..author_email
 00000050: 203d 2074 6276 6572 6865 7940 7563 616c   = tbverhey@ucal
 00000060: 6761 7279 2e63 610d 0a64 6573 6372 6970  gary.ca..descrip
 00000070: 7469 6f6e 203d 206d 6f73 6169 634d 5049  tion = mosaicMPI
 00000080: 3a20 4d6f 7361 6963 204d 756c 7469 2d72  : Mosaic Multi-r
 00000090: 6573 6f6c 7574 696f 6e20 5072 6f67 7261  esolution Progra
```

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/__init__.py` & `mosaicmpi-2.5.0/src/mosaicmpi/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/biomart.py` & `mosaicmpi-2.5.0/src/mosaicmpi/biomart.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/cli.py` & `mosaicmpi-2.5.0/src/mosaicmpi/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/cnmf.py` & `mosaicmpi-2.5.0/src/mosaicmpi/cnmf.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/colors.py` & `mosaicmpi-2.5.0/src/mosaicmpi/colors.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/config.py` & `mosaicmpi-2.5.0/src/mosaicmpi/config.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/dataset.py` & `mosaicmpi-2.5.0/src/mosaicmpi/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -833,2818 +833,3090 @@
 00003400: 7375 6d22 5d2c 206f 7074 696f 6e61 6c0d  sum"], optional.
 00003410: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
 00003420: 756e 6d61 7070 6564 5f70 7265 6669 783a  unmapped_prefix:
 00003430: 2046 6f72 2075 6e6d 6170 7065 6420 6665   For unmapped fe
 00003440: 6174 7572 6573 2c20 7072 6570 656e 6420  atures, prepend 
 00003450: 7468 6973 2074 6578 7420 746f 2074 6865  this text to the
 00003460: 6972 2049 442c 2064 6566 6175 6c74 7320  ir ID, defaults 
-00003470: 746f 2022 756e 6d61 7070 6564 5c5f 220d  to "unmapped\_".
-00003480: 0a20 2020 2020 2020 203a 7479 7065 2075  .        :type u
-00003490: 6e6d 6170 7065 645f 7072 6566 6978 3a20  nmapped_prefix: 
-000034a0: 7374 722c 206f 7074 696f 6e61 6c0d 0a20  str, optional.. 
-000034b0: 2020 2020 2020 203a 7061 7261 6d20 6361         :param ca
-000034c0: 7365 5f73 656e 7369 7469 7665 3a20 4361  se_sensitive: Ca
-000034d0: 7365 2d73 656e 7369 7469 7665 2049 4420  se-sensitive ID 
-000034e0: 6d61 7463 6869 6e67 2c20 6465 6661 756c  matching, defaul
-000034f0: 7473 2074 6f20 4661 6c73 650d 0a20 2020  ts to False..   
-00003500: 2020 2020 203a 7479 7065 2063 6173 655f       :type case_
-00003510: 7365 6e73 6974 6976 653a 2062 6f6f 6c2c  sensitive: bool,
-00003520: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-00003530: 2020 203a 7061 7261 6d20 6269 6f6d 6172     :param biomar
-00003540: 745f 7572 6c3a 2055 524c 2074 6f20 636f  t_url: URL to co
-00003550: 6e6e 6563 7420 746f 2074 6865 2042 696f  nnect to the Bio
-00003560: 6d61 7274 2077 6562 2073 6572 7665 722c  mart web server,
-00003570: 2064 6566 6175 6c74 7320 746f 0d0a 2020   defaults to..  
+00003470: 746f 2022 756e 6d61 7070 6564 5c5c 5f22  to "unmapped\\_"
+00003480: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00003490: 756e 6d61 7070 6564 5f70 7265 6669 783a  unmapped_prefix:
+000034a0: 2073 7472 2c20 6f70 7469 6f6e 616c 0d0a   str, optional..
+000034b0: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
+000034c0: 6173 655f 7365 6e73 6974 6976 653a 2043  ase_sensitive: C
+000034d0: 6173 652d 7365 6e73 6974 6976 6520 4944  ase-sensitive ID
+000034e0: 206d 6174 6368 696e 672c 2064 6566 6175   matching, defau
+000034f0: 6c74 7320 746f 2046 616c 7365 0d0a 2020  lts to False..  
+00003500: 2020 2020 2020 3a74 7970 6520 6361 7365        :type case
+00003510: 5f73 656e 7369 7469 7665 3a20 626f 6f6c  _sensitive: bool
+00003520: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00003530: 2020 2020 3a70 6172 616d 2062 696f 6d61      :param bioma
+00003540: 7274 5f75 726c 3a20 5552 4c20 746f 2063  rt_url: URL to c
+00003550: 6f6e 6e65 6374 2074 6f20 7468 6520 4269  onnect to the Bi
+00003560: 6f6d 6172 7420 7765 6220 7365 7276 6572  omart web server
+00003570: 2c20 6465 6661 756c 7473 2074 6f0d 0a20  , defaults to.. 
 00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003590: 2020 2020 2020 2020 2020 2268 7474 703a            "http:
-000035a0: 2f2f 7777 772e 656e 7365 6d62 6c2e 6f72  //www.ensembl.or
-000035b0: 673a 3830 2f62 696f 6d61 7274 2f6d 6172  g:80/biomart/mar
-000035c0: 7473 6572 7669 6365 220d 0a20 2020 2020  tservice"..     
-000035d0: 2020 203a 7479 7065 2062 696f 6d61 7274     :type biomart
-000035e0: 5f75 726c 3a20 7374 722c 206f 7074 696f  _url: str, optio
-000035f0: 6e61 6c0d 0a20 2020 2020 2020 203a 7261  nal..        :ra
-00003600: 6973 6573 204e 6f74 496d 706c 656d 656e  ises NotImplemen
-00003610: 7465 6445 7272 6f72 3a20 666f 7220 6665  tedError: for fe
-00003620: 6174 7572 6573 206e 6574 2079 6574 2069  atures net yet i
-00003630: 6d70 6c65 6d65 6e74 6564 2c20 696e 636c  mplemented, incl
-00003640: 7564 696e 6720 6d61 6e79 2d74 6f2d 6f6e  uding many-to-on
-00003650: 6520 616e 6420 6d61 6e79 2d74 6f2d 6d61  e and many-to-ma
-00003660: 6e79 2067 656e 6520 6d61 7070 696e 6773  ny gene mappings
-00003670: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00003680: 2020 2020 2020 206c 6f67 6769 6e67 2e69         logging.i
-00003690: 6e66 6f28 2244 6f77 6e6c 6f61 6469 6e67  nfo("Downloading
-000036a0: 2067 656e 6520 4944 2074 6162 6c65 2066   gene ID table f
-000036b0: 726f 6d20 456e 7365 6d62 6c20 4269 6f6d  rom Ensembl Biom
-000036c0: 6172 7422 290d 0a20 2020 2020 2020 2067  art")..        g
-000036d0: 656e 655f 6461 7461 7365 7420 3d20 6269  ene_dataset = bi
-000036e0: 6f6d 6172 742e 4269 6f6d 6172 7453 6572  omart.BiomartSer
-000036f0: 7665 7228 7572 6c3d 6269 6f6d 6172 745f  ver(url=biomart_
-00003700: 7572 6c29 2e64 6174 6173 6574 735b 6622  url).datasets[f"
-00003710: 7b73 6f75 7263 655f 7370 6563 6965 737d  {source_species}
-00003720: 5f67 656e 655f 656e 7365 6d62 6c22 5d0d  _gene_ensembl"].
-00003730: 0a20 2020 2020 2020 2069 6620 736f 7572  .        if sour
-00003740: 6365 5f73 7065 6369 6573 203d 3d20 6465  ce_species == de
-00003750: 7374 5f73 7065 6369 6573 3a0d 0a20 2020  st_species:..   
-00003760: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-00003770: 3d20 6765 6e65 5f64 6174 6173 6574 2e73  = gene_dataset.s
-00003780: 6561 7263 6828 7061 7261 6d73 3d7b 2261  earch(params={"a
-00003790: 7474 7269 6275 7465 7322 3a20 5b22 6578  ttributes": ["ex
-000037a0: 7465 726e 616c 5f67 656e 655f 6e61 6d65  ternal_gene_name
-000037b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00003590: 2020 2020 2020 2020 2020 2022 6874 7470             "http
+000035a0: 3a2f 2f77 7777 2e65 6e73 656d 626c 2e6f  ://www.ensembl.o
+000035b0: 7267 3a38 302f 6269 6f6d 6172 742f 6d61  rg:80/biomart/ma
+000035c0: 7274 7365 7276 6963 6522 0d0a 2020 2020  rtservice"..    
+000035d0: 2020 2020 3a74 7970 6520 6269 6f6d 6172      :type biomar
+000035e0: 745f 7572 6c3a 2073 7472 2c20 6f70 7469  t_url: str, opti
+000035f0: 6f6e 616c 0d0a 2020 2020 2020 2020 3a72  onal..        :r
+00003600: 6169 7365 7320 4e6f 7449 6d70 6c65 6d65  aises NotImpleme
+00003610: 6e74 6564 4572 726f 723a 2066 6f72 2066  ntedError: for f
+00003620: 6561 7475 7265 7320 6e65 7420 7965 7420  eatures net yet 
+00003630: 696d 706c 656d 656e 7465 642c 2069 6e63  implemented, inc
+00003640: 6c75 6469 6e67 206d 616e 792d 746f 2d6f  luding many-to-o
+00003650: 6e65 2061 6e64 206d 616e 792d 746f 2d6d  ne and many-to-m
+00003660: 616e 7920 6765 6e65 206d 6170 7069 6e67  any gene mapping
+00003670: 730d 0a20 2020 2020 2020 2022 2222 0d0a  s..        """..
+00003680: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+00003690: 696e 666f 2822 446f 776e 6c6f 6164 696e  info("Downloadin
+000036a0: 6720 6765 6e65 2049 4420 7461 626c 6520  g gene ID table 
+000036b0: 6672 6f6d 2045 6e73 656d 626c 2042 696f  from Ensembl Bio
+000036c0: 6d61 7274 2229 0d0a 2020 2020 2020 2020  mart")..        
+000036d0: 6765 6e65 5f64 6174 6173 6574 203d 2062  gene_dataset = b
+000036e0: 696f 6d61 7274 2e42 696f 6d61 7274 5365  iomart.BiomartSe
+000036f0: 7276 6572 2875 726c 3d62 696f 6d61 7274  rver(url=biomart
+00003700: 5f75 726c 292e 6461 7461 7365 7473 5b66  _url).datasets[f
+00003710: 227b 736f 7572 6365 5f73 7065 6369 6573  "{source_species
+00003720: 7d5f 6765 6e65 5f65 6e73 656d 626c 225d  }_gene_ensembl"]
+00003730: 0d0a 2020 2020 2020 2020 6966 2073 6f75  ..        if sou
+00003740: 7263 655f 7370 6563 6965 7320 3d3d 2064  rce_species == d
+00003750: 6573 745f 7370 6563 6965 733a 0d0a 2020  est_species:..  
+00003760: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00003770: 203d 2067 656e 655f 6461 7461 7365 742e   = gene_dataset.
+00003780: 7365 6172 6368 2870 6172 616d 733d 7b22  search(params={"
+00003790: 6174 7472 6962 7574 6573 223a 205b 2265  attributes": ["e
+000037a0: 7874 6572 6e61 6c5f 6765 6e65 5f6e 616d  xternal_gene_nam
+000037b0: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
 000037c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000037d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037f0: 2020 2020 2265 6e73 656d 626c 5f67 656e      "ensembl_gen
-00003800: 655f 6964 225d 7d29 0d0a 2020 2020 2020  e_id"]})..      
-00003810: 2020 2020 2020 636f 6c75 6d6e 733d 5b27        columns=['
-00003820: 736f 7572 6365 5f67 656e 655f 6e61 6d65  source_gene_name
-00003830: 272c 2773 6f75 7263 655f 656e 7365 6d62  ','source_ensemb
-00003840: 6c5f 6765 6e65 275d 0d0a 2020 2020 2020  l_gene']..      
-00003850: 2020 2020 2020 7265 7375 6c74 203d 2070        result = p
-00003860: 642e 7265 6164 5f63 7376 2853 7472 696e  d.read_csv(Strin
-00003870: 6749 4f28 7265 7375 6c74 2e74 6578 7429  gIO(result.text)
-00003880: 2c20 7365 703d 225c 7422 2c20 6865 6164  , sep="\t", head
-00003890: 6572 3d4e 6f6e 652c 206e 616d 6573 3d63  er=None, names=c
-000038a0: 6f6c 756d 6e73 290d 0a20 2020 2020 2020  olumns)..       
-000038b0: 2020 2020 2073 6f75 7263 655f 636f 6c20       source_col 
-000038c0: 3d20 6622 736f 7572 6365 5f7b 736f 7572  = f"source_{sour
-000038d0: 6365 5f69 6473 7d22 0d0a 2020 2020 2020  ce_ids}"..      
-000038e0: 2020 2020 2020 6465 7374 5f63 6f6c 203d        dest_col =
-000038f0: 2066 2273 6f75 7263 655f 7b64 6573 745f   f"source_{dest_
-00003900: 6964 737d 220d 0a20 2020 2020 2020 2065  ids}"..        e
-00003910: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00003920: 2020 7265 7375 6c74 203d 2067 656e 655f    result = gene_
-00003930: 6461 7461 7365 742e 7365 6172 6368 2870  dataset.search(p
-00003940: 6172 616d 733d 7b22 6174 7472 6962 7574  arams={"attribut
-00003950: 6573 223a 205b 2265 7874 6572 6e61 6c5f  es": ["external_
-00003960: 6765 6e65 5f6e 616d 6522 2c0d 0a20 2020  gene_name",..   
+000037f0: 2020 2020 2022 656e 7365 6d62 6c5f 6765       "ensembl_ge
+00003800: 6e65 5f69 6422 5d7d 290d 0a20 2020 2020  ne_id"]})..     
+00003810: 2020 2020 2020 2063 6f6c 756d 6e73 3d5b         columns=[
+00003820: 2773 6f75 7263 655f 6765 6e65 5f6e 616d  'source_gene_nam
+00003830: 6527 2c27 736f 7572 6365 5f65 6e73 656d  e','source_ensem
+00003840: 626c 5f67 656e 6527 5d0d 0a20 2020 2020  bl_gene']..     
+00003850: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00003860: 7064 2e72 6561 645f 6373 7628 5374 7269  pd.read_csv(Stri
+00003870: 6e67 494f 2872 6573 756c 742e 7465 7874  ngIO(result.text
+00003880: 292c 2073 6570 3d22 5c74 222c 2068 6561  ), sep="\t", hea
+00003890: 6465 723d 4e6f 6e65 2c20 6e61 6d65 733d  der=None, names=
+000038a0: 636f 6c75 6d6e 7329 0d0a 2020 2020 2020  columns)..      
+000038b0: 2020 2020 2020 736f 7572 6365 5f63 6f6c        source_col
+000038c0: 203d 2066 2273 6f75 7263 655f 7b73 6f75   = f"source_{sou
+000038d0: 7263 655f 6964 737d 220d 0a20 2020 2020  rce_ids}"..     
+000038e0: 2020 2020 2020 2064 6573 745f 636f 6c20         dest_col 
+000038f0: 3d20 6622 736f 7572 6365 5f7b 6465 7374  = f"source_{dest
+00003900: 5f69 6473 7d22 0d0a 2020 2020 2020 2020  _ids}"..        
+00003910: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00003920: 2020 2072 6573 756c 7420 3d20 6765 6e65     result = gene
+00003930: 5f64 6174 6173 6574 2e73 6561 7263 6828  _dataset.search(
+00003940: 7061 7261 6d73 3d7b 2261 7474 7269 6275  params={"attribu
+00003950: 7465 7322 3a20 5b22 6578 7465 726e 616c  tes": ["external
+00003960: 5f67 656e 655f 6e61 6d65 222c 0d0a 2020  _gene_name",..  
 00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039a0: 2020 2020 2020 2020 2022 656e 7365 6d62           "ensemb
-000039b0: 6c5f 6765 6e65 5f69 6422 2c0d 0a20 2020  l_gene_id",..   
+000039a0: 2020 2020 2020 2020 2020 2265 6e73 656d            "ensem
+000039b0: 626c 5f67 656e 655f 6964 222c 0d0a 2020  bl_gene_id",..  
 000039c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000039e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039f0: 2020 2020 2020 2020 2066 227b 6465 7374           f"{dest
-00003a00: 5f73 7065 6369 6573 7d5f 686f 6d6f 6c6f  _species}_homolo
-00003a10: 675f 6173 736f 6369 6174 6564 5f67 656e  g_associated_gen
-00003a20: 655f 6e61 6d65 222c 0d0a 2020 2020 2020  e_name",..      
+000039f0: 2020 2020 2020 2020 2020 6622 7b64 6573            f"{des
+00003a00: 745f 7370 6563 6965 737d 5f68 6f6d 6f6c  t_species}_homol
+00003a10: 6f67 5f61 7373 6f63 6961 7465 645f 6765  og_associated_ge
+00003a20: 6e65 5f6e 616d 6522 2c0d 0a20 2020 2020  ne_name",..     
 00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 2020 2020 2020 6622 7b64 6573 745f 7370        f"{dest_sp
-00003a70: 6563 6965 737d 5f68 6f6d 6f6c 6f67 5f65  ecies}_homolog_e
-00003a80: 6e73 656d 626c 5f67 656e 6522 5d7d 290d  nsembl_gene"]}).
-00003a90: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00003aa0: 756d 6e73 3d5b 2773 6f75 7263 655f 6765  umns=['source_ge
-00003ab0: 6e65 5f6e 616d 6527 2c27 736f 7572 6365  ne_name','source
-00003ac0: 5f65 6e73 656d 626c 5f67 656e 6527 2c20  _ensembl_gene', 
-00003ad0: 2764 6573 745f 6765 6e65 5f6e 616d 6527  'dest_gene_name'
-00003ae0: 2c20 2764 6573 745f 656e 7365 6d62 6c5f  , 'dest_ensembl_
-00003af0: 6765 6e65 275d 0d0a 2020 2020 2020 2020  gene']..        
-00003b00: 2020 2020 7265 7375 6c74 203d 2070 642e      result = pd.
-00003b10: 7265 6164 5f63 7376 2853 7472 696e 6749  read_csv(StringI
-00003b20: 4f28 7265 7375 6c74 2e74 6578 7429 2c20  O(result.text), 
-00003b30: 7365 703d 225c 7422 2c20 6865 6164 6572  sep="\t", header
-00003b40: 3d4e 6f6e 652c 206e 616d 6573 3d63 6f6c  =None, names=col
-00003b50: 756d 6e73 290d 0a20 2020 2020 2020 2020  umns)..         
-00003b60: 2020 2073 6f75 7263 655f 636f 6c20 3d20     source_col = 
-00003b70: 6622 736f 7572 6365 5f7b 736f 7572 6365  f"source_{source
-00003b80: 5f69 6473 7d22 0d0a 2020 2020 2020 2020  _ids}"..        
-00003b90: 2020 2020 6465 7374 5f63 6f6c 203d 2066      dest_col = f
-00003ba0: 2264 6573 745f 7b64 6573 745f 6964 737d  "dest_{dest_ids}
-00003bb0: 220d 0a0d 0a20 2020 2020 2020 206c 6f67  "....        log
-00003bc0: 6769 6e67 2e69 6e66 6f28 224d 6170 7069  ging.info("Mappi
-00003bd0: 6e67 2067 656e 6520 4944 7322 290d 0a0d  ng gene IDs")...
-00003be0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00003bf0: 6361 7365 5f73 656e 7369 7469 7665 3a0d  case_sensitive:.
-00003c00: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00003c10: 756c 745b 736f 7572 6365 5f63 6f6c 5d20  ult[source_col] 
-00003c20: 3d20 7265 7375 6c74 5b73 6f75 7263 655f  = result[source_
-00003c30: 636f 6c5d 2e73 7472 2e63 6173 6566 6f6c  col].str.casefol
-00003c40: 6428 290d 0a0d 0a20 2020 2020 2020 2069  d()....        i
-00003c50: 645f 6d61 7070 696e 6720 3d20 7265 7375  d_mapping = resu
-00003c60: 6c74 2e67 726f 7570 6279 285b 736f 7572  lt.groupby([sour
-00003c70: 6365 5f63 6f6c 2c20 6465 7374 5f63 6f6c  ce_col, dest_col
-00003c80: 5d29 2e61 7070 6c79 286c 616d 6264 6120  ]).apply(lambda 
-00003c90: 7820 3a20 782e 636f 756e 7428 2929 2e69  x : x.count()).i
-00003ca0: 6c6f 635b 3a2c 305d 0d0a 2020 2020 2020  loc[:,0]..      
-00003cb0: 2020 6964 5f6d 6170 7069 6e67 203d 2070    id_mapping = p
-00003cc0: 642e 4461 7461 4672 616d 6528 6964 5f6d  d.DataFrame(id_m
-00003cd0: 6170 7069 6e67 2e72 656e 616d 6528 2270  apping.rename("p
-00003ce0: 6174 685f 636f 756e 7473 2229 290d 0a20  ath_counts")).. 
-00003cf0: 2020 2020 2020 2061 7373 6572 7420 6964         assert id
-00003d00: 5f6d 6170 7069 6e67 2e69 6e64 6578 2e69  _mapping.index.i
-00003d10: 735f 756e 6971 7565 0d0a 2020 2020 2020  s_unique..      
-00003d20: 2020 736f 7572 6365 5f69 645f 636f 756e    source_id_coun
-00003d30: 7473 203d 2069 645f 6d61 7070 696e 672e  ts = id_mapping.
-00003d40: 696e 6465 782e 6765 745f 6c65 7665 6c5f  index.get_level_
-00003d50: 7661 6c75 6573 2830 292e 7661 6c75 655f  values(0).value_
-00003d60: 636f 756e 7473 2829 0d0a 2020 2020 2020  counts()..      
-00003d70: 2020 6465 7374 5f69 645f 636f 756e 7473    dest_id_counts
-00003d80: 203d 2069 645f 6d61 7070 696e 672e 696e   = id_mapping.in
-00003d90: 6465 782e 6765 745f 6c65 7665 6c5f 7661  dex.get_level_va
-00003da0: 6c75 6573 2831 292e 7661 6c75 655f 636f  lues(1).value_co
-00003db0: 756e 7473 2829 0d0a 2020 2020 2020 2020  unts()..        
-00003dc0: 6964 5f6d 6170 7069 6e67 5b22 736f 7572  id_mapping["sour
-00003dd0: 6365 5f69 645f 636f 756e 7422 5d20 3d20  ce_id_count"] = 
-00003de0: 6964 5f6d 6170 7069 6e67 2e69 6e64 6578  id_mapping.index
-00003df0: 2e67 6574 5f6c 6576 656c 5f76 616c 7565  .get_level_value
-00003e00: 7328 3029 2e6d 6170 2873 6f75 7263 655f  s(0).map(source_
-00003e10: 6964 5f63 6f75 6e74 7329 0d0a 2020 2020  id_counts)..    
-00003e20: 2020 2020 6964 5f6d 6170 7069 6e67 5b22      id_mapping["
-00003e30: 6465 7374 5f69 645f 636f 756e 7422 5d20  dest_id_count"] 
-00003e40: 3d20 6964 5f6d 6170 7069 6e67 2e69 6e64  = id_mapping.ind
-00003e50: 6578 2e67 6574 5f6c 6576 656c 5f76 616c  ex.get_level_val
-00003e60: 7565 7328 3129 2e6d 6170 2864 6573 745f  ues(1).map(dest_
-00003e70: 6964 5f63 6f75 6e74 7329 0d0a 0d0a 2020  id_counts)....  
-00003e80: 2020 2020 2020 2320 6372 6561 7465 206f        # create o
-00003e90: 7264 6572 6564 206c 6973 7473 206f 6620  rdered lists of 
-00003ea0: 7468 6520 4944 7320 666f 7220 696e 6465  the IDs for inde
-00003eb0: 7869 6e67 2074 6865 2061 6e6e 6461 7461  xing the anndata
-00003ec0: 206f 626a 6563 740d 0a20 2020 2020 2020   object..       
-00003ed0: 2073 6f75 7263 655f 6964 5f6c 6973 7420   source_id_list 
-00003ee0: 3d20 5b5d 0d0a 2020 2020 2020 2020 6465  = []..        de
-00003ef0: 7374 5f69 645f 6c69 7374 3d20 5b5d 0d0a  st_id_list= []..
-00003f00: 2020 2020 2020 2020 6d61 7070 696e 675f          mapping_
-00003f10: 7265 6c61 7469 6f6e 7368 6970 203d 205b  relationship = [
-00003f20: 5d0d 0a0d 0a20 2020 2020 2020 2023 204f  ]....        # O
-00003f30: 6e65 2d74 6f2d 6e6f 6e65 3a20 4944 7320  ne-to-none: IDs 
-00003f40: 7468 6174 2061 7265 206e 6f74 2066 6f75  that are not fou
-00003f50: 6e64 2069 6e20 7468 6520 4944 206d 6170  nd in the ID map
-00003f60: 7069 6e67 2074 6162 6c65 0d0a 2020 2020  ping table..    
-00003f70: 2020 2020 6966 2063 6173 655f 7365 6e73      if case_sens
-00003f80: 6974 6976 653a 0d0a 2020 2020 2020 2020  itive:..        
-00003f90: 2020 2020 6964 5f69 6478 203d 207e 7365      id_idx = ~se
-00003fa0: 6c66 2e61 6461 7461 2e76 6172 5f6e 616d  lf.adata.var_nam
-00003fb0: 6573 2e69 7369 6e28 6964 5f6d 6170 7069  es.isin(id_mappi
-00003fc0: 6e67 2e69 6e64 6578 2e67 6574 5f6c 6576  ng.index.get_lev
-00003fd0: 656c 5f76 616c 7565 7328 3029 290d 0a20  el_values(0)).. 
-00003fe0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00003ff0: 2020 2020 2020 2020 2020 6964 5f69 6478            id_idx
-00004000: 203d 207e 7365 6c66 2e61 6461 7461 2e76   = ~self.adata.v
-00004010: 6172 5f6e 616d 6573 2e73 7472 2e63 6173  ar_names.str.cas
-00004020: 6566 6f6c 6428 292e 6973 696e 2869 645f  efold().isin(id_
-00004030: 6d61 7070 696e 672e 696e 6465 782e 6765  mapping.index.ge
-00004040: 745f 6c65 7665 6c5f 7661 6c75 6573 2830  t_level_values(0
-00004050: 2929 0d0a 2020 2020 2020 2020 7372 635f  ))..        src_
-00004060: 6964 7320 3d20 7365 6c66 2e61 6461 7461  ids = self.adata
-00004070: 2e76 6172 5f6e 616d 6573 5b69 645f 6964  .var_names[id_id
-00004080: 785d 0d0a 2020 2020 2020 2020 6465 7374  x]..        dest
-00004090: 5f69 6473 203d 2075 6e6d 6170 7065 645f  _ids = unmapped_
-000040a0: 7072 6566 6978 202b 2073 7263 5f69 6473  prefix + src_ids
-000040b0: 0d0a 2020 2020 2020 2020 736f 7572 6365  ..        source
-000040c0: 5f69 645f 6c69 7374 2e65 7874 656e 6428  _id_list.extend(
-000040d0: 7372 635f 6964 7329 0d0a 2020 2020 2020  src_ids)..      
-000040e0: 2020 6465 7374 5f69 645f 6c69 7374 2e65    dest_id_list.e
-000040f0: 7874 656e 6428 756e 6d61 7070 6564 5f70  xtend(unmapped_p
-00004100: 7265 6669 7820 2b20 7372 635f 6964 7329  refix + src_ids)
-00004110: 0d0a 2020 2020 2020 2020 6d61 7070 696e  ..        mappin
-00004120: 675f 7265 6c61 7469 6f6e 7368 6970 2e65  g_relationship.e
-00004130: 7874 656e 6428 6c65 6e28 7372 635f 6964  xtend(len(src_id
-00004140: 7329 202a 205b 226f 6e65 2d74 6f2d 6e6f  s) * ["one-to-no
-00004150: 6e65 225d 290d 0a0d 0a20 2020 2020 2020  ne"])....       
-00004160: 2023 204f 6e65 2d74 6f2d 6f6e 650d 0a20   # One-to-one.. 
-00004170: 2020 2020 2020 206f 326f 203d 2069 645f         o2o = id_
-00004180: 6d61 7070 696e 675b 2869 645f 6d61 7070  mapping[(id_mapp
-00004190: 696e 675b 2273 6f75 7263 655f 6964 5f63  ing["source_id_c
-000041a0: 6f75 6e74 225d 203d 3d20 3129 2026 2028  ount"] == 1) & (
-000041b0: 6964 5f6d 6170 7069 6e67 5b22 6465 7374  id_mapping["dest
-000041c0: 5f69 645f 636f 756e 7422 5d20 3d3d 2031  _id_count"] == 1
-000041d0: 295d 0d0a 2020 2020 2020 2020 6966 2063  )]..        if c
-000041e0: 6173 655f 7365 6e73 6974 6976 653a 0d0a  ase_sensitive:..
-000041f0: 2020 2020 2020 2020 2020 2020 6964 5f69              id_i
-00004200: 6478 203d 2073 656c 662e 6164 6174 612e  dx = self.adata.
-00004210: 7661 725f 6e61 6d65 732e 6973 696e 286f  var_names.isin(o
-00004220: 326f 2e69 6e64 6578 2e67 6574 5f6c 6576  2o.index.get_lev
-00004230: 656c 5f76 616c 7565 7328 3029 290d 0a20  el_values(0)).. 
-00004240: 2020 2020 2020 2020 2020 2069 6473 5f74             ids_t
-00004250: 6f5f 6d61 7020 3d20 7365 6c66 2e61 6461  o_map = self.ada
-00004260: 7461 2e76 6172 5f6e 616d 6573 5b69 645f  ta.var_names[id_
-00004270: 6964 785d 0d0a 2020 2020 2020 2020 656c  idx]..        el
-00004280: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00004290: 2069 645f 6964 7820 3d20 7365 6c66 2e61   id_idx = self.a
-000042a0: 6461 7461 2e76 6172 5f6e 616d 6573 2e73  data.var_names.s
-000042b0: 7472 2e63 6173 6566 6f6c 6428 292e 6973  tr.casefold().is
-000042c0: 696e 286f 326f 2e69 6e64 6578 2e67 6574  in(o2o.index.get
-000042d0: 5f6c 6576 656c 5f76 616c 7565 7328 3029  _level_values(0)
-000042e0: 2e73 7472 2e63 6173 6566 6f6c 6428 2929  .str.casefold())
-000042f0: 0d0a 2020 2020 2020 2020 2020 2020 6964  ..            id
-00004300: 735f 746f 5f6d 6170 203d 2073 656c 662e  s_to_map = self.
-00004310: 6164 6174 612e 7661 725f 6e61 6d65 735b  adata.var_names[
-00004320: 6964 5f69 6478 5d2e 7374 722e 6361 7365  id_idx].str.case
-00004330: 666f 6c64 2829 0d0a 2020 2020 2020 2020  fold()..        
-00004340: 7372 635f 6964 7320 3d20 7365 6c66 2e61  src_ids = self.a
-00004350: 6461 7461 2e76 6172 5f6e 616d 6573 5b69  data.var_names[i
-00004360: 645f 6964 785d 0d0a 2020 2020 2020 2020  d_idx]..        
-00004370: 6966 206f 6e65 5f74 6f5f 6f6e 653a 0d0a  if one_to_one:..
-00004380: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00004390: 5f69 6473 203d 206f 326f 2e69 6e64 6578  _ids = o2o.index
-000043a0: 2e74 6f5f 6672 616d 6528 292e 7265 7365  .to_frame().rese
-000043b0: 745f 696e 6465 7828 6c65 7665 6c3d 312c  t_index(level=1,
-000043c0: 2064 726f 703d 5472 7565 295b 6465 7374   drop=True)[dest
-000043d0: 5f63 6f6c 5d2e 6c6f 635b 6964 735f 746f  _col].loc[ids_to
-000043e0: 5f6d 6170 5d0d 0a20 2020 2020 2020 2065  _map]..        e
-000043f0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00004400: 2020 6465 7374 5f69 6473 203d 2075 6e6d    dest_ids = unm
-00004410: 6170 7065 645f 7072 6566 6978 202b 2073  apped_prefix + s
-00004420: 7263 5f69 6473 0d0a 2020 2020 2020 2020  rc_ids..        
-00004430: 736f 7572 6365 5f69 645f 6c69 7374 2e65  source_id_list.e
-00004440: 7874 656e 6428 7372 635f 6964 7329 0d0a  xtend(src_ids)..
-00004450: 2020 2020 2020 2020 6465 7374 5f69 645f          dest_id_
-00004460: 6c69 7374 2e65 7874 656e 6428 6465 7374  list.extend(dest
-00004470: 5f69 6473 290d 0a20 2020 2020 2020 206d  _ids)..        m
-00004480: 6170 7069 6e67 5f72 656c 6174 696f 6e73  apping_relations
-00004490: 6869 702e 6578 7465 6e64 286c 656e 2873  hip.extend(len(s
-000044a0: 7263 5f69 6473 2920 2a20 5b22 6f6e 652d  rc_ids) * ["one-
-000044b0: 746f 2d6f 6e65 225d 290d 0a0d 0a20 2020  to-one"])....   
-000044c0: 2020 2020 2023 204f 6e65 2d74 6f2d 6d61       # One-to-ma
-000044d0: 6e79 0d0a 2020 2020 2020 2020 6f32 6d20  ny..        o2m 
-000044e0: 3d20 6964 5f6d 6170 7069 6e67 5b28 6964  = id_mapping[(id
-000044f0: 5f6d 6170 7069 6e67 5b22 736f 7572 6365  _mapping["source
-00004500: 5f69 645f 636f 756e 7422 5d20 3d3d 2031  _id_count"] == 1
-00004510: 2920 2620 2869 645f 6d61 7070 696e 675b  ) & (id_mapping[
-00004520: 2264 6573 745f 6964 5f63 6f75 6e74 225d  "dest_id_count"]
-00004530: 203e 2031 295d 0d0a 2020 2020 2020 2020   > 1)]..        
-00004540: 6966 2063 6173 655f 7365 6e73 6974 6976  if case_sensitiv
-00004550: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00004560: 6964 5f69 6478 203d 2073 656c 662e 6164  id_idx = self.ad
-00004570: 6174 612e 7661 725f 6e61 6d65 732e 6973  ata.var_names.is
-00004580: 696e 286f 326d 2e69 6e64 6578 2e67 6574  in(o2m.index.get
-00004590: 5f6c 6576 656c 5f76 616c 7565 7328 3029  _level_values(0)
-000045a0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-000045b0: 6473 5f74 6f5f 6d61 7020 3d20 7365 6c66  ds_to_map = self
-000045c0: 2e61 6461 7461 2e76 6172 5f6e 616d 6573  .adata.var_names
-000045d0: 5b69 645f 6964 785d 0d0a 2020 2020 2020  [id_idx]..      
-000045e0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000045f0: 2020 2020 2069 645f 6964 7820 3d20 7365       id_idx = se
-00004600: 6c66 2e61 6461 7461 2e76 6172 5f6e 616d  lf.adata.var_nam
-00004610: 6573 2e73 7472 2e63 6173 6566 6f6c 6428  es.str.casefold(
-00004620: 292e 6973 696e 286f 326d 2e69 6e64 6578  ).isin(o2m.index
-00004630: 2e67 6574 5f6c 6576 656c 5f76 616c 7565  .get_level_value
-00004640: 7328 3029 2e73 7472 2e63 6173 6566 6f6c  s(0).str.casefol
-00004650: 6428 2929 0d0a 2020 2020 2020 2020 2020  d())..          
-00004660: 2020 6964 735f 746f 5f6d 6170 203d 2073    ids_to_map = s
-00004670: 656c 662e 6164 6174 612e 7661 725f 6e61  elf.adata.var_na
-00004680: 6d65 735b 6964 5f69 6478 5d2e 7374 722e  mes[id_idx].str.
-00004690: 6361 7365 666f 6c64 2829 0d0a 2020 2020  casefold()..    
-000046a0: 2020 2020 7372 635f 6964 7320 3d20 7365      src_ids = se
-000046b0: 6c66 2e61 6461 7461 2e76 6172 5f6e 616d  lf.adata.var_nam
-000046c0: 6573 5b69 645f 6964 785d 0d0a 2020 2020  es[id_idx]..    
-000046d0: 2020 2020 6966 206f 6e65 5f74 6f5f 6d61      if one_to_ma
-000046e0: 6e79 203d 3d20 2264 7570 6c69 6361 7465  ny == "duplicate
-000046f0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-00004700: 2320 6475 706c 6963 6174 6573 2074 6865  # duplicates the
-00004710: 2076 616c 7565 7320 6f66 2074 6865 2065   values of the e
-00004720: 7869 7374 696e 6720 4944 2066 6f72 2074  xisting ID for t
-00004730: 6865 206e 6577 206d 756c 7469 706c 6520  he new multiple 
-00004740: 4944 730d 0a20 2020 2020 2020 2020 2020  IDs..           
-00004750: 2066 6f72 2073 7263 5f69 642c 2069 645f   for src_id, id_
-00004760: 746f 5f6d 6170 2069 6e20 7a69 7028 7372  to_map in zip(sr
-00004770: 635f 6964 732c 2069 6473 5f74 6f5f 6d61  c_ids, ids_to_ma
-00004780: 7029 3a0d 0a20 2020 2020 2020 2020 2020  p):..           
-00004790: 2020 2020 2064 6573 7420 3d20 6f32 6d2e       dest = o2m.
-000047a0: 6c6f 635b 6964 5f74 6f5f 6d61 705d 2e69  loc[id_to_map].i
-000047b0: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
-000047c0: 2020 2020 2020 736f 7572 6365 5f69 645f        source_id_
-000047d0: 6c69 7374 2e65 7874 656e 6428 6c65 6e28  list.extend(len(
-000047e0: 6465 7374 2920 2a20 5b73 7263 5f69 645d  dest) * [src_id]
-000047f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004800: 2020 2064 6573 745f 6964 5f6c 6973 742e     dest_id_list.
-00004810: 6578 7465 6e64 2864 6573 7429 0d0a 2020  extend(dest)..  
-00004820: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00004830: 7070 696e 675f 7265 6c61 7469 6f6e 7368  pping_relationsh
-00004840: 6970 2e65 7874 656e 6428 6c65 6e28 6465  ip.extend(len(de
-00004850: 7374 2920 2a20 5b22 6f6e 652d 746f 2d6d  st) * ["one-to-m
-00004860: 616e 7922 5d29 0d0a 2020 2020 2020 2020  any"])..        
-00004870: 656c 6966 206f 6e65 5f74 6f5f 6d61 6e79  elif one_to_many
-00004880: 2069 7320 4661 6c73 653a 0d0a 2020 2020   is False:..    
-00004890: 2020 2020 2020 2020 6465 7374 5f69 6473          dest_ids
-000048a0: 203d 2075 6e6d 6170 7065 645f 7072 6566   = unmapped_pref
-000048b0: 6978 202b 2073 7263 5f69 6473 0d0a 2020  ix + src_ids..  
-000048c0: 2020 2020 2020 2020 2020 736f 7572 6365            source
-000048d0: 5f69 645f 6c69 7374 2e65 7874 656e 6428  _id_list.extend(
-000048e0: 7372 635f 6964 7329 0d0a 2020 2020 2020  src_ids)..      
-000048f0: 2020 2020 2020 6465 7374 5f69 645f 6c69        dest_id_li
-00004900: 7374 2e65 7874 656e 6428 6465 7374 5f69  st.extend(dest_i
-00004910: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
-00004920: 206d 6170 7069 6e67 5f72 656c 6174 696f   mapping_relatio
-00004930: 6e73 6869 702e 6578 7465 6e64 286c 656e  nship.extend(len
-00004940: 2873 7263 5f69 6473 2920 2a20 5b22 6f6e  (src_ids) * ["on
-00004950: 652d 746f 2d6d 616e 7922 5d29 0d0a 2020  e-to-many"])..  
-00004960: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00004970: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
-00004980: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-00004990: 6f72 2866 2260 7b6f 6e65 5f74 6f5f 6d61  or(f"`{one_to_ma
-000049a0: 6e79 7d60 2069 7320 6e6f 7420 6375 7272  ny}` is not curr
-000049b0: 656e 746c 7920 696d 706c 656d 656e 7465  ently implemente
-000049c0: 6420 666f 7220 6f6e 652d 746f 2d6d 616e  d for one-to-man
-000049d0: 7920 6765 6e65 206d 6170 7069 6e67 732e  y gene mappings.
-000049e0: 2229 0d0a 0d0a 2020 2020 2020 2020 2320  ")....        # 
-000049f0: 4d61 6e79 2d74 6f2d 6f6e 6520 6f6e 6c79  Many-to-one only
-00004a00: 0d0a 2020 2020 2020 2020 6d32 6f20 3d20  ..        m2o = 
-00004a10: 6964 5f6d 6170 7069 6e67 5b28 6964 5f6d  id_mapping[(id_m
-00004a20: 6170 7069 6e67 5b22 736f 7572 6365 5f69  apping["source_i
-00004a30: 645f 636f 756e 7422 5d20 3e20 3129 2026  d_count"] > 1) &
-00004a40: 2028 6964 5f6d 6170 7069 6e67 5b22 6465   (id_mapping["de
-00004a50: 7374 5f69 645f 636f 756e 7422 5d20 3d3d  st_id_count"] ==
-00004a60: 2031 295d 0d0a 2020 2020 2020 2020 6d32   1)]..        m2
-00004a70: 6d20 3d20 6964 5f6d 6170 7069 6e67 5b28  m = id_mapping[(
-00004a80: 6964 5f6d 6170 7069 6e67 5b22 736f 7572  id_mapping["sour
-00004a90: 6365 5f69 645f 636f 756e 7422 5d20 3e20  ce_id_count"] > 
-00004aa0: 3129 2026 2028 6964 5f6d 6170 7069 6e67  1) & (id_mapping
-00004ab0: 5b22 6465 7374 5f69 645f 636f 756e 7422  ["dest_id_count"
-00004ac0: 5d20 3e20 3129 5d0d 0a0d 0a20 2020 2020  ] > 1)]....     
-00004ad0: 2020 2069 6620 6361 7365 5f73 656e 7369     if case_sensi
-00004ae0: 7469 7665 3a0d 0a20 2020 2020 2020 2020  tive:..         
-00004af0: 2020 2069 645f 6964 7820 3d20 7365 6c66     id_idx = self
-00004b00: 2e61 6461 7461 2e76 6172 5f6e 616d 6573  .adata.var_names
-00004b10: 2e69 7369 6e28 6d32 6f2e 696e 6465 782e  .isin(m2o.index.
-00004b20: 6765 745f 6c65 7665 6c5f 7661 6c75 6573  get_level_values
-00004b30: 2830 2929 2026 207e 7365 6c66 2e61 6461  (0)) & ~self.ada
-00004b40: 7461 2e76 6172 5f6e 616d 6573 2e69 7369  ta.var_names.isi
-00004b50: 6e28 6d32 6d2e 696e 6465 782e 6765 745f  n(m2m.index.get_
-00004b60: 6c65 7665 6c5f 7661 6c75 6573 2830 2929  level_values(0))
-00004b70: 0d0a 2020 2020 2020 2020 2020 2020 6964  ..            id
-00004b80: 735f 746f 5f6d 6170 203d 2073 656c 662e  s_to_map = self.
-00004b90: 6164 6174 612e 7661 725f 6e61 6d65 735b  adata.var_names[
-00004ba0: 6964 5f69 6478 5d0d 0a20 2020 2020 2020  id_idx]..       
-00004bb0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00004bc0: 2020 2020 6964 5f69 6478 203d 2073 656c      id_idx = sel
-00004bd0: 662e 6164 6174 612e 7661 725f 6e61 6d65  f.adata.var_name
-00004be0: 732e 7374 722e 6361 7365 666f 6c64 2829  s.str.casefold()
-00004bf0: 2e69 7369 6e28 6d32 6f2e 696e 6465 782e  .isin(m2o.index.
-00004c00: 6765 745f 6c65 7665 6c5f 7661 6c75 6573  get_level_values
-00004c10: 2830 292e 7374 722e 6361 7365 666f 6c64  (0).str.casefold
-00004c20: 2829 2920 2620 7e73 656c 662e 6164 6174  ()) & ~self.adat
-00004c30: 612e 7661 725f 6e61 6d65 732e 7374 722e  a.var_names.str.
-00004c40: 6361 7365 666f 6c64 2829 2e69 7369 6e28  casefold().isin(
-00004c50: 6d32 6d2e 696e 6465 782e 6765 745f 6c65  m2m.index.get_le
-00004c60: 7665 6c5f 7661 6c75 6573 2830 292e 7374  vel_values(0).st
-00004c70: 722e 6361 7365 666f 6c64 2829 290d 0a20  r.casefold()).. 
-00004c80: 2020 2020 2020 2020 2020 2069 6473 5f74             ids_t
-00004c90: 6f5f 6d61 7020 3d20 7365 6c66 2e61 6461  o_map = self.ada
-00004ca0: 7461 2e76 6172 5f6e 616d 6573 5b69 645f  ta.var_names[id_
-00004cb0: 6964 785d 2e73 7472 2e63 6173 6566 6f6c  idx].str.casefol
-00004cc0: 6428 290d 0a20 2020 2020 2020 2073 7263  d()..        src
-00004cd0: 5f69 6473 203d 2073 656c 662e 6164 6174  _ids = self.adat
-00004ce0: 612e 7661 725f 6e61 6d65 735b 6964 5f69  a.var_names[id_i
-00004cf0: 6478 5d0d 0a20 2020 2020 2020 2069 6620  dx]..        if 
-00004d00: 6d61 6e79 5f74 6f5f 6f6e 6520 6973 2046  many_to_one is F
-00004d10: 616c 7365 3a0d 0a20 2020 2020 2020 2020  alse:..         
-00004d20: 2020 2064 6573 745f 6964 7320 3d20 756e     dest_ids = un
-00004d30: 6d61 7070 6564 5f70 7265 6669 7820 2b20  mapped_prefix + 
-00004d40: 7372 635f 6964 730d 0a20 2020 2020 2020  src_ids..       
-00004d50: 2020 2020 2073 6f75 7263 655f 6964 5f6c       source_id_l
-00004d60: 6973 742e 6578 7465 6e64 2873 7263 5f69  ist.extend(src_i
-00004d70: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
-00004d80: 2064 6573 745f 6964 5f6c 6973 742e 6578   dest_id_list.ex
-00004d90: 7465 6e64 2864 6573 745f 6964 7329 0d0a  tend(dest_ids)..
-00004da0: 2020 2020 2020 2020 2020 2020 6d61 7070              mapp
-00004db0: 696e 675f 7265 6c61 7469 6f6e 7368 6970  ing_relationship
-00004dc0: 2e65 7874 656e 6428 6c65 6e28 7372 635f  .extend(len(src_
-00004dd0: 6964 7329 202a 205b 226d 616e 792d 746f  ids) * ["many-to
-00004de0: 2d6f 6e65 225d 290d 0a20 2020 2020 2020  -one"])..       
-00004df0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00004e00: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-00004e10: 6c65 6d65 6e74 6564 4572 726f 7228 6622  lementedError(f"
-00004e20: 607b 6d61 6e79 5f74 6f5f 6f6e 657d 6020  `{many_to_one}` 
-00004e30: 6973 206e 6f74 2063 7572 7265 6e74 6c79  is not currently
-00004e40: 2069 6d70 6c65 6d65 6e74 6564 2066 6f72   implemented for
-00004e50: 206d 616e 792d 746f 2d6f 6e65 2067 656e   many-to-one gen
-00004e60: 6520 6d61 7070 696e 6773 2e22 290d 0a0d  e mappings.")...
-00004e70: 0a20 2020 2020 2020 2023 204d 616e 792d  .        # Many-
-00004e80: 746f 2d6d 616e 7920 6f6e 6c79 0d0a 2020  to-many only..  
-00004e90: 2020 2020 2020 6966 2063 6173 655f 7365        if case_se
-00004ea0: 6e73 6974 6976 653a 0d0a 2020 2020 2020  nsitive:..      
-00004eb0: 2020 2020 2020 6964 5f69 6478 203d 2073        id_idx = s
-00004ec0: 656c 662e 6164 6174 612e 7661 725f 6e61  elf.adata.var_na
-00004ed0: 6d65 732e 6973 696e 286d 326d 2e69 6e64  mes.isin(m2m.ind
-00004ee0: 6578 2e67 6574 5f6c 6576 656c 5f76 616c  ex.get_level_val
-00004ef0: 7565 7328 3029 2920 2620 7e73 656c 662e  ues(0)) & ~self.
-00004f00: 6164 6174 612e 7661 725f 6e61 6d65 732e  adata.var_names.
-00004f10: 6973 696e 286d 326f 2e69 6e64 6578 2e67  isin(m2o.index.g
-00004f20: 6574 5f6c 6576 656c 5f76 616c 7565 7328  et_level_values(
-00004f30: 3029 290d 0a20 2020 2020 2020 2020 2020  0))..           
-00004f40: 2069 6473 5f74 6f5f 6d61 7020 3d20 7365   ids_to_map = se
-00004f50: 6c66 2e61 6461 7461 2e76 6172 5f6e 616d  lf.adata.var_nam
-00004f60: 6573 5b69 645f 6964 785d 0d0a 2020 2020  es[id_idx]..    
-00004f70: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00004f80: 2020 2020 2020 2069 645f 6964 7820 3d20         id_idx = 
-00004f90: 7365 6c66 2e61 6461 7461 2e76 6172 5f6e  self.adata.var_n
-00004fa0: 616d 6573 2e73 7472 2e63 6173 6566 6f6c  ames.str.casefol
-00004fb0: 6428 292e 6973 696e 286d 326d 2e69 6e64  d().isin(m2m.ind
-00004fc0: 6578 2e67 6574 5f6c 6576 656c 5f76 616c  ex.get_level_val
-00004fd0: 7565 7328 3029 2e73 7472 2e63 6173 6566  ues(0).str.casef
-00004fe0: 6f6c 6428 2929 2026 207e 7365 6c66 2e61  old()) & ~self.a
-00004ff0: 6461 7461 2e76 6172 5f6e 616d 6573 2e73  data.var_names.s
-00005000: 7472 2e63 6173 6566 6f6c 6428 292e 6973  tr.casefold().is
-00005010: 696e 286d 326f 2e69 6e64 6578 2e67 6574  in(m2o.index.get
-00005020: 5f6c 6576 656c 5f76 616c 7565 7328 3029  _level_values(0)
-00005030: 2e73 7472 2e63 6173 6566 6f6c 6428 2929  .str.casefold())
-00005040: 0d0a 2020 2020 2020 2020 2020 2020 6964  ..            id
-00005050: 735f 746f 5f6d 6170 203d 2073 656c 662e  s_to_map = self.
-00005060: 6164 6174 612e 7661 725f 6e61 6d65 735b  adata.var_names[
-00005070: 6964 5f69 6478 5d2e 7374 722e 6361 7365  id_idx].str.case
-00005080: 666f 6c64 2829 0d0a 2020 2020 2020 2020  fold()..        
-00005090: 7372 635f 6964 7320 3d20 7365 6c66 2e61  src_ids = self.a
-000050a0: 6461 7461 2e76 6172 5f6e 616d 6573 5b69  data.var_names[i
-000050b0: 645f 6964 785d 0d0a 2020 2020 2020 2020  d_idx]..        
-000050c0: 6966 206d 616e 795f 746f 5f6d 616e 7920  if many_to_many 
-000050d0: 6973 2046 616c 7365 3a0d 0a20 2020 2020  is False:..     
-000050e0: 2020 2020 2020 2064 6573 745f 6964 7320         dest_ids 
-000050f0: 3d20 756e 6d61 7070 6564 5f70 7265 6669  = unmapped_prefi
-00005100: 7820 2b20 7372 635f 6964 730d 0a20 2020  x + src_ids..   
-00005110: 2020 2020 2020 2020 2073 6f75 7263 655f           source_
-00005120: 6964 5f6c 6973 742e 6578 7465 6e64 2873  id_list.extend(s
-00005130: 7263 5f69 6473 290d 0a20 2020 2020 2020  rc_ids)..       
-00005140: 2020 2020 2064 6573 745f 6964 5f6c 6973       dest_id_lis
-00005150: 742e 6578 7465 6e64 2864 6573 745f 6964  t.extend(dest_id
-00005160: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00005170: 6d61 7070 696e 675f 7265 6c61 7469 6f6e  mapping_relation
-00005180: 7368 6970 2e65 7874 656e 6428 6c65 6e28  ship.extend(len(
-00005190: 7372 635f 6964 7329 202a 205b 226d 616e  src_ids) * ["man
-000051a0: 792d 746f 2d6d 616e 7922 5d29 0d0a 2020  y-to-many"])..  
-000051b0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-000051c0: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
-000051d0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-000051e0: 6f72 2866 2260 7b6d 616e 795f 746f 5f6d  or(f"`{many_to_m
-000051f0: 616e 797d 6020 6973 206e 6f74 2063 7572  any}` is not cur
-00005200: 7265 6e74 6c79 2069 6d70 6c65 6d65 6e74  rently implement
-00005210: 6564 2066 6f72 206d 616e 792d 746f 2d6d  ed for many-to-m
-00005220: 616e 7920 6765 6e65 206d 6170 7069 6e67  any gene mapping
-00005230: 732e 2229 0d0a 0d0a 2020 2020 2020 2020  s.")....        
-00005240: 2320 4944 7320 7769 7468 2062 6f74 6820  # IDs with both 
-00005250: 6d61 6e79 2d74 6f2d 6d61 6e79 2061 6e64  many-to-many and
-00005260: 206d 616e 792d 746f 2d6f 6e65 2072 656c   many-to-one rel
-00005270: 6174 696f 6e73 6869 700d 0a20 2020 2020  ationship..     
-00005280: 2020 2069 6620 6361 7365 5f73 656e 7369     if case_sensi
-00005290: 7469 7665 3a0d 0a20 2020 2020 2020 2020  tive:..         
-000052a0: 2020 2069 645f 6964 7820 3d20 7365 6c66     id_idx = self
-000052b0: 2e61 6461 7461 2e76 6172 5f6e 616d 6573  .adata.var_names
-000052c0: 2e69 7369 6e28 6d32 6d2e 696e 6465 782e  .isin(m2m.index.
-000052d0: 6765 745f 6c65 7665 6c5f 7661 6c75 6573  get_level_values
-000052e0: 2830 2929 2026 2073 656c 662e 6164 6174  (0)) & self.adat
-000052f0: 612e 7661 725f 6e61 6d65 732e 6973 696e  a.var_names.isin
-00005300: 286d 326f 2e69 6e64 6578 2e67 6574 5f6c  (m2o.index.get_l
-00005310: 6576 656c 5f76 616c 7565 7328 3029 290d  evel_values(0)).
-00005320: 0a20 2020 2020 2020 2020 2020 2069 6473  .            ids
-00005330: 5f74 6f5f 6d61 7020 3d20 7365 6c66 2e61  _to_map = self.a
-00005340: 6461 7461 2e76 6172 5f6e 616d 6573 5b69  data.var_names[i
-00005350: 645f 6964 785d 0d0a 2020 2020 2020 2020  d_idx]..        
-00005360: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00005370: 2020 2069 645f 6964 7820 3d20 7365 6c66     id_idx = self
-00005380: 2e61 6461 7461 2e76 6172 5f6e 616d 6573  .adata.var_names
-00005390: 2e73 7472 2e63 6173 6566 6f6c 6428 292e  .str.casefold().
-000053a0: 6973 696e 286d 326d 2e69 6e64 6578 2e67  isin(m2m.index.g
-000053b0: 6574 5f6c 6576 656c 5f76 616c 7565 7328  et_level_values(
-000053c0: 3029 2e73 7472 2e63 6173 6566 6f6c 6428  0).str.casefold(
-000053d0: 2929 2026 2073 656c 662e 6164 6174 612e  )) & self.adata.
-000053e0: 7661 725f 6e61 6d65 732e 7374 722e 6361  var_names.str.ca
-000053f0: 7365 666f 6c64 2829 2e69 7369 6e28 6d32  sefold().isin(m2
-00005400: 6f2e 696e 6465 782e 6765 745f 6c65 7665  o.index.get_leve
-00005410: 6c5f 7661 6c75 6573 2830 292e 7374 722e  l_values(0).str.
-00005420: 6361 7365 666f 6c64 2829 290d 0a20 2020  casefold())..   
-00005430: 2020 2020 2020 2020 2069 6473 5f74 6f5f           ids_to_
-00005440: 6d61 7020 3d20 7365 6c66 2e61 6461 7461  map = self.adata
-00005450: 2e76 6172 5f6e 616d 6573 5b69 645f 6964  .var_names[id_id
-00005460: 785d 2e73 7472 2e63 6173 6566 6f6c 6428  x].str.casefold(
-00005470: 290d 0a20 2020 2020 2020 2073 7263 5f69  )..        src_i
-00005480: 6473 203d 2073 656c 662e 6164 6174 612e  ds = self.adata.
-00005490: 7661 725f 6e61 6d65 735b 6964 5f69 6478  var_names[id_idx
-000054a0: 5d0d 0a20 2020 2020 2020 2064 6573 745f  ]..        dest_
-000054b0: 6964 7320 3d20 756e 6d61 7070 6564 5f70  ids = unmapped_p
-000054c0: 7265 6669 7820 2b20 7372 635f 6964 730d  refix + src_ids.
-000054d0: 0a20 2020 2020 2020 2073 6f75 7263 655f  .        source_
-000054e0: 6964 5f6c 6973 742e 6578 7465 6e64 2873  id_list.extend(s
-000054f0: 7263 5f69 6473 290d 0a20 2020 2020 2020  rc_ids)..       
-00005500: 2064 6573 745f 6964 5f6c 6973 742e 6578   dest_id_list.ex
-00005510: 7465 6e64 2864 6573 745f 6964 7329 0d0a  tend(dest_ids)..
-00005520: 2020 2020 2020 2020 6d61 7070 696e 675f          mapping_
-00005530: 7265 6c61 7469 6f6e 7368 6970 2e65 7874  relationship.ext
-00005540: 656e 6428 6c65 6e28 7372 635f 6964 7329  end(len(src_ids)
-00005550: 202a 205b 226d 616e 792d 746f 2d6d 616e   * ["many-to-man
-00005560: 793b 206d 616e 792d 746f 2d6f 6e65 225d  y; many-to-one"]
-00005570: 290d 0a20 2020 200d 0a20 2020 2020 2020  )..    ..       
-00005580: 2023 2063 7265 6174 6520 6e65 7720 616e   # create new an
-00005590: 6e64 6174 6120 6f62 6a65 6374 0d0a 2020  ndata object..  
-000055a0: 2020 2020 2020 6e65 775f 6164 6174 6120        new_adata 
-000055b0: 3d20 7365 6c66 2e61 6461 7461 5b3a 2c20  = self.adata[:, 
-000055c0: 736f 7572 6365 5f69 645f 6c69 7374 5d0d  source_id_list].
-000055d0: 0a20 2020 2020 2020 206e 6577 5f61 6461  .        new_ada
-000055e0: 7461 2e76 6172 5f6e 616d 6573 203d 2064  ta.var_names = d
-000055f0: 6573 745f 6964 5f6c 6973 740d 0a20 2020  est_id_list..   
-00005600: 2020 2020 206e 6577 5f61 6461 7461 2e76       new_adata.v
-00005610: 6172 5b22 736f 7572 6365 5f69 6422 5d20  ar["source_id"] 
-00005620: 3d20 736f 7572 6365 5f69 645f 6c69 7374  = source_id_list
-00005630: 0d0a 2020 2020 2020 2020 6e65 775f 6164  ..        new_ad
-00005640: 6174 612e 7661 725b 226d 6170 7069 6e67  ata.var["mapping
-00005650: 5f72 656c 6174 696f 6e73 6869 7022 5d20  _relationship"] 
-00005660: 3d20 6d61 7070 696e 675f 7265 6c61 7469  = mapping_relati
-00005670: 6f6e 7368 6970 0d0a 2020 2020 2020 2020  onship..        
-00005680: 6e65 775f 6164 6174 612e 7661 725b 226d  new_adata.var["m
-00005690: 6170 7069 6e67 5f72 656c 6174 696f 6e73  apping_relations
-000056a0: 6869 7022 5d20 3d20 6e65 775f 6164 6174  hip"] = new_adat
-000056b0: 612e 7661 725b 226d 6170 7069 6e67 5f72  a.var["mapping_r
-000056c0: 656c 6174 696f 6e73 6869 7022 5d2e 6173  elationship"].as
-000056d0: 7479 7065 2822 6361 7465 676f 7279 2229  type("category")
-000056e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-000056f0: 6461 7461 203d 206e 6577 5f61 6461 7461  data = new_adata
-00005700: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00005710: 7070 656e 645f 746f 5f68 6973 746f 7279  ppend_to_history
-00005720: 2866 224d 6170 7065 6420 6665 6174 7572  (f"Mapped featur
-00005730: 6520 4944 732e 2073 6f75 7263 6520 7370  e IDs. source sp
-00005740: 6563 6965 733d 7b73 6f75 7263 655f 7370  ecies={source_sp
-00005750: 6563 6965 737d 2c20 736f 7572 6365 5f69  ecies}, source_i
-00005760: 6473 3d7b 736f 7572 6365 5f69 6473 7d2c  ds={source_ids},
-00005770: 2064 6573 745f 7370 6563 6965 733d 7b64   dest_species={d
-00005780: 6573 745f 7370 6563 6965 737d 2c20 6465  est_species}, de
-00005790: 7374 5f69 6473 3d7b 6465 7374 5f69 6473  st_ids={dest_ids
-000057a0: 7d2c 2022 0d0a 2020 2020 2020 2020 2020  }, "..          
+00003a60: 2020 2020 2020 2066 227b 6465 7374 5f73         f"{dest_s
+00003a70: 7065 6369 6573 7d5f 686f 6d6f 6c6f 675f  pecies}_homolog_
+00003a80: 656e 7365 6d62 6c5f 6765 6e65 225d 7d29  ensembl_gene"]})
+00003a90: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+00003aa0: 6c75 6d6e 733d 5b27 736f 7572 6365 5f67  lumns=['source_g
+00003ab0: 656e 655f 6e61 6d65 272c 2773 6f75 7263  ene_name','sourc
+00003ac0: 655f 656e 7365 6d62 6c5f 6765 6e65 272c  e_ensembl_gene',
+00003ad0: 2027 6465 7374 5f67 656e 655f 6e61 6d65   'dest_gene_name
+00003ae0: 272c 2027 6465 7374 5f65 6e73 656d 626c  ', 'dest_ensembl
+00003af0: 5f67 656e 6527 5d0d 0a20 2020 2020 2020  _gene']..       
+00003b00: 2020 2020 2072 6573 756c 7420 3d20 7064       result = pd
+00003b10: 2e72 6561 645f 6373 7628 5374 7269 6e67  .read_csv(String
+00003b20: 494f 2872 6573 756c 742e 7465 7874 292c  IO(result.text),
+00003b30: 2073 6570 3d22 5c74 222c 2068 6561 6465   sep="\t", heade
+00003b40: 723d 4e6f 6e65 2c20 6e61 6d65 733d 636f  r=None, names=co
+00003b50: 6c75 6d6e 7329 0d0a 2020 2020 2020 2020  lumns)..        
+00003b60: 2020 2020 736f 7572 6365 5f63 6f6c 203d      source_col =
+00003b70: 2066 2273 6f75 7263 655f 7b73 6f75 7263   f"source_{sourc
+00003b80: 655f 6964 737d 220d 0a20 2020 2020 2020  e_ids}"..       
+00003b90: 2020 2020 2064 6573 745f 636f 6c20 3d20       dest_col = 
+00003ba0: 6622 6465 7374 5f7b 6465 7374 5f69 6473  f"dest_{dest_ids
+00003bb0: 7d22 0d0a 0d0a 2020 2020 2020 2020 6c6f  }"....        lo
+00003bc0: 6767 696e 672e 696e 666f 2822 4d61 7070  gging.info("Mapp
+00003bd0: 696e 6720 6765 6e65 2049 4473 2229 0d0a  ing gene IDs")..
+00003be0: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00003bf0: 2063 6173 655f 7365 6e73 6974 6976 653a   case_sensitive:
+00003c00: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00003c10: 7375 6c74 5b73 6f75 7263 655f 636f 6c5d  sult[source_col]
+00003c20: 203d 2072 6573 756c 745b 736f 7572 6365   = result[source
+00003c30: 5f63 6f6c 5d2e 7374 722e 6361 7365 666f  _col].str.casefo
+00003c40: 6c64 2829 0d0a 0d0a 2020 2020 2020 2020  ld()....        
+00003c50: 6964 5f6d 6170 7069 6e67 203d 2072 6573  id_mapping = res
+00003c60: 756c 742e 6772 6f75 7062 7928 5b73 6f75  ult.groupby([sou
+00003c70: 7263 655f 636f 6c2c 2064 6573 745f 636f  rce_col, dest_co
+00003c80: 6c5d 292e 6170 706c 7928 6c61 6d62 6461  l]).apply(lambda
+00003c90: 2078 203a 2078 2e63 6f75 6e74 2829 292e   x : x.count()).
+00003ca0: 696c 6f63 5b3a 2c30 5d0d 0a20 2020 2020  iloc[:,0]..     
+00003cb0: 2020 2069 645f 6d61 7070 696e 6720 3d20     id_mapping = 
+00003cc0: 7064 2e44 6174 6146 7261 6d65 2869 645f  pd.DataFrame(id_
+00003cd0: 6d61 7070 696e 672e 7265 6e61 6d65 2822  mapping.rename("
+00003ce0: 7061 7468 5f63 6f75 6e74 7322 2929 0d0a  path_counts"))..
+00003cf0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+00003d00: 645f 6d61 7070 696e 672e 696e 6465 782e  d_mapping.index.
+00003d10: 6973 5f75 6e69 7175 650d 0a20 2020 2020  is_unique..     
+00003d20: 2020 2073 6f75 7263 655f 6964 5f63 6f75     source_id_cou
+00003d30: 6e74 7320 3d20 6964 5f6d 6170 7069 6e67  nts = id_mapping
+00003d40: 2e69 6e64 6578 2e67 6574 5f6c 6576 656c  .index.get_level
+00003d50: 5f76 616c 7565 7328 3029 2e76 616c 7565  _values(0).value
+00003d60: 5f63 6f75 6e74 7328 290d 0a20 2020 2020  _counts()..     
+00003d70: 2020 2064 6573 745f 6964 5f63 6f75 6e74     dest_id_count
+00003d80: 7320 3d20 6964 5f6d 6170 7069 6e67 2e69  s = id_mapping.i
+00003d90: 6e64 6578 2e67 6574 5f6c 6576 656c 5f76  ndex.get_level_v
+00003da0: 616c 7565 7328 3129 2e76 616c 7565 5f63  alues(1).value_c
+00003db0: 6f75 6e74 7328 290d 0a20 2020 2020 2020  ounts()..       
+00003dc0: 2069 645f 6d61 7070 696e 675b 2273 6f75   id_mapping["sou
+00003dd0: 7263 655f 6964 5f63 6f75 6e74 225d 203d  rce_id_count"] =
+00003de0: 2069 645f 6d61 7070 696e 672e 696e 6465   id_mapping.inde
+00003df0: 782e 6765 745f 6c65 7665 6c5f 7661 6c75  x.get_level_valu
+00003e00: 6573 2830 292e 6d61 7028 736f 7572 6365  es(0).map(source
+00003e10: 5f69 645f 636f 756e 7473 290d 0a20 2020  _id_counts)..   
+00003e20: 2020 2020 2069 645f 6d61 7070 696e 675b       id_mapping[
+00003e30: 2264 6573 745f 6964 5f63 6f75 6e74 225d  "dest_id_count"]
+00003e40: 203d 2069 645f 6d61 7070 696e 672e 696e   = id_mapping.in
+00003e50: 6465 782e 6765 745f 6c65 7665 6c5f 7661  dex.get_level_va
+00003e60: 6c75 6573 2831 292e 6d61 7028 6465 7374  lues(1).map(dest
+00003e70: 5f69 645f 636f 756e 7473 290d 0a0d 0a20  _id_counts).... 
+00003e80: 2020 2020 2020 2023 2063 7265 6174 6520         # create 
+00003e90: 6f72 6465 7265 6420 6c69 7374 7320 6f66  ordered lists of
+00003ea0: 2074 6865 2049 4473 2066 6f72 2069 6e64   the IDs for ind
+00003eb0: 6578 696e 6720 7468 6520 616e 6e64 6174  exing the anndat
+00003ec0: 6120 6f62 6a65 6374 0d0a 2020 2020 2020  a object..      
+00003ed0: 2020 736f 7572 6365 5f69 645f 6c69 7374    source_id_list
+00003ee0: 203d 205b 5d0d 0a20 2020 2020 2020 2064   = []..        d
+00003ef0: 6573 745f 6964 5f6c 6973 743d 205b 5d0d  est_id_list= [].
+00003f00: 0a20 2020 2020 2020 206d 6170 7069 6e67  .        mapping
+00003f10: 5f72 656c 6174 696f 6e73 6869 7020 3d20  _relationship = 
+00003f20: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2320  []....        # 
+00003f30: 4f6e 652d 746f 2d6e 6f6e 653a 2049 4473  One-to-none: IDs
+00003f40: 2074 6861 7420 6172 6520 6e6f 7420 666f   that are not fo
+00003f50: 756e 6420 696e 2074 6865 2049 4420 6d61  und in the ID ma
+00003f60: 7070 696e 6720 7461 626c 650d 0a20 2020  pping table..   
+00003f70: 2020 2020 2069 6620 6361 7365 5f73 656e       if case_sen
+00003f80: 7369 7469 7665 3a0d 0a20 2020 2020 2020  sitive:..       
+00003f90: 2020 2020 2069 645f 6964 7820 3d20 7e73       id_idx = ~s
+00003fa0: 656c 662e 6164 6174 612e 7661 725f 6e61  elf.adata.var_na
+00003fb0: 6d65 732e 6973 696e 2869 645f 6d61 7070  mes.isin(id_mapp
+00003fc0: 696e 672e 696e 6465 782e 6765 745f 6c65  ing.index.get_le
+00003fd0: 7665 6c5f 7661 6c75 6573 2830 2929 0d0a  vel_values(0))..
+00003fe0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00003ff0: 2020 2020 2020 2020 2020 2069 645f 6964             id_id
+00004000: 7820 3d20 7e73 656c 662e 6164 6174 612e  x = ~self.adata.
+00004010: 7661 725f 6e61 6d65 732e 7374 722e 6361  var_names.str.ca
+00004020: 7365 666f 6c64 2829 2e69 7369 6e28 6964  sefold().isin(id
+00004030: 5f6d 6170 7069 6e67 2e69 6e64 6578 2e67  _mapping.index.g
+00004040: 6574 5f6c 6576 656c 5f76 616c 7565 7328  et_level_values(
+00004050: 3029 290d 0a20 2020 2020 2020 2073 7263  0))..        src
+00004060: 5f69 6473 203d 2073 656c 662e 6164 6174  _ids = self.adat
+00004070: 612e 7661 725f 6e61 6d65 735b 6964 5f69  a.var_names[id_i
+00004080: 6478 5d0d 0a20 2020 2020 2020 2064 6573  dx]..        des
+00004090: 745f 6964 7320 3d20 756e 6d61 7070 6564  t_ids = unmapped
+000040a0: 5f70 7265 6669 7820 2b20 7372 635f 6964  _prefix + src_id
+000040b0: 730d 0a20 2020 2020 2020 2073 6f75 7263  s..        sourc
+000040c0: 655f 6964 5f6c 6973 742e 6578 7465 6e64  e_id_list.extend
+000040d0: 2873 7263 5f69 6473 290d 0a20 2020 2020  (src_ids)..     
+000040e0: 2020 2064 6573 745f 6964 5f6c 6973 742e     dest_id_list.
+000040f0: 6578 7465 6e64 2875 6e6d 6170 7065 645f  extend(unmapped_
+00004100: 7072 6566 6978 202b 2073 7263 5f69 6473  prefix + src_ids
+00004110: 290d 0a20 2020 2020 2020 206d 6170 7069  )..        mappi
+00004120: 6e67 5f72 656c 6174 696f 6e73 6869 702e  ng_relationship.
+00004130: 6578 7465 6e64 286c 656e 2873 7263 5f69  extend(len(src_i
+00004140: 6473 2920 2a20 5b22 6f6e 652d 746f 2d6e  ds) * ["one-to-n
+00004150: 6f6e 6522 5d29 0d0a 0d0a 2020 2020 2020  one"])....      
+00004160: 2020 2320 4f6e 652d 746f 2d6f 6e65 0d0a    # One-to-one..
+00004170: 2020 2020 2020 2020 6f32 6f20 3d20 6964          o2o = id
+00004180: 5f6d 6170 7069 6e67 5b28 6964 5f6d 6170  _mapping[(id_map
+00004190: 7069 6e67 5b22 736f 7572 6365 5f69 645f  ping["source_id_
+000041a0: 636f 756e 7422 5d20 3d3d 2031 2920 2620  count"] == 1) & 
+000041b0: 2869 645f 6d61 7070 696e 675b 2264 6573  (id_mapping["des
+000041c0: 745f 6964 5f63 6f75 6e74 225d 203d 3d20  t_id_count"] == 
+000041d0: 3129 5d0d 0a20 2020 2020 2020 2069 6620  1)]..        if 
+000041e0: 6361 7365 5f73 656e 7369 7469 7665 3a0d  case_sensitive:.
+000041f0: 0a20 2020 2020 2020 2020 2020 2069 645f  .            id_
+00004200: 6964 7820 3d20 7365 6c66 2e61 6461 7461  idx = self.adata
+00004210: 2e76 6172 5f6e 616d 6573 2e69 7369 6e28  .var_names.isin(
+00004220: 6f32 6f2e 696e 6465 782e 6765 745f 6c65  o2o.index.get_le
+00004230: 7665 6c5f 7661 6c75 6573 2830 2929 0d0a  vel_values(0))..
+00004240: 2020 2020 2020 2020 2020 2020 6964 735f              ids_
+00004250: 746f 5f6d 6170 203d 2073 656c 662e 6164  to_map = self.ad
+00004260: 6174 612e 7661 725f 6e61 6d65 735b 6964  ata.var_names[id
+00004270: 5f69 6478 5d0d 0a20 2020 2020 2020 2065  _idx]..        e
+00004280: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00004290: 2020 6964 5f69 6478 203d 2073 656c 662e    id_idx = self.
+000042a0: 6164 6174 612e 7661 725f 6e61 6d65 732e  adata.var_names.
+000042b0: 7374 722e 6361 7365 666f 6c64 2829 2e69  str.casefold().i
+000042c0: 7369 6e28 6f32 6f2e 696e 6465 782e 6765  sin(o2o.index.ge
+000042d0: 745f 6c65 7665 6c5f 7661 6c75 6573 2830  t_level_values(0
+000042e0: 292e 7374 722e 6361 7365 666f 6c64 2829  ).str.casefold()
+000042f0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00004300: 6473 5f74 6f5f 6d61 7020 3d20 7365 6c66  ds_to_map = self
+00004310: 2e61 6461 7461 2e76 6172 5f6e 616d 6573  .adata.var_names
+00004320: 5b69 645f 6964 785d 2e73 7472 2e63 6173  [id_idx].str.cas
+00004330: 6566 6f6c 6428 290d 0a20 2020 2020 2020  efold()..       
+00004340: 2073 7263 5f69 6473 203d 2073 656c 662e   src_ids = self.
+00004350: 6164 6174 612e 7661 725f 6e61 6d65 735b  adata.var_names[
+00004360: 6964 5f69 6478 5d0d 0a20 2020 2020 2020  id_idx]..       
+00004370: 2069 6620 6f6e 655f 746f 5f6f 6e65 3a0d   if one_to_one:.
+00004380: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+00004390: 745f 6964 7320 3d20 6f32 6f2e 696e 6465  t_ids = o2o.inde
+000043a0: 782e 746f 5f66 7261 6d65 2829 2e72 6573  x.to_frame().res
+000043b0: 6574 5f69 6e64 6578 286c 6576 656c 3d31  et_index(level=1
+000043c0: 2c20 6472 6f70 3d54 7275 6529 5b64 6573  , drop=True)[des
+000043d0: 745f 636f 6c5d 2e6c 6f63 5b69 6473 5f74  t_col].loc[ids_t
+000043e0: 6f5f 6d61 705d 0d0a 2020 2020 2020 2020  o_map]..        
+000043f0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00004400: 2020 2064 6573 745f 6964 7320 3d20 756e     dest_ids = un
+00004410: 6d61 7070 6564 5f70 7265 6669 7820 2b20  mapped_prefix + 
+00004420: 7372 635f 6964 730d 0a20 2020 2020 2020  src_ids..       
+00004430: 2073 6f75 7263 655f 6964 5f6c 6973 742e   source_id_list.
+00004440: 6578 7465 6e64 2873 7263 5f69 6473 290d  extend(src_ids).
+00004450: 0a20 2020 2020 2020 2064 6573 745f 6964  .        dest_id
+00004460: 5f6c 6973 742e 6578 7465 6e64 2864 6573  _list.extend(des
+00004470: 745f 6964 7329 0d0a 2020 2020 2020 2020  t_ids)..        
+00004480: 6d61 7070 696e 675f 7265 6c61 7469 6f6e  mapping_relation
+00004490: 7368 6970 2e65 7874 656e 6428 6c65 6e28  ship.extend(len(
+000044a0: 7372 635f 6964 7329 202a 205b 226f 6e65  src_ids) * ["one
+000044b0: 2d74 6f2d 6f6e 6522 5d29 0d0a 0d0a 2020  -to-one"])....  
+000044c0: 2020 2020 2020 2320 4f6e 652d 746f 2d6d        # One-to-m
+000044d0: 616e 790d 0a20 2020 2020 2020 206f 326d  any..        o2m
+000044e0: 203d 2069 645f 6d61 7070 696e 675b 2869   = id_mapping[(i
+000044f0: 645f 6d61 7070 696e 675b 2273 6f75 7263  d_mapping["sourc
+00004500: 655f 6964 5f63 6f75 6e74 225d 203d 3d20  e_id_count"] == 
+00004510: 3129 2026 2028 6964 5f6d 6170 7069 6e67  1) & (id_mapping
+00004520: 5b22 6465 7374 5f69 645f 636f 756e 7422  ["dest_id_count"
+00004530: 5d20 3e20 3129 5d0d 0a20 2020 2020 2020  ] > 1)]..       
+00004540: 2069 6620 6361 7365 5f73 656e 7369 7469   if case_sensiti
+00004550: 7665 3a0d 0a20 2020 2020 2020 2020 2020  ve:..           
+00004560: 2069 645f 6964 7820 3d20 7365 6c66 2e61   id_idx = self.a
+00004570: 6461 7461 2e76 6172 5f6e 616d 6573 2e69  data.var_names.i
+00004580: 7369 6e28 6f32 6d2e 696e 6465 782e 6765  sin(o2m.index.ge
+00004590: 745f 6c65 7665 6c5f 7661 6c75 6573 2830  t_level_values(0
+000045a0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000045b0: 6964 735f 746f 5f6d 6170 203d 2073 656c  ids_to_map = sel
+000045c0: 662e 6164 6174 612e 7661 725f 6e61 6d65  f.adata.var_name
+000045d0: 735b 6964 5f69 6478 5d0d 0a20 2020 2020  s[id_idx]..     
+000045e0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+000045f0: 2020 2020 2020 6964 5f69 6478 203d 2073        id_idx = s
+00004600: 656c 662e 6164 6174 612e 7661 725f 6e61  elf.adata.var_na
+00004610: 6d65 732e 7374 722e 6361 7365 666f 6c64  mes.str.casefold
+00004620: 2829 2e69 7369 6e28 6f32 6d2e 696e 6465  ().isin(o2m.inde
+00004630: 782e 6765 745f 6c65 7665 6c5f 7661 6c75  x.get_level_valu
+00004640: 6573 2830 292e 7374 722e 6361 7365 666f  es(0).str.casefo
+00004650: 6c64 2829 290d 0a20 2020 2020 2020 2020  ld())..         
+00004660: 2020 2069 6473 5f74 6f5f 6d61 7020 3d20     ids_to_map = 
+00004670: 7365 6c66 2e61 6461 7461 2e76 6172 5f6e  self.adata.var_n
+00004680: 616d 6573 5b69 645f 6964 785d 2e73 7472  ames[id_idx].str
+00004690: 2e63 6173 6566 6f6c 6428 290d 0a20 2020  .casefold()..   
+000046a0: 2020 2020 2073 7263 5f69 6473 203d 2073       src_ids = s
+000046b0: 656c 662e 6164 6174 612e 7661 725f 6e61  elf.adata.var_na
+000046c0: 6d65 735b 6964 5f69 6478 5d0d 0a20 2020  mes[id_idx]..   
+000046d0: 2020 2020 2069 6620 6f6e 655f 746f 5f6d       if one_to_m
+000046e0: 616e 7920 3d3d 2022 6475 706c 6963 6174  any == "duplicat
+000046f0: 6522 3a0d 0a20 2020 2020 2020 2020 2020  e":..           
+00004700: 2023 2064 7570 6c69 6361 7465 7320 7468   # duplicates th
+00004710: 6520 7661 6c75 6573 206f 6620 7468 6520  e values of the 
+00004720: 6578 6973 7469 6e67 2049 4420 666f 7220  existing ID for 
+00004730: 7468 6520 6e65 7720 6d75 6c74 6970 6c65  the new multiple
+00004740: 2049 4473 0d0a 2020 2020 2020 2020 2020   IDs..          
+00004750: 2020 666f 7220 7372 635f 6964 2c20 6964    for src_id, id
+00004760: 5f74 6f5f 6d61 7020 696e 207a 6970 2873  _to_map in zip(s
+00004770: 7263 5f69 6473 2c20 6964 735f 746f 5f6d  rc_ids, ids_to_m
+00004780: 6170 293a 0d0a 2020 2020 2020 2020 2020  ap):..          
+00004790: 2020 2020 2020 6465 7374 203d 206f 326d        dest = o2m
+000047a0: 2e6c 6f63 5b69 645f 746f 5f6d 6170 5d2e  .loc[id_to_map].
+000047b0: 696e 6465 780d 0a20 2020 2020 2020 2020  index..         
+000047c0: 2020 2020 2020 2073 6f75 7263 655f 6964         source_id
+000047d0: 5f6c 6973 742e 6578 7465 6e64 286c 656e  _list.extend(len
+000047e0: 2864 6573 7429 202a 205b 7372 635f 6964  (dest) * [src_id
+000047f0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00004800: 2020 2020 6465 7374 5f69 645f 6c69 7374      dest_id_list
+00004810: 2e65 7874 656e 6428 6465 7374 290d 0a20  .extend(dest).. 
+00004820: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00004830: 6170 7069 6e67 5f72 656c 6174 696f 6e73  apping_relations
+00004840: 6869 702e 6578 7465 6e64 286c 656e 2864  hip.extend(len(d
+00004850: 6573 7429 202a 205b 226f 6e65 2d74 6f2d  est) * ["one-to-
+00004860: 6d61 6e79 225d 290d 0a20 2020 2020 2020  many"])..       
+00004870: 2065 6c69 6620 6f6e 655f 746f 5f6d 616e   elif one_to_man
+00004880: 7920 6973 2046 616c 7365 3a0d 0a20 2020  y is False:..   
+00004890: 2020 2020 2020 2020 2064 6573 745f 6964           dest_id
+000048a0: 7320 3d20 756e 6d61 7070 6564 5f70 7265  s = unmapped_pre
+000048b0: 6669 7820 2b20 7372 635f 6964 730d 0a20  fix + src_ids.. 
+000048c0: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+000048d0: 655f 6964 5f6c 6973 742e 6578 7465 6e64  e_id_list.extend
+000048e0: 2873 7263 5f69 6473 290d 0a20 2020 2020  (src_ids)..     
+000048f0: 2020 2020 2020 2064 6573 745f 6964 5f6c         dest_id_l
+00004900: 6973 742e 6578 7465 6e64 2864 6573 745f  ist.extend(dest_
+00004910: 6964 7329 0d0a 2020 2020 2020 2020 2020  ids)..          
+00004920: 2020 6d61 7070 696e 675f 7265 6c61 7469    mapping_relati
+00004930: 6f6e 7368 6970 2e65 7874 656e 6428 6c65  onship.extend(le
+00004940: 6e28 7372 635f 6964 7329 202a 205b 226f  n(src_ids) * ["o
+00004950: 6e65 2d74 6f2d 6d61 6e79 225d 290d 0a20  ne-to-many"]).. 
+00004960: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00004970: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00004980: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00004990: 726f 7228 6622 607b 6f6e 655f 746f 5f6d  ror(f"`{one_to_m
+000049a0: 616e 797d 6020 6973 206e 6f74 2063 7572  any}` is not cur
+000049b0: 7265 6e74 6c79 2069 6d70 6c65 6d65 6e74  rently implement
+000049c0: 6564 2066 6f72 206f 6e65 2d74 6f2d 6d61  ed for one-to-ma
+000049d0: 6e79 2067 656e 6520 6d61 7070 696e 6773  ny gene mappings
+000049e0: 2e22 290d 0a0d 0a20 2020 2020 2020 2023  .")....        #
+000049f0: 204d 616e 792d 746f 2d6f 6e65 206f 6e6c   Many-to-one onl
+00004a00: 790d 0a20 2020 2020 2020 206d 326f 203d  y..        m2o =
+00004a10: 2069 645f 6d61 7070 696e 675b 2869 645f   id_mapping[(id_
+00004a20: 6d61 7070 696e 675b 2273 6f75 7263 655f  mapping["source_
+00004a30: 6964 5f63 6f75 6e74 225d 203e 2031 2920  id_count"] > 1) 
+00004a40: 2620 2869 645f 6d61 7070 696e 675b 2264  & (id_mapping["d
+00004a50: 6573 745f 6964 5f63 6f75 6e74 225d 203d  est_id_count"] =
+00004a60: 3d20 3129 5d0d 0a20 2020 2020 2020 206d  = 1)]..        m
+00004a70: 326d 203d 2069 645f 6d61 7070 696e 675b  2m = id_mapping[
+00004a80: 2869 645f 6d61 7070 696e 675b 2273 6f75  (id_mapping["sou
+00004a90: 7263 655f 6964 5f63 6f75 6e74 225d 203e  rce_id_count"] >
+00004aa0: 2031 2920 2620 2869 645f 6d61 7070 696e   1) & (id_mappin
+00004ab0: 675b 2264 6573 745f 6964 5f63 6f75 6e74  g["dest_id_count
+00004ac0: 225d 203e 2031 295d 0d0a 0d0a 2020 2020  "] > 1)]....    
+00004ad0: 2020 2020 6966 2063 6173 655f 7365 6e73      if case_sens
+00004ae0: 6974 6976 653a 0d0a 2020 2020 2020 2020  itive:..        
+00004af0: 2020 2020 6964 5f69 6478 203d 2073 656c      id_idx = sel
+00004b00: 662e 6164 6174 612e 7661 725f 6e61 6d65  f.adata.var_name
+00004b10: 732e 6973 696e 286d 326f 2e69 6e64 6578  s.isin(m2o.index
+00004b20: 2e67 6574 5f6c 6576 656c 5f76 616c 7565  .get_level_value
+00004b30: 7328 3029 2920 2620 7e73 656c 662e 6164  s(0)) & ~self.ad
+00004b40: 6174 612e 7661 725f 6e61 6d65 732e 6973  ata.var_names.is
+00004b50: 696e 286d 326d 2e69 6e64 6578 2e67 6574  in(m2m.index.get
+00004b60: 5f6c 6576 656c 5f76 616c 7565 7328 3029  _level_values(0)
+00004b70: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00004b80: 6473 5f74 6f5f 6d61 7020 3d20 7365 6c66  ds_to_map = self
+00004b90: 2e61 6461 7461 2e76 6172 5f6e 616d 6573  .adata.var_names
+00004ba0: 5b69 645f 6964 785d 0d0a 2020 2020 2020  [id_idx]..      
+00004bb0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00004bc0: 2020 2020 2069 645f 6964 7820 3d20 7365       id_idx = se
+00004bd0: 6c66 2e61 6461 7461 2e76 6172 5f6e 616d  lf.adata.var_nam
+00004be0: 6573 2e73 7472 2e63 6173 6566 6f6c 6428  es.str.casefold(
+00004bf0: 292e 6973 696e 286d 326f 2e69 6e64 6578  ).isin(m2o.index
+00004c00: 2e67 6574 5f6c 6576 656c 5f76 616c 7565  .get_level_value
+00004c10: 7328 3029 2e73 7472 2e63 6173 6566 6f6c  s(0).str.casefol
+00004c20: 6428 2929 2026 207e 7365 6c66 2e61 6461  d()) & ~self.ada
+00004c30: 7461 2e76 6172 5f6e 616d 6573 2e73 7472  ta.var_names.str
+00004c40: 2e63 6173 6566 6f6c 6428 292e 6973 696e  .casefold().isin
+00004c50: 286d 326d 2e69 6e64 6578 2e67 6574 5f6c  (m2m.index.get_l
+00004c60: 6576 656c 5f76 616c 7565 7328 3029 2e73  evel_values(0).s
+00004c70: 7472 2e63 6173 6566 6f6c 6428 2929 0d0a  tr.casefold())..
+00004c80: 2020 2020 2020 2020 2020 2020 6964 735f              ids_
+00004c90: 746f 5f6d 6170 203d 2073 656c 662e 6164  to_map = self.ad
+00004ca0: 6174 612e 7661 725f 6e61 6d65 735b 6964  ata.var_names[id
+00004cb0: 5f69 6478 5d2e 7374 722e 6361 7365 666f  _idx].str.casefo
+00004cc0: 6c64 2829 0d0a 2020 2020 2020 2020 7372  ld()..        sr
+00004cd0: 635f 6964 7320 3d20 7365 6c66 2e61 6461  c_ids = self.ada
+00004ce0: 7461 2e76 6172 5f6e 616d 6573 5b69 645f  ta.var_names[id_
+00004cf0: 6964 785d 0d0a 2020 2020 2020 2020 6966  idx]..        if
+00004d00: 206d 616e 795f 746f 5f6f 6e65 2069 7320   many_to_one is 
+00004d10: 4661 6c73 653a 0d0a 2020 2020 2020 2020  False:..        
+00004d20: 2020 2020 6465 7374 5f69 6473 203d 2075      dest_ids = u
+00004d30: 6e6d 6170 7065 645f 7072 6566 6978 202b  nmapped_prefix +
+00004d40: 2073 7263 5f69 6473 0d0a 2020 2020 2020   src_ids..      
+00004d50: 2020 2020 2020 736f 7572 6365 5f69 645f        source_id_
+00004d60: 6c69 7374 2e65 7874 656e 6428 7372 635f  list.extend(src_
+00004d70: 6964 7329 0d0a 2020 2020 2020 2020 2020  ids)..          
+00004d80: 2020 6465 7374 5f69 645f 6c69 7374 2e65    dest_id_list.e
+00004d90: 7874 656e 6428 6465 7374 5f69 6473 290d  xtend(dest_ids).
+00004da0: 0a20 2020 2020 2020 2020 2020 206d 6170  .            map
+00004db0: 7069 6e67 5f72 656c 6174 696f 6e73 6869  ping_relationshi
+00004dc0: 702e 6578 7465 6e64 286c 656e 2873 7263  p.extend(len(src
+00004dd0: 5f69 6473 2920 2a20 5b22 6d61 6e79 2d74  _ids) * ["many-t
+00004de0: 6f2d 6f6e 6522 5d29 0d0a 2020 2020 2020  o-one"])..      
+00004df0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00004e00: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
+00004e10: 706c 656d 656e 7465 6445 7272 6f72 2866  plementedError(f
+00004e20: 2260 7b6d 616e 795f 746f 5f6f 6e65 7d60  "`{many_to_one}`
+00004e30: 2069 7320 6e6f 7420 6375 7272 656e 746c   is not currentl
+00004e40: 7920 696d 706c 656d 656e 7465 6420 666f  y implemented fo
+00004e50: 7220 6d61 6e79 2d74 6f2d 6f6e 6520 6765  r many-to-one ge
+00004e60: 6e65 206d 6170 7069 6e67 732e 2229 0d0a  ne mappings.")..
+00004e70: 0d0a 2020 2020 2020 2020 2320 4d61 6e79  ..        # Many
+00004e80: 2d74 6f2d 6d61 6e79 206f 6e6c 790d 0a20  -to-many only.. 
+00004e90: 2020 2020 2020 2069 6620 6361 7365 5f73         if case_s
+00004ea0: 656e 7369 7469 7665 3a0d 0a20 2020 2020  ensitive:..     
+00004eb0: 2020 2020 2020 2069 645f 6964 7820 3d20         id_idx = 
+00004ec0: 7365 6c66 2e61 6461 7461 2e76 6172 5f6e  self.adata.var_n
+00004ed0: 616d 6573 2e69 7369 6e28 6d32 6d2e 696e  ames.isin(m2m.in
+00004ee0: 6465 782e 6765 745f 6c65 7665 6c5f 7661  dex.get_level_va
+00004ef0: 6c75 6573 2830 2929 2026 207e 7365 6c66  lues(0)) & ~self
+00004f00: 2e61 6461 7461 2e76 6172 5f6e 616d 6573  .adata.var_names
+00004f10: 2e69 7369 6e28 6d32 6f2e 696e 6465 782e  .isin(m2o.index.
+00004f20: 6765 745f 6c65 7665 6c5f 7661 6c75 6573  get_level_values
+00004f30: 2830 2929 0d0a 2020 2020 2020 2020 2020  (0))..          
+00004f40: 2020 6964 735f 746f 5f6d 6170 203d 2073    ids_to_map = s
+00004f50: 656c 662e 6164 6174 612e 7661 725f 6e61  elf.adata.var_na
+00004f60: 6d65 735b 6964 5f69 6478 5d0d 0a20 2020  mes[id_idx]..   
+00004f70: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00004f80: 2020 2020 2020 2020 6964 5f69 6478 203d          id_idx =
+00004f90: 2073 656c 662e 6164 6174 612e 7661 725f   self.adata.var_
+00004fa0: 6e61 6d65 732e 7374 722e 6361 7365 666f  names.str.casefo
+00004fb0: 6c64 2829 2e69 7369 6e28 6d32 6d2e 696e  ld().isin(m2m.in
+00004fc0: 6465 782e 6765 745f 6c65 7665 6c5f 7661  dex.get_level_va
+00004fd0: 6c75 6573 2830 292e 7374 722e 6361 7365  lues(0).str.case
+00004fe0: 666f 6c64 2829 2920 2620 7e73 656c 662e  fold()) & ~self.
+00004ff0: 6164 6174 612e 7661 725f 6e61 6d65 732e  adata.var_names.
+00005000: 7374 722e 6361 7365 666f 6c64 2829 2e69  str.casefold().i
+00005010: 7369 6e28 6d32 6f2e 696e 6465 782e 6765  sin(m2o.index.ge
+00005020: 745f 6c65 7665 6c5f 7661 6c75 6573 2830  t_level_values(0
+00005030: 292e 7374 722e 6361 7365 666f 6c64 2829  ).str.casefold()
+00005040: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00005050: 6473 5f74 6f5f 6d61 7020 3d20 7365 6c66  ds_to_map = self
+00005060: 2e61 6461 7461 2e76 6172 5f6e 616d 6573  .adata.var_names
+00005070: 5b69 645f 6964 785d 2e73 7472 2e63 6173  [id_idx].str.cas
+00005080: 6566 6f6c 6428 290d 0a20 2020 2020 2020  efold()..       
+00005090: 2073 7263 5f69 6473 203d 2073 656c 662e   src_ids = self.
+000050a0: 6164 6174 612e 7661 725f 6e61 6d65 735b  adata.var_names[
+000050b0: 6964 5f69 6478 5d0d 0a20 2020 2020 2020  id_idx]..       
+000050c0: 2069 6620 6d61 6e79 5f74 6f5f 6d61 6e79   if many_to_many
+000050d0: 2069 7320 4661 6c73 653a 0d0a 2020 2020   is False:..    
+000050e0: 2020 2020 2020 2020 6465 7374 5f69 6473          dest_ids
+000050f0: 203d 2075 6e6d 6170 7065 645f 7072 6566   = unmapped_pref
+00005100: 6978 202b 2073 7263 5f69 6473 0d0a 2020  ix + src_ids..  
+00005110: 2020 2020 2020 2020 2020 736f 7572 6365            source
+00005120: 5f69 645f 6c69 7374 2e65 7874 656e 6428  _id_list.extend(
+00005130: 7372 635f 6964 7329 0d0a 2020 2020 2020  src_ids)..      
+00005140: 2020 2020 2020 6465 7374 5f69 645f 6c69        dest_id_li
+00005150: 7374 2e65 7874 656e 6428 6465 7374 5f69  st.extend(dest_i
+00005160: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
+00005170: 206d 6170 7069 6e67 5f72 656c 6174 696f   mapping_relatio
+00005180: 6e73 6869 702e 6578 7465 6e64 286c 656e  nship.extend(len
+00005190: 2873 7263 5f69 6473 2920 2a20 5b22 6d61  (src_ids) * ["ma
+000051a0: 6e79 2d74 6f2d 6d61 6e79 225d 290d 0a20  ny-to-many"]).. 
+000051b0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000051c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000051d0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+000051e0: 726f 7228 6622 607b 6d61 6e79 5f74 6f5f  ror(f"`{many_to_
+000051f0: 6d61 6e79 7d60 2069 7320 6e6f 7420 6375  many}` is not cu
+00005200: 7272 656e 746c 7920 696d 706c 656d 656e  rrently implemen
+00005210: 7465 6420 666f 7220 6d61 6e79 2d74 6f2d  ted for many-to-
+00005220: 6d61 6e79 2067 656e 6520 6d61 7070 696e  many gene mappin
+00005230: 6773 2e22 290d 0a0d 0a20 2020 2020 2020  gs.")....       
+00005240: 2023 2049 4473 2077 6974 6820 626f 7468   # IDs with both
+00005250: 206d 616e 792d 746f 2d6d 616e 7920 616e   many-to-many an
+00005260: 6420 6d61 6e79 2d74 6f2d 6f6e 6520 7265  d many-to-one re
+00005270: 6c61 7469 6f6e 7368 6970 0d0a 2020 2020  lationship..    
+00005280: 2020 2020 6966 2063 6173 655f 7365 6e73      if case_sens
+00005290: 6974 6976 653a 0d0a 2020 2020 2020 2020  itive:..        
+000052a0: 2020 2020 6964 5f69 6478 203d 2073 656c      id_idx = sel
+000052b0: 662e 6164 6174 612e 7661 725f 6e61 6d65  f.adata.var_name
+000052c0: 732e 6973 696e 286d 326d 2e69 6e64 6578  s.isin(m2m.index
+000052d0: 2e67 6574 5f6c 6576 656c 5f76 616c 7565  .get_level_value
+000052e0: 7328 3029 2920 2620 7365 6c66 2e61 6461  s(0)) & self.ada
+000052f0: 7461 2e76 6172 5f6e 616d 6573 2e69 7369  ta.var_names.isi
+00005300: 6e28 6d32 6f2e 696e 6465 782e 6765 745f  n(m2o.index.get_
+00005310: 6c65 7665 6c5f 7661 6c75 6573 2830 2929  level_values(0))
+00005320: 0d0a 2020 2020 2020 2020 2020 2020 6964  ..            id
+00005330: 735f 746f 5f6d 6170 203d 2073 656c 662e  s_to_map = self.
+00005340: 6164 6174 612e 7661 725f 6e61 6d65 735b  adata.var_names[
+00005350: 6964 5f69 6478 5d0d 0a20 2020 2020 2020  id_idx]..       
+00005360: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00005370: 2020 2020 6964 5f69 6478 203d 2073 656c      id_idx = sel
+00005380: 662e 6164 6174 612e 7661 725f 6e61 6d65  f.adata.var_name
+00005390: 732e 7374 722e 6361 7365 666f 6c64 2829  s.str.casefold()
+000053a0: 2e69 7369 6e28 6d32 6d2e 696e 6465 782e  .isin(m2m.index.
+000053b0: 6765 745f 6c65 7665 6c5f 7661 6c75 6573  get_level_values
+000053c0: 2830 292e 7374 722e 6361 7365 666f 6c64  (0).str.casefold
+000053d0: 2829 2920 2620 7365 6c66 2e61 6461 7461  ()) & self.adata
+000053e0: 2e76 6172 5f6e 616d 6573 2e73 7472 2e63  .var_names.str.c
+000053f0: 6173 6566 6f6c 6428 292e 6973 696e 286d  asefold().isin(m
+00005400: 326f 2e69 6e64 6578 2e67 6574 5f6c 6576  2o.index.get_lev
+00005410: 656c 5f76 616c 7565 7328 3029 2e73 7472  el_values(0).str
+00005420: 2e63 6173 6566 6f6c 6428 2929 0d0a 2020  .casefold())..  
+00005430: 2020 2020 2020 2020 2020 6964 735f 746f            ids_to
+00005440: 5f6d 6170 203d 2073 656c 662e 6164 6174  _map = self.adat
+00005450: 612e 7661 725f 6e61 6d65 735b 6964 5f69  a.var_names[id_i
+00005460: 6478 5d2e 7374 722e 6361 7365 666f 6c64  dx].str.casefold
+00005470: 2829 0d0a 2020 2020 2020 2020 7372 635f  ()..        src_
+00005480: 6964 7320 3d20 7365 6c66 2e61 6461 7461  ids = self.adata
+00005490: 2e76 6172 5f6e 616d 6573 5b69 645f 6964  .var_names[id_id
+000054a0: 785d 0d0a 2020 2020 2020 2020 6465 7374  x]..        dest
+000054b0: 5f69 6473 203d 2075 6e6d 6170 7065 645f  _ids = unmapped_
+000054c0: 7072 6566 6978 202b 2073 7263 5f69 6473  prefix + src_ids
+000054d0: 0d0a 2020 2020 2020 2020 736f 7572 6365  ..        source
+000054e0: 5f69 645f 6c69 7374 2e65 7874 656e 6428  _id_list.extend(
+000054f0: 7372 635f 6964 7329 0d0a 2020 2020 2020  src_ids)..      
+00005500: 2020 6465 7374 5f69 645f 6c69 7374 2e65    dest_id_list.e
+00005510: 7874 656e 6428 6465 7374 5f69 6473 290d  xtend(dest_ids).
+00005520: 0a20 2020 2020 2020 206d 6170 7069 6e67  .        mapping
+00005530: 5f72 656c 6174 696f 6e73 6869 702e 6578  _relationship.ex
+00005540: 7465 6e64 286c 656e 2873 7263 5f69 6473  tend(len(src_ids
+00005550: 2920 2a20 5b22 6d61 6e79 2d74 6f2d 6d61  ) * ["many-to-ma
+00005560: 6e79 3b20 6d61 6e79 2d74 6f2d 6f6e 6522  ny; many-to-one"
+00005570: 5d29 0d0a 2020 2020 0d0a 2020 2020 2020  ])..    ..      
+00005580: 2020 2320 6372 6561 7465 206e 6577 2061    # create new a
+00005590: 6e6e 6461 7461 206f 626a 6563 740d 0a20  nndata object.. 
+000055a0: 2020 2020 2020 206e 6577 5f61 6461 7461         new_adata
+000055b0: 203d 2073 656c 662e 6164 6174 615b 3a2c   = self.adata[:,
+000055c0: 2073 6f75 7263 655f 6964 5f6c 6973 745d   source_id_list]
+000055d0: 0d0a 2020 2020 2020 2020 6e65 775f 6164  ..        new_ad
+000055e0: 6174 612e 7661 725f 6e61 6d65 7320 3d20  ata.var_names = 
+000055f0: 6465 7374 5f69 645f 6c69 7374 0d0a 2020  dest_id_list..  
+00005600: 2020 2020 2020 6e65 775f 6164 6174 612e        new_adata.
+00005610: 7661 725b 2273 6f75 7263 655f 6964 225d  var["source_id"]
+00005620: 203d 2073 6f75 7263 655f 6964 5f6c 6973   = source_id_lis
+00005630: 740d 0a20 2020 2020 2020 206e 6577 5f61  t..        new_a
+00005640: 6461 7461 2e76 6172 5b22 6d61 7070 696e  data.var["mappin
+00005650: 675f 7265 6c61 7469 6f6e 7368 6970 225d  g_relationship"]
+00005660: 203d 206d 6170 7069 6e67 5f72 656c 6174   = mapping_relat
+00005670: 696f 6e73 6869 700d 0a20 2020 2020 2020  ionship..       
+00005680: 206e 6577 5f61 6461 7461 2e76 6172 5b22   new_adata.var["
+00005690: 6d61 7070 696e 675f 7265 6c61 7469 6f6e  mapping_relation
+000056a0: 7368 6970 225d 203d 206e 6577 5f61 6461  ship"] = new_ada
+000056b0: 7461 2e76 6172 5b22 6d61 7070 696e 675f  ta.var["mapping_
+000056c0: 7265 6c61 7469 6f6e 7368 6970 225d 2e61  relationship"].a
+000056d0: 7374 7970 6528 2263 6174 6567 6f72 7922  stype("category"
+000056e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000056f0: 6164 6174 6120 3d20 6e65 775f 6164 6174  adata = new_adat
+00005700: 610d 0a20 2020 2020 2020 2073 656c 662e  a..        self.
+00005710: 6170 7065 6e64 5f74 6f5f 6869 7374 6f72  append_to_histor
+00005720: 7928 6622 4d61 7070 6564 2066 6561 7475  y(f"Mapped featu
+00005730: 7265 2049 4473 2e20 736f 7572 6365 2073  re IDs. source s
+00005740: 7065 6369 6573 3d7b 736f 7572 6365 5f73  pecies={source_s
+00005750: 7065 6369 6573 7d2c 2073 6f75 7263 655f  pecies}, source_
+00005760: 6964 733d 7b73 6f75 7263 655f 6964 737d  ids={source_ids}
+00005770: 2c20 6465 7374 5f73 7065 6369 6573 3d7b  , dest_species={
+00005780: 6465 7374 5f73 7065 6369 6573 7d2c 2064  dest_species}, d
+00005790: 6573 745f 6964 733d 7b64 6573 745f 6964  est_ids={dest_id
+000057a0: 737d 2c20 220d 0a20 2020 2020 2020 2020  s}, "..         
 000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057c0: 2020 2020 2066 226f 6e65 5f74 6f5f 6f6e       f"one_to_on
-000057d0: 653d 7b6f 6e65 5f74 6f5f 6f6e 657d 2c20  e={one_to_one}, 
-000057e0: 6f6e 655f 746f 5f6d 616e 793d 7b6f 6e65  one_to_many={one
-000057f0: 5f74 6f5f 6d61 6e79 7d2c 206d 616e 795f  _to_many}, many_
-00005800: 746f 5f6f 6e65 3d7b 6d61 6e79 5f74 6f5f  to_one={many_to_
-00005810: 6f6e 657d 2c20 6d61 6e79 5f74 6f5f 6d61  one}, many_to_ma
-00005820: 6e79 3d7b 6d61 6e79 5f74 6f5f 6d61 6e79  ny={many_to_many
-00005830: 7d2c 2075 6e6d 6170 7065 645f 7072 6566  }, unmapped_pref
-00005840: 6978 3d7b 756e 6d61 7070 6564 5f70 7265  ix={unmapped_pre
-00005850: 6669 787d 2229 0d0a 0d0a 2020 2020 6465  fix}")....    de
-00005860: 6620 7570 6461 7465 5f6f 6273 2873 656c  f update_obs(sel
-00005870: 662c 206f 6273 293a 0d0a 2020 2020 2020  f, obs):..      
-00005880: 2020 2222 2255 7064 6174 6520 7468 6520    """Update the 
-00005890: 6f62 7365 7276 6174 696f 6e20 6d65 7461  observation meta
-000058a0: 6461 7461 2077 6974 6820 6120 6e65 7720  data with a new 
-000058b0: 6d65 7461 6461 7461 206d 6174 7269 780d  metadata matrix.
-000058c0: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-000058d0: 6d20 6f62 733a 2041 6e20 6f62 7365 7276  m obs: An observ
-000058e0: 6174 696f 6e73 20c3 9720 6d65 7461 6461  ations .. metada
-000058f0: 7461 206d 6174 7269 782c 2064 6566 6175  ta matrix, defau
-00005900: 6c74 7320 746f 204e 6f6e 650d 0a20 2020  lts to None..   
-00005910: 2020 2020 203a 7479 7065 206f 6273 3a20       :type obs: 
-00005920: 6070 642e 4461 7461 4672 616d 6560 2c20  `pd.DataFrame`, 
-00005930: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00005940: 2020 2222 220d 0a20 2020 2020 2020 2023    """..        #
-00005950: 2063 6f6e 7665 7274 2027 6f62 6a65 6374   convert 'object
-00005960: 2720 6474 7970 6520 746f 2063 6174 6567  ' dtype to categ
-00005970: 6f72 6963 616c 2c20 636f 6e76 6572 7469  orical, converti
-00005980: 6e67 2062 6f6f 6c20 7661 6c75 6573 2074  ng bool values t
-00005990: 6f20 7374 7269 6e67 7320 6173 2074 6865  o strings as the
-000059a0: 7365 2061 7265 206e 6f74 2073 7570 706f  se are not suppo
-000059b0: 7274 6564 2062 7920 416e 6e44 6174 6120  rted by AnnData 
-000059c0: 6f6e 2d64 6973 6b20 666f 726d 6174 0d0a  on-disk format..
-000059d0: 2020 2020 2020 2020 666f 7220 636f 6c20          for col 
-000059e0: 696e 206f 6273 2e73 656c 6563 745f 6474  in obs.select_dt
-000059f0: 7970 6573 2869 6e63 6c75 6465 3d28 2262  ypes(include=("b
-00005a00: 6f6f 6c22 2c20 226f 626a 6563 7422 2929  ool", "object"))
-00005a10: 2e63 6f6c 756d 6e73 3a0d 0a20 2020 2020  .columns:..     
-00005a20: 2020 2020 2020 206f 6273 5b63 6f6c 5d20         obs[col] 
-00005a30: 3d20 6f62 735b 636f 6c5d 2e61 7374 7970  = obs[col].astyp
-00005a40: 6528 2273 7472 2229 2e61 7374 7970 6528  e("str").astype(
-00005a50: 2263 6174 6567 6f72 7922 290d 0a20 2020  "category")..   
-00005a60: 2020 2020 206d 6973 7369 6e67 5f73 616d       missing_sam
-00005a70: 706c 6573 5f69 6e5f 5820 3d20 6f62 732e  ples_in_X = obs.
-00005a80: 696e 6465 782e 6469 6666 6572 656e 6365  index.difference
-00005a90: 2873 656c 662e 6164 6174 612e 6f62 732e  (self.adata.obs.
-00005aa0: 696e 6465 7829 2e61 7374 7970 6528 7374  index).astype(st
-00005ab0: 7229 2e74 6f5f 6c69 7374 2829 0d0a 2020  r).to_list()..  
-00005ac0: 2020 2020 2020 6966 206d 6973 7369 6e67        if missing
-00005ad0: 5f73 616d 706c 6573 5f69 6e5f 583a 0d0a  _samples_in_X:..
-00005ae0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00005af0: 696e 672e 7761 726e 696e 6728 2254 6865  ing.warning("The
-00005b00: 2066 6f6c 6c6f 7769 6e67 2073 616d 706c   following sampl
-00005b10: 6573 2069 6e20 7468 6520 6d65 7461 6461  es in the metada
-00005b20: 7461 2077 6572 6520 6e6f 7420 7072 6573  ta were not pres
-00005b30: 656e 7420 696e 2074 6865 2064 6174 6120  ent in the data 
-00005b40: 2860 6164 6174 612e 5860 293a 5c6e 2020  (`adata.X`):\n  
-00005b50: 2d20 2220 2b20 225c 6e20 202d 2022 2e6a  - " + "\n  - ".j
-00005b60: 6f69 6e28 6d69 7373 696e 675f 7361 6d70  oin(missing_samp
-00005b70: 6c65 735f 696e 5f58 2929 0d0a 2020 2020  les_in_X))..    
-00005b80: 2020 2020 6d69 7373 696e 675f 7361 6d70      missing_samp
-00005b90: 6c65 735f 696e 5f6d 6420 3d20 7365 6c66  les_in_md = self
-00005ba0: 2e61 6461 7461 2e6f 6273 2e69 6e64 6578  .adata.obs.index
-00005bb0: 2e64 6966 6665 7265 6e63 6528 6f62 732e  .difference(obs.
-00005bc0: 696e 6465 7829 2e61 7374 7970 6528 7374  index).astype(st
-00005bd0: 7229 2e74 6f5f 6c69 7374 2829 0d0a 2020  r).to_list()..  
-00005be0: 2020 2020 2020 6966 206d 6973 7369 6e67        if missing
-00005bf0: 5f73 616d 706c 6573 5f69 6e5f 6d64 3a0d  _samples_in_md:.
-00005c00: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00005c10: 6769 6e67 2e77 6172 6e69 6e67 2822 5468  ging.warning("Th
-00005c20: 6520 666f 6c6c 6f77 696e 6720 7361 6d70  e following samp
-00005c30: 6c65 7320 696e 2074 6865 2064 6174 6120  les in the data 
-00005c40: 2860 6164 6174 612e 5860 2920 7765 7265  (`adata.X`) were
-00005c50: 2061 6273 656e 7420 696e 2074 6865 206d   absent in the m
-00005c60: 6574 6164 6174 613a 5c6e 2020 2d20 2220  etadata:\n  - " 
-00005c70: 2b20 225c 6e20 202d 2022 2e6a 6f69 6e28  + "\n  - ".join(
-00005c80: 6d69 7373 696e 675f 7361 6d70 6c65 735f  missing_samples_
-00005c90: 696e 5f6d 6429 290d 0a20 2020 2020 2020  in_md))..       
-00005ca0: 2073 656c 662e 6164 6174 612e 6f62 7320   self.adata.obs 
-00005cb0: 3d20 6f62 732e 7265 696e 6465 7828 7365  = obs.reindex(se
-00005cc0: 6c66 2e61 6461 7461 2e6f 6273 2e69 6e64  lf.adata.obs.ind
-00005cd0: 6578 290d 0a20 2020 2020 2020 2073 656c  ex)..        sel
-00005ce0: 662e 6170 7065 6e64 5f74 6f5f 6869 7374  f.append_to_hist
-00005cf0: 6f72 7928 6622 6d65 7461 6461 7461 2028  ory(f"metadata (
-00005d00: 6164 6174 612e 6f62 7329 2075 7064 6174  adata.obs) updat
-00005d10: 6564 2e22 290d 0a20 2020 200d 0a20 2020  ed.")..    ..   
-00005d20: 2064 6566 2067 6574 5f70 7269 6e74 6162   def get_printab
-00005d30: 6c65 5f6d 6574 6164 6174 615f 7479 7065  le_metadata_type
-00005d40: 5f73 756d 6d61 7279 2873 656c 6629 3a0d  _summary(self):.
-00005d50: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00005d60: 726e 2061 2070 7269 6e74 6162 6c65 2073  rn a printable s
-00005d70: 756d 6d61 7279 206f 6620 6d65 7461 6461  ummary of metada
-00005d80: 7461 2061 6e64 2074 6865 2074 7970 6573  ta and the types
-00005d90: 2e0d 0a0d 0a20 2020 2020 2020 203a 7265  .....        :re
-00005da0: 7475 726e 3a20 5375 6d6d 6172 7920 6f66  turn: Summary of
-00005db0: 206d 6574 6164 6174 610d 0a20 2020 2020   metadata..     
-00005dc0: 2020 203a 7274 7970 653a 2073 7472 0d0a     :rtype: str..
-00005dd0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00005de0: 2020 2020 206d 7367 203d 2022 5375 6d6d       msg = "Summ
-00005df0: 6172 7920 6f66 206d 6574 6164 6174 6120  ary of metadata 
-00005e00: 7479 7065 735c 6e5c 6e20 2020 2053 616d  types\n\n    Sam
-00005e10: 706c 6520 6d65 7461 6461 7461 3a5c 6e22  ple metadata:\n"
-00005e20: 0d0a 2020 2020 2020 2020 666f 7220 636f  ..        for co
-00005e30: 6c20 696e 2073 656c 662e 6164 6174 612e  l in self.adata.
-00005e40: 6f62 732e 636f 6c75 6d6e 733a 0d0a 2020  obs.columns:..  
-00005e50: 2020 2020 2020 2020 2020 6d73 6720 2b3d            msg +=
-00005e60: 2022 2020 2020 2020 2020 2220 2b20 636f   "        " + co
-00005e70: 6c20 2b20 223a 2022 202b 2073 656c 662e  l + ": " + self.
-00005e80: 6164 6174 612e 6f62 735b 636f 6c5d 2e64  adata.obs[col].d
-00005e90: 7479 7065 2e6e 616d 6520 2b20 225c 6e22  type.name + "\n"
-00005ea0: 0d0a 2020 2020 2020 2020 6d73 6720 2b3d  ..        msg +=
-00005eb0: 2022 2020 2020 4665 6174 7572 6520 6d65   "    Feature me
-00005ec0: 7461 6461 7461 3a5c 6e22 0d0a 2020 2020  tadata:\n"..    
-00005ed0: 2020 2020 666f 7220 636f 6c20 696e 2073      for col in s
-00005ee0: 656c 662e 6164 6174 612e 7661 722e 636f  elf.adata.var.co
-00005ef0: 6c75 6d6e 733a 0d0a 2020 2020 2020 2020  lumns:..        
-00005f00: 2020 2020 6d73 6720 2b3d 2022 2020 2020      msg += "    
-00005f10: 2020 2020 2220 2b20 636f 6c20 2b20 223a      " + col + ":
-00005f20: 2022 202b 2073 656c 662e 6164 6174 612e   " + self.adata.
-00005f30: 7661 725b 636f 6c5d 2e64 7479 7065 2e6e  var[col].dtype.n
-00005f40: 616d 6520 2b20 225c 6e22 0d0a 2020 2020  ame + "\n"..    
-00005f50: 2020 2020 7265 7475 726e 206d 7367 0d0a      return msg..
-00005f60: 2020 2020 0d0a 2020 2020 6465 6620 7772      ..    def wr
-00005f70: 6974 655f 6835 6164 2873 656c 662c 0d0a  ite_h5ad(self,..
-00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 2020 2066 696c 656e 616d 653a 2073 7472     filename: str
-00005fa0: 293a 0d0a 2020 2020 2020 2020 2222 2257  ):..        """W
-00005fb0: 7269 7465 2064 6174 6173 6574 2074 6f20  rite dataset to 
-00005fc0: 2e68 3561 6420 6669 6c65 2e0d 0a0d 0a20  .h5ad file..... 
-00005fd0: 2020 2020 2020 203a 7061 7261 6d20 6669         :param fi
-00005fe0: 6c65 6e61 6d65 3a20 6669 6c65 7061 7468  lename: filepath
-00005ff0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00006000: 6669 6c65 6e61 6d65 3a20 7374 720d 0a20  filename: str.. 
-00006010: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00006020: 2020 2020 6669 6c65 6e61 6d65 203d 206f      filename = o
-00006030: 732e 7061 7468 2e61 6273 7061 7468 2866  s.path.abspath(f
-00006040: 696c 656e 616d 6529 0d0a 2020 2020 2020  ilename)..      
-00006050: 2020 6c6f 6767 696e 672e 696e 666f 2866    logging.info(f
-00006060: 2257 7269 7469 6e67 2074 6f20 7b66 696c  "Writing to {fil
-00006070: 656e 616d 657d 2229 0d0a 2020 2020 2020  ename}")..      
-00006080: 2020 7365 6c66 2e61 7070 656e 645f 746f    self.append_to
-00006090: 5f68 6973 746f 7279 2822 5772 6974 696e  _history("Writin
-000060a0: 6720 746f 207b 6669 6c65 6e61 6d65 7d22  g to {filename}"
-000060b0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000060c0: 6164 6174 612e 7772 6974 655f 6835 6164  adata.write_h5ad
-000060d0: 2866 696c 656e 616d 6529 0d0a 2020 2020  (filename)..    
-000060e0: 2020 2020 6c6f 6767 696e 672e 696e 666f      logging.info
-000060f0: 2866 2257 7269 7465 2063 6f6d 706c 6574  (f"Write complet
-00006100: 6564 2e22 290d 0a20 2020 200d 0a20 2020  ed.")..    ..   
-00006110: 2064 6566 2074 6f5f 6466 2873 656c 662c   def to_df(self,
-00006120: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006130: 6e6f 726d 616c 697a 6564 3a20 626f 6f6c  normalized: bool
-00006140: 203d 2046 616c 7365 293a 0d0a 2020 2020   = False):..    
-00006150: 2020 2020 2222 2247 6574 2064 6174 6120      """Get data 
-00006160: 6d61 7472 6978 2061 7320 6120 6070 642e  matrix as a `pd.
-00006170: 4461 7461 4672 616d 6560 0d0a 0d0a 2020  DataFrame`....  
-00006180: 2020 2020 2020 3a70 6172 616d 206e 6f72        :param nor
-00006190: 6d61 6c69 7a65 643a 2053 6574 2074 7275  malized: Set tru
-000061a0: 6520 666f 7220 5450 4d20 6e6f 726d 616c  e for TPM normal
-000061b0: 697a 6564 206f 7574 7075 742c 2064 6566  ized output, def
-000061c0: 6175 6c74 7320 746f 2046 616c 7365 0d0a  aults to False..
-000061d0: 2020 2020 2020 2020 3a74 7970 6520 6e6f          :type no
-000061e0: 726d 616c 697a 6564 3a20 626f 6f6c 2c20  rmalized: bool, 
-000061f0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00006200: 2020 3a72 6574 7572 6e3a 206f 6273 6572    :return: obser
-00006210: 7661 7469 6f6e 7320 c397 2066 6561 7475  vations .. featu
-00006220: 7265 7320 6461 7461 206d 6174 7269 780d  res data matrix.
-00006230: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00006240: 2070 642e 4461 7461 4672 616d 650d 0a20   pd.DataFrame.. 
-00006250: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00006260: 2020 2020 6466 203d 2073 656c 662e 6164      df = self.ad
-00006270: 6174 612e 746f 5f64 6628 290d 0a20 2020  ata.to_df()..   
-00006280: 2020 2020 2069 6620 6e6f 726d 616c 697a       if normaliz
-00006290: 6564 2061 6e64 206e 6f74 2073 656c 662e  ed and not self.
-000062a0: 6973 5f6e 6f72 6d61 6c69 7a65 643a 0d0a  is_normalized:..
-000062b0: 2020 2020 2020 2020 2020 2020 6466 203d              df =
-000062c0: 2064 662e 6469 7628 6466 2e73 756d 2861   df.div(df.sum(a
-000062d0: 7869 733d 3129 2c20 6178 6973 3d30 2920  xis=1), axis=0) 
-000062e0: 2a20 3165 3620 2023 2054 504d 206e 6f72  * 1e6  # TPM nor
-000062f0: 6d61 6c69 7a61 7469 6f6e 0d0a 2020 2020  malization..    
-00006300: 2020 2020 7265 7475 726e 2064 660d 0a0d      return df...
-00006310: 0a20 2020 2064 6566 2072 656d 6f76 655f  .    def remove_
-00006320: 756e 6661 6374 6f72 697a 6162 6c65 5f6f  unfactorizable_o
-00006330: 6273 6572 7661 7469 6f6e 7328 7365 6c66  bservations(self
-00006340: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
-00006350: 656d 6f76 6573 206f 6273 6572 7661 7469  emoves observati
-00006360: 6f6e 7320 7769 7468 2061 6c6c 207a 6572  ons with all zer
-00006370: 6f73 2066 726f 6d20 7468 6520 6461 7461  os from the data
-00006380: 206d 6174 7269 782e 0d0a 2020 2020 2020   matrix...      
-00006390: 2020 2222 220d 0a20 2020 2020 2020 2064    """..        d
-000063a0: 6620 3d20 7365 6c66 2e74 6f5f 6466 286e  f = self.to_df(n
-000063b0: 6f72 6d61 6c69 7a65 643d 4661 6c73 6529  ormalized=False)
-000063c0: 0d0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
-000063d0: 6b20 666f 7220 6f62 7365 7276 6174 696f  k for observatio
-000063e0: 6e73 2077 6974 6820 616c 6c20 7a65 726f  ns with all zero
-000063f0: 730d 0a20 2020 2020 2020 206f 6273 5f7a  s..        obs_z
-00006400: 6572 6f73 203d 2028 6466 2e54 203d 3d20  eros = (df.T == 
-00006410: 3029 2e61 6c6c 2829 0d0a 2020 2020 2020  0).all()..      
-00006420: 2020 6e5f 6f62 735f 7a65 726f 7320 3d20    n_obs_zeros = 
-00006430: 6f62 735f 7a65 726f 732e 7375 6d28 290d  obs_zeros.sum().
-00006440: 0a20 2020 2020 2020 206c 6f67 6769 6e67  .        logging
-00006450: 2e69 6e66 6f28 6622 7b6e 5f6f 6273 5f7a  .info(f"{n_obs_z
-00006460: 6572 6f73 7d20 6f66 207b 7365 6c66 2e61  eros} of {self.a
-00006470: 6461 7461 2e6e 5f6f 6273 7d20 6f62 7365  data.n_obs} obse
-00006480: 7276 6174 696f 6e73 2061 7265 2061 6c6c  rvations are all
-00006490: 207a 6572 6f73 2e22 290d 0a20 2020 2020   zeros.")..     
-000064a0: 2020 2069 6620 6e5f 6f62 735f 7a65 726f     if n_obs_zero
-000064b0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000064c0: 6c6f 6767 696e 672e 7761 726e 696e 6728  logging.warning(
-000064d0: 6622 5375 6273 6574 7469 6e67 206f 6273  f"Subsetting obs
-000064e0: 6572 7661 7469 6f6e 7320 746f 2074 686f  ervations to tho
-000064f0: 7365 2077 6974 6820 6174 206c 6561 7374  se with at least
-00006500: 2031 2070 6f73 6974 6976 6520 7661 6c75   1 positive valu
-00006510: 652e 2229 0d0a 2020 2020 2020 2020 2020  e.")..          
-00006520: 2020 6d73 675f 7374 7269 6e67 203d 2072    msg_string = r
-00006530: 6570 7228 6f62 735f 7a65 726f 735b 6f62  epr(obs_zeros[ob
-00006540: 735f 7a65 726f 735d 2e69 6e64 6578 2e74  s_zeros].index.t
-00006550: 6f5f 6c69 7374 2829 290d 0a20 2020 2020  o_list())..     
-00006560: 2020 2020 2020 2073 656c 662e 6170 7065         self.appe
-00006570: 6e64 5f74 6f5f 6869 7374 6f72 7928 6622  nd_to_history(f"
-00006580: 5265 6d6f 7669 6e67 206f 6273 6572 7661  Removing observa
-00006590: 7469 6f6e 7320 7769 7468 206f 6e6c 7920  tions with only 
-000065a0: 7a65 726f 733a 207b 6d73 675f 7374 7269  zeros: {msg_stri
-000065b0: 6e67 7d22 290d 0a20 2020 2020 2020 200d  ng}")..        .
-000065c0: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-000065d0: 6174 6120 3d20 7365 6c66 2e61 6461 7461  ata = self.adata
-000065e0: 5b7e 6f62 735f 7a65 726f 732c 3a5d 2e63  [~obs_zeros,:].c
-000065f0: 6f70 7928 290d 0a0d 0a0d 0a20 2020 2064  opy()......    d
-00006600: 6566 2072 656d 6f76 655f 756e 6661 6374  ef remove_unfact
-00006610: 6f72 697a 6162 6c65 5f66 6561 7475 7265  orizable_feature
-00006620: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
-00006630: 2020 2222 2252 656d 6f76 6573 2066 6561    """Removes fea
-00006640: 7475 7265 7320 7769 7468 206d 6973 7369  tures with missi
-00006650: 6e67 2076 616c 7565 7320 6f72 207a 6572  ng values or zer
-00006660: 6f20 7661 7269 616e 6365 2066 726f 6d20  o variance from 
-00006670: 7468 6520 6461 7461 206d 6174 7269 782e  the data matrix.
-00006680: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00006690: 2020 2020 2020 2064 6620 3d20 7365 6c66         df = self
-000066a0: 2e74 6f5f 6466 286e 6f72 6d61 6c69 7a65  .to_df(normalize
-000066b0: 643d 4661 6c73 6529 0d0a 2020 2020 2020  d=False)..      
-000066c0: 2020 2320 4368 6563 6b20 666f 7220 6665    # Check for fe
-000066d0: 6174 7572 6573 2077 6974 6820 6d69 7373  atures with miss
-000066e0: 696e 6720 7661 6c75 6573 0d0a 2020 2020  ing values..    
-000066f0: 2020 2020 6765 6e65 735f 7769 7468 5f6d      genes_with_m
-00006700: 6973 7369 6e67 7661 6c75 6573 203d 2064  issingvalues = d
-00006710: 662e 6973 6e75 6c6c 2829 2e61 6e79 2829  f.isnull().any()
-00006720: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00006730: 2020 2020 6e5f 6d69 7373 696e 6720 3d20      n_missing = 
-00006740: 6765 6e65 735f 7769 7468 5f6d 6973 7369  genes_with_missi
-00006750: 6e67 7661 6c75 6573 2e73 756d 2829 0d0a  ngvalues.sum()..
-00006760: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-00006770: 696e 666f 2866 227b 6e5f 6d69 7373 696e  info(f"{n_missin
-00006780: 677d 206f 6620 7b73 656c 662e 6164 6174  g} of {self.adat
-00006790: 612e 6e5f 7661 7273 7d20 6665 6174 7572  a.n_vars} featur
-000067a0: 6573 2061 7265 206d 6973 7369 6e67 2076  es are missing v
-000067b0: 616c 7565 732e 2229 0d0a 2020 2020 2020  alues.")..      
-000067c0: 2020 6966 206e 5f6d 6973 7369 6e67 3a0d    if n_missing:.
-000067d0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-000067e0: 6769 6e67 2e77 6172 6e69 6e67 2866 2253  ging.warning(f"S
-000067f0: 7562 7365 7474 696e 6720 6665 6174 7572  ubsetting featur
-00006800: 6573 2074 6f20 7468 6f73 6520 7769 7468  es to those with
-00006810: 206e 6f20 6d69 7373 696e 6720 7661 6c75   no missing valu
-00006820: 6573 2e22 290d 0a20 2020 2020 2020 2020  es.")..         
-00006830: 2020 206d 7367 5f73 7472 696e 6720 3d20     msg_string = 
-00006840: 7265 7072 2867 656e 6573 5f77 6974 685f  repr(genes_with_
-00006850: 6d69 7373 696e 6776 616c 7565 735b 6765  missingvalues[ge
-00006860: 6e65 735f 7769 7468 5f6d 6973 7369 6e67  nes_with_missing
-00006870: 7661 6c75 6573 5d2e 696e 6465 782e 746f  values].index.to
-00006880: 5f6c 6973 7428 2929 0d0a 2020 2020 2020  _list())..      
-00006890: 2020 2020 2020 7365 6c66 2e61 7070 656e        self.appen
-000068a0: 645f 746f 5f68 6973 746f 7279 2866 2252  d_to_history(f"R
-000068b0: 656d 6f76 696e 6720 6665 6174 7572 6573  emoving features
-000068c0: 2077 6974 6820 6d69 7373 696e 6720 7661   with missing va
-000068d0: 6c75 6573 3a20 7b6d 7367 5f73 7472 696e  lues: {msg_strin
-000068e0: 677d 2229 0d0a 2020 2020 2020 2020 2320  g}")..        # 
-000068f0: 4368 6563 6b20 666f 7220 6765 6e65 7320  Check for genes 
-00006900: 7769 7468 207a 6572 6f20 7661 7269 616e  with zero varian
-00006910: 6365 0d0a 2020 2020 2020 2020 7a65 726f  ce..        zero
-00006920: 7661 7267 656e 6573 203d 2028 6466 2e76  vargenes = (df.v
-00006930: 6172 2829 203d 3d20 3029 0d0a 2020 2020  ar() == 0)..    
-00006940: 2020 2020 6e5f 7a65 726f 7661 7220 3d20      n_zerovar = 
-00006950: 7a65 726f 7661 7267 656e 6573 2e73 756d  zerovargenes.sum
-00006960: 2829 0d0a 2020 2020 2020 2020 6c6f 6767  ()..        logg
-00006970: 696e 672e 696e 666f 2866 227b 6e5f 7a65  ing.info(f"{n_ze
-00006980: 726f 7661 727d 206f 6620 7b73 656c 662e  rovar} of {self.
-00006990: 6164 6174 612e 6e5f 7661 7273 7d20 6665  adata.n_vars} fe
-000069a0: 6174 7572 6573 2068 6176 6520 6120 7661  atures have a va
-000069b0: 7269 616e 6365 206f 6620 7a65 726f 2e22  riance of zero."
-000069c0: 290d 0a20 2020 2020 2020 2069 6620 6e5f  )..        if n_
-000069d0: 7a65 726f 7661 723a 0d0a 2020 2020 2020  zerovar:..      
-000069e0: 2020 2020 2020 6c6f 6767 696e 672e 7761        logging.wa
-000069f0: 726e 696e 6728 6622 5375 6273 6574 7469  rning(f"Subsetti
-00006a00: 6e67 2066 6561 7475 7265 7320 746f 2074  ng features to t
-00006a10: 686f 7365 2077 6974 6820 6e6f 6e7a 6572  hose with nonzer
-00006a20: 6f20 7661 7269 616e 6365 2e22 290d 0a20  o variance.").. 
-00006a30: 2020 2020 2020 2020 2020 206d 7367 5f73             msg_s
-00006a40: 7472 696e 6720 3d20 7265 7072 287a 6572  tring = repr(zer
-00006a50: 6f76 6172 6765 6e65 735b 7a65 726f 7661  ovargenes[zerova
-00006a60: 7267 656e 6573 5d2e 696e 6465 782e 746f  rgenes].index.to
-00006a70: 5f6c 6973 7428 2929 0d0a 2020 2020 2020  _list())..      
-00006a80: 2020 2020 2020 7365 6c66 2e61 7070 656e        self.appen
-00006a90: 645f 746f 5f68 6973 746f 7279 2866 2252  d_to_history(f"R
-00006aa0: 656d 6f76 696e 6720 6665 6174 7572 6573  emoving features
-00006ab0: 2077 6974 6820 7a65 726f 2076 6172 6961   with zero varia
-00006ac0: 6e63 653a 207b 6d73 675f 7374 7269 6e67  nce: {msg_string
-00006ad0: 7d22 290d 0a20 2020 2020 2020 2067 656e  }")..        gen
-00006ae0: 6573 5f74 6f5f 6b65 6570 203d 2028 7e67  es_to_keep = (~g
-00006af0: 656e 6573 5f77 6974 685f 6d69 7373 696e  enes_with_missin
-00006b00: 6776 616c 7565 7329 2026 2028 7e7a 6572  gvalues) & (~zer
-00006b10: 6f76 6172 6765 6e65 7329 0d0a 2020 2020  ovargenes)..    
-00006b20: 2020 2020 7365 6c66 2e61 6461 7461 203d      self.adata =
-00006b30: 2073 656c 662e 6164 6174 615b 3a2c 6765   self.adata[:,ge
-00006b40: 6e65 735f 746f 5f6b 6565 705d 2e63 6f70  nes_to_keep].cop
-00006b50: 7928 290d 0a0d 0a20 2020 2064 6566 2063  y()....    def c
-00006b60: 726f 7373 5f76 616c 6964 6174 655f 696d  ross_validate_im
-00006b70: 7075 7461 7469 6f6e 2873 656c 662c 2069  putation(self, i
-00006b80: 6d70 7574 6572 3a20 556e 696f 6e5b 4b4e  mputer: Union[KN
-00006b90: 4e49 6d70 7574 6572 2c20 5369 6d70 6c65  NImputer, Simple
-00006ba0: 496d 7075 7465 725d 2c20 6e5f 666f 6c64  Imputer], n_fold
-00006bb0: 733a 2069 6e74 203d 2031 3030 293a 0d0a  s: int = 100):..
-00006bc0: 2020 2020 2020 2020 2222 2250 6572 666f          """Perfo
-00006bd0: 726d 206b 2d66 6f6c 6420 6372 6f73 7320  rm k-fold cross 
-00006be0: 7661 6c69 6461 7469 6f6e 206f 6620 696d  validation of im
-00006bf0: 7075 7461 7469 6f6e 206f 6e20 7468 6520  putation on the 
-00006c00: 6461 7461 7365 7420 7769 7468 6f75 7420  dataset without 
-00006c10: 6d6f 6469 6679 696e 6720 7468 6520 6461  modifying the da
-00006c20: 7461 2e0d 0a0d 0a20 2020 2020 2020 203a  ta.....        :
-00006c30: 7061 7261 6d20 696d 7075 7465 723a 2069  param imputer: i
-00006c40: 6d70 7574 6572 206f 626a 6563 7420 6672  mputer object fr
-00006c50: 6f6d 2073 6369 6b69 742d 6c65 6172 6e0d  om scikit-learn.
-00006c60: 0a20 2020 2020 2020 203a 7479 7065 2069  .        :type i
-00006c70: 6d70 7574 6572 3a20 556e 696f 6e5b 4b4e  mputer: Union[KN
-00006c80: 4e49 6d70 7574 6572 2c20 5369 6d70 6c65  NImputer, Simple
-00006c90: 496d 7075 7465 725d 0d0a 2020 2020 2020  Imputer]..      
-00006ca0: 2020 3a70 6172 616d 206e 5f66 6f6c 6473    :param n_folds
-00006cb0: 3a20 6e75 6d62 6572 206f 6620 666f 6c64  : number of fold
-00006cc0: 732c 2064 6566 6175 6c74 7320 746f 2031  s, defaults to 1
-00006cd0: 3030 0d0a 2020 2020 2020 2020 3a74 7970  00..        :typ
-00006ce0: 6520 6e5f 666f 6c64 733a 2069 6e74 2c20  e n_folds: int, 
-00006cf0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00006d00: 2020 3a72 6574 7572 6e3a 2044 6174 6166    :return: Dataf
-00006d10: 7261 6d20 7769 7468 2073 7461 7469 7374  ram with statist
-00006d20: 6963 7320 666f 7220 6561 6368 2067 656e  ics for each gen
-00006d30: 652c 2069 6e63 6c75 6469 6e67 2070 7265  e, including pre
-00006d40: 696d 7075 7461 7469 6f6e 206c 6f67 2d6d  imputation log-m
-00006d50: 6561 6e20 616e 6420 6c6f 672d 7661 7269  ean and log-vari
-00006d60: 616e 6365 2c20 616e 6420 4e52 4d53 4420  ance, and NRMSD 
-00006d70: 6d65 616e 2061 6e64 2076 6172 6961 6e63  mean and varianc
-00006d80: 6520 6163 726f 7373 2061 6c6c 2066 6f6c  e across all fol
-00006d90: 6473 2e0d 0a20 2020 2020 2020 203a 7274  ds...        :rt
-00006da0: 7970 653a 203a 636c 6173 733a 6070 616e  ype: :class:`pan
-00006db0: 6461 732e 4461 7461 4672 616d 6560 0d0a  das.DataFrame`..
-00006dc0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00006dd0: 2020 2020 206c 6f67 6769 6e67 2e69 6e66       logging.inf
-00006de0: 6f28 6622 5065 7266 6f72 6d69 6e67 206b  o(f"Performing k
-00006df0: 2d66 6f6c 6420 6372 6f73 732d 7661 6c69  -fold cross-vali
-00006e00: 6461 7469 6f6e 2c20 7769 7468 207b 6e5f  dation, with {n_
-00006e10: 666f 6c64 737d 2066 6f6c 6473 2229 0d0a  folds} folds")..
-00006e20: 2020 2020 2020 2020 2320 6b2d 666f 6c64          # k-fold
-00006e30: 2063 726f 7373 2d76 616c 6964 6174 696f   cross-validatio
-00006e40: 6e0d 0a20 2020 2020 2020 2072 6d73 645f  n..        rmsd_
-00006e50: 666f 6c64 7320 3d20 5b5d 2020 2023 2073  folds = []   # s
-00006e60: 746f 7265 2067 656e 652d 7769 7365 2072  tore gene-wise r
-00006e70: 6d73 640d 0a20 2020 2020 2020 2064 6174  msd..        dat
-00006e80: 6120 3d20 7365 6c66 2e61 6461 7461 2e74  a = self.adata.t
-00006e90: 6f5f 6466 2829 0d0a 2020 2020 2020 2020  o_df()..        
-00006ea0: 7261 6e64 6f6d 5f6e 756d 6265 7273 203d  random_numbers =
-00006eb0: 206e 702e 7261 6e64 6f6d 2e72 616e 646f   np.random.rando
-00006ec0: 6d28 6461 7461 2e73 6861 7065 2920 2023  m(data.shape)  #
-00006ed0: 2075 7365 6420 746f 2061 7373 6967 6e20   used to assign 
-00006ee0: 6561 6368 2064 6174 6120 706f 696e 7420  each data point 
-00006ef0: 746f 2061 2066 6f6c 640d 0a20 2020 2020  to a fold..     
-00006f00: 2020 2062 696e 7320 3d20 6e70 2e6c 696e     bins = np.lin
-00006f10: 7370 6163 6528 302c 2031 2c20 6e5f 666f  space(0, 1, n_fo
-00006f20: 6c64 7320 2b20 3129 0d0a 2020 2020 2020  lds + 1)..      
-00006f30: 2020 666f 7220 666f 6c64 2069 6e20 7471    for fold in tq
-00006f40: 646d 2872 616e 6765 286e 5f66 6f6c 6473  dm(range(n_folds
-00006f50: 292c 2075 6e69 743d 2266 6f6c 6422 293a  ), unit="fold"):
-00006f60: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
-00006f70: 7765 722c 2075 7070 6572 203d 2062 696e  wer, upper = bin
-00006f80: 735b 666f 6c64 3a66 6f6c 6420 2b20 325d  s[fold:fold + 2]
-00006f90: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
-00006fa0: 736b 203d 2028 7261 6e64 6f6d 5f6e 756d  sk = (random_num
-00006fb0: 6265 7273 203e 3d20 6c6f 7765 7229 2026  bers >= lower) &
-00006fc0: 2028 7261 6e64 6f6d 5f6e 756d 6265 7273   (random_numbers
-00006fd0: 203c 2075 7070 6572 290d 0a20 2020 2020   < upper)..     
-00006fe0: 2020 2020 2020 2074 6573 7420 3d20 6461         test = da
-00006ff0: 7461 2e6d 6173 6b28 7e6d 6173 6b29 0d0a  ta.mask(~mask)..
-00007000: 2020 2020 2020 2020 2020 2020 7472 6169              trai
-00007010: 6e69 6e67 203d 2064 6174 612e 6d61 736b  ning = data.mask
-00007020: 286d 6173 6b29 0d0a 2020 2020 2020 2020  (mask)..        
-00007030: 2020 2020 696d 7075 7465 6420 3d20 696d      imputed = im
-00007040: 7075 7465 722e 6669 745f 7472 616e 7366  puter.fit_transf
-00007050: 6f72 6d28 7472 6169 6e69 6e67 290d 0a20  orm(training).. 
-00007060: 2020 2020 2020 2020 2020 2069 6d70 7574             imput
-00007070: 6564 203d 2070 642e 4461 7461 4672 616d  ed = pd.DataFram
-00007080: 6528 696d 7075 7465 642c 2069 6e64 6578  e(imputed, index
-00007090: 3d64 6174 612e 696e 6465 782c 2063 6f6c  =data.index, col
-000070a0: 756d 6e73 3d64 6174 612e 636f 6c75 6d6e  umns=data.column
-000070b0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-000070c0: 7265 7369 6420 3d20 2869 6d70 7574 6564  resid = (imputed
-000070d0: 202d 2074 6573 7429 0d0a 2020 2020 2020   - test)..      
-000070e0: 2020 2020 2020 726d 7364 203d 206e 702e        rmsd = np.
-000070f0: 7371 7274 2828 7265 7369 6420 2a2a 2032  sqrt((resid ** 2
-00007100: 292e 7375 6d28 2920 2f20 7265 7369 642e  ).sum() / resid.
-00007110: 6e6f 746e 756c 6c28 292e 7375 6d28 2929  notnull().sum())
-00007120: 0d0a 2020 2020 2020 2020 2020 2020 726d  ..            rm
-00007130: 7364 5f66 6f6c 6473 2e61 7070 656e 6428  sd_folds.append(
-00007140: 726d 7364 290d 0a20 2020 2020 2020 2072  rmsd)..        r
-00007150: 6d73 645f 666f 6c64 7320 3d20 7064 2e63  msd_folds = pd.c
-00007160: 6f6e 6361 7428 726d 7364 5f66 6f6c 6473  oncat(rmsd_folds
-00007170: 2c20 6178 6973 3d31 290d 0a20 2020 2020  , axis=1)..     
-00007180: 2020 206e 726d 7364 5f66 6f6c 6473 203d     nrmsd_folds =
-00007190: 2072 6d73 645f 666f 6c64 732e 6469 7628   rmsd_folds.div(
-000071a0: 6461 7461 2e6d 6561 6e28 292c 2061 7869  data.mean(), axi
-000071b0: 733d 3029 0d0a 2020 2020 2020 2020 0d0a  s=0)..        ..
-000071c0: 2020 2020 2020 2020 2320 7265 636f 7264          # record
-000071d0: 2073 7461 7473 2069 6e20 6164 6174 612e   stats in adata.
-000071e0: 7661 720d 0a20 2020 2020 2020 2063 7673  var..        cvs
-000071f0: 7461 7473 203d 2070 642e 4461 7461 4672  tats = pd.DataFr
-00007200: 616d 6528 7b0d 0a20 2020 2020 2020 2020  ame({..         
-00007210: 2020 2022 6c6f 675f 6d65 616e 5f70 7265     "log_mean_pre
-00007220: 696d 7075 7461 7469 6f6e 223a 206e 702e  imputation": np.
-00007230: 6c6f 6731 3028 6461 7461 2e6d 6561 6e28  log10(data.mean(
-00007240: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-00007250: 2022 6c6f 675f 7661 7269 616e 6365 5f70   "log_variance_p
-00007260: 7265 696d 7075 7461 7469 6f6e 223a 206e  reimputation": n
-00007270: 702e 6c6f 6731 3028 6461 7461 2e76 6172  p.log10(data.var
-00007280: 2829 292c 0d0a 2020 2020 2020 2020 2020  ()),..          
-00007290: 2020 2269 6d70 7574 6174 696f 6e5f 6e72    "imputation_nr
-000072a0: 6d73 645f 6d65 616e 223a 206e 726d 7364  msd_mean": nrmsd
-000072b0: 5f66 6f6c 6473 2e6d 6561 6e28 6178 6973  _folds.mean(axis
-000072c0: 3d31 292c 0d0a 2020 2020 2020 2020 2020  =1),..          
-000072d0: 2020 2269 6d70 7574 6174 696f 6e5f 6e72    "imputation_nr
-000072e0: 6d73 645f 7661 7222 3a20 6e72 6d73 645f  msd_var": nrmsd_
-000072f0: 666f 6c64 732e 6d65 616e 2861 7869 733d  folds.mean(axis=
-00007300: 3129 0d0a 2020 2020 2020 2020 7d29 0d0a  1)..        })..
-00007310: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00007320: 2063 7673 7461 7473 0d0a 0d0a 2020 2020   cvstats....    
-00007330: 6465 6620 696d 7075 7465 5f6b 6e6e 2873  def impute_knn(s
-00007340: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
-00007350: 2020 2020 2020 2020 206e 5f6e 6569 6768           n_neigh
-00007360: 626f 7273 3a20 696e 7420 3d20 352c 0d0a  bors: int = 5,..
-00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007380: 2020 2077 6569 6768 7473 3a20 4c69 7465     weights: Lite
-00007390: 7261 6c5b 2264 6973 7461 6e63 6522 2c20  ral["distance", 
-000073a0: 2275 6e69 666f 726d 225d 203d 2022 6469  "uniform"] = "di
-000073b0: 7374 616e 6365 222c 0d0a 2020 2020 2020  stance",..      
-000073c0: 2020 2020 2020 2020 2020 2020 2063 726f               cro
-000073d0: 7373 5f76 616c 6964 6174 653a 2062 6f6f  ss_validate: boo
-000073e0: 6c20 3d20 5472 7565 2c0d 0a20 2020 2020  l = True,..     
-000073f0: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
-00007400: 666f 6c64 733a 2069 6e74 203d 2031 3030  folds: int = 100
-00007410: 293a 0d0a 2020 2020 2020 2020 0d0a 2020  ):..        ..  
-00007420: 2020 2020 2020 2222 2249 6d70 7574 6174        """Imputat
-00007430: 696f 6e20 666f 7220 636f 6d70 6c65 7469  ion for completi
-00007440: 6e67 206d 6973 7369 6e67 2076 616c 7565  ng missing value
-00007450: 7320 7573 696e 6720 6b2d 4e65 6172 6573  s using k-Neares
-00007460: 7420 4e65 6967 6862 6f72 732e 0d0a 2020  t Neighbors...  
-00007470: 2020 2020 2020 2020 2045 6163 6820 7361           Each sa
-00007480: 6d70 6c65 2773 206d 6973 7369 6e67 2076  mple's missing v
-00007490: 616c 7565 7320 6172 6520 696d 7075 7465  alues are impute
-000074a0: 6420 7573 696e 6720 7468 6520 6d65 616e  d using the mean
-000074b0: 2076 616c 7565 2066 726f 6d0d 0a20 2020   value from..   
-000074c0: 2020 2020 2020 2020 606e 5f6e 6569 6768          `n_neigh
-000074d0: 626f 7273 6020 6e65 6172 6573 7420 6e65  bors` nearest ne
-000074e0: 6967 6862 6f72 732e 2054 776f 2073 616d  ighbors. Two sam
-000074f0: 706c 6573 2061 7265 0d0a 2020 2020 2020  ples are..      
-00007500: 2020 2020 2063 6c6f 7365 2069 6620 7468       close if th
-00007510: 6520 6665 6174 7572 6573 2074 6861 7420  e features that 
-00007520: 6e65 6974 6865 7220 6973 206d 6973 7369  neither is missi
-00007530: 6e67 2061 7265 2063 6c6f 7365 2e20 0d0a  ng are close. ..
-00007540: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00007550: 206e 5f6e 6569 6768 626f 7273 3a20 4e75   n_neighbors: Nu
-00007560: 6d62 6572 206f 6620 6e65 6967 6862 6f72  mber of neighbor
-00007570: 696e 6720 7361 6d70 6c65 7320 746f 2075  ing samples to u
-00007580: 7365 2066 6f72 2069 6d70 7574 6174 696f  se for imputatio
-00007590: 6e2c 2064 6566 6175 6c74 7320 746f 2035  n, defaults to 5
-000075a0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-000075b0: 6e5f 6e65 6967 6862 6f72 733a 2069 6e74  n_neighbors: int
-000075c0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-000075d0: 2020 2020 3a70 6172 616d 2077 6569 6768      :param weigh
-000075e0: 7473 3a20 5765 6967 6874 2066 756e 6374  ts: Weight funct
-000075f0: 696f 6e20 7573 6564 2069 6e20 7072 6564  ion used in pred
-00007600: 6963 7469 6f6e 2c20 6465 6661 756c 7473  iction, defaults
-00007610: 2074 6f20 2764 6973 7461 6e63 6527 2e20   to 'distance'. 
-00007620: 506f 7373 6962 6c65 2076 616c 7565 733a  Possible values:
-00007630: 0d0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
-00007640: 2775 6e69 666f 726d 2720 3a20 756e 6966  'uniform' : unif
-00007650: 6f72 6d20 7765 6967 6874 732e 2041 6c6c  orm weights. All
-00007660: 2070 6f69 6e74 7320 696e 2065 6163 6820   points in each 
-00007670: 6e65 6967 6862 6f72 686f 6f64 2061 7265  neighborhood are
-00007680: 0d0a 2020 2020 2020 2020 2020 2020 7765  ..            we
-00007690: 6967 6874 6564 2065 7175 616c 6c79 2e0d  ighted equally..
-000076a0: 0a20 2020 2020 2020 2020 2020 202d 2027  .            - '
-000076b0: 6469 7374 616e 6365 2720 3a20 7765 6967  distance' : weig
-000076c0: 6874 2070 6f69 6e74 7320 6279 2074 6865  ht points by the
-000076d0: 2069 6e76 6572 7365 206f 6620 7468 6569   inverse of thei
-000076e0: 7220 6469 7374 616e 6365 2e0d 0a20 2020  r distance...   
-000076f0: 2020 2020 2020 2020 2069 6e20 7468 6973           in this
-00007700: 2063 6173 652c 2063 6c6f 7365 7220 6e65   case, closer ne
-00007710: 6967 6862 6f72 7320 6f66 2061 2071 7565  ighbors of a que
-00007720: 7279 2070 6f69 6e74 2077 696c 6c20 6861  ry point will ha
-00007730: 7665 2061 0d0a 2020 2020 2020 2020 2020  ve a..          
-00007740: 2020 6772 6561 7465 7220 696e 666c 7565    greater influe
-00007750: 6e63 6520 7468 616e 206e 6569 6768 626f  nce than neighbo
-00007760: 7273 2077 6869 6368 2061 7265 2066 7572  rs which are fur
-00007770: 7468 6572 2061 7761 792e 0d0a 2020 2020  ther away...    
-00007780: 2020 2020 3a74 7970 6520 7765 6967 6874      :type weight
-00007790: 733a 204c 6974 6572 616c 5b22 6469 7374  s: Literal["dist
-000077a0: 616e 6365 222c 2022 756e 6966 6f72 6d22  ance", "uniform"
-000077b0: 5d2c 206f 7074 696f 6e61 6c0d 0a20 2020  ], optional..   
-000077c0: 2020 2020 203a 7061 7261 6d20 6372 6f73       :param cros
-000077d0: 735f 7661 6c69 6461 7465 3a20 7065 7266  s_validate: perf
-000077e0: 6f72 6d20 6b2d 666f 6c64 2063 726f 7373  orm k-fold cross
-000077f0: 2d76 616c 6964 6174 696f 6e2c 2064 6566  -validation, def
-00007800: 6175 6c74 7320 746f 2054 7275 650d 0a20  aults to True.. 
-00007810: 2020 2020 2020 203a 7479 7065 2063 726f         :type cro
-00007820: 7373 5f76 616c 6964 6174 653a 2062 6f6f  ss_validate: boo
-00007830: 6c2c 206f 7074 696f 6e61 6c0d 0a20 2020  l, optional..   
-00007840: 2020 2020 203a 7061 7261 6d20 6e5f 666f       :param n_fo
-00007850: 6c64 733a 206e 756d 6265 7220 6f66 2066  lds: number of f
-00007860: 6f6c 6473 2066 6f72 206b 2d66 6f6c 6420  olds for k-fold 
-00007870: 6372 6f73 732d 7661 6c69 6461 7469 6f6e  cross-validation
-00007880: 2c20 6465 6661 756c 7473 2074 6f20 3130  , defaults to 10
-00007890: 300d 0a20 2020 2020 2020 203a 7479 7065  0..        :type
-000078a0: 206e 5f66 6f6c 6473 3a20 696e 742c 206f   n_folds: int, o
-000078b0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-000078c0: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-000078d0: 6c6f 6767 696e 672e 696e 666f 2866 2249  logging.info(f"I
-000078e0: 6d70 7574 696e 6720 6461 7461 2077 6974  mputing data wit
-000078f0: 6820 6b2d 4e65 6172 6573 7420 4e65 6967  h k-Nearest Neig
-00007900: 6862 6f72 732c 206b 3d7b 6e5f 6e65 6967  hbors, k={n_neig
-00007910: 6862 6f72 737d 2c20 7b77 6569 6768 7473  hbors}, {weights
-00007920: 7d20 7765 6967 6874 7322 290d 0a0d 0a20  } weights").... 
-00007930: 2020 2020 2020 2069 6d70 7574 6572 203d         imputer =
-00007940: 204b 4e4e 496d 7075 7465 7228 6e5f 6e65   KNNImputer(n_ne
-00007950: 6967 6862 6f72 733d 6e5f 6e65 6967 6862  ighbors=n_neighb
-00007960: 6f72 732c 2077 6569 6768 7473 3d77 6569  ors, weights=wei
-00007970: 6768 7473 2c20 6b65 6570 5f65 6d70 7479  ghts, keep_empty
-00007980: 5f66 6561 7475 7265 733d 5472 7565 290d  _features=True).
-00007990: 0a20 2020 2020 2020 2069 6620 6e5f 666f  .        if n_fo
-000079a0: 6c64 7320 3c20 323a 0d0a 2020 2020 2020  lds < 2:..      
-000079b0: 2020 2020 2020 6c6f 6767 696e 672e 7761        logging.wa
-000079c0: 726e 696e 6728 6622 6e5f 666f 6c64 7320  rning(f"n_folds 
-000079d0: 3d20 7b6e 5f66 6f6c 6473 7d20 6973 206c  = {n_folds} is l
-000079e0: 6573 7320 7468 616e 2032 2e20 536b 6970  ess than 2. Skip
-000079f0: 7069 6e67 2063 726f 7373 2d76 616c 6964  ping cross-valid
-00007a00: 6174 696f 6e2e 2229 0d0a 2020 2020 2020  ation.")..      
-00007a10: 2020 2020 2020 6372 6f73 735f 7661 6c69        cross_vali
-00007a20: 6461 7465 203d 2046 616c 7365 0d0a 2020  date = False..  
-00007a30: 2020 2020 2020 6966 2063 726f 7373 5f76        if cross_v
-00007a40: 616c 6964 6174 653a 0d0a 2020 2020 2020  alidate:..      
-00007a50: 2020 2020 2020 6376 7374 6174 7320 3d20        cvstats = 
-00007a60: 7365 6c66 2e63 726f 7373 5f76 616c 6964  self.cross_valid
-00007a70: 6174 655f 696d 7075 7461 7469 6f6e 2869  ate_imputation(i
-00007a80: 6d70 7574 6572 3d69 6d70 7574 6572 2c20  mputer=imputer, 
-00007a90: 6e5f 666f 6c64 733d 6e5f 666f 6c64 7329  n_folds=n_folds)
-00007aa0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00007ab0: 6c66 2e61 6461 7461 2e76 6172 203d 2073  lf.adata.var = s
-00007ac0: 656c 662e 6164 6174 612e 7661 722e 6a6f  elf.adata.var.jo
-00007ad0: 696e 2863 7673 7461 7473 2c20 7661 6c69  in(cvstats, vali
-00007ae0: 6461 7465 3d22 313a 3122 290d 0a20 2020  date="1:1")..   
-00007af0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00007b00: 2020 2073 656c 662e 6164 6174 612e 5820     self.adata.X 
-00007b10: 3d20 696d 7075 7465 722e 6669 745f 7472  = imputer.fit_tr
-00007b20: 616e 7366 6f72 6d28 7365 6c66 2e61 6461  ansform(self.ada
-00007b30: 7461 2e58 290d 0a20 2020 2020 2020 2073  ta.X)..        s
-00007b40: 656c 662e 6170 7065 6e64 5f74 6f5f 6869  elf.append_to_hi
-00007b50: 7374 6f72 7928 6622 4b4e 4e20 496d 7075  story(f"KNN Impu
-00007b60: 7461 7469 6f6e 3a20 6e5f 6e65 6967 6862  tation: n_neighb
-00007b70: 6f72 7320 3d20 7b6e 5f6e 6569 6768 626f  ors = {n_neighbo
-00007b80: 7273 7d2c 2077 6569 6768 7473 203d 207b  rs}, weights = {
-00007b90: 7765 6967 6874 737d 2229 0d0a 2020 2020  weights}")..    
-00007ba0: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
-00007bb0: 6e73 5b22 696d 7075 7461 7469 6f6e 225d  ns["imputation"]
-00007bc0: 203d 207b 226d 6574 686f 6422 3a20 226b   = {"method": "k
-00007bd0: 6e6e 222c 0d0a 2020 2020 2020 2020 2020  nn",..          
+000057c0: 2020 2020 2020 6622 6f6e 655f 746f 5f6f        f"one_to_o
+000057d0: 6e65 3d7b 6f6e 655f 746f 5f6f 6e65 7d2c  ne={one_to_one},
+000057e0: 206f 6e65 5f74 6f5f 6d61 6e79 3d7b 6f6e   one_to_many={on
+000057f0: 655f 746f 5f6d 616e 797d 2c20 6d61 6e79  e_to_many}, many
+00005800: 5f74 6f5f 6f6e 653d 7b6d 616e 795f 746f  _to_one={many_to
+00005810: 5f6f 6e65 7d2c 206d 616e 795f 746f 5f6d  _one}, many_to_m
+00005820: 616e 793d 7b6d 616e 795f 746f 5f6d 616e  any={many_to_man
+00005830: 797d 2c20 756e 6d61 7070 6564 5f70 7265  y}, unmapped_pre
+00005840: 6669 783d 7b75 6e6d 6170 7065 645f 7072  fix={unmapped_pr
+00005850: 6566 6978 7d22 290d 0a0d 0a20 2020 2064  efix}")....    d
+00005860: 6566 2075 7064 6174 655f 6f62 7328 7365  ef update_obs(se
+00005870: 6c66 2c20 6f62 7329 3a0d 0a20 2020 2020  lf, obs):..     
+00005880: 2020 2022 2222 5570 6461 7465 2074 6865     """Update the
+00005890: 206f 6273 6572 7661 7469 6f6e 206d 6574   observation met
+000058a0: 6164 6174 6120 7769 7468 2061 206e 6577  adata with a new
+000058b0: 206d 6574 6164 6174 6120 6d61 7472 6978   metadata matrix
+000058c0: 0d0a 0d0a 2020 2020 2020 2020 3a70 6172  ....        :par
+000058d0: 616d 206f 6273 3a20 416e 206f 6273 6572  am obs: An obser
+000058e0: 7661 7469 6f6e 7320 c397 206d 6574 6164  vations .. metad
+000058f0: 6174 6120 6d61 7472 6978 2c20 6465 6661  ata matrix, defa
+00005900: 756c 7473 2074 6f20 4e6f 6e65 0d0a 2020  ults to None..  
+00005910: 2020 2020 2020 3a74 7970 6520 6f62 733a        :type obs:
+00005920: 2060 7064 2e44 6174 6146 7261 6d65 602c   `pd.DataFrame`,
+00005930: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00005940: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00005950: 2320 636f 6e76 6572 7420 276f 626a 6563  # convert 'objec
+00005960: 7427 2064 7479 7065 2074 6f20 6361 7465  t' dtype to cate
+00005970: 676f 7269 6361 6c2c 2063 6f6e 7665 7274  gorical, convert
+00005980: 696e 6720 626f 6f6c 2076 616c 7565 7320  ing bool values 
+00005990: 746f 2073 7472 696e 6773 2061 7320 7468  to strings as th
+000059a0: 6573 6520 6172 6520 6e6f 7420 7375 7070  ese are not supp
+000059b0: 6f72 7465 6420 6279 2041 6e6e 4461 7461  orted by AnnData
+000059c0: 206f 6e2d 6469 736b 2066 6f72 6d61 740d   on-disk format.
+000059d0: 0a20 2020 2020 2020 2066 6f72 2063 6f6c  .        for col
+000059e0: 2069 6e20 6f62 732e 7365 6c65 6374 5f64   in obs.select_d
+000059f0: 7479 7065 7328 696e 636c 7564 653d 2822  types(include=("
+00005a00: 626f 6f6c 222c 2022 6f62 6a65 6374 2229  bool", "object")
+00005a10: 292e 636f 6c75 6d6e 733a 0d0a 2020 2020  ).columns:..    
+00005a20: 2020 2020 2020 2020 6f62 735b 636f 6c5d          obs[col]
+00005a30: 203d 206f 6273 5b63 6f6c 5d2e 6173 7479   = obs[col].asty
+00005a40: 7065 2822 7374 7222 292e 6173 7479 7065  pe("str").astype
+00005a50: 2822 6361 7465 676f 7279 2229 0d0a 2020  ("category")..  
+00005a60: 2020 2020 2020 6d69 7373 696e 675f 7361        missing_sa
+00005a70: 6d70 6c65 735f 696e 5f58 203d 206f 6273  mples_in_X = obs
+00005a80: 2e69 6e64 6578 2e64 6966 6665 7265 6e63  .index.differenc
+00005a90: 6528 7365 6c66 2e61 6461 7461 2e6f 6273  e(self.adata.obs
+00005aa0: 2e69 6e64 6578 292e 6173 7479 7065 2873  .index).astype(s
+00005ab0: 7472 292e 746f 5f6c 6973 7428 290d 0a20  tr).to_list().. 
+00005ac0: 2020 2020 2020 2069 6620 6d69 7373 696e         if missin
+00005ad0: 675f 7361 6d70 6c65 735f 696e 5f58 3a0d  g_samples_in_X:.
+00005ae0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00005af0: 6769 6e67 2e77 6172 6e69 6e67 2822 5468  ging.warning("Th
+00005b00: 6520 666f 6c6c 6f77 696e 6720 7361 6d70  e following samp
+00005b10: 6c65 7320 696e 2074 6865 206d 6574 6164  les in the metad
+00005b20: 6174 6120 7765 7265 206e 6f74 2070 7265  ata were not pre
+00005b30: 7365 6e74 2069 6e20 7468 6520 6461 7461  sent in the data
+00005b40: 2028 6061 6461 7461 2e58 6029 3a5c 6e20   (`adata.X`):\n 
+00005b50: 202d 2022 202b 2022 5c6e 2020 2d20 222e   - " + "\n  - ".
+00005b60: 6a6f 696e 286d 6973 7369 6e67 5f73 616d  join(missing_sam
+00005b70: 706c 6573 5f69 6e5f 5829 290d 0a20 2020  ples_in_X))..   
+00005b80: 2020 2020 206d 6973 7369 6e67 5f73 616d       missing_sam
+00005b90: 706c 6573 5f69 6e5f 6d64 203d 2073 656c  ples_in_md = sel
+00005ba0: 662e 6164 6174 612e 6f62 732e 696e 6465  f.adata.obs.inde
+00005bb0: 782e 6469 6666 6572 656e 6365 286f 6273  x.difference(obs
+00005bc0: 2e69 6e64 6578 292e 6173 7479 7065 2873  .index).astype(s
+00005bd0: 7472 292e 746f 5f6c 6973 7428 290d 0a20  tr).to_list().. 
+00005be0: 2020 2020 2020 2069 6620 6d69 7373 696e         if missin
+00005bf0: 675f 7361 6d70 6c65 735f 696e 5f6d 643a  g_samples_in_md:
+00005c00: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00005c10: 6767 696e 672e 7761 726e 696e 6728 2254  gging.warning("T
+00005c20: 6865 2066 6f6c 6c6f 7769 6e67 2073 616d  he following sam
+00005c30: 706c 6573 2069 6e20 7468 6520 6461 7461  ples in the data
+00005c40: 2028 6061 6461 7461 2e58 6029 2077 6572   (`adata.X`) wer
+00005c50: 6520 6162 7365 6e74 2069 6e20 7468 6520  e absent in the 
+00005c60: 6d65 7461 6461 7461 3a5c 6e20 202d 2022  metadata:\n  - "
+00005c70: 202b 2022 5c6e 2020 2d20 222e 6a6f 696e   + "\n  - ".join
+00005c80: 286d 6973 7369 6e67 5f73 616d 706c 6573  (missing_samples
+00005c90: 5f69 6e5f 6d64 2929 0d0a 2020 2020 2020  _in_md))..      
+00005ca0: 2020 7365 6c66 2e61 6461 7461 2e6f 6273    self.adata.obs
+00005cb0: 203d 206f 6273 2e72 6569 6e64 6578 2873   = obs.reindex(s
+00005cc0: 656c 662e 6164 6174 612e 6f62 732e 696e  elf.adata.obs.in
+00005cd0: 6465 7829 0d0a 2020 2020 2020 2020 7365  dex)..        se
+00005ce0: 6c66 2e61 7070 656e 645f 746f 5f68 6973  lf.append_to_his
+00005cf0: 746f 7279 2866 226d 6574 6164 6174 6120  tory(f"metadata 
+00005d00: 2861 6461 7461 2e6f 6273 2920 7570 6461  (adata.obs) upda
+00005d10: 7465 642e 2229 0d0a 2020 2020 0d0a 2020  ted.")..    ..  
+00005d20: 2020 6465 6620 6765 745f 7072 696e 7461    def get_printa
+00005d30: 626c 655f 6d65 7461 6461 7461 5f74 7970  ble_metadata_typ
+00005d40: 655f 7375 6d6d 6172 7928 7365 6c66 293a  e_summary(self):
+00005d50: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
+00005d60: 7572 6e20 6120 7072 696e 7461 626c 6520  urn a printable 
+00005d70: 7375 6d6d 6172 7920 6f66 206d 6574 6164  summary of metad
+00005d80: 6174 6120 616e 6420 7468 6520 7479 7065  ata and the type
+00005d90: 732e 0d0a 0d0a 2020 2020 2020 2020 3a72  s.....        :r
+00005da0: 6574 7572 6e3a 2053 756d 6d61 7279 206f  eturn: Summary o
+00005db0: 6620 6d65 7461 6461 7461 0d0a 2020 2020  f metadata..    
+00005dc0: 2020 2020 3a72 7479 7065 3a20 7374 720d      :rtype: str.
+00005dd0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00005de0: 2020 2020 2020 6d73 6720 3d20 2253 756d        msg = "Sum
+00005df0: 6d61 7279 206f 6620 6d65 7461 6461 7461  mary of metadata
+00005e00: 2074 7970 6573 5c6e 5c6e 2020 2020 5361   types\n\n    Sa
+00005e10: 6d70 6c65 206d 6574 6164 6174 613a 5c6e  mple metadata:\n
+00005e20: 220d 0a20 2020 2020 2020 2066 6f72 2063  "..        for c
+00005e30: 6f6c 2069 6e20 7365 6c66 2e61 6461 7461  ol in self.adata
+00005e40: 2e6f 6273 2e63 6f6c 756d 6e73 3a0d 0a20  .obs.columns:.. 
+00005e50: 2020 2020 2020 2020 2020 206d 7367 202b             msg +
+00005e60: 3d20 2220 2020 2020 2020 2022 202b 2063  = "        " + c
+00005e70: 6f6c 202b 2022 3a20 2220 2b20 7365 6c66  ol + ": " + self
+00005e80: 2e61 6461 7461 2e6f 6273 5b63 6f6c 5d2e  .adata.obs[col].
+00005e90: 6474 7970 652e 6e61 6d65 202b 2022 5c6e  dtype.name + "\n
+00005ea0: 220d 0a20 2020 2020 2020 206d 7367 202b  "..        msg +
+00005eb0: 3d20 2220 2020 2046 6561 7475 7265 206d  = "    Feature m
+00005ec0: 6574 6164 6174 613a 5c6e 220d 0a20 2020  etadata:\n"..   
+00005ed0: 2020 2020 2066 6f72 2063 6f6c 2069 6e20       for col in 
+00005ee0: 7365 6c66 2e61 6461 7461 2e76 6172 2e63  self.adata.var.c
+00005ef0: 6f6c 756d 6e73 3a0d 0a20 2020 2020 2020  olumns:..       
+00005f00: 2020 2020 206d 7367 202b 3d20 2220 2020       msg += "   
+00005f10: 2020 2020 2022 202b 2063 6f6c 202b 2022       " + col + "
+00005f20: 3a20 2220 2b20 7365 6c66 2e61 6461 7461  : " + self.adata
+00005f30: 2e76 6172 5b63 6f6c 5d2e 6474 7970 652e  .var[col].dtype.
+00005f40: 6e61 6d65 202b 2022 5c6e 220d 0a20 2020  name + "\n"..   
+00005f50: 2020 2020 2072 6574 7572 6e20 6d73 670d       return msg.
+00005f60: 0a20 2020 200d 0a20 2020 2064 6566 2077  .    ..    def w
+00005f70: 7269 7465 5f68 3561 6428 7365 6c66 2c0d  rite_h5ad(self,.
+00005f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005f90: 2020 2020 6669 6c65 6e61 6d65 3a20 7374      filename: st
+00005fa0: 7229 3a0d 0a20 2020 2020 2020 2022 2222  r):..        """
+00005fb0: 5772 6974 6520 6461 7461 7365 7420 746f  Write dataset to
+00005fc0: 202e 6835 6164 2066 696c 652e 0d0a 0d0a   .h5ad file.....
+00005fd0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
+00005fe0: 696c 656e 616d 653a 2066 696c 6570 6174  ilename: filepat
+00005ff0: 680d 0a20 2020 2020 2020 203a 7479 7065  h..        :type
+00006000: 2066 696c 656e 616d 653a 2073 7472 0d0a   filename: str..
+00006010: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00006020: 2020 2020 2066 696c 656e 616d 6520 3d20       filename = 
+00006030: 6f73 2e70 6174 682e 6162 7370 6174 6828  os.path.abspath(
+00006040: 6669 6c65 6e61 6d65 290d 0a20 2020 2020  filename)..     
+00006050: 2020 206c 6f67 6769 6e67 2e69 6e66 6f28     logging.info(
+00006060: 6622 5772 6974 696e 6720 746f 207b 6669  f"Writing to {fi
+00006070: 6c65 6e61 6d65 7d22 290d 0a20 2020 2020  lename}")..     
+00006080: 2020 2073 656c 662e 6170 7065 6e64 5f74     self.append_t
+00006090: 6f5f 6869 7374 6f72 7928 2257 7269 7469  o_history("Writi
+000060a0: 6e67 2074 6f20 7b66 696c 656e 616d 657d  ng to {filename}
+000060b0: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+000060c0: 2e61 6461 7461 2e77 7269 7465 5f68 3561  .adata.write_h5a
+000060d0: 6428 6669 6c65 6e61 6d65 290d 0a20 2020  d(filename)..   
+000060e0: 2020 2020 206c 6f67 6769 6e67 2e69 6e66       logging.inf
+000060f0: 6f28 6622 5772 6974 6520 636f 6d70 6c65  o(f"Write comple
+00006100: 7465 642e 2229 0d0a 2020 2020 0d0a 2020  ted.")..    ..  
+00006110: 2020 6465 6620 746f 5f64 6628 7365 6c66    def to_df(self
+00006120: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00006130: 206e 6f72 6d61 6c69 7a65 643a 2062 6f6f   normalized: boo
+00006140: 6c20 3d20 4661 6c73 6529 3a0d 0a20 2020  l = False):..   
+00006150: 2020 2020 2022 2222 4765 7420 6461 7461       """Get data
+00006160: 206d 6174 7269 7820 6173 2061 2060 7064   matrix as a `pd
+00006170: 2e44 6174 6146 7261 6d65 600d 0a0d 0a20  .DataFrame`.... 
+00006180: 2020 2020 2020 203a 7061 7261 6d20 6e6f         :param no
+00006190: 726d 616c 697a 6564 3a20 5365 7420 7472  rmalized: Set tr
+000061a0: 7565 2066 6f72 2054 504d 206e 6f72 6d61  ue for TPM norma
+000061b0: 6c69 7a65 6420 6f75 7470 7574 2c20 6465  lized output, de
+000061c0: 6661 756c 7473 2074 6f20 4661 6c73 650d  faults to False.
+000061d0: 0a20 2020 2020 2020 203a 7479 7065 206e  .        :type n
+000061e0: 6f72 6d61 6c69 7a65 643a 2062 6f6f 6c2c  ormalized: bool,
+000061f0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00006200: 2020 203a 7265 7475 726e 3a20 6f62 7365     :return: obse
+00006210: 7276 6174 696f 6e73 20c3 9720 6665 6174  rvations .. feat
+00006220: 7572 6573 2064 6174 6120 6d61 7472 6978  ures data matrix
+00006230: 0d0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00006240: 3a20 7064 2e44 6174 6146 7261 6d65 0d0a  : pd.DataFrame..
+00006250: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00006260: 2020 2020 2064 6620 3d20 7365 6c66 2e61       df = self.a
+00006270: 6461 7461 2e74 6f5f 6466 2829 0d0a 2020  data.to_df()..  
+00006280: 2020 2020 2020 6966 206e 6f72 6d61 6c69        if normali
+00006290: 7a65 6420 616e 6420 6e6f 7420 7365 6c66  zed and not self
+000062a0: 2e69 735f 6e6f 726d 616c 697a 6564 3a0d  .is_normalized:.
+000062b0: 0a20 2020 2020 2020 2020 2020 2064 6620  .            df 
+000062c0: 3d20 6466 2e64 6976 2864 662e 7375 6d28  = df.div(df.sum(
+000062d0: 6178 6973 3d31 292c 2061 7869 733d 3029  axis=1), axis=0)
+000062e0: 202a 2031 6536 2020 2320 5450 4d20 6e6f   * 1e6  # TPM no
+000062f0: 726d 616c 697a 6174 696f 6e0d 0a20 2020  rmalization..   
+00006300: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
+00006310: 0d0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
+00006320: 5f75 6e66 6163 746f 7269 7a61 626c 655f  _unfactorizable_
+00006330: 6f62 7365 7276 6174 696f 6e73 2873 656c  observations(sel
+00006340: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
+00006350: 5265 6d6f 7665 7320 6f62 7365 7276 6174  Removes observat
+00006360: 696f 6e73 2077 6974 6820 616c 6c20 7a65  ions with all ze
+00006370: 726f 7320 6672 6f6d 2074 6865 2064 6174  ros from the dat
+00006380: 6120 6d61 7472 6978 2e0d 0a20 2020 2020  a matrix...     
+00006390: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000063a0: 6466 203d 2073 656c 662e 746f 5f64 6628  df = self.to_df(
+000063b0: 6e6f 726d 616c 697a 6564 3d46 616c 7365  normalized=False
+000063c0: 290d 0a20 2020 2020 2020 2023 2043 6865  )..        # Che
+000063d0: 636b 2066 6f72 206f 6273 6572 7661 7469  ck for observati
+000063e0: 6f6e 7320 7769 7468 2061 6c6c 207a 6572  ons with all zer
+000063f0: 6f73 0d0a 2020 2020 2020 2020 6f62 735f  os..        obs_
+00006400: 7a65 726f 7320 3d20 2864 662e 5420 3d3d  zeros = (df.T ==
+00006410: 2030 292e 616c 6c28 290d 0a20 2020 2020   0).all()..     
+00006420: 2020 206e 5f6f 6273 5f7a 6572 6f73 203d     n_obs_zeros =
+00006430: 206f 6273 5f7a 6572 6f73 2e73 756d 2829   obs_zeros.sum()
+00006440: 0d0a 2020 2020 2020 2020 6c6f 6767 696e  ..        loggin
+00006450: 672e 696e 666f 2866 227b 6e5f 6f62 735f  g.info(f"{n_obs_
+00006460: 7a65 726f 737d 206f 6620 7b73 656c 662e  zeros} of {self.
+00006470: 6164 6174 612e 6e5f 6f62 737d 206f 6273  adata.n_obs} obs
+00006480: 6572 7661 7469 6f6e 7320 6172 6520 616c  ervations are al
+00006490: 6c20 7a65 726f 732e 2229 0d0a 2020 2020  l zeros.")..    
+000064a0: 2020 2020 6966 206e 5f6f 6273 5f7a 6572      if n_obs_zer
+000064b0: 6f73 3a0d 0a20 2020 2020 2020 2020 2020  os:..           
+000064c0: 206c 6f67 6769 6e67 2e77 6172 6e69 6e67   logging.warning
+000064d0: 2866 2253 7562 7365 7474 696e 6720 6f62  (f"Subsetting ob
+000064e0: 7365 7276 6174 696f 6e73 2074 6f20 7468  servations to th
+000064f0: 6f73 6520 7769 7468 2061 7420 6c65 6173  ose with at leas
+00006500: 7420 3120 706f 7369 7469 7665 2076 616c  t 1 positive val
+00006510: 7565 2e22 290d 0a20 2020 2020 2020 2020  ue.")..         
+00006520: 2020 206d 7367 5f73 7472 696e 6720 3d20     msg_string = 
+00006530: 7265 7072 286f 6273 5f7a 6572 6f73 5b6f  repr(obs_zeros[o
+00006540: 6273 5f7a 6572 6f73 5d2e 696e 6465 782e  bs_zeros].index.
+00006550: 746f 5f6c 6973 7428 2929 0d0a 2020 2020  to_list())..    
+00006560: 2020 2020 2020 2020 7365 6c66 2e61 7070          self.app
+00006570: 656e 645f 746f 5f68 6973 746f 7279 2866  end_to_history(f
+00006580: 2252 656d 6f76 696e 6720 6f62 7365 7276  "Removing observ
+00006590: 6174 696f 6e73 2077 6974 6820 6f6e 6c79  ations with only
+000065a0: 207a 6572 6f73 3a20 7b6d 7367 5f73 7472   zeros: {msg_str
+000065b0: 696e 677d 2229 0d0a 2020 2020 2020 2020  ing}")..        
+000065c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+000065d0: 6461 7461 203d 2073 656c 662e 6164 6174  data = self.adat
+000065e0: 615b 7e6f 6273 5f7a 6572 6f73 2c3a 5d2e  a[~obs_zeros,:].
+000065f0: 636f 7079 2829 0d0a 0d0a 0d0a 2020 2020  copy()......    
+00006600: 6465 6620 7265 6d6f 7665 5f75 6e66 6163  def remove_unfac
+00006610: 746f 7269 7a61 626c 655f 6665 6174 7572  torizable_featur
+00006620: 6573 2873 656c 6629 3a0d 0a20 2020 2020  es(self):..     
+00006630: 2020 2022 2222 5265 6d6f 7665 7320 6665     """Removes fe
+00006640: 6174 7572 6573 2077 6974 6820 6d69 7373  atures with miss
+00006650: 696e 6720 7661 6c75 6573 206f 7220 7a65  ing values or ze
+00006660: 726f 2076 6172 6961 6e63 6520 6672 6f6d  ro variance from
+00006670: 2074 6865 2064 6174 6120 6d61 7472 6978   the data matrix
+00006680: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00006690: 2020 2020 2020 2020 6466 203d 2073 656c          df = sel
+000066a0: 662e 746f 5f64 6628 6e6f 726d 616c 697a  f.to_df(normaliz
+000066b0: 6564 3d46 616c 7365 290d 0a20 2020 2020  ed=False)..     
+000066c0: 2020 2023 2043 6865 636b 2066 6f72 2066     # Check for f
+000066d0: 6561 7475 7265 7320 7769 7468 206d 6973  eatures with mis
+000066e0: 7369 6e67 2076 616c 7565 730d 0a20 2020  sing values..   
+000066f0: 2020 2020 2067 656e 6573 5f77 6974 685f       genes_with_
+00006700: 6d69 7373 696e 6776 616c 7565 7320 3d20  missingvalues = 
+00006710: 6466 2e69 736e 756c 6c28 292e 616e 7928  df.isnull().any(
+00006720: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+00006730: 2020 2020 206e 5f6d 6973 7369 6e67 203d       n_missing =
+00006740: 2067 656e 6573 5f77 6974 685f 6d69 7373   genes_with_miss
+00006750: 696e 6776 616c 7565 732e 7375 6d28 290d  ingvalues.sum().
+00006760: 0a20 2020 2020 2020 206c 6f67 6769 6e67  .        logging
+00006770: 2e69 6e66 6f28 6622 7b6e 5f6d 6973 7369  .info(f"{n_missi
+00006780: 6e67 7d20 6f66 207b 7365 6c66 2e61 6461  ng} of {self.ada
+00006790: 7461 2e6e 5f76 6172 737d 2066 6561 7475  ta.n_vars} featu
+000067a0: 7265 7320 6172 6520 6d69 7373 696e 6720  res are missing 
+000067b0: 7661 6c75 6573 2e22 290d 0a20 2020 2020  values.")..     
+000067c0: 2020 2069 6620 6e5f 6d69 7373 696e 673a     if n_missing:
+000067d0: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+000067e0: 6767 696e 672e 7761 726e 696e 6728 6622  gging.warning(f"
+000067f0: 5375 6273 6574 7469 6e67 2066 6561 7475  Subsetting featu
+00006800: 7265 7320 746f 2074 686f 7365 2077 6974  res to those wit
+00006810: 6820 6e6f 206d 6973 7369 6e67 2076 616c  h no missing val
+00006820: 7565 732e 2229 0d0a 2020 2020 2020 2020  ues.")..        
+00006830: 2020 2020 6d73 675f 7374 7269 6e67 203d      msg_string =
+00006840: 2072 6570 7228 6765 6e65 735f 7769 7468   repr(genes_with
+00006850: 5f6d 6973 7369 6e67 7661 6c75 6573 5b67  _missingvalues[g
+00006860: 656e 6573 5f77 6974 685f 6d69 7373 696e  enes_with_missin
+00006870: 6776 616c 7565 735d 2e69 6e64 6578 2e74  gvalues].index.t
+00006880: 6f5f 6c69 7374 2829 290d 0a20 2020 2020  o_list())..     
+00006890: 2020 2020 2020 2073 656c 662e 6170 7065         self.appe
+000068a0: 6e64 5f74 6f5f 6869 7374 6f72 7928 6622  nd_to_history(f"
+000068b0: 5265 6d6f 7669 6e67 2066 6561 7475 7265  Removing feature
+000068c0: 7320 7769 7468 206d 6973 7369 6e67 2076  s with missing v
+000068d0: 616c 7565 733a 207b 6d73 675f 7374 7269  alues: {msg_stri
+000068e0: 6e67 7d22 290d 0a20 2020 2020 2020 2023  ng}")..        #
+000068f0: 2043 6865 636b 2066 6f72 2067 656e 6573   Check for genes
+00006900: 2077 6974 6820 7a65 726f 2076 6172 6961   with zero varia
+00006910: 6e63 650d 0a20 2020 2020 2020 207a 6572  nce..        zer
+00006920: 6f76 6172 6765 6e65 7320 3d20 2864 662e  ovargenes = (df.
+00006930: 7661 7228 2920 3d3d 2030 290d 0a20 2020  var() == 0)..   
+00006940: 2020 2020 206e 5f7a 6572 6f76 6172 203d       n_zerovar =
+00006950: 207a 6572 6f76 6172 6765 6e65 732e 7375   zerovargenes.su
+00006960: 6d28 290d 0a20 2020 2020 2020 206c 6f67  m()..        log
+00006970: 6769 6e67 2e69 6e66 6f28 6622 7b6e 5f7a  ging.info(f"{n_z
+00006980: 6572 6f76 6172 7d20 6f66 207b 7365 6c66  erovar} of {self
+00006990: 2e61 6461 7461 2e6e 5f76 6172 737d 2066  .adata.n_vars} f
+000069a0: 6561 7475 7265 7320 6861 7665 2061 2076  eatures have a v
+000069b0: 6172 6961 6e63 6520 6f66 207a 6572 6f2e  ariance of zero.
+000069c0: 2229 0d0a 2020 2020 2020 2020 6966 206e  ")..        if n
+000069d0: 5f7a 6572 6f76 6172 3a0d 0a20 2020 2020  _zerovar:..     
+000069e0: 2020 2020 2020 206c 6f67 6769 6e67 2e77         logging.w
+000069f0: 6172 6e69 6e67 2866 2253 7562 7365 7474  arning(f"Subsett
+00006a00: 696e 6720 6665 6174 7572 6573 2074 6f20  ing features to 
+00006a10: 7468 6f73 6520 7769 7468 206e 6f6e 7a65  those with nonze
+00006a20: 726f 2076 6172 6961 6e63 652e 2229 0d0a  ro variance.")..
+00006a30: 2020 2020 2020 2020 2020 2020 6d73 675f              msg_
+00006a40: 7374 7269 6e67 203d 2072 6570 7228 7a65  string = repr(ze
+00006a50: 726f 7661 7267 656e 6573 5b7a 6572 6f76  rovargenes[zerov
+00006a60: 6172 6765 6e65 735d 2e69 6e64 6578 2e74  argenes].index.t
+00006a70: 6f5f 6c69 7374 2829 290d 0a20 2020 2020  o_list())..     
+00006a80: 2020 2020 2020 2073 656c 662e 6170 7065         self.appe
+00006a90: 6e64 5f74 6f5f 6869 7374 6f72 7928 6622  nd_to_history(f"
+00006aa0: 5265 6d6f 7669 6e67 2066 6561 7475 7265  Removing feature
+00006ab0: 7320 7769 7468 207a 6572 6f20 7661 7269  s with zero vari
+00006ac0: 616e 6365 3a20 7b6d 7367 5f73 7472 696e  ance: {msg_strin
+00006ad0: 677d 2229 0d0a 2020 2020 2020 2020 6765  g}")..        ge
+00006ae0: 6e65 735f 746f 5f6b 6565 7020 3d20 287e  nes_to_keep = (~
+00006af0: 6765 6e65 735f 7769 7468 5f6d 6973 7369  genes_with_missi
+00006b00: 6e67 7661 6c75 6573 2920 2620 287e 7a65  ngvalues) & (~ze
+00006b10: 726f 7661 7267 656e 6573 290d 0a20 2020  rovargenes)..   
+00006b20: 2020 2020 2073 656c 662e 6164 6174 6120       self.adata 
+00006b30: 3d20 7365 6c66 2e61 6461 7461 5b3a 2c67  = self.adata[:,g
+00006b40: 656e 6573 5f74 6f5f 6b65 6570 5d2e 636f  enes_to_keep].co
+00006b50: 7079 2829 0d0a 0d0a 2020 2020 6465 6620  py()....    def 
+00006b60: 6372 6f73 735f 7661 6c69 6461 7465 5f69  cross_validate_i
+00006b70: 6d70 7574 6174 696f 6e28 7365 6c66 2c20  mputation(self, 
+00006b80: 696d 7075 7465 723a 2055 6e69 6f6e 5b4b  imputer: Union[K
+00006b90: 4e4e 496d 7075 7465 722c 2053 696d 706c  NNImputer, Simpl
+00006ba0: 6549 6d70 7574 6572 5d2c 206e 5f66 6f6c  eImputer], n_fol
+00006bb0: 6473 3a20 696e 7420 3d20 3130 3029 3a0d  ds: int = 100):.
+00006bc0: 0a20 2020 2020 2020 2022 2222 5065 7266  .        """Perf
+00006bd0: 6f72 6d20 6b2d 666f 6c64 2063 726f 7373  orm k-fold cross
+00006be0: 2076 616c 6964 6174 696f 6e20 6f66 2069   validation of i
+00006bf0: 6d70 7574 6174 696f 6e20 6f6e 2074 6865  mputation on the
+00006c00: 2064 6174 6173 6574 2077 6974 686f 7574   dataset without
+00006c10: 206d 6f64 6966 7969 6e67 2074 6865 2064   modifying the d
+00006c20: 6174 612e 0d0a 0d0a 2020 2020 2020 2020  ata.....        
+00006c30: 3a70 6172 616d 2069 6d70 7574 6572 3a20  :param imputer: 
+00006c40: 696d 7075 7465 7220 6f62 6a65 6374 2066  imputer object f
+00006c50: 726f 6d20 7363 696b 6974 2d6c 6561 726e  rom scikit-learn
+00006c60: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00006c70: 696d 7075 7465 723a 2055 6e69 6f6e 5b4b  imputer: Union[K
+00006c80: 4e4e 496d 7075 7465 722c 2053 696d 706c  NNImputer, Simpl
+00006c90: 6549 6d70 7574 6572 5d0d 0a20 2020 2020  eImputer]..     
+00006ca0: 2020 203a 7061 7261 6d20 6e5f 666f 6c64     :param n_fold
+00006cb0: 733a 206e 756d 6265 7220 6f66 2066 6f6c  s: number of fol
+00006cc0: 6473 2c20 6465 6661 756c 7473 2074 6f20  ds, defaults to 
+00006cd0: 3130 300d 0a20 2020 2020 2020 203a 7479  100..        :ty
+00006ce0: 7065 206e 5f66 6f6c 6473 3a20 696e 742c  pe n_folds: int,
+00006cf0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00006d00: 2020 203a 7265 7475 726e 3a20 4461 7461     :return: Data
+00006d10: 6672 616d 2077 6974 6820 7374 6174 6973  fram with statis
+00006d20: 7469 6373 2066 6f72 2065 6163 6820 6765  tics for each ge
+00006d30: 6e65 2c20 696e 636c 7564 696e 6720 7072  ne, including pr
+00006d40: 6569 6d70 7574 6174 696f 6e20 6c6f 672d  eimputation log-
+00006d50: 6d65 616e 2061 6e64 206c 6f67 2d76 6172  mean and log-var
+00006d60: 6961 6e63 652c 2061 6e64 204e 524d 5344  iance, and NRMSD
+00006d70: 206d 6561 6e20 616e 6420 7661 7269 616e   mean and varian
+00006d80: 6365 2061 6372 6f73 7320 616c 6c20 666f  ce across all fo
+00006d90: 6c64 732e 0d0a 2020 2020 2020 2020 3a72  lds...        :r
+00006da0: 7479 7065 3a20 3a63 6c61 7373 3a60 7061  type: :class:`pa
+00006db0: 6e64 6173 2e44 6174 6146 7261 6d65 600d  ndas.DataFrame`.
+00006dc0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00006dd0: 2020 2020 2020 6c6f 6767 696e 672e 696e        logging.in
+00006de0: 666f 2866 2250 6572 666f 726d 696e 6720  fo(f"Performing 
+00006df0: 6b2d 666f 6c64 2063 726f 7373 2d76 616c  k-fold cross-val
+00006e00: 6964 6174 696f 6e2c 2077 6974 6820 7b6e  idation, with {n
+00006e10: 5f66 6f6c 6473 7d20 666f 6c64 7322 290d  _folds} folds").
+00006e20: 0a20 2020 2020 2020 2023 206b 2d66 6f6c  .        # k-fol
+00006e30: 6420 6372 6f73 732d 7661 6c69 6461 7469  d cross-validati
+00006e40: 6f6e 0d0a 2020 2020 2020 2020 726d 7364  on..        rmsd
+00006e50: 5f66 6f6c 6473 203d 205b 5d20 2020 2320  _folds = []   # 
+00006e60: 7374 6f72 6520 6765 6e65 2d77 6973 6520  store gene-wise 
+00006e70: 726d 7364 0d0a 2020 2020 2020 2020 6461  rmsd..        da
+00006e80: 7461 203d 2073 656c 662e 6164 6174 612e  ta = self.adata.
+00006e90: 746f 5f64 6628 290d 0a20 2020 2020 2020  to_df()..       
+00006ea0: 2072 616e 646f 6d5f 6e75 6d62 6572 7320   random_numbers 
+00006eb0: 3d20 6e70 2e72 616e 646f 6d2e 7261 6e64  = np.random.rand
+00006ec0: 6f6d 2864 6174 612e 7368 6170 6529 2020  om(data.shape)  
+00006ed0: 2320 7573 6564 2074 6f20 6173 7369 676e  # used to assign
+00006ee0: 2065 6163 6820 6461 7461 2070 6f69 6e74   each data point
+00006ef0: 2074 6f20 6120 666f 6c64 0d0a 2020 2020   to a fold..    
+00006f00: 2020 2020 6269 6e73 203d 206e 702e 6c69      bins = np.li
+00006f10: 6e73 7061 6365 2830 2c20 312c 206e 5f66  nspace(0, 1, n_f
+00006f20: 6f6c 6473 202b 2031 290d 0a20 2020 2020  olds + 1)..     
+00006f30: 2020 2066 6f72 2066 6f6c 6420 696e 2074     for fold in t
+00006f40: 7164 6d28 7261 6e67 6528 6e5f 666f 6c64  qdm(range(n_fold
+00006f50: 7329 2c20 756e 6974 3d22 666f 6c64 2229  s), unit="fold")
+00006f60: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
+00006f70: 6f77 6572 2c20 7570 7065 7220 3d20 6269  ower, upper = bi
+00006f80: 6e73 5b66 6f6c 643a 666f 6c64 202b 2032  ns[fold:fold + 2
+00006f90: 5d0d 0a20 2020 2020 2020 2020 2020 206d  ]..            m
+00006fa0: 6173 6b20 3d20 2872 616e 646f 6d5f 6e75  ask = (random_nu
+00006fb0: 6d62 6572 7320 3e3d 206c 6f77 6572 2920  mbers >= lower) 
+00006fc0: 2620 2872 616e 646f 6d5f 6e75 6d62 6572  & (random_number
+00006fd0: 7320 3c20 7570 7065 7229 0d0a 2020 2020  s < upper)..    
+00006fe0: 2020 2020 2020 2020 7465 7374 203d 2064          test = d
+00006ff0: 6174 612e 6d61 736b 287e 6d61 736b 290d  ata.mask(~mask).
+00007000: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+00007010: 696e 696e 6720 3d20 6461 7461 2e6d 6173  ining = data.mas
+00007020: 6b28 6d61 736b 290d 0a20 2020 2020 2020  k(mask)..       
+00007030: 2020 2020 2069 6d70 7574 6564 203d 2069       imputed = i
+00007040: 6d70 7574 6572 2e66 6974 5f74 7261 6e73  mputer.fit_trans
+00007050: 666f 726d 2874 7261 696e 696e 6729 0d0a  form(training)..
+00007060: 2020 2020 2020 2020 2020 2020 696d 7075              impu
+00007070: 7465 6420 3d20 7064 2e44 6174 6146 7261  ted = pd.DataFra
+00007080: 6d65 2869 6d70 7574 6564 2c20 696e 6465  me(imputed, inde
+00007090: 783d 6461 7461 2e69 6e64 6578 2c20 636f  x=data.index, co
+000070a0: 6c75 6d6e 733d 6461 7461 2e63 6f6c 756d  lumns=data.colum
+000070b0: 6e73 290d 0a20 2020 2020 2020 2020 2020  ns)..           
+000070c0: 2072 6573 6964 203d 2028 696d 7075 7465   resid = (impute
+000070d0: 6420 2d20 7465 7374 290d 0a20 2020 2020  d - test)..     
+000070e0: 2020 2020 2020 2072 6d73 6420 3d20 6e70         rmsd = np
+000070f0: 2e73 7172 7428 2872 6573 6964 202a 2a20  .sqrt((resid ** 
+00007100: 3229 2e73 756d 2829 202f 2072 6573 6964  2).sum() / resid
+00007110: 2e6e 6f74 6e75 6c6c 2829 2e73 756d 2829  .notnull().sum()
+00007120: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00007130: 6d73 645f 666f 6c64 732e 6170 7065 6e64  msd_folds.append
+00007140: 2872 6d73 6429 0d0a 2020 2020 2020 2020  (rmsd)..        
+00007150: 726d 7364 5f66 6f6c 6473 203d 2070 642e  rmsd_folds = pd.
+00007160: 636f 6e63 6174 2872 6d73 645f 666f 6c64  concat(rmsd_fold
+00007170: 732c 2061 7869 733d 3129 0d0a 2020 2020  s, axis=1)..    
+00007180: 2020 2020 6e72 6d73 645f 666f 6c64 7320      nrmsd_folds 
+00007190: 3d20 726d 7364 5f66 6f6c 6473 2e64 6976  = rmsd_folds.div
+000071a0: 2864 6174 612e 6d65 616e 2829 2c20 6178  (data.mean(), ax
+000071b0: 6973 3d30 290d 0a20 2020 2020 2020 200d  is=0)..        .
+000071c0: 0a20 2020 2020 2020 2023 2072 6563 6f72  .        # recor
+000071d0: 6420 7374 6174 7320 696e 2061 6461 7461  d stats in adata
+000071e0: 2e76 6172 0d0a 2020 2020 2020 2020 6376  .var..        cv
+000071f0: 7374 6174 7320 3d20 7064 2e44 6174 6146  stats = pd.DataF
+00007200: 7261 6d65 287b 0d0a 2020 2020 2020 2020  rame({..        
+00007210: 2020 2020 226c 6f67 5f6d 6561 6e5f 7072      "log_mean_pr
+00007220: 6569 6d70 7574 6174 696f 6e22 3a20 6e70  eimputation": np
+00007230: 2e6c 6f67 3130 2864 6174 612e 6d65 616e  .log10(data.mean
+00007240: 2829 292c 0d0a 2020 2020 2020 2020 2020  ()),..          
+00007250: 2020 226c 6f67 5f76 6172 6961 6e63 655f    "log_variance_
+00007260: 7072 6569 6d70 7574 6174 696f 6e22 3a20  preimputation": 
+00007270: 6e70 2e6c 6f67 3130 2864 6174 612e 7661  np.log10(data.va
+00007280: 7228 2929 2c0d 0a20 2020 2020 2020 2020  r()),..         
+00007290: 2020 2022 696d 7075 7461 7469 6f6e 5f6e     "imputation_n
+000072a0: 726d 7364 5f6d 6561 6e22 3a20 6e72 6d73  rmsd_mean": nrms
+000072b0: 645f 666f 6c64 732e 6d65 616e 2861 7869  d_folds.mean(axi
+000072c0: 733d 3129 2c0d 0a20 2020 2020 2020 2020  s=1),..         
+000072d0: 2020 2022 696d 7075 7461 7469 6f6e 5f6e     "imputation_n
+000072e0: 726d 7364 5f76 6172 223a 206e 726d 7364  rmsd_var": nrmsd
+000072f0: 5f66 6f6c 6473 2e6d 6561 6e28 6178 6973  _folds.mean(axis
+00007300: 3d31 290d 0a20 2020 2020 2020 207d 290d  =1)..        }).
+00007310: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00007320: 6e20 6376 7374 6174 730d 0a0d 0a20 2020  n cvstats....   
+00007330: 2064 6566 2069 6d70 7574 655f 6b6e 6e28   def impute_knn(
+00007340: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+00007350: 2020 2020 2020 2020 2020 6e5f 6e65 6967            n_neig
+00007360: 6862 6f72 733a 2069 6e74 203d 2035 2c0d  hbors: int = 5,.
+00007370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007380: 2020 2020 7765 6967 6874 733a 204c 6974      weights: Lit
+00007390: 6572 616c 5b22 6469 7374 616e 6365 222c  eral["distance",
+000073a0: 2022 756e 6966 6f72 6d22 5d20 3d20 2264   "uniform"] = "d
+000073b0: 6973 7461 6e63 6522 2c0d 0a20 2020 2020  istance",..     
+000073c0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
+000073d0: 6f73 735f 7661 6c69 6461 7465 3a20 626f  oss_validate: bo
+000073e0: 6f6c 203d 2054 7275 652c 0d0a 2020 2020  ol = True,..    
+000073f0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00007400: 5f66 6f6c 6473 3a20 696e 7420 3d20 3130  _folds: int = 10
+00007410: 3029 3a0d 0a20 2020 2020 2020 200d 0a20  0):..        .. 
+00007420: 2020 2020 2020 2022 2222 496d 7075 7461         """Imputa
+00007430: 7469 6f6e 2066 6f72 2063 6f6d 706c 6574  tion for complet
+00007440: 696e 6720 6d69 7373 696e 6720 7661 6c75  ing missing valu
+00007450: 6573 2075 7369 6e67 206b 2d4e 6561 7265  es using k-Neare
+00007460: 7374 204e 6569 6768 626f 7273 2e0d 0a20  st Neighbors... 
+00007470: 2020 2020 2020 2020 2020 4561 6368 2073            Each s
+00007480: 616d 706c 6527 7320 6d69 7373 696e 6720  ample's missing 
+00007490: 7661 6c75 6573 2061 7265 2069 6d70 7574  values are imput
+000074a0: 6564 2075 7369 6e67 2074 6865 206d 6561  ed using the mea
+000074b0: 6e20 7661 6c75 6520 6672 6f6d 0d0a 2020  n value from..  
+000074c0: 2020 2020 2020 2020 2060 6e5f 6e65 6967           `n_neig
+000074d0: 6862 6f72 7360 206e 6561 7265 7374 206e  hbors` nearest n
+000074e0: 6569 6768 626f 7273 2e20 5477 6f20 7361  eighbors. Two sa
+000074f0: 6d70 6c65 7320 6172 650d 0a20 2020 2020  mples are..     
+00007500: 2020 2020 2020 636c 6f73 6520 6966 2074        close if t
+00007510: 6865 2066 6561 7475 7265 7320 7468 6174  he features that
+00007520: 206e 6569 7468 6572 2069 7320 6d69 7373   neither is miss
+00007530: 696e 6720 6172 6520 636c 6f73 652e 200d  ing are close. .
+00007540: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00007550: 6d20 6e5f 6e65 6967 6862 6f72 733a 204e  m n_neighbors: N
+00007560: 756d 6265 7220 6f66 206e 6569 6768 626f  umber of neighbo
+00007570: 7269 6e67 2073 616d 706c 6573 2074 6f20  ring samples to 
+00007580: 7573 6520 666f 7220 696d 7075 7461 7469  use for imputati
+00007590: 6f6e 2c20 6465 6661 756c 7473 2074 6f20  on, defaults to 
+000075a0: 350d 0a20 2020 2020 2020 203a 7479 7065  5..        :type
+000075b0: 206e 5f6e 6569 6768 626f 7273 3a20 696e   n_neighbors: in
+000075c0: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
+000075d0: 2020 2020 203a 7061 7261 6d20 7765 6967       :param weig
+000075e0: 6874 733a 2057 6569 6768 7420 6675 6e63  hts: Weight func
+000075f0: 7469 6f6e 2075 7365 6420 696e 2070 7265  tion used in pre
+00007600: 6469 6374 696f 6e2c 2064 6566 6175 6c74  diction, default
+00007610: 7320 746f 2027 6469 7374 616e 6365 272e  s to 'distance'.
+00007620: 2050 6f73 7369 626c 6520 7661 6c75 6573   Possible values
+00007630: 3a0d 0a20 2020 2020 2020 2020 2020 202d  :..            -
+00007640: 2027 756e 6966 6f72 6d27 203a 2075 6e69   'uniform' : uni
+00007650: 666f 726d 2077 6569 6768 7473 2e20 416c  form weights. Al
+00007660: 6c20 706f 696e 7473 2069 6e20 6561 6368  l points in each
+00007670: 206e 6569 6768 626f 7268 6f6f 6420 6172   neighborhood ar
+00007680: 650d 0a20 2020 2020 2020 2020 2020 2077  e..            w
+00007690: 6569 6768 7465 6420 6571 7561 6c6c 792e  eighted equally.
+000076a0: 0d0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
+000076b0: 2764 6973 7461 6e63 6527 203a 2077 6569  'distance' : wei
+000076c0: 6768 7420 706f 696e 7473 2062 7920 7468  ght points by th
+000076d0: 6520 696e 7665 7273 6520 6f66 2074 6865  e inverse of the
+000076e0: 6972 2064 6973 7461 6e63 652e 0d0a 2020  ir distance...  
+000076f0: 2020 2020 2020 2020 2020 696e 2074 6869            in thi
+00007700: 7320 6361 7365 2c20 636c 6f73 6572 206e  s case, closer n
+00007710: 6569 6768 626f 7273 206f 6620 6120 7175  eighbors of a qu
+00007720: 6572 7920 706f 696e 7420 7769 6c6c 2068  ery point will h
+00007730: 6176 6520 610d 0a20 2020 2020 2020 2020  ave a..         
+00007740: 2020 2067 7265 6174 6572 2069 6e66 6c75     greater influ
+00007750: 656e 6365 2074 6861 6e20 6e65 6967 6862  ence than neighb
+00007760: 6f72 7320 7768 6963 6820 6172 6520 6675  ors which are fu
+00007770: 7274 6865 7220 6177 6179 2e0d 0a20 2020  rther away...   
+00007780: 2020 2020 203a 7479 7065 2077 6569 6768       :type weigh
+00007790: 7473 3a20 4c69 7465 7261 6c5b 2264 6973  ts: Literal["dis
+000077a0: 7461 6e63 6522 2c20 2275 6e69 666f 726d  tance", "uniform
+000077b0: 225d 2c20 6f70 7469 6f6e 616c 0d0a 2020  "], optional..  
+000077c0: 2020 2020 2020 3a70 6172 616d 2063 726f        :param cro
+000077d0: 7373 5f76 616c 6964 6174 653a 2070 6572  ss_validate: per
+000077e0: 666f 726d 206b 2d66 6f6c 6420 6372 6f73  form k-fold cros
+000077f0: 732d 7661 6c69 6461 7469 6f6e 2c20 6465  s-validation, de
+00007800: 6661 756c 7473 2074 6f20 5472 7565 0d0a  faults to True..
+00007810: 2020 2020 2020 2020 3a74 7970 6520 6372          :type cr
+00007820: 6f73 735f 7661 6c69 6461 7465 3a20 626f  oss_validate: bo
+00007830: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 2020  ol, optional..  
+00007840: 2020 2020 2020 3a70 6172 616d 206e 5f66        :param n_f
+00007850: 6f6c 6473 3a20 6e75 6d62 6572 206f 6620  olds: number of 
+00007860: 666f 6c64 7320 666f 7220 6b2d 666f 6c64  folds for k-fold
+00007870: 2063 726f 7373 2d76 616c 6964 6174 696f   cross-validatio
+00007880: 6e2c 2064 6566 6175 6c74 7320 746f 2031  n, defaults to 1
+00007890: 3030 0d0a 2020 2020 2020 2020 3a74 7970  00..        :typ
+000078a0: 6520 6e5f 666f 6c64 733a 2069 6e74 2c20  e n_folds: int, 
+000078b0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+000078c0: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
+000078d0: 206c 6f67 6769 6e67 2e69 6e66 6f28 6622   logging.info(f"
+000078e0: 496d 7075 7469 6e67 2064 6174 6120 7769  Imputing data wi
+000078f0: 7468 206b 2d4e 6561 7265 7374 204e 6569  th k-Nearest Nei
+00007900: 6768 626f 7273 2c20 6b3d 7b6e 5f6e 6569  ghbors, k={n_nei
+00007910: 6768 626f 7273 7d2c 207b 7765 6967 6874  ghbors}, {weight
+00007920: 737d 2077 6569 6768 7473 2229 0d0a 0d0a  s} weights")....
+00007930: 2020 2020 2020 2020 696d 7075 7465 7220          imputer 
+00007940: 3d20 4b4e 4e49 6d70 7574 6572 286e 5f6e  = KNNImputer(n_n
+00007950: 6569 6768 626f 7273 3d6e 5f6e 6569 6768  eighbors=n_neigh
+00007960: 626f 7273 2c20 7765 6967 6874 733d 7765  bors, weights=we
+00007970: 6967 6874 732c 206b 6565 705f 656d 7074  ights, keep_empt
+00007980: 795f 6665 6174 7572 6573 3d54 7275 6529  y_features=True)
+00007990: 0d0a 2020 2020 2020 2020 6966 206e 5f66  ..        if n_f
+000079a0: 6f6c 6473 203c 2032 3a0d 0a20 2020 2020  olds < 2:..     
+000079b0: 2020 2020 2020 206c 6f67 6769 6e67 2e77         logging.w
+000079c0: 6172 6e69 6e67 2866 226e 5f66 6f6c 6473  arning(f"n_folds
+000079d0: 203d 207b 6e5f 666f 6c64 737d 2069 7320   = {n_folds} is 
+000079e0: 6c65 7373 2074 6861 6e20 322e 2053 6b69  less than 2. Ski
+000079f0: 7070 696e 6720 6372 6f73 732d 7661 6c69  pping cross-vali
+00007a00: 6461 7469 6f6e 2e22 290d 0a20 2020 2020  dation.")..     
+00007a10: 2020 2020 2020 2063 726f 7373 5f76 616c         cross_val
+00007a20: 6964 6174 6520 3d20 4661 6c73 650d 0a20  idate = False.. 
+00007a30: 2020 2020 2020 2069 6620 6372 6f73 735f         if cross_
+00007a40: 7661 6c69 6461 7465 3a0d 0a20 2020 2020  validate:..     
+00007a50: 2020 2020 2020 2063 7673 7461 7473 203d         cvstats =
+00007a60: 2073 656c 662e 6372 6f73 735f 7661 6c69   self.cross_vali
+00007a70: 6461 7465 5f69 6d70 7574 6174 696f 6e28  date_imputation(
+00007a80: 696d 7075 7465 723d 696d 7075 7465 722c  imputer=imputer,
+00007a90: 206e 5f66 6f6c 6473 3d6e 5f66 6f6c 6473   n_folds=n_folds
+00007aa0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00007ab0: 656c 662e 6164 6174 612e 7661 7220 3d20  elf.adata.var = 
+00007ac0: 7365 6c66 2e61 6461 7461 2e76 6172 2e6a  self.adata.var.j
+00007ad0: 6f69 6e28 6376 7374 6174 732c 2076 616c  oin(cvstats, val
+00007ae0: 6964 6174 653d 2231 3a31 2229 0d0a 2020  idate="1:1")..  
+00007af0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00007b00: 2020 2020 7365 6c66 2e61 6461 7461 2e58      self.adata.X
+00007b10: 203d 2069 6d70 7574 6572 2e66 6974 5f74   = imputer.fit_t
+00007b20: 7261 6e73 666f 726d 2873 656c 662e 6164  ransform(self.ad
+00007b30: 6174 612e 5829 0d0a 2020 2020 2020 2020  ata.X)..        
+00007b40: 7365 6c66 2e61 7070 656e 645f 746f 5f68  self.append_to_h
+00007b50: 6973 746f 7279 2866 224b 4e4e 2049 6d70  istory(f"KNN Imp
+00007b60: 7574 6174 696f 6e3a 206e 5f6e 6569 6768  utation: n_neigh
+00007b70: 626f 7273 203d 207b 6e5f 6e65 6967 6862  bors = {n_neighb
+00007b80: 6f72 737d 2c20 7765 6967 6874 7320 3d20  ors}, weights = 
+00007b90: 7b77 6569 6768 7473 7d22 290d 0a20 2020  {weights}")..   
+00007ba0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00007bb0: 756e 735b 2269 6d70 7574 6174 696f 6e22  uns["imputation"
+00007bc0: 5d20 3d20 7b22 6d65 7468 6f64 223a 2022  ] = {"method": "
+00007bd0: 6b6e 6e22 2c0d 0a20 2020 2020 2020 2020  knn",..         
 00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bf0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00007c00: 5f6e 6569 6768 626f 7273 223a 206e 5f6e  _neighbors": n_n
-00007c10: 6569 6768 626f 7273 2c0d 0a20 2020 2020  eighbors,..     
+00007bf0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007c00: 6e5f 6e65 6967 6862 6f72 7322 3a20 6e5f  n_neighbors": n_
+00007c10: 6e65 6967 6862 6f72 732c 0d0a 2020 2020  neighbors,..    
 00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c40: 2020 2022 7765 6967 6874 7322 3a20 7765     "weights": we
-00007c50: 6967 6874 732c 0d0a 2020 2020 2020 2020  ights,..        
+00007c40: 2020 2020 2277 6569 6768 7473 223a 2077      "weights": w
+00007c50: 6569 6768 7473 2c0d 0a20 2020 2020 2020  eights,..       
 00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c80: 2263 726f 7373 5f76 616c 6964 6174 696f  "cross_validatio
-00007c90: 6e22 3a20 6372 6f73 735f 7661 6c69 6461  n": cross_valida
-00007ca0: 7465 7d0d 0a20 2020 2020 2020 2069 6620  te}..        if 
-00007cb0: 6372 6f73 735f 7661 6c69 6461 7465 3a0d  cross_validate:.
-00007cc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007cd0: 662e 6164 6174 612e 756e 735b 2269 6d70  f.adata.uns["imp
-00007ce0: 7574 6174 696f 6e22 5d5b 226e 5f66 6f6c  utation"]["n_fol
-00007cf0: 6473 225d 203d 206e 5f66 6f6c 6473 0d0a  ds"] = n_folds..
-00007d00: 0d0a 2020 2020 6465 6620 696d 7075 7465  ..    def impute
-00007d10: 5f7a 6572 6f73 2873 656c 662c 0d0a 2020  _zeros(self,..  
+00007c80: 2022 6372 6f73 735f 7661 6c69 6461 7469   "cross_validati
+00007c90: 6f6e 223a 2063 726f 7373 5f76 616c 6964  on": cross_valid
+00007ca0: 6174 657d 0d0a 2020 2020 2020 2020 6966  ate}..        if
+00007cb0: 2063 726f 7373 5f76 616c 6964 6174 653a   cross_validate:
+00007cc0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00007cd0: 6c66 2e61 6461 7461 2e75 6e73 5b22 696d  lf.adata.uns["im
+00007ce0: 7075 7461 7469 6f6e 225d 5b22 6e5f 666f  putation"]["n_fo
+00007cf0: 6c64 7322 5d20 3d20 6e5f 666f 6c64 730d  lds"] = n_folds.
+00007d00: 0a0d 0a20 2020 2064 6566 2069 6d70 7574  ...    def imput
+00007d10: 655f 7a65 726f 7328 7365 6c66 2c0d 0a20  e_zeros(self,.. 
 00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 2020 2063 726f 7373 5f76 616c 6964 6174     cross_validat
-00007d40: 653a 2062 6f6f 6c20 3d20 5472 7565 2c0d  e: bool = True,.
-00007d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007d60: 2020 2020 2020 6e5f 666f 6c64 733a 2069        n_folds: i
-00007d70: 6e74 203d 2031 3030 293a 0d0a 0d0a 2020  nt = 100):....  
-00007d80: 2020 2020 2020 2222 2249 6d70 7574 6174        """Imputat
-00007d90: 696f 6e20 6279 2066 696c 6c69 6e67 206d  ion by filling m
-00007da0: 6973 7369 6e67 2076 616c 7565 7320 7769  issing values wi
-00007db0: 7468 207a 6572 6f73 2e0d 0a0d 0a20 2020  th zeros.....   
-00007dc0: 2020 2020 203a 7061 7261 6d20 6372 6f73       :param cros
-00007dd0: 735f 7661 6c69 6461 7465 3a20 7065 7266  s_validate: perf
-00007de0: 6f72 6d20 6b2d 666f 6c64 2063 726f 7373  orm k-fold cross
-00007df0: 2d76 616c 6964 6174 696f 6e2c 2064 6566  -validation, def
-00007e00: 6175 6c74 7320 746f 2054 7275 650d 0a20  aults to True.. 
-00007e10: 2020 2020 2020 203a 7479 7065 2063 726f         :type cro
-00007e20: 7373 5f76 616c 6964 6174 653a 2062 6f6f  ss_validate: boo
-00007e30: 6c2c 206f 7074 696f 6e61 6c0d 0a20 2020  l, optional..   
-00007e40: 2020 2020 203a 7061 7261 6d20 6e5f 666f       :param n_fo
-00007e50: 6c64 733a 206e 756d 6265 7220 6f66 2066  lds: number of f
-00007e60: 6f6c 6473 2066 6f72 206b 2d66 6f6c 6420  olds for k-fold 
-00007e70: 6372 6f73 732d 7661 6c69 6461 7469 6f6e  cross-validation
-00007e80: 2c20 6465 6661 756c 7473 2074 6f20 3130  , defaults to 10
-00007e90: 300d 0a20 2020 2020 2020 203a 7479 7065  0..        :type
-00007ea0: 206e 5f66 6f6c 6473 3a20 696e 742c 206f   n_folds: int, o
-00007eb0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-00007ec0: 2022 2222 0d0a 2020 2020 2020 2020 6c6f   """..        lo
-00007ed0: 6767 696e 672e 696e 666f 2866 2249 6d70  gging.info(f"Imp
-00007ee0: 7574 696e 6720 6461 7461 2077 6974 6820  uting data with 
-00007ef0: 7a65 726f 7322 290d 0a20 2020 2020 2020  zeros")..       
-00007f00: 200d 0a20 2020 2020 2020 2069 6d70 7574   ..        imput
-00007f10: 6572 203d 2053 696d 706c 6549 6d70 7574  er = SimpleImput
-00007f20: 6572 2873 7472 6174 6567 793d 2263 6f6e  er(strategy="con
-00007f30: 7374 616e 7422 2c20 6669 6c6c 5f76 616c  stant", fill_val
-00007f40: 7565 3d30 2e30 2c20 6b65 6570 5f65 6d70  ue=0.0, keep_emp
-00007f50: 7479 5f66 6561 7475 7265 733d 5472 7565  ty_features=True
-00007f60: 290d 0a20 2020 2020 2020 2069 6620 6e5f  )..        if n_
-00007f70: 666f 6c64 7320 3c20 323a 0d0a 2020 2020  folds < 2:..    
-00007f80: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-00007f90: 7761 726e 696e 6728 6622 6e5f 666f 6c64  warning(f"n_fold
-00007fa0: 7320 3d20 7b6e 5f66 6f6c 6473 7d20 6973  s = {n_folds} is
-00007fb0: 206c 6573 7320 7468 616e 2032 2e20 536b   less than 2. Sk
-00007fc0: 6970 7069 6e67 2063 726f 7373 2d76 616c  ipping cross-val
-00007fd0: 6964 6174 696f 6e2e 2229 0d0a 2020 2020  idation.")..    
-00007fe0: 2020 2020 2020 2020 6372 6f73 735f 7661          cross_va
-00007ff0: 6c69 6461 7465 203d 2046 616c 7365 0d0a  lidate = False..
-00008000: 2020 2020 2020 2020 6966 2063 726f 7373          if cross
-00008010: 5f76 616c 6964 6174 653a 0d0a 2020 2020  _validate:..    
-00008020: 2020 2020 2020 2020 6376 7374 6174 7320          cvstats 
-00008030: 3d20 7365 6c66 2e63 726f 7373 5f76 616c  = self.cross_val
-00008040: 6964 6174 655f 696d 7075 7461 7469 6f6e  idate_imputation
-00008050: 2869 6d70 7574 6572 3d69 6d70 7574 6572  (imputer=imputer
-00008060: 2c20 6e5f 666f 6c64 733d 6e5f 666f 6c64  , n_folds=n_fold
-00008070: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00008080: 7365 6c66 2e61 6461 7461 2e76 6172 203d  self.adata.var =
-00008090: 2073 656c 662e 6164 6174 612e 7661 722e   self.adata.var.
-000080a0: 6a6f 696e 2863 7673 7461 7473 2c20 7661  join(cvstats, va
-000080b0: 6c69 6461 7465 3d22 313a 3122 290d 0a20  lidate="1:1").. 
-000080c0: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-000080d0: 612e 5820 3d20 696d 7075 7465 722e 6669  a.X = imputer.fi
-000080e0: 745f 7472 616e 7366 6f72 6d28 7365 6c66  t_transform(self
-000080f0: 2e61 6461 7461 2e58 290d 0a20 2020 2020  .adata.X)..     
-00008100: 2020 2073 656c 662e 6170 7065 6e64 5f74     self.append_t
-00008110: 6f5f 6869 7374 6f72 7928 6622 5a65 726f  o_history(f"Zero
-00008120: 2069 6d70 7574 6174 696f 6e22 290d 0a20   imputation").. 
-00008130: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-00008140: 612e 756e 735b 2269 6d70 7574 6174 696f  a.uns["imputatio
-00008150: 6e22 5d20 3d20 7b22 6d65 7468 6f64 223a  n"] = {"method":
-00008160: 2022 7a65 726f 222c 0d0a 2020 2020 2020   "zero",..      
+00007d30: 2020 2020 6372 6f73 735f 7661 6c69 6461      cross_valida
+00007d40: 7465 3a20 626f 6f6c 203d 2054 7275 652c  te: bool = True,
+00007d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007d60: 2020 2020 2020 206e 5f66 6f6c 6473 3a20         n_folds: 
+00007d70: 696e 7420 3d20 3130 3029 3a0d 0a0d 0a20  int = 100):.... 
+00007d80: 2020 2020 2020 2022 2222 496d 7075 7461         """Imputa
+00007d90: 7469 6f6e 2062 7920 6669 6c6c 696e 6720  tion by filling 
+00007da0: 6d69 7373 696e 6720 7661 6c75 6573 2077  missing values w
+00007db0: 6974 6820 7a65 726f 732e 0d0a 0d0a 2020  ith zeros.....  
+00007dc0: 2020 2020 2020 3a70 6172 616d 2063 726f        :param cro
+00007dd0: 7373 5f76 616c 6964 6174 653a 2070 6572  ss_validate: per
+00007de0: 666f 726d 206b 2d66 6f6c 6420 6372 6f73  form k-fold cros
+00007df0: 732d 7661 6c69 6461 7469 6f6e 2c20 6465  s-validation, de
+00007e00: 6661 756c 7473 2074 6f20 5472 7565 0d0a  faults to True..
+00007e10: 2020 2020 2020 2020 3a74 7970 6520 6372          :type cr
+00007e20: 6f73 735f 7661 6c69 6461 7465 3a20 626f  oss_validate: bo
+00007e30: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 2020  ol, optional..  
+00007e40: 2020 2020 2020 3a70 6172 616d 206e 5f66        :param n_f
+00007e50: 6f6c 6473 3a20 6e75 6d62 6572 206f 6620  olds: number of 
+00007e60: 666f 6c64 7320 666f 7220 6b2d 666f 6c64  folds for k-fold
+00007e70: 2063 726f 7373 2d76 616c 6964 6174 696f   cross-validatio
+00007e80: 6e2c 2064 6566 6175 6c74 7320 746f 2031  n, defaults to 1
+00007e90: 3030 0d0a 2020 2020 2020 2020 3a74 7970  00..        :typ
+00007ea0: 6520 6e5f 666f 6c64 733a 2069 6e74 2c20  e n_folds: int, 
+00007eb0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00007ec0: 2020 2222 220d 0a20 2020 2020 2020 206c    """..        l
+00007ed0: 6f67 6769 6e67 2e69 6e66 6f28 6622 496d  ogging.info(f"Im
+00007ee0: 7075 7469 6e67 2064 6174 6120 7769 7468  puting data with
+00007ef0: 207a 6572 6f73 2229 0d0a 2020 2020 2020   zeros")..      
+00007f00: 2020 0d0a 2020 2020 2020 2020 696d 7075    ..        impu
+00007f10: 7465 7220 3d20 5369 6d70 6c65 496d 7075  ter = SimpleImpu
+00007f20: 7465 7228 7374 7261 7465 6779 3d22 636f  ter(strategy="co
+00007f30: 6e73 7461 6e74 222c 2066 696c 6c5f 7661  nstant", fill_va
+00007f40: 6c75 653d 302e 302c 206b 6565 705f 656d  lue=0.0, keep_em
+00007f50: 7074 795f 6665 6174 7572 6573 3d54 7275  pty_features=Tru
+00007f60: 6529 0d0a 2020 2020 2020 2020 6966 206e  e)..        if n
+00007f70: 5f66 6f6c 6473 203c 2032 3a0d 0a20 2020  _folds < 2:..   
+00007f80: 2020 2020 2020 2020 206c 6f67 6769 6e67           logging
+00007f90: 2e77 6172 6e69 6e67 2866 226e 5f66 6f6c  .warning(f"n_fol
+00007fa0: 6473 203d 207b 6e5f 666f 6c64 737d 2069  ds = {n_folds} i
+00007fb0: 7320 6c65 7373 2074 6861 6e20 322e 2053  s less than 2. S
+00007fc0: 6b69 7070 696e 6720 6372 6f73 732d 7661  kipping cross-va
+00007fd0: 6c69 6461 7469 6f6e 2e22 290d 0a20 2020  lidation.")..   
+00007fe0: 2020 2020 2020 2020 2063 726f 7373 5f76           cross_v
+00007ff0: 616c 6964 6174 6520 3d20 4661 6c73 650d  alidate = False.
+00008000: 0a20 2020 2020 2020 2069 6620 6372 6f73  .        if cros
+00008010: 735f 7661 6c69 6461 7465 3a0d 0a20 2020  s_validate:..   
+00008020: 2020 2020 2020 2020 2063 7673 7461 7473           cvstats
+00008030: 203d 2073 656c 662e 6372 6f73 735f 7661   = self.cross_va
+00008040: 6c69 6461 7465 5f69 6d70 7574 6174 696f  lidate_imputatio
+00008050: 6e28 696d 7075 7465 723d 696d 7075 7465  n(imputer=impute
+00008060: 722c 206e 5f66 6f6c 6473 3d6e 5f66 6f6c  r, n_folds=n_fol
+00008070: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
+00008080: 2073 656c 662e 6164 6174 612e 7661 7220   self.adata.var 
+00008090: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
+000080a0: 2e6a 6f69 6e28 6376 7374 6174 732c 2076  .join(cvstats, v
+000080b0: 616c 6964 6174 653d 2231 3a31 2229 0d0a  alidate="1:1")..
+000080c0: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+000080d0: 7461 2e58 203d 2069 6d70 7574 6572 2e66  ta.X = imputer.f
+000080e0: 6974 5f74 7261 6e73 666f 726d 2873 656c  it_transform(sel
+000080f0: 662e 6164 6174 612e 5829 0d0a 2020 2020  f.adata.X)..    
+00008100: 2020 2020 7365 6c66 2e61 7070 656e 645f      self.append_
+00008110: 746f 5f68 6973 746f 7279 2866 225a 6572  to_history(f"Zer
+00008120: 6f20 696d 7075 7461 7469 6f6e 2229 0d0a  o imputation")..
+00008130: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+00008140: 7461 2e75 6e73 5b22 696d 7075 7461 7469  ta.uns["imputati
+00008150: 6f6e 225d 203d 207b 226d 6574 686f 6422  on"] = {"method"
+00008160: 3a20 227a 6572 6f22 2c0d 0a20 2020 2020  : "zero",..     
 00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008190: 2020 2263 726f 7373 5f76 616c 6964 6174    "cross_validat
-000081a0: 696f 6e22 3a20 6372 6f73 735f 7661 6c69  ion": cross_vali
-000081b0: 6461 7465 7d0d 0a20 2020 2020 2020 2069  date}..        i
-000081c0: 6620 6372 6f73 735f 7661 6c69 6461 7465  f cross_validate
-000081d0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000081e0: 656c 662e 6164 6174 612e 756e 735b 2269  elf.adata.uns["i
-000081f0: 6d70 7574 6174 696f 6e22 5d5b 226e 5f66  mputation"]["n_f
-00008200: 6f6c 6473 225d 203d 206e 5f66 6f6c 6473  olds"] = n_folds
-00008210: 0d0a 0d0a 2020 2020 6465 6620 6d6f 6465  ....    def mode
-00008220: 6c5f 6f76 6572 6469 7370 6572 7365 645f  l_overdispersed_
-00008230: 6765 6e65 7328 7365 6c66 2c20 6f64 675f  genes(self, odg_
-00008240: 6465 6661 756c 745f 7370 6c69 6e65 5f64  default_spline_d
-00008250: 6567 7265 653a 2069 6e74 203d 2033 2c20  egree: int = 3, 
-00008260: 6f64 675f 6465 6661 756c 745f 646f 663a  odg_default_dof:
-00008270: 2069 6e74 203d 2038 2c20 6d61 785f 6d69   int = 8, max_mi
-00008280: 7373 696e 676e 6573 733a 2066 6c6f 6174  ssingness: float
-00008290: 203d 2030 2e35 293a 0d0a 2020 2020 2020   = 0.5):..      
-000082a0: 2020 2222 220d 0a20 2020 2020 2020 2043    """..        C
-000082b0: 6f6d 7075 7465 7320 6765 6e65 2073 7461  omputes gene sta
-000082c0: 7469 7374 6963 7320 616e 6420 6669 7473  tistics and fits
-000082d0: 2074 776f 206d 6f64 656c 7320 6f66 206d   two models of m
-000082e0: 6561 6e20 616e 6420 7661 7269 616e 6365  ean and variance
-000082f0: 206f 6620 6765 6e65 7320 696e 2074 6865   of genes in the
-00008300: 2064 6174 6173 6574 2e20 5468 6520 6669   dataset. The fi
-00008310: 7273 7420 6d65 7468 6f64 2069 7320 7468  rst method is th
-00008320: 650d 0a20 2020 2020 2020 2067 656e 6572  e..        gener
-00008330: 616c 697a 6564 2061 6464 6974 6976 6520  alized additive 
-00008340: 6d6f 6465 6c20 7769 7468 2073 6d6f 6f74  model with smoot
-00008350: 6820 636f 6d70 6f6e 656e 7473 2028 422d  h components (B-
-00008360: 7370 6c69 6e65 7329 2074 6f20 6d6f 6465  splines) to mode
-00008370: 6c20 7468 6520 7265 6c61 7469 6f6e 7368  l the relationsh
-00008380: 6970 206f 6620 6d65 616e 2061 6e64 2076  ip of mean and v
-00008390: 6172 6961 6e63 650d 0a20 2020 2020 2020  ariance..       
-000083a0: 2062 6574 7765 656e 2067 656e 6573 2069   between genes i
-000083b0: 6e20 7468 6520 6461 7461 7365 742e 2049  n the dataset. I
-000083c0: 7420 7072 6f64 7563 6573 2061 6e20 6f64  t produces an od
-000083d0: 7363 6f72 6520 6d65 7472 6963 2066 6f72  score metric for
-000083e0: 206f 7665 7264 6973 7065 7273 696f 6e2e   overdispersion.
-000083f0: 2054 6865 2073 6563 6f6e 6420 6973 2074   The second is t
-00008400: 6865 2063 6f75 6e74 2d73 7461 7469 7374  he count-statist
-00008410: 6963 730d 0a20 2020 2020 2020 206d 6574  ics..        met
-00008420: 686f 6420 666f 756e 6420 696e 2074 6865  hod found in the
-00008430: 2063 4e4d 4620 7061 636b 6167 652c 2077   cNMF package, w
-00008440: 6869 6368 2070 726f 6475 6365 7320 6120  hich produces a 
-00008450: 6d6f 6469 6669 6564 2076 2d73 636f 7265  modified v-score
-00008460: 206d 6574 7269 632e 2041 6c6c 2067 656e   metric. All gen
-00008470: 6520 7374 6174 6973 7469 6373 2061 7265  e statistics are
-00008480: 2073 746f 7265 6420 7769 7468 696e 2074   stored within t
-00008490: 6865 0d0a 2020 2020 2020 2020 6461 7461  he..        data
-000084a0: 7365 7420 6f62 6a65 6374 2061 6e64 2061  set object and a
-000084b0: 7265 2061 6363 6573 7369 626c 6520 7573  re accessible us
-000084c0: 696e 6720 6064 6174 6173 6574 2e61 6e6e  ing `dataset.ann
-000084d0: 6461 7461 2e76 6172 602e 0d0a 0d0a 2020  data.var`.....  
-000084e0: 2020 2020 2020 3a70 6172 616d 206f 6467        :param odg
-000084f0: 5f64 6566 6175 6c74 5f73 706c 696e 655f  _default_spline_
-00008500: 6465 6772 6565 3a20 422d 5370 6c69 6e65  degree: B-Spline
-00008510: 2064 6567 7265 6520 666f 7220 474c 4d2d   degree for GLM-
-00008520: 4741 4d20 6d6f 6465 6c6c 696e 6720 6f66  GAM modelling of
-00008530: 206d 6561 6e2d 7661 7269 616e 6365 2072   mean-variance r
-00008540: 656c 6174 696f 6e73 6869 702c 2064 6566  elationship, def
-00008550: 6175 6c74 7320 746f 2033 0d0a 2020 2020  aults to 3..    
-00008560: 2020 2020 3a74 7970 6520 6f64 675f 6465      :type odg_de
-00008570: 6661 756c 745f 7370 6c69 6e65 5f64 6567  fault_spline_deg
-00008580: 7265 653a 2069 6e74 2c20 6f70 7469 6f6e  ree: int, option
-00008590: 616c 0d0a 2020 2020 2020 2020 3a70 6172  al..        :par
-000085a0: 616d 206f 6467 5f64 6566 6175 6c74 5f64  am odg_default_d
-000085b0: 6f66 3a20 4465 6772 6565 7320 6f66 2066  of: Degrees of f
-000085c0: 7265 6564 6f6d 2066 6f72 2047 4c4d 2d47  reedom for GLM-G
-000085d0: 414d 206d 6f64 656c 6c69 6e67 206f 6620  AM modelling of 
-000085e0: 6d65 616e 2d76 6172 616e 6365 2c20 6465  mean-varance, de
-000085f0: 6661 756c 7473 2074 6f20 380d 0a20 2020  faults to 8..   
-00008600: 2020 2020 203a 7479 7065 206f 6467 5f64       :type odg_d
-00008610: 6566 6175 6c74 5f64 6f66 3a20 696e 742c  efault_dof: int,
-00008620: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-00008630: 2020 203a 7061 7261 6d20 6d61 785f 6d69     :param max_mi
-00008640: 7373 696e 676e 6573 733a 2045 7863 6c75  ssingness: Exclu
-00008650: 6465 2066 6561 7475 7265 7320 7769 7468  de features with
-00008660: 2068 6967 6820 7072 652d 696d 7075 7461   high pre-imputa
-00008670: 7469 6f6e 206d 6973 7369 6e67 6e65 7373  tion missingness
-00008680: 2e20 5661 6c75 6520 6d75 7374 2062 6520  . Value must be 
-00008690: 6265 7477 6565 6e20 3020 616e 6420 312c  between 0 and 1,
-000086a0: 2064 6566 6175 6c74 7320 746f 2030 2e35   defaults to 0.5
-000086b0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-000086c0: 6d61 785f 6d69 7373 696e 676e 6573 733a  max_missingness:
-000086d0: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
-000086e0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000086f0: 2020 2020 2020 2064 6174 615f 7261 7720         data_raw 
-00008700: 3d20 7365 6c66 2e74 6f5f 6466 2829 0d0a  = self.to_df()..
-00008710: 2020 2020 2020 2020 6461 7461 5f6e 6f72          data_nor
-00008720: 6d61 6c69 7a65 6420 3d20 7365 6c66 2e74  malized = self.t
-00008730: 6f5f 6466 286e 6f72 6d61 6c69 7a65 643d  o_df(normalized=
-00008740: 5472 7565 290d 0a20 2020 2020 2020 200d  True)..        .
-00008750: 0a20 2020 2020 2020 2023 2063 7265 6174  .        # creat
-00008760: 6520 6461 7461 6672 616d 6520 6f66 2070  e dataframe of p
-00008770: 6572 2d67 656e 6520 7374 6174 6973 7469  er-gene statisti
-00008780: 6373 0d0a 2020 2020 2020 2020 7365 6c66  cs..        self
-00008790: 2e61 6461 7461 2e76 6172 5b22 6d65 616e  .adata.var["mean
-000087a0: 225d 203d 2064 6174 615f 6e6f 726d 616c  "] = data_normal
-000087b0: 697a 6564 2e6d 6561 6e28 290d 0a20 2020  ized.mean()..   
-000087c0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-000087d0: 7661 725b 2272 616e 6b5f 6d65 616e 225d  var["rank_mean"]
-000087e0: 203d 2073 656c 662e 6164 6174 612e 7661   = self.adata.va
-000087f0: 725b 226d 6561 6e22 5d2e 7261 6e6b 2829  r["mean"].rank()
-00008800: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00008810: 6461 7461 2e76 6172 5b22 7661 7269 616e  data.var["varian
-00008820: 6365 225d 203d 2064 6174 615f 6e6f 726d  ce"] = data_norm
-00008830: 616c 697a 6564 2e76 6172 2829 0d0a 2020  alized.var()..  
-00008840: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
-00008850: 2e76 6172 5b22 7364 225d 203d 2064 6174  .var["sd"] = dat
-00008860: 615f 6e6f 726d 616c 697a 6564 2e73 7464  a_normalized.std
-00008870: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-00008880: 2e61 6461 7461 2e76 6172 5b5b 226c 6f67  .adata.var[["log
-00008890: 5f6d 6561 6e22 2c20 226c 6f67 5f76 6172  _mean", "log_var
-000088a0: 6961 6e63 6522 5d5d 203d 206e 702e 6c6f  iance"]] = np.lo
-000088b0: 6731 3028 7365 6c66 2e61 6461 7461 2e76  g10(self.adata.v
-000088c0: 6172 5b5b 226d 6561 6e22 2c20 2276 6172  ar[["mean", "var
-000088d0: 6961 6e63 6522 5d5d 290d 0a20 2020 2020  iance"]])..     
-000088e0: 2020 2073 656c 662e 6164 6174 612e 7661     self.adata.va
-000088f0: 725b 226d 6561 6e5f 636f 756e 7473 225d  r["mean_counts"]
-00008900: 203d 2064 6174 615f 7261 772e 6d65 616e   = data_raw.mean
-00008910: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-00008920: 2e61 6461 7461 2e76 6172 5b22 6f64 7363  .adata.var["odsc
-00008930: 6f72 655f 6578 636c 7564 6564 225d 203d  ore_excluded"] =
-00008940: 2028 2873 656c 662e 6164 6174 612e 7661   ((self.adata.va
-00008950: 725b 226d 6973 7369 6e67 6e65 7373 225d  r["missingness"]
-00008960: 203e 206d 6178 5f6d 6973 7369 6e67 6e65   > max_missingne
-00008970: 7373 2920 7c0d 0a20 2020 2020 2020 2020  ss) |..         
+00008190: 2020 2022 6372 6f73 735f 7661 6c69 6461     "cross_valida
+000081a0: 7469 6f6e 223a 2063 726f 7373 5f76 616c  tion": cross_val
+000081b0: 6964 6174 657d 0d0a 2020 2020 2020 2020  idate}..        
+000081c0: 6966 2063 726f 7373 5f76 616c 6964 6174  if cross_validat
+000081d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000081e0: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
+000081f0: 696d 7075 7461 7469 6f6e 225d 5b22 6e5f  imputation"]["n_
+00008200: 666f 6c64 7322 5d20 3d20 6e5f 666f 6c64  folds"] = n_fold
+00008210: 730d 0a0d 0a20 2020 2064 6566 206d 6f64  s....    def mod
+00008220: 656c 5f6f 7665 7264 6973 7065 7273 6564  el_overdispersed
+00008230: 5f67 656e 6573 2873 656c 662c 206f 6467  _genes(self, odg
+00008240: 5f64 6566 6175 6c74 5f73 706c 696e 655f  _default_spline_
+00008250: 6465 6772 6565 3a20 696e 7420 3d20 332c  degree: int = 3,
+00008260: 206f 6467 5f64 6566 6175 6c74 5f64 6f66   odg_default_dof
+00008270: 3a20 696e 7420 3d20 382c 206d 6178 5f6d  : int = 8, max_m
+00008280: 6973 7369 6e67 6e65 7373 3a20 666c 6f61  issingness: floa
+00008290: 7420 3d20 302e 3529 3a0d 0a20 2020 2020  t = 0.5):..     
+000082a0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000082b0: 436f 6d70 7574 6573 2067 656e 6520 7374  Computes gene st
+000082c0: 6174 6973 7469 6373 2061 6e64 2066 6974  atistics and fit
+000082d0: 7320 7477 6f20 6d6f 6465 6c73 206f 6620  s two models of 
+000082e0: 6d65 616e 2061 6e64 2076 6172 6961 6e63  mean and varianc
+000082f0: 6520 6f66 2067 656e 6573 2069 6e20 7468  e of genes in th
+00008300: 6520 6461 7461 7365 742e 2054 6865 2066  e dataset. The f
+00008310: 6972 7374 206d 6574 686f 6420 6973 2074  irst method is t
+00008320: 6865 0d0a 2020 2020 2020 2020 6765 6e65  he..        gene
+00008330: 7261 6c69 7a65 6420 6164 6469 7469 7665  ralized additive
+00008340: 206d 6f64 656c 2077 6974 6820 736d 6f6f   model with smoo
+00008350: 7468 2063 6f6d 706f 6e65 6e74 7320 2842  th components (B
+00008360: 2d73 706c 696e 6573 2920 746f 206d 6f64  -splines) to mod
+00008370: 656c 2074 6865 2072 656c 6174 696f 6e73  el the relations
+00008380: 6869 7020 6f66 206d 6561 6e20 616e 6420  hip of mean and 
+00008390: 7661 7269 616e 6365 0d0a 2020 2020 2020  variance..      
+000083a0: 2020 6265 7477 6565 6e20 6765 6e65 7320    between genes 
+000083b0: 696e 2074 6865 2064 6174 6173 6574 2e20  in the dataset. 
+000083c0: 4974 2070 726f 6475 6365 7320 616e 206f  It produces an o
+000083d0: 6473 636f 7265 206d 6574 7269 6320 666f  dscore metric fo
+000083e0: 7220 6f76 6572 6469 7370 6572 7369 6f6e  r overdispersion
+000083f0: 2e20 5468 6520 7365 636f 6e64 2069 7320  . The second is 
+00008400: 7468 6520 636f 756e 742d 7374 6174 6973  the count-statis
+00008410: 7469 6373 0d0a 2020 2020 2020 2020 6d65  tics..        me
+00008420: 7468 6f64 2066 6f75 6e64 2069 6e20 7468  thod found in th
+00008430: 6520 634e 4d46 2070 6163 6b61 6765 2c20  e cNMF package, 
+00008440: 7768 6963 6820 7072 6f64 7563 6573 2061  which produces a
+00008450: 206d 6f64 6966 6965 6420 762d 7363 6f72   modified v-scor
+00008460: 6520 6d65 7472 6963 2e20 416c 6c20 6765  e metric. All ge
+00008470: 6e65 2073 7461 7469 7374 6963 7320 6172  ne statistics ar
+00008480: 6520 7374 6f72 6564 2077 6974 6869 6e20  e stored within 
+00008490: 7468 650d 0a20 2020 2020 2020 2064 6174  the..        dat
+000084a0: 6173 6574 206f 626a 6563 7420 616e 6420  aset object and 
+000084b0: 6172 6520 6163 6365 7373 6962 6c65 2075  are accessible u
+000084c0: 7369 6e67 2060 6461 7461 7365 742e 616e  sing `dataset.an
+000084d0: 6e64 6174 612e 7661 7260 2e0d 0a0d 0a20  ndata.var`..... 
+000084e0: 2020 2020 2020 203a 7061 7261 6d20 6f64         :param od
+000084f0: 675f 6465 6661 756c 745f 7370 6c69 6e65  g_default_spline
+00008500: 5f64 6567 7265 653a 2042 2d53 706c 696e  _degree: B-Splin
+00008510: 6520 6465 6772 6565 2066 6f72 2047 4c4d  e degree for GLM
+00008520: 2d47 414d 206d 6f64 656c 6c69 6e67 206f  -GAM modelling o
+00008530: 6620 6d65 616e 2d76 6172 6961 6e63 6520  f mean-variance 
+00008540: 7265 6c61 7469 6f6e 7368 6970 2c20 6465  relationship, de
+00008550: 6661 756c 7473 2074 6f20 330d 0a20 2020  faults to 3..   
+00008560: 2020 2020 203a 7479 7065 206f 6467 5f64       :type odg_d
+00008570: 6566 6175 6c74 5f73 706c 696e 655f 6465  efault_spline_de
+00008580: 6772 6565 3a20 696e 742c 206f 7074 696f  gree: int, optio
+00008590: 6e61 6c0d 0a20 2020 2020 2020 203a 7061  nal..        :pa
+000085a0: 7261 6d20 6f64 675f 6465 6661 756c 745f  ram odg_default_
+000085b0: 646f 663a 2044 6567 7265 6573 206f 6620  dof: Degrees of 
+000085c0: 6672 6565 646f 6d20 666f 7220 474c 4d2d  freedom for GLM-
+000085d0: 4741 4d20 6d6f 6465 6c6c 696e 6720 6f66  GAM modelling of
+000085e0: 206d 6561 6e2d 7661 7261 6e63 652c 2064   mean-varance, d
+000085f0: 6566 6175 6c74 7320 746f 2038 0d0a 2020  efaults to 8..  
+00008600: 2020 2020 2020 3a74 7970 6520 6f64 675f        :type odg_
+00008610: 6465 6661 756c 745f 646f 663a 2069 6e74  default_dof: int
+00008620: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00008630: 2020 2020 3a70 6172 616d 206d 6178 5f6d      :param max_m
+00008640: 6973 7369 6e67 6e65 7373 3a20 4578 636c  issingness: Excl
+00008650: 7564 6520 6665 6174 7572 6573 2077 6974  ude features wit
+00008660: 6820 6869 6768 2070 7265 2d69 6d70 7574  h high pre-imput
+00008670: 6174 696f 6e20 6d69 7373 696e 676e 6573  ation missingnes
+00008680: 732e 2056 616c 7565 206d 7573 7420 6265  s. Value must be
+00008690: 2062 6574 7765 656e 2030 2061 6e64 2031   between 0 and 1
+000086a0: 2c20 6465 6661 756c 7473 2074 6f20 302e  , defaults to 0.
+000086b0: 350d 0a20 2020 2020 2020 203a 7479 7065  5..        :type
+000086c0: 206d 6178 5f6d 6973 7369 6e67 6e65 7373   max_missingness
+000086d0: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
+000086e0: 6c0d 0a20 2020 2020 2020 2022 2222 0d0a  l..        """..
+000086f0: 2020 2020 2020 2020 6461 7461 5f72 6177          data_raw
+00008700: 203d 2073 656c 662e 746f 5f64 6628 290d   = self.to_df().
+00008710: 0a20 2020 2020 2020 2064 6174 615f 6e6f  .        data_no
+00008720: 726d 616c 697a 6564 203d 2073 656c 662e  rmalized = self.
+00008730: 746f 5f64 6628 6e6f 726d 616c 697a 6564  to_df(normalized
+00008740: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00008750: 0d0a 2020 2020 2020 2020 2320 6372 6561  ..        # crea
+00008760: 7465 2064 6174 6166 7261 6d65 206f 6620  te dataframe of 
+00008770: 7065 722d 6765 6e65 2073 7461 7469 7374  per-gene statist
+00008780: 6963 730d 0a20 2020 2020 2020 2073 656c  ics..        sel
+00008790: 662e 6164 6174 612e 7661 725b 226d 6561  f.adata.var["mea
+000087a0: 6e22 5d20 3d20 6461 7461 5f6e 6f72 6d61  n"] = data_norma
+000087b0: 6c69 7a65 642e 6d65 616e 2829 0d0a 2020  lized.mean()..  
+000087c0: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
+000087d0: 2e76 6172 5b22 7261 6e6b 5f6d 6561 6e22  .var["rank_mean"
+000087e0: 5d20 3d20 7365 6c66 2e61 6461 7461 2e76  ] = self.adata.v
+000087f0: 6172 5b22 6d65 616e 225d 2e72 616e 6b28  ar["mean"].rank(
+00008800: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008810: 6164 6174 612e 7661 725b 2276 6172 6961  adata.var["varia
+00008820: 6e63 6522 5d20 3d20 6461 7461 5f6e 6f72  nce"] = data_nor
+00008830: 6d61 6c69 7a65 642e 7661 7228 290d 0a20  malized.var().. 
+00008840: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+00008850: 612e 7661 725b 2273 6422 5d20 3d20 6461  a.var["sd"] = da
+00008860: 7461 5f6e 6f72 6d61 6c69 7a65 642e 7374  ta_normalized.st
+00008870: 6428 290d 0a20 2020 2020 2020 2073 656c  d()..        sel
+00008880: 662e 6164 6174 612e 7661 725b 5b22 6c6f  f.adata.var[["lo
+00008890: 675f 6d65 616e 222c 2022 6c6f 675f 7661  g_mean", "log_va
+000088a0: 7269 616e 6365 225d 5d20 3d20 6e70 2e6c  riance"]] = np.l
+000088b0: 6f67 3130 2873 656c 662e 6164 6174 612e  og10(self.adata.
+000088c0: 7661 725b 5b22 6d65 616e 222c 2022 7661  var[["mean", "va
+000088d0: 7269 616e 6365 225d 5d29 0d0a 2020 2020  riance"]])..    
+000088e0: 2020 2020 7365 6c66 2e61 6461 7461 2e76      self.adata.v
+000088f0: 6172 5b22 6d65 616e 5f63 6f75 6e74 7322  ar["mean_counts"
+00008900: 5d20 3d20 6461 7461 5f72 6177 2e6d 6561  ] = data_raw.mea
+00008910: 6e28 290d 0a20 2020 2020 2020 2073 656c  n()..        sel
+00008920: 662e 6164 6174 612e 7661 725b 226f 6473  f.adata.var["ods
+00008930: 636f 7265 5f65 7863 6c75 6465 6422 5d20  core_excluded"] 
+00008940: 3d20 2828 7365 6c66 2e61 6461 7461 2e76  = ((self.adata.v
+00008950: 6172 5b22 6d69 7373 696e 676e 6573 7322  ar["missingness"
+00008960: 5d20 3e20 6d61 785f 6d69 7373 696e 676e  ] > max_missingn
+00008970: 6573 7329 207c 0d0a 2020 2020 2020 2020  ess) |..        
 00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089a0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-000089b0: 7661 725b 226c 6f67 5f6d 6561 6e22 5d2e  var["log_mean"].
-000089c0: 6973 6e75 6c6c 2829 207c 0d0a 2020 2020  isnull() |..    
+000089a0: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
+000089b0: 2e76 6172 5b22 6c6f 675f 6d65 616e 225d  .var["log_mean"]
+000089c0: 2e69 736e 756c 6c28 2920 7c0d 0a20 2020  .isnull() |..   
 000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089f0: 2020 2020 2020 2020 2020 2873 656c 662e            (self.
-00008a00: 6164 6174 612e 7661 725b 226d 6561 6e22  adata.var["mean"
-00008a10: 5d20 3d3d 2030 2920 7c0d 0a20 2020 2020  ] == 0) |..     
+000089f0: 2020 2020 2020 2020 2020 2028 7365 6c66             (self
+00008a00: 2e61 6461 7461 2e76 6172 5b22 6d65 616e  .adata.var["mean
+00008a10: 225d 203d 3d20 3029 207c 0d0a 2020 2020  "] == 0) |..    
 00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a40: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
-00008a50: 6174 612e 7661 725b 226c 6f67 5f76 6172  ata.var["log_var
-00008a60: 6961 6e63 6522 5d2e 6973 6e75 6c6c 2829  iance"].isnull()
-00008a70: 290d 0a0d 0a20 2020 2020 2020 2023 206d  )....        # m
-00008a80: 6f64 656c 206d 6561 6e2d 7661 7269 616e  odel mean-varian
-00008a90: 6365 2072 656c 6174 696f 6e73 6869 7020  ce relationship 
-00008aa0: 7573 696e 6720 6765 6e65 7261 6c69 7a65  using generalize
-00008ab0: 6420 6164 6469 7469 7665 206d 6f64 656c  d additive model
-00008ac0: 2077 6974 6820 736d 6f6f 7468 2063 6f6d   with smooth com
-00008ad0: 706f 6e65 6e74 730d 0a20 2020 2020 2020  ponents..       
-00008ae0: 2064 665f 6d6f 6465 6c20 3d20 7365 6c66   df_model = self
-00008af0: 2e61 6461 7461 2e76 6172 5b7e 7365 6c66  .adata.var[~self
-00008b00: 2e61 6461 7461 2e76 6172 5b22 6f64 7363  .adata.var["odsc
-00008b10: 6f72 655f 6578 636c 7564 6564 225d 5d0d  ore_excluded"]].
-00008b20: 0a20 2020 2020 2020 2062 7320 3d20 4253  .        bs = BS
-00008b30: 706c 696e 6573 2864 665f 6d6f 6465 6c5b  plines(df_model[
-00008b40: 226d 6561 6e22 5d2c 2064 663d 6f64 675f  "mean"], df=odg_
-00008b50: 6465 6661 756c 745f 646f 662c 2064 6567  default_dof, deg
-00008b60: 7265 653d 6f64 675f 6465 6661 756c 745f  ree=odg_default_
-00008b70: 7370 6c69 6e65 5f64 6567 7265 6529 0d0a  spline_degree)..
-00008b80: 2020 2020 2020 2020 6761 6d20 3d20 474c          gam = GL
-00008b90: 4d47 616d 2e66 726f 6d5f 666f 726d 756c  MGam.from_formul
-00008ba0: 6128 226c 6f67 5f76 6172 6961 6e63 6520  a("log_variance 
-00008bb0: 7e20 6c6f 675f 6d65 616e 222c 2064 6174  ~ log_mean", dat
-00008bc0: 613d 6466 5f6d 6f64 656c 2c20 736d 6f6f  a=df_model, smoo
-00008bd0: 7468 6572 3d62 7329 2e66 6974 2829 0d0a  ther=bs).fit()..
-00008be0: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
-00008bf0: 7461 2e76 6172 5b22 7265 7369 645f 6c6f  ta.var["resid_lo
-00008c00: 675f 7661 7269 616e 6365 225d 203d 2067  g_variance"] = g
-00008c10: 616d 2e72 6573 6964 5f72 6573 706f 6e73  am.resid_respons
-00008c20: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00008c30: 6164 6174 612e 7661 725b 226f 6473 636f  adata.var["odsco
-00008c40: 7265 225d 203d 206e 702e 7371 7274 2831  re"] = np.sqrt(1
-00008c50: 3020 2a2a 2073 656c 662e 6164 6174 612e  0 ** self.adata.
-00008c60: 7661 725b 2272 6573 6964 5f6c 6f67 5f76  var["resid_log_v
-00008c70: 6172 6961 6e63 6522 5d29 0d0a 2020 2020  ariance"])..    
-00008c80: 2020 2020 7365 6c66 2e61 6461 7461 2e76      self.adata.v
-00008c90: 6172 5b22 6761 6d5f 6669 7474 6564 7661  ar["gam_fittedva
-00008ca0: 6c75 6573 225d 203d 2067 616d 2e66 6974  lues"] = gam.fit
-00008cb0: 7465 6476 616c 7565 730d 0a0d 0a0d 0a20  tedvalues...... 
-00008cc0: 2020 2020 2020 2023 206d 6f64 656c 206d         # model m
-00008cd0: 6561 6e2d 7661 7269 616e 6365 2072 656c  ean-variance rel
-00008ce0: 6174 696f 6e73 6869 7020 7573 696e 6720  ationship using 
-00008cf0: 634e 4d46 2773 206d 6574 686f 6420 6261  cNMF's method ba
-00008d00: 7365 6420 6f6e 2076 2d73 636f 7265 2061  sed on v-score a
-00008d10: 6e64 206d 696e 696d 756d 2065 7870 7265  nd minimum expre
-00008d20: 7373 696f 6e20 7468 7265 7368 6f6c 640d  ssion threshold.
-00008d30: 0a20 2020 2020 2020 2076 7363 6f72 655f  .        vscore_
-00008d40: 7374 6174 7320 3d20 7064 2e44 6174 6146  stats = pd.DataF
-00008d50: 7261 6d65 2863 6e6d 662e 6765 745f 6869  rame(cnmf.get_hi
-00008d60: 6768 7661 725f 6765 6e65 7328 696e 7075  ghvar_genes(inpu
-00008d70: 745f 636f 756e 7473 3d64 6174 615f 6e6f  t_counts=data_no
-00008d80: 726d 616c 697a 6564 2e76 616c 7565 732c  rmalized.values,
-00008d90: 206d 696e 696d 616c 5f6d 6561 6e3d 3029   minimal_mean=0)
-00008da0: 5b30 5d29 0d0a 2020 2020 2020 2020 7673  [0])..        vs
-00008db0: 636f 7265 5f73 7461 7473 2e69 6e64 6578  core_stats.index
-00008dc0: 203d 2064 6174 615f 6e6f 726d 616c 697a   = data_normaliz
-00008dd0: 6564 2e63 6f6c 756d 6e73 0d0a 2020 2020  ed.columns..    
-00008de0: 2020 2020 7365 6c66 2e61 6461 7461 2e76      self.adata.v
-00008df0: 6172 5b22 7673 636f 7265 225d 203d 2076  ar["vscore"] = v
-00008e00: 7363 6f72 655f 7374 6174 735b 2266 616e  score_stats["fan
-00008e10: 6f5f 7261 7469 6f22 5d0d 0a20 2020 2020  o_ratio"]..     
-00008e20: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
-00008e30: 735b 226f 6467 225d 5b22 6f64 675f 6465  s["odg"]["odg_de
-00008e40: 6661 756c 745f 7370 6c69 6e65 5f64 6567  fault_spline_deg
-00008e50: 7265 6522 5d20 3d20 6f64 675f 6465 6661  ree"] = odg_defa
-00008e60: 756c 745f 7370 6c69 6e65 5f64 6567 7265  ult_spline_degre
-00008e70: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00008e80: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
-00008e90: 5b22 6f64 675f 6465 6661 756c 745f 646f  ["odg_default_do
-00008ea0: 6622 5d20 3d20 6f64 675f 6465 6661 756c  f"] = odg_defaul
-00008eb0: 745f 646f 660d 0a20 2020 2020 2020 2073  t_dof..        s
-00008ec0: 656c 662e 6170 7065 6e64 5f74 6f5f 6869  elf.append_to_hi
-00008ed0: 7374 6f72 7928 2247 656e 652d 6c65 7665  story("Gene-leve
-00008ee0: 6c20 7374 6174 6973 7469 6373 2061 6e64  l statistics and
-00008ef0: 206f 7665 7264 6973 7065 7273 696f 6e20   overdispersion 
-00008f00: 6d6f 6465 6c6c 696e 6720 636f 6d70 6c65  modelling comple
-00008f10: 7465 642e 2229 0d0a 2020 2020 2020 2020  ted.")..        
-00008f20: 0d0a 2020 2020 6465 6620 7365 6c65 6374  ..    def select
-00008f30: 5f6f 7665 7264 6973 7065 7273 6564 5f67  _overdispersed_g
-00008f40: 656e 6573 5f66 726f 6d5f 6765 6e65 6c69  enes_from_geneli
-00008f50: 7374 2873 656c 662c 2067 656e 6573 3a20  st(self, genes: 
-00008f60: 436f 6c6c 6563 7469 6f6e 5b73 7472 5d2c  Collection[str],
-00008f70: 206d 696e 5f6d 6561 6e3d 3029 3a0d 0a20   min_mean=0):.. 
-00008f80: 2020 2020 2020 2022 2222 5365 6c65 6374         """Select
-00008f90: 206f 7665 7264 6973 7065 7273 6564 2067   overdispersed g
-00008fa0: 656e 6573 2f66 6561 7475 7265 7320 7573  enes/features us
-00008fb0: 696e 6720 6120 6375 7374 6f6d 206c 6973  ing a custom lis
-00008fc0: 742e 2047 656e 6573 2f66 6561 7475 7265  t. Genes/feature
-00008fd0: 7320 6e6f 7420 7072 6573 656e 7420 696e  s not present in
-00008fe0: 2074 6865 2064 6174 6173 6574 2061 7265   the dataset are
-00008ff0: 2061 7574 6f6d 6174 6963 616c 6c79 2066   automatically f
-00009000: 696c 7465 7265 6420 6f75 742e 0d0a 0d0a  iltered out.....
-00009010: 2020 2020 2020 2020 3a70 6172 616d 2067          :param g
-00009020: 656e 6573 3a20 6765 6e65 206c 6973 740d  enes: gene list.
-00009030: 0a20 2020 2020 2020 203a 7479 7065 2067  .        :type g
-00009040: 656e 6573 3a20 436f 6c6c 6563 7469 6f6e  enes: Collection
-00009050: 5b73 7472 5d0d 0a20 2020 2020 2020 203a  [str]..        :
-00009060: 7061 7261 6d20 6d69 6e5f 6d65 616e 3a20  param min_mean: 
-00009070: 6d69 6e69 6d75 6d20 6765 6e65 2065 7870  minimum gene exp
-00009080: 7265 7373 696f 6e20 666f 7220 6765 6e65  ression for gene
-00009090: 7320 746f 2062 6520 636f 756e 7465 6420  s to be counted 
-000090a0: 6173 206f 7665 7264 6973 7065 7273 6564  as overdispersed
-000090b0: 2c20 6465 6661 756c 7473 2074 6f20 300d  , defaults to 0.
-000090c0: 0a20 2020 2020 2020 203a 7479 7065 206d  .        :type m
-000090d0: 696e 5f6d 6561 6e3a 2069 6e74 2c20 6f70  in_mean: int, op
-000090e0: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-000090f0: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-00009100: 662e 6164 6174 612e 7661 725b 2273 656c  f.adata.var["sel
-00009110: 6563 7465 6422 5d20 3d20 7365 6c66 2e61  ected"] = self.a
-00009120: 6461 7461 2e76 6172 2e69 6e64 6578 2e69  data.var.index.i
-00009130: 7369 6e28 6765 6e65 7329 2026 2028 7365  sin(genes) & (se
-00009140: 6c66 2e61 6461 7461 2e76 6172 5b22 6d65  lf.adata.var["me
-00009150: 616e 5f63 6f75 6e74 7322 5d20 3e3d 206d  an_counts"] >= m
-00009160: 696e 5f6d 6561 6e29 0d0a 2020 2020 2020  in_mean)..      
-00009170: 2020 7365 6c66 2e61 6461 7461 2e75 6e73    self.adata.uns
-00009180: 5b22 6f64 6722 5d5b 226f 7665 7264 6973  ["odg"]["overdis
-00009190: 7065 7273 696f 6e5f 6d65 7472 6963 225d  persion_metric"]
-000091a0: 203d 2022 220d 0a20 2020 2020 2020 2073   = ""..        s
-000091b0: 656c 662e 6164 6174 612e 756e 735b 226f  elf.adata.uns["o
-000091c0: 6467 225d 5b22 6d69 6e5f 6d65 616e 225d  dg"]["min_mean"]
-000091d0: 203d 206d 696e 5f6d 6561 6e0d 0a20 2020   = min_mean..   
-000091e0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-000091f0: 756e 735b 226f 6467 225d 5b22 6d69 6e5f  uns["odg"]["min_
-00009200: 7363 6f72 6522 5d20 3d20 2222 0d0a 2020  score"] = ""..  
-00009210: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
-00009220: 2e75 6e73 5b22 6f64 6722 5d5b 2274 6f70  .uns["odg"]["top
-00009230: 5f6e 225d 203d 2022 220d 0a20 2020 2020  _n"] = ""..     
-00009240: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
-00009250: 735b 226f 6467 225d 5b22 7175 616e 7469  s["odg"]["quanti
-00009260: 6c65 225d 203d 2022 220d 0a20 2020 2020  le"] = ""..     
-00009270: 2020 2073 656c 662e 6170 7065 6e64 5f74     self.append_t
-00009280: 6f5f 6869 7374 6f72 7928 224f 7665 7264  o_history("Overd
-00009290: 6973 7065 7273 6564 2067 656e 6573 2073  ispersed genes s
-000092a0: 656c 6563 7465 6420 6672 6f6d 2063 7573  elected from cus
-000092b0: 746f 6d20 6765 6e65 206c 6973 7422 290d  tom gene list").
-000092c0: 0a20 2020 2020 2020 200d 0a20 2020 2064  .        ..    d
-000092d0: 6566 2073 656c 6563 745f 6f76 6572 6469  ef select_overdi
-000092e0: 7370 6572 7365 645f 6765 6e65 7328 7365  spersed_genes(se
-000092f0: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+00008a40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00008a50: 6461 7461 2e76 6172 5b22 6c6f 675f 7661  data.var["log_va
+00008a60: 7269 616e 6365 225d 2e69 736e 756c 6c28  riance"].isnull(
+00008a70: 2929 0d0a 0d0a 2020 2020 2020 2020 2320  ))....        # 
+00008a80: 6d6f 6465 6c20 6d65 616e 2d76 6172 6961  model mean-varia
+00008a90: 6e63 6520 7265 6c61 7469 6f6e 7368 6970  nce relationship
+00008aa0: 2075 7369 6e67 2067 656e 6572 616c 697a   using generaliz
+00008ab0: 6564 2061 6464 6974 6976 6520 6d6f 6465  ed additive mode
+00008ac0: 6c20 7769 7468 2073 6d6f 6f74 6820 636f  l with smooth co
+00008ad0: 6d70 6f6e 656e 7473 0d0a 2020 2020 2020  mponents..      
+00008ae0: 2020 6466 5f6d 6f64 656c 203d 2073 656c    df_model = sel
+00008af0: 662e 6164 6174 612e 7661 725b 7e73 656c  f.adata.var[~sel
+00008b00: 662e 6164 6174 612e 7661 725b 226f 6473  f.adata.var["ods
+00008b10: 636f 7265 5f65 7863 6c75 6465 6422 5d5d  core_excluded"]]
+00008b20: 0d0a 2020 2020 2020 2020 6273 203d 2042  ..        bs = B
+00008b30: 5370 6c69 6e65 7328 6466 5f6d 6f64 656c  Splines(df_model
+00008b40: 5b22 6d65 616e 225d 2c20 6466 3d6f 6467  ["mean"], df=odg
+00008b50: 5f64 6566 6175 6c74 5f64 6f66 2c20 6465  _default_dof, de
+00008b60: 6772 6565 3d6f 6467 5f64 6566 6175 6c74  gree=odg_default
+00008b70: 5f73 706c 696e 655f 6465 6772 6565 290d  _spline_degree).
+00008b80: 0a20 2020 2020 2020 2067 616d 203d 2047  .        gam = G
+00008b90: 4c4d 4761 6d2e 6672 6f6d 5f66 6f72 6d75  LMGam.from_formu
+00008ba0: 6c61 2822 6c6f 675f 7661 7269 616e 6365  la("log_variance
+00008bb0: 207e 206c 6f67 5f6d 6561 6e22 2c20 6461   ~ log_mean", da
+00008bc0: 7461 3d64 665f 6d6f 6465 6c2c 2073 6d6f  ta=df_model, smo
+00008bd0: 6f74 6865 723d 6273 292e 6669 7428 290d  other=bs).fit().
+00008be0: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+00008bf0: 6174 612e 7661 725b 2272 6573 6964 5f6c  ata.var["resid_l
+00008c00: 6f67 5f76 6172 6961 6e63 6522 5d20 3d20  og_variance"] = 
+00008c10: 6761 6d2e 7265 7369 645f 7265 7370 6f6e  gam.resid_respon
+00008c20: 7365 0d0a 2020 2020 2020 2020 7365 6c66  se..        self
+00008c30: 2e61 6461 7461 2e76 6172 5b22 6f64 7363  .adata.var["odsc
+00008c40: 6f72 6522 5d20 3d20 6e70 2e73 7172 7428  ore"] = np.sqrt(
+00008c50: 3130 202a 2a20 7365 6c66 2e61 6461 7461  10 ** self.adata
+00008c60: 2e76 6172 5b22 7265 7369 645f 6c6f 675f  .var["resid_log_
+00008c70: 7661 7269 616e 6365 225d 290d 0a20 2020  variance"])..   
+00008c80: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00008c90: 7661 725b 2267 616d 5f66 6974 7465 6476  var["gam_fittedv
+00008ca0: 616c 7565 7322 5d20 3d20 6761 6d2e 6669  alues"] = gam.fi
+00008cb0: 7474 6564 7661 6c75 6573 0d0a 0d0a 0d0a  ttedvalues......
+00008cc0: 2020 2020 2020 2020 2320 6d6f 6465 6c20          # model 
+00008cd0: 6d65 616e 2d76 6172 6961 6e63 6520 7265  mean-variance re
+00008ce0: 6c61 7469 6f6e 7368 6970 2075 7369 6e67  lationship using
+00008cf0: 2063 4e4d 4627 7320 6d65 7468 6f64 2062   cNMF's method b
+00008d00: 6173 6564 206f 6e20 762d 7363 6f72 6520  ased on v-score 
+00008d10: 616e 6420 6d69 6e69 6d75 6d20 6578 7072  and minimum expr
+00008d20: 6573 7369 6f6e 2074 6872 6573 686f 6c64  ession threshold
+00008d30: 0d0a 2020 2020 2020 2020 7673 636f 7265  ..        vscore
+00008d40: 5f73 7461 7473 203d 2070 642e 4461 7461  _stats = pd.Data
+00008d50: 4672 616d 6528 636e 6d66 2e67 6574 5f68  Frame(cnmf.get_h
+00008d60: 6967 6876 6172 5f67 656e 6573 2869 6e70  ighvar_genes(inp
+00008d70: 7574 5f63 6f75 6e74 733d 6461 7461 5f6e  ut_counts=data_n
+00008d80: 6f72 6d61 6c69 7a65 642e 7661 6c75 6573  ormalized.values
+00008d90: 2c20 6d69 6e69 6d61 6c5f 6d65 616e 3d30  , minimal_mean=0
+00008da0: 295b 305d 290d 0a20 2020 2020 2020 2076  )[0])..        v
+00008db0: 7363 6f72 655f 7374 6174 732e 696e 6465  score_stats.inde
+00008dc0: 7820 3d20 6461 7461 5f6e 6f72 6d61 6c69  x = data_normali
+00008dd0: 7a65 642e 636f 6c75 6d6e 730d 0a20 2020  zed.columns..   
+00008de0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00008df0: 7661 725b 2276 7363 6f72 6522 5d20 3d20  var["vscore"] = 
+00008e00: 7673 636f 7265 5f73 7461 7473 5b22 6661  vscore_stats["fa
+00008e10: 6e6f 5f72 6174 696f 225d 0d0a 2020 2020  no_ratio"]..    
+00008e20: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
+00008e30: 6e73 5b22 6f64 6722 5d5b 226f 6467 5f64  ns["odg"]["odg_d
+00008e40: 6566 6175 6c74 5f73 706c 696e 655f 6465  efault_spline_de
+00008e50: 6772 6565 225d 203d 206f 6467 5f64 6566  gree"] = odg_def
+00008e60: 6175 6c74 5f73 706c 696e 655f 6465 6772  ault_spline_degr
+00008e70: 6565 0d0a 2020 2020 2020 2020 7365 6c66  ee..        self
+00008e80: 2e61 6461 7461 2e75 6e73 5b22 6f64 6722  .adata.uns["odg"
+00008e90: 5d5b 226f 6467 5f64 6566 6175 6c74 5f64  ]["odg_default_d
+00008ea0: 6f66 225d 203d 206f 6467 5f64 6566 6175  of"] = odg_defau
+00008eb0: 6c74 5f64 6f66 0d0a 2020 2020 2020 2020  lt_dof..        
+00008ec0: 7365 6c66 2e61 7070 656e 645f 746f 5f68  self.append_to_h
+00008ed0: 6973 746f 7279 2822 4765 6e65 2d6c 6576  istory("Gene-lev
+00008ee0: 656c 2073 7461 7469 7374 6963 7320 616e  el statistics an
+00008ef0: 6420 6f76 6572 6469 7370 6572 7369 6f6e  d overdispersion
+00008f00: 206d 6f64 656c 6c69 6e67 2063 6f6d 706c   modelling compl
+00008f10: 6574 6564 2e22 290d 0a20 2020 2020 2020  eted.")..       
+00008f20: 200d 0a20 2020 2064 6566 2073 656c 6563   ..    def selec
+00008f30: 745f 6f76 6572 6469 7370 6572 7365 645f  t_overdispersed_
+00008f40: 6765 6e65 735f 6672 6f6d 5f67 656e 656c  genes_from_genel
+00008f50: 6973 7428 7365 6c66 2c20 6765 6e65 733a  ist(self, genes:
+00008f60: 2043 6f6c 6c65 6374 696f 6e5b 7374 725d   Collection[str]
+00008f70: 2c20 6d69 6e5f 6d65 616e 3d30 293a 0d0a  , min_mean=0):..
+00008f80: 2020 2020 2020 2020 2222 2253 656c 6563          """Selec
+00008f90: 7420 6f76 6572 6469 7370 6572 7365 6420  t overdispersed 
+00008fa0: 6765 6e65 732f 6665 6174 7572 6573 2075  genes/features u
+00008fb0: 7369 6e67 2061 2063 7573 746f 6d20 6c69  sing a custom li
+00008fc0: 7374 2e20 4765 6e65 732f 6665 6174 7572  st. Genes/featur
+00008fd0: 6573 206e 6f74 2070 7265 7365 6e74 2069  es not present i
+00008fe0: 6e20 7468 6520 6461 7461 7365 7420 6172  n the dataset ar
+00008ff0: 6520 6175 746f 6d61 7469 6361 6c6c 7920  e automatically 
+00009000: 6669 6c74 6572 6564 206f 7574 2e0d 0a0d  filtered out....
+00009010: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00009020: 6765 6e65 733a 2067 656e 6520 6c69 7374  genes: gene list
+00009030: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00009040: 6765 6e65 733a 2043 6f6c 6c65 6374 696f  genes: Collectio
+00009050: 6e5b 7374 725d 0d0a 2020 2020 2020 2020  n[str]..        
+00009060: 3a70 6172 616d 206d 696e 5f6d 6561 6e3a  :param min_mean:
+00009070: 206d 696e 696d 756d 2067 656e 6520 6578   minimum gene ex
+00009080: 7072 6573 7369 6f6e 2066 6f72 2067 656e  pression for gen
+00009090: 6573 2074 6f20 6265 2063 6f75 6e74 6564  es to be counted
+000090a0: 2061 7320 6f76 6572 6469 7370 6572 7365   as overdisperse
+000090b0: 642c 2064 6566 6175 6c74 7320 746f 2030  d, defaults to 0
+000090c0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+000090d0: 6d69 6e5f 6d65 616e 3a20 696e 742c 206f  min_mean: int, o
+000090e0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+000090f0: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
+00009100: 6c66 2e61 6461 7461 2e76 6172 5b22 7365  lf.adata.var["se
+00009110: 6c65 6374 6564 225d 203d 2073 656c 662e  lected"] = self.
+00009120: 6164 6174 612e 7661 722e 696e 6465 782e  adata.var.index.
+00009130: 6973 696e 2867 656e 6573 2920 2620 2873  isin(genes) & (s
+00009140: 656c 662e 6164 6174 612e 7661 725b 226d  elf.adata.var["m
+00009150: 6561 6e5f 636f 756e 7473 225d 203e 3d20  ean_counts"] >= 
+00009160: 6d69 6e5f 6d65 616e 290d 0a20 2020 2020  min_mean)..     
+00009170: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
+00009180: 735b 226f 6467 225d 5b22 6f76 6572 6469  s["odg"]["overdi
+00009190: 7370 6572 7369 6f6e 5f6d 6574 7269 6322  spersion_metric"
+000091a0: 5d20 3d20 2222 0d0a 2020 2020 2020 2020  ] = ""..        
+000091b0: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
+000091c0: 6f64 6722 5d5b 226d 696e 5f6d 6561 6e22  odg"]["min_mean"
+000091d0: 5d20 3d20 6d69 6e5f 6d65 616e 0d0a 2020  ] = min_mean..  
+000091e0: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
+000091f0: 2e75 6e73 5b22 6f64 6722 5d5b 226d 696e  .uns["odg"]["min
+00009200: 5f73 636f 7265 225d 203d 2022 220d 0a20  _score"] = "".. 
+00009210: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+00009220: 612e 756e 735b 226f 6467 225d 5b22 746f  a.uns["odg"]["to
+00009230: 705f 6e22 5d20 3d20 2222 0d0a 2020 2020  p_n"] = ""..    
+00009240: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
+00009250: 6e73 5b22 6f64 6722 5d5b 2271 7561 6e74  ns["odg"]["quant
+00009260: 696c 6522 5d20 3d20 2222 0d0a 2020 2020  ile"] = ""..    
+00009270: 2020 2020 7365 6c66 2e61 7070 656e 645f      self.append_
+00009280: 746f 5f68 6973 746f 7279 2822 4f76 6572  to_history("Over
+00009290: 6469 7370 6572 7365 6420 6765 6e65 7320  dispersed genes 
+000092a0: 7365 6c65 6374 6564 2066 726f 6d20 6375  selected from cu
+000092b0: 7374 6f6d 2067 656e 6520 6c69 7374 2229  stom gene list")
+000092c0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000092d0: 6465 6620 7365 6c65 6374 5f6f 7665 7264  def select_overd
+000092e0: 6973 7065 7273 6564 5f67 656e 6573 2873  ispersed_genes(s
+000092f0: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
 00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009310: 2020 2020 2020 2020 6f76 6572 6469 7370          overdisp
-00009320: 6572 7369 6f6e 5f6d 6574 7269 633a 2073  ersion_metric: s
-00009330: 7472 203d 2022 6f64 7363 6f72 6522 2c0d  tr = "odscore",.
-00009340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009310: 2020 2020 2020 2020 206f 7665 7264 6973           overdis
+00009320: 7065 7273 696f 6e5f 6d65 7472 6963 3a20  persion_metric: 
+00009330: 7374 7220 3d20 226f 6473 636f 7265 222c  str = "odscore",
+00009340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00009350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009360: 2020 2020 6d69 6e5f 6d65 616e 3a20 666c      min_mean: fl
-00009370: 6f61 7420 3d20 302c 0d0a 2020 2020 2020  oat = 0,..      
+00009360: 2020 2020 206d 696e 5f6d 6561 6e3a 2066       min_mean: f
+00009370: 6c6f 6174 203d 2030 2c0d 0a20 2020 2020  loat = 0,..     
 00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009390: 2020 2020 2020 2020 2020 2020 206d 696e               min
-000093a0: 5f73 636f 7265 3a20 666c 6f61 7420 3d20  _score: float = 
-000093b0: 312e 302c 0d0a 2020 2020 2020 2020 2020  1.0,..          
+00009390: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+000093a0: 6e5f 7363 6f72 653a 2066 6c6f 6174 203d  n_score: float =
+000093b0: 2031 2e30 2c0d 0a20 2020 2020 2020 2020   1.0,..         
 000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093d0: 2020 2020 2020 2020 2074 6f70 5f6e 3a20           top_n: 
-000093e0: 696e 7420 3d20 4e6f 6e65 2c0d 0a20 2020  int = None,..   
+000093d0: 2020 2020 2020 2020 2020 746f 705f 6e3a            top_n:
+000093e0: 2069 6e74 203d 204e 6f6e 652c 0d0a 2020   int = None,..  
 000093f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009410: 7175 616e 7469 6c65 3a20 666c 6f61 7420  quantile: float 
-00009420: 3d20 4e6f 6e65 293a 0d0a 2020 2020 2020  = None):..      
-00009430: 2020 2222 2253 656c 6563 7420 6f76 6572    """Select over
-00009440: 6469 7370 6572 7365 6420 6765 6e65 732f  dispersed genes/
-00009450: 6665 6174 7572 6573 2075 7369 6e67 2061  features using a
-00009460: 6e20 6f76 6572 6469 7370 6572 7369 6f6e  n overdispersion
-00009470: 206d 6574 7269 632e 204f 7074 696f 6e61   metric. Optiona
-00009480: 6c6c 7920 7365 7420 6120 6d69 6e69 6d75  lly set a minimu
-00009490: 6d20 6765 6e65 2065 7870 7265 7373 696f  m gene expressio
-000094a0: 6e20 6c65 7665 6c2e 0d0a 2020 2020 2020  n level...      
-000094b0: 2020 5365 7420 6120 7468 7265 7368 6f6c    Set a threshol
-000094c0: 6420 7573 696e 6720 7468 6520 746f 7020  d using the top 
-000094d0: 4e20 2827 746f 705f 6e27 292c 206d 696e  N ('top_n'), min
-000094e0: 696d 756d 2073 636f 7265 2028 276d 696e  imum score ('min
-000094f0: 5f73 636f 7265 2729 2c20 6f72 2070 726f  _score'), or pro
-00009500: 706f 7274 696f 6e20 6f66 2066 6561 7475  portion of featu
-00009510: 7265 7320 2827 7175 616e 7469 6c65 2729  res ('quantile')
-00009520: 206d 6574 686f 6473 2e0d 0a20 2020 2020   methods...     
-00009530: 2020 204f 7665 7264 6973 7065 7273 6564     Overdispersed
-00009540: 2067 656e 6520 6c69 7374 2069 7320 7361   gene list is sa
-00009550: 7665 6420 696e 2074 6865 2044 6174 6173  ved in the Datas
-00009560: 6574 206f 626a 6563 742e 0d0a 0d0a 2020  et object.....  
-00009570: 2020 2020 2020 3a70 6172 616d 206f 7665        :param ove
-00009580: 7264 6973 7065 7273 696f 6e5f 6d65 7472  rdispersion_metr
-00009590: 6963 3a20 226f 6473 636f 7265 2220 6f72  ic: "odscore" or
-000095a0: 2022 7673 636f 7265 222c 2064 6566 6175   "vscore", defau
-000095b0: 6c74 7320 746f 2022 6f64 7363 6f72 6522  lts to "odscore"
-000095c0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-000095d0: 6f76 6572 6469 7370 6572 7369 6f6e 5f6d  overdispersion_m
-000095e0: 6574 7269 633a 2073 7472 2c20 6f70 7469  etric: str, opti
-000095f0: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
-00009600: 6172 616d 206d 696e 5f6d 6561 6e3a 206d  aram min_mean: m
-00009610: 696e 696d 756d 2067 656e 6520 6578 7072  inimum gene expr
-00009620: 6573 7369 6f6e 2066 6f72 2067 656e 6573  ession for genes
-00009630: 2074 6f20 6265 2063 6f75 6e74 6564 2061   to be counted a
-00009640: 7320 6f76 6572 6469 7370 6572 7365 642c  s overdispersed,
-00009650: 2064 6566 6175 6c74 7320 746f 2030 0d0a   defaults to 0..
-00009660: 2020 2020 2020 2020 3a74 7970 6520 6d69          :type mi
-00009670: 6e5f 6d65 616e 3a20 696e 742c 206f 7074  n_mean: int, opt
-00009680: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
-00009690: 7061 7261 6d20 6d69 6e5f 7363 6f72 653a  param min_score:
-000096a0: 206d 696e 696d 756d 2073 636f 7265 2066   minimum score f
-000096b0: 6f72 206f 7665 7264 6973 7065 7273 696f  or overdispersio
-000096c0: 6e2c 2064 6566 6175 6c74 7320 746f 2031  n, defaults to 1
-000096d0: 2e30 0d0a 2020 2020 2020 2020 3a74 7970  .0..        :typ
-000096e0: 6520 6d69 6e5f 7363 6f72 653a 2066 6c6f  e min_score: flo
-000096f0: 6174 2c20 6f70 7469 6f6e 616c 0d0a 2020  at, optional..  
-00009700: 2020 2020 2020 3a70 6172 616d 2074 6f70        :param top
-00009710: 5f6e 3a20 4368 6f6f 7365 2074 6865 2074  _n: Choose the t
-00009720: 6f70 204e 206d 6f73 7420 6f76 6572 6469  op N most overdi
-00009730: 7370 6572 7365 6420 6765 6e65 732c 2064  spersed genes, d
-00009740: 6566 6175 6c74 7320 746f 204e 6f6e 650d  efaults to None.
-00009750: 0a20 2020 2020 2020 203a 7479 7065 2074  .        :type t
-00009760: 6f70 5f6e 3a20 696e 742c 206f 7074 696f  op_n: int, optio
-00009770: 6e61 6c0d 0a20 2020 2020 2020 203a 7061  nal..        :pa
-00009780: 7261 6d20 7175 616e 7469 6c65 3a20 4368  ram quantile: Ch
-00009790: 6f6f 7365 2061 2071 7561 6e74 696c 6520  oose a quantile 
-000097a0: 6f66 206f 7665 7264 6973 7065 7273 696f  of overdispersio
-000097b0: 6e2e 2046 6f72 2065 7861 6d70 6c65 2c20  n. For example, 
-000097c0: 7468 6520 746f 7020 3130 2520 6f66 206f  the top 10% of o
-000097d0: 7665 7264 6973 7065 7273 6564 2067 656e  verdispersed gen
-000097e0: 6573 2077 6f75 6c64 2062 6520 302e 3130  es would be 0.10
-000097f0: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-00009800: 6e65 0d0a 2020 2020 2020 2020 3a74 7970  ne..        :typ
-00009810: 6520 7175 616e 7469 6c65 3a20 666c 6f61  e quantile: floa
-00009820: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-00009830: 2020 2020 203a 7261 6973 6573 2056 616c       :raises Val
-00009840: 7565 4572 726f 723a 2045 7272 6f72 2069  ueError: Error i
-00009850: 6620 696e 7661 6c69 6420 6f76 6572 6469  f invalid overdi
-00009860: 7370 6572 7369 6f6e 206d 6574 7269 6320  spersion metric 
-00009870: 6973 2063 686f 7365 6e2e 0d0a 2020 2020  is chosen...    
-00009880: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00009890: 200d 0a20 2020 2020 2020 2069 6620 6f76   ..        if ov
-000098a0: 6572 6469 7370 6572 7369 6f6e 5f6d 6574  erdispersion_met
-000098b0: 7269 6320 6e6f 7420 696e 2073 656c 662e  ric not in self.
-000098c0: 6164 6174 612e 7661 722e 636f 6c75 6d6e  adata.var.column
-000098d0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000098e0: 6966 206f 7665 7264 6973 7065 7273 696f  if overdispersio
-000098f0: 6e5f 6d65 7472 6963 2069 6e20 2822 6f64  n_metric in ("od
-00009900: 7363 6f72 6522 2c20 2276 7363 6f72 6522  score", "vscore"
-00009910: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00009920: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00009930: 7272 6f72 280d 0a20 2020 2020 2020 2020  rror(..         
-00009940: 2020 2020 2020 2020 2020 2066 227b 6f76             f"{ov
-00009950: 6572 6469 7370 6572 7369 6f6e 5f6d 6574  erdispersion_met
-00009960: 7269 637d 2068 6173 206e 6f74 2062 6565  ric} has not bee
-00009970: 6e20 6361 6c63 756c 6174 6564 2066 6f72  n calculated for
-00009980: 2074 6869 7320 6461 7461 7365 742e 2022   this dataset. "
-00009990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000099a0: 2020 2020 2020 2245 6e73 7572 6520 7468        "Ensure th
-000099b0: 6174 2079 6f75 2063 616c 6c20 7468 6520  at you call the 
-000099c0: 6044 6174 6173 6574 2e63 6f6d 7075 7465  `Dataset.compute
-000099d0: 5f67 656e 655f 7374 6174 7328 2960 2066  _gene_stats()` f
-000099e0: 6972 7374 2e22 0d0a 2020 2020 2020 2020  irst."..        
-000099f0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00009a00: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00009a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009a20: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00009a30: 6f72 280d 0a20 2020 2020 2020 2020 2020  or(..           
-00009a40: 2020 2020 2020 2020 2066 227b 6f76 6572           f"{over
-00009a50: 6469 7370 6572 7369 6f6e 5f6d 6574 7269  dispersion_metri
-00009a60: 637d 2069 7320 6e6f 7420 6120 7661 6c69  c} is not a vali
-00009a70: 6420 6f76 6572 6469 7370 6572 7369 6f6e  d overdispersion
-00009a80: 206d 6574 7269 632e 220d 0a20 2020 2020   metric."..     
-00009a90: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00009aa0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00009ab0: 2020 2020 2320 7761 726e 2069 6620 6d75      # warn if mu
-00009ac0: 6c74 6970 6c65 206d 6574 686f 6473 2061  ltiple methods a
-00009ad0: 7265 2073 656c 6563 7465 640d 0a20 2020  re selected..   
-00009ae0: 2020 2020 2073 656c 6563 7465 645f 6d65       selected_me
-00009af0: 7468 6f64 7320 3d20 5b5d 0d0a 2020 2020  thods = []..    
-00009b00: 2020 2020 6966 206d 696e 5f73 636f 7265      if min_score
-00009b10: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00009b20: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-00009b30: 7465 645f 6d65 7468 6f64 732e 6170 7065  ted_methods.appe
-00009b40: 6e64 2822 6d69 6e5f 7363 6f72 6522 290d  nd("min_score").
-00009b50: 0a20 2020 2020 2020 2069 6620 746f 705f  .        if top_
-00009b60: 6e20 6973 206e 6f74 204e 6f6e 653a 0d0a  n is not None:..
-00009b70: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-00009b80: 6374 6564 5f6d 6574 686f 6473 2e61 7070  cted_methods.app
-00009b90: 656e 6428 2274 6f70 5f6e 2229 0d0a 2020  end("top_n")..  
-00009ba0: 2020 2020 2020 6966 2071 7561 6e74 696c        if quantil
-00009bb0: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
-00009bc0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-00009bd0: 6374 6564 5f6d 6574 686f 6473 2e61 7070  cted_methods.app
-00009be0: 656e 6428 2271 7561 6e74 696c 6522 290d  end("quantile").
-00009bf0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00009c00: 7365 6c65 6374 6564 5f6d 6574 686f 6473  selected_methods
-00009c10: 2920 3e20 313a 0d0a 2020 2020 2020 2020  ) > 1:..        
-00009c20: 2020 2020 6d65 7468 6f64 7761 726e 7374      methodwarnst
-00009c30: 7220 3d20 222c 2022 2e6a 6f69 6e28 7365  r = ", ".join(se
-00009c40: 6c65 6374 6564 5f6d 6574 686f 6473 290d  lected_methods).
-00009c50: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00009c60: 6769 6e67 2e77 6172 6e69 6e67 2866 224d  ging.warning(f"M
-00009c70: 756c 7469 706c 6520 636f 6e66 6c69 6374  ultiple conflict
-00009c80: 696e 6720 6f76 6572 6469 7370 6572 7365  ing overdisperse
-00009c90: 6420 6765 6e65 2073 656c 6563 7469 6f6e  d gene selection
-00009ca0: 2063 7269 7465 7269 6120 6861 7665 2062   criteria have b
-00009cb0: 6565 6e20 7365 6c65 6374 6564 3a20 7b6d  een selected: {m
-00009cc0: 6574 686f 6477 6172 6e73 7472 7d2e 2022  ethodwarnstr}. "
-00009cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009ce0: 2020 2020 2020 2020 2020 2020 2020 224f                "O
-00009cf0: 6e6c 7920 7468 6520 696e 7465 7273 6563  nly the intersec
-00009d00: 7469 6f6e 206f 6620 7468 6573 6520 6d65  tion of these me
-00009d10: 7468 6f64 7320 7769 6c6c 2062 6520 7365  thods will be se
-00009d20: 6c65 6374 6564 2e22 290d 0a20 2020 2020  lected.")..     
-00009d30: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00009d40: 2020 2020 2023 206d 696e 5f6d 6561 6e20       # min_mean 
-00009d50: 6669 6c74 6572 0d0a 2020 2020 2020 2020  filter..        
-00009d60: 7365 6c65 6374 6564 5f67 656e 6573 203d  selected_genes =
-00009d70: 2073 656c 662e 6164 6174 612e 7661 725b   self.adata.var[
-00009d80: 226d 6561 6e5f 636f 756e 7473 225d 203e  "mean_counts"] >
-00009d90: 3d20 6d69 6e5f 6d65 616e 0d0a 2020 2020  = min_mean..    
-00009da0: 2020 2020 2320 6d69 6e5f 7363 6f72 6520      # min_score 
-00009db0: 6669 6c74 6572 0d0a 2020 2020 2020 2020  filter..        
-00009dc0: 6966 206d 696e 5f73 636f 7265 2069 7320  if min_score is 
-00009dd0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00009de0: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
-00009df0: 6765 6e65 7320 3d20 7365 6c65 6374 6564  genes = selected
-00009e00: 5f67 656e 6573 2026 2028 7365 6c66 2e61  _genes & (self.a
-00009e10: 6461 7461 2e76 6172 5b6f 7665 7264 6973  data.var[overdis
-00009e20: 7065 7273 696f 6e5f 6d65 7472 6963 5d20  persion_metric] 
-00009e30: 3e3d 206d 696e 5f73 636f 7265 290d 0a20  >= min_score).. 
-00009e40: 2020 2020 2020 2023 2074 6f70 5f6e 2066         # top_n f
-00009e50: 696c 7465 720d 0a20 2020 2020 2020 2069  ilter..        i
-00009e60: 6620 746f 705f 6e20 6973 206e 6f74 204e  f top_n is not N
-00009e70: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00009e80: 2020 6765 6e65 7320 3d20 7365 6c66 2e61    genes = self.a
-00009e90: 6461 7461 2e76 6172 5b6f 7665 7264 6973  data.var[overdis
-00009ea0: 7065 7273 696f 6e5f 6d65 7472 6963 5d2e  persion_metric].
-00009eb0: 736f 7274 5f76 616c 7565 7328 6173 6365  sort_values(asce
-00009ec0: 6e64 696e 673d 4661 6c73 6529 2e68 6561  nding=False).hea
-00009ed0: 6428 696e 7428 746f 705f 6e29 292e 696e  d(int(top_n)).in
-00009ee0: 6465 780d 0a20 2020 2020 2020 2020 2020  dex..           
-00009ef0: 2073 656c 6563 7465 645f 6765 6e65 7320   selected_genes 
-00009f00: 3d20 7365 6c65 6374 6564 5f67 656e 6573  = selected_genes
-00009f10: 2026 2073 656c 662e 6164 6174 612e 7661   & self.adata.va
-00009f20: 722e 696e 6465 782e 6973 696e 2867 656e  r.index.isin(gen
-00009f30: 6573 290d 0a20 2020 2020 2020 2023 2071  es)..        # q
-00009f40: 7561 6e74 696c 6520 6669 6c74 6572 0d0a  uantile filter..
-00009f50: 2020 2020 2020 2020 6966 2071 7561 6e74          if quant
-00009f60: 696c 6520 6973 206e 6f74 204e 6f6e 653a  ile is not None:
-00009f70: 0d0a 2020 2020 2020 2020 2020 2020 6e5f  ..            n_
-00009f80: 746f 7461 6c5f 6765 6e65 7320 3d20 7365  total_genes = se
-00009f90: 6c66 2e61 6461 7461 2e76 6172 5b6f 7665  lf.adata.var[ove
-00009fa0: 7264 6973 7065 7273 696f 6e5f 6d65 7472  rdispersion_metr
-00009fb0: 6963 5d2e 6e6f 746e 756c 6c28 292e 7375  ic].notnull().su
-00009fc0: 6d28 290d 0a20 2020 2020 2020 2020 2020  m()..           
-00009fd0: 2067 656e 6573 203d 2073 656c 662e 6164   genes = self.ad
-00009fe0: 6174 612e 7661 725b 6f76 6572 6469 7370  ata.var[overdisp
-00009ff0: 6572 7369 6f6e 5f6d 6574 7269 635d 2e73  ersion_metric].s
-0000a000: 6f72 745f 7661 6c75 6573 2861 7363 656e  ort_values(ascen
-0000a010: 6469 6e67 3d46 616c 7365 292e 6865 6164  ding=False).head
-0000a020: 2869 6e74 2871 7561 6e74 696c 6520 2a20  (int(quantile * 
-0000a030: 6e5f 746f 7461 6c5f 6765 6e65 7329 292e  n_total_genes)).
-0000a040: 696e 6465 780d 0a20 2020 2020 2020 2020  index..         
-0000a050: 2020 2073 656c 6563 7465 645f 6765 6e65     selected_gene
-0000a060: 7320 3d20 7365 6c65 6374 6564 5f67 656e  s = selected_gen
-0000a070: 6573 2026 2073 656c 662e 6164 6174 612e  es & self.adata.
-0000a080: 7661 722e 696e 6465 782e 6973 696e 2867  var.index.isin(g
-0000a090: 656e 6573 290d 0a0d 0a20 2020 2020 2020  enes)....       
-0000a0a0: 206e 5f73 656c 6563 7465 645f 6765 6e65   n_selected_gene
-0000a0b0: 7320 3d20 7365 6c65 6374 6564 5f67 656e  s = selected_gen
-0000a0c0: 6573 2e73 756d 2829 0d0a 2020 2020 2020  es.sum()..      
-0000a0d0: 2020 6c6f 6767 696e 672e 696e 666f 2866    logging.info(f
-0000a0e0: 227b 6e5f 7365 6c65 6374 6564 5f67 656e  "{n_selected_gen
-0000a0f0: 6573 7d20 6765 6e65 7320 7365 6c65 6374  es} genes select
-0000a100: 6564 2066 6f72 2066 6163 746f 7269 7a61  ed for factoriza
-0000a110: 7469 6f6e 2229 0d0a 2020 2020 2020 2020  tion")..        
-0000a120: 0d0a 2020 2020 2020 2020 2320 6d61 6b65  ..        # make
-0000a130: 2063 6861 6e67 6573 2074 6f20 4461 7461   changes to Data
-0000a140: 7365 7420 6f62 6a65 6374 0d0a 2020 2020  set object..    
-0000a150: 2020 2020 7365 6c66 2e61 6461 7461 2e76      self.adata.v
-0000a160: 6172 5b22 7365 6c65 6374 6564 225d 203d  ar["selected"] =
-0000a170: 2073 656c 6563 7465 645f 6765 6e65 730d   selected_genes.
-0000a180: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-0000a190: 6174 612e 6f62 735b 2268 7667 5f61 6c6c  ata.obs["hvg_all
-0000a1a0: 5f30 225d 203d 2028 7365 6c66 2e74 6f5f  _0"] = (self.to_
-0000a1b0: 6466 286e 6f72 6d61 6c69 7a65 643d 5472  df(normalized=Tr
-0000a1c0: 7565 292e 6c6f 635b 3a2c 2073 656c 6563  ue).loc[:, selec
-0000a1d0: 7465 645f 6765 6e65 735d 2e73 756d 2861  ted_genes].sum(a
-0000a1e0: 7869 733d 3129 203d 3d20 3029 2e61 7374  xis=1) == 0).ast
-0000a1f0: 7970 6528 2273 7472 2229 2e61 7374 7970  ype("str").astyp
-0000a200: 6528 2263 6174 6567 6f72 7922 290d 0a20  e("category").. 
-0000a210: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-0000a220: 612e 756e 735b 226f 6467 225d 5b22 6f76  a.uns["odg"]["ov
-0000a230: 6572 6469 7370 6572 7369 6f6e 5f6d 6574  erdispersion_met
-0000a240: 7269 6322 5d20 3d20 6f76 6572 6469 7370  ric"] = overdisp
-0000a250: 6572 7369 6f6e 5f6d 6574 7269 630d 0a20  ersion_metric.. 
-0000a260: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-0000a270: 612e 756e 735b 226f 6467 225d 5b22 6d69  a.uns["odg"]["mi
-0000a280: 6e5f 6d65 616e 225d 203d 206d 696e 5f6d  n_mean"] = min_m
-0000a290: 6561 6e0d 0a20 2020 2020 2020 2073 656c  ean..        sel
-0000a2a0: 662e 6164 6174 612e 756e 735b 226f 6467  f.adata.uns["odg
-0000a2b0: 225d 5b22 6d69 6e5f 7363 6f72 6522 5d20  "]["min_score"] 
-0000a2c0: 3d20 6d69 6e5f 7363 6f72 6520 6966 206d  = min_score if m
-0000a2d0: 696e 5f73 636f 7265 2069 7320 6e6f 7420  in_score is not 
-0000a2e0: 4e6f 6e65 2065 6c73 6520 2222 0d0a 2020  None else ""..  
-0000a2f0: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
-0000a300: 2e75 6e73 5b22 6f64 6722 5d5b 2274 6f70  .uns["odg"]["top
-0000a310: 5f6e 225d 203d 2074 6f70 5f6e 2069 6620  _n"] = top_n if 
-0000a320: 746f 705f 6e20 6973 206e 6f74 204e 6f6e  top_n is not Non
-0000a330: 6520 656c 7365 2022 220d 0a20 2020 2020  e else ""..     
-0000a340: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
-0000a350: 735b 226f 6467 225d 5b22 7175 616e 7469  s["odg"]["quanti
-0000a360: 6c65 225d 203d 2071 7561 6e74 696c 6520  le"] = quantile 
-0000a370: 6966 2071 7561 6e74 696c 6520 6973 206e  if quantile is n
-0000a380: 6f74 204e 6f6e 6520 656c 7365 2022 220d  ot None else "".
-0000a390: 0a20 2020 2020 2020 2073 656c 662e 6170  .        self.ap
-0000a3a0: 7065 6e64 5f74 6f5f 6869 7374 6f72 7928  pend_to_history(
-0000a3b0: 224f 7665 7264 6973 7065 7273 6564 2067  "Overdispersed g
-0000a3c0: 656e 6573 2073 656c 6563 7465 6422 290d  enes selected").
-0000a3d0: 0a20 2020 200d 0a20 2020 2064 6566 2069  .    ..    def i
-0000a3e0: 6e69 7469 616c 697a 655f 636e 6d66 2873  nitialize_cnmf(s
-0000a3f0: 656c 662c 2063 6e6d 665f 6f75 7470 7574  elf, cnmf_output
-0000a400: 5f64 6972 3a20 7374 722c 0d0a 2020 2020  _dir: str,..    
+00009410: 2071 7561 6e74 696c 653a 2066 6c6f 6174   quantile: float
+00009420: 203d 204e 6f6e 6529 3a0d 0a20 2020 2020   = None):..     
+00009430: 2020 2022 2222 5365 6c65 6374 206f 7665     """Select ove
+00009440: 7264 6973 7065 7273 6564 2067 656e 6573  rdispersed genes
+00009450: 2f66 6561 7475 7265 7320 7573 696e 6720  /features using 
+00009460: 616e 206f 7665 7264 6973 7065 7273 696f  an overdispersio
+00009470: 6e20 6d65 7472 6963 2e20 4f70 7469 6f6e  n metric. Option
+00009480: 616c 6c79 2073 6574 2061 206d 696e 696d  ally set a minim
+00009490: 756d 2067 656e 6520 6578 7072 6573 7369  um gene expressi
+000094a0: 6f6e 206c 6576 656c 2e0d 0a20 2020 2020  on level...     
+000094b0: 2020 2053 6574 2061 2074 6872 6573 686f     Set a thresho
+000094c0: 6c64 2075 7369 6e67 2074 6865 2074 6f70  ld using the top
+000094d0: 204e 2028 2774 6f70 5f6e 2729 2c20 6d69   N ('top_n'), mi
+000094e0: 6e69 6d75 6d20 7363 6f72 6520 2827 6d69  nimum score ('mi
+000094f0: 6e5f 7363 6f72 6527 292c 206f 7220 7072  n_score'), or pr
+00009500: 6f70 6f72 7469 6f6e 206f 6620 6665 6174  oportion of feat
+00009510: 7572 6573 2028 2771 7561 6e74 696c 6527  ures ('quantile'
+00009520: 2920 6d65 7468 6f64 732e 0d0a 2020 2020  ) methods...    
+00009530: 2020 2020 4f76 6572 6469 7370 6572 7365      Overdisperse
+00009540: 6420 6765 6e65 206c 6973 7420 6973 2073  d gene list is s
+00009550: 6176 6564 2069 6e20 7468 6520 4461 7461  aved in the Data
+00009560: 7365 7420 6f62 6a65 6374 2e0d 0a0d 0a20  set object..... 
+00009570: 2020 2020 2020 203a 7061 7261 6d20 6f76         :param ov
+00009580: 6572 6469 7370 6572 7369 6f6e 5f6d 6574  erdispersion_met
+00009590: 7269 633a 2022 6f64 7363 6f72 6522 206f  ric: "odscore" o
+000095a0: 7220 2276 7363 6f72 6522 2c20 6465 6661  r "vscore", defa
+000095b0: 756c 7473 2074 6f20 226f 6473 636f 7265  ults to "odscore
+000095c0: 220d 0a20 2020 2020 2020 203a 7479 7065  "..        :type
+000095d0: 206f 7665 7264 6973 7065 7273 696f 6e5f   overdispersion_
+000095e0: 6d65 7472 6963 3a20 7374 722c 206f 7074  metric: str, opt
+000095f0: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
+00009600: 7061 7261 6d20 6d69 6e5f 6d65 616e 3a20  param min_mean: 
+00009610: 6d69 6e69 6d75 6d20 6765 6e65 2065 7870  minimum gene exp
+00009620: 7265 7373 696f 6e20 666f 7220 6765 6e65  ression for gene
+00009630: 7320 746f 2062 6520 636f 756e 7465 6420  s to be counted 
+00009640: 6173 206f 7665 7264 6973 7065 7273 6564  as overdispersed
+00009650: 2c20 6465 6661 756c 7473 2074 6f20 300d  , defaults to 0.
+00009660: 0a20 2020 2020 2020 203a 7479 7065 206d  .        :type m
+00009670: 696e 5f6d 6561 6e3a 2069 6e74 2c20 6f70  in_mean: int, op
+00009680: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00009690: 3a70 6172 616d 206d 696e 5f73 636f 7265  :param min_score
+000096a0: 3a20 6d69 6e69 6d75 6d20 7363 6f72 6520  : minimum score 
+000096b0: 666f 7220 6f76 6572 6469 7370 6572 7369  for overdispersi
+000096c0: 6f6e 2c20 6465 6661 756c 7473 2074 6f20  on, defaults to 
+000096d0: 312e 300d 0a20 2020 2020 2020 203a 7479  1.0..        :ty
+000096e0: 7065 206d 696e 5f73 636f 7265 3a20 666c  pe min_score: fl
+000096f0: 6f61 742c 206f 7074 696f 6e61 6c0d 0a20  oat, optional.. 
+00009700: 2020 2020 2020 203a 7061 7261 6d20 746f         :param to
+00009710: 705f 6e3a 2043 686f 6f73 6520 7468 6520  p_n: Choose the 
+00009720: 746f 7020 4e20 6d6f 7374 206f 7665 7264  top N most overd
+00009730: 6973 7065 7273 6564 2067 656e 6573 2c20  ispersed genes, 
+00009740: 6465 6661 756c 7473 2074 6f20 4e6f 6e65  defaults to None
+00009750: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00009760: 746f 705f 6e3a 2069 6e74 2c20 6f70 7469  top_n: int, opti
+00009770: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
+00009780: 6172 616d 2071 7561 6e74 696c 653a 2043  aram quantile: C
+00009790: 686f 6f73 6520 6120 7175 616e 7469 6c65  hoose a quantile
+000097a0: 206f 6620 6f76 6572 6469 7370 6572 7369   of overdispersi
+000097b0: 6f6e 2e20 466f 7220 6578 616d 706c 652c  on. For example,
+000097c0: 2074 6865 2074 6f70 2031 3025 206f 6620   the top 10% of 
+000097d0: 6f76 6572 6469 7370 6572 7365 6420 6765  overdispersed ge
+000097e0: 6e65 7320 776f 756c 6420 6265 2030 2e31  nes would be 0.1
+000097f0: 302e 2044 6566 6175 6c74 7320 746f 204e  0. Defaults to N
+00009800: 6f6e 650d 0a20 2020 2020 2020 203a 7479  one..        :ty
+00009810: 7065 2071 7561 6e74 696c 653a 2066 6c6f  pe quantile: flo
+00009820: 6174 2c20 6f70 7469 6f6e 616c 0d0a 2020  at, optional..  
+00009830: 2020 2020 2020 3a72 6169 7365 7320 5661        :raises Va
+00009840: 6c75 6545 7272 6f72 3a20 4572 726f 7220  lueError: Error 
+00009850: 6966 2069 6e76 616c 6964 206f 7665 7264  if invalid overd
+00009860: 6973 7065 7273 696f 6e20 6d65 7472 6963  ispersion metric
+00009870: 2069 7320 6368 6f73 656e 2e0d 0a20 2020   is chosen...   
+00009880: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00009890: 2020 0d0a 2020 2020 2020 2020 6966 206f    ..        if o
+000098a0: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
+000098b0: 7472 6963 206e 6f74 2069 6e20 7365 6c66  tric not in self
+000098c0: 2e61 6461 7461 2e76 6172 2e63 6f6c 756d  .adata.var.colum
+000098d0: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
+000098e0: 2069 6620 6f76 6572 6469 7370 6572 7369   if overdispersi
+000098f0: 6f6e 5f6d 6574 7269 6320 696e 2028 226f  on_metric in ("o
+00009900: 6473 636f 7265 222c 2022 7673 636f 7265  dscore", "vscore
+00009910: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
+00009920: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00009930: 4572 726f 7228 0d0a 2020 2020 2020 2020  Error(..        
+00009940: 2020 2020 2020 2020 2020 2020 6622 7b6f              f"{o
+00009950: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
+00009960: 7472 6963 7d20 6861 7320 6e6f 7420 6265  tric} has not be
+00009970: 656e 2063 616c 6375 6c61 7465 6420 666f  en calculated fo
+00009980: 7220 7468 6973 2064 6174 6173 6574 2e20  r this dataset. 
+00009990: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+000099a0: 2020 2020 2020 2022 456e 7375 7265 2074         "Ensure t
+000099b0: 6861 7420 796f 7520 6361 6c6c 2074 6865  hat you call the
+000099c0: 2060 4461 7461 7365 742e 636f 6d70 7574   `Dataset.comput
+000099d0: 655f 6765 6e65 5f73 7461 7473 2829 6020  e_gene_stats()` 
+000099e0: 6669 7273 742e 220d 0a20 2020 2020 2020  first."..       
+000099f0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+00009a00: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00009a10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00009a20: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00009a30: 726f 7228 0d0a 2020 2020 2020 2020 2020  ror(..          
+00009a40: 2020 2020 2020 2020 2020 6622 7b6f 7665            f"{ove
+00009a50: 7264 6973 7065 7273 696f 6e5f 6d65 7472  rdispersion_metr
+00009a60: 6963 7d20 6973 206e 6f74 2061 2076 616c  ic} is not a val
+00009a70: 6964 206f 7665 7264 6973 7065 7273 696f  id overdispersio
+00009a80: 6e20 6d65 7472 6963 2e22 0d0a 2020 2020  n metric."..    
+00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009aa0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+00009ab0: 2020 2020 2023 2077 6172 6e20 6966 206d       # warn if m
+00009ac0: 756c 7469 706c 6520 6d65 7468 6f64 7320  ultiple methods 
+00009ad0: 6172 6520 7365 6c65 6374 6564 0d0a 2020  are selected..  
+00009ae0: 2020 2020 2020 7365 6c65 6374 6564 5f6d        selected_m
+00009af0: 6574 686f 6473 203d 205b 5d0d 0a20 2020  ethods = []..   
+00009b00: 2020 2020 2069 6620 6d69 6e5f 7363 6f72       if min_scor
+00009b10: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
+00009b20: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
+00009b30: 6374 6564 5f6d 6574 686f 6473 2e61 7070  cted_methods.app
+00009b40: 656e 6428 226d 696e 5f73 636f 7265 2229  end("min_score")
+00009b50: 0d0a 2020 2020 2020 2020 6966 2074 6f70  ..        if top
+00009b60: 5f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0d  _n is not None:.
+00009b70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009b80: 6563 7465 645f 6d65 7468 6f64 732e 6170  ected_methods.ap
+00009b90: 7065 6e64 2822 746f 705f 6e22 290d 0a20  pend("top_n").. 
+00009ba0: 2020 2020 2020 2069 6620 7175 616e 7469         if quanti
+00009bb0: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0d  le is not None:.
+00009bc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009bd0: 6563 7465 645f 6d65 7468 6f64 732e 6170  ected_methods.ap
+00009be0: 7065 6e64 2822 7175 616e 7469 6c65 2229  pend("quantile")
+00009bf0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+00009c00: 2873 656c 6563 7465 645f 6d65 7468 6f64  (selected_method
+00009c10: 7329 203e 2031 3a0d 0a20 2020 2020 2020  s) > 1:..       
+00009c20: 2020 2020 206d 6574 686f 6477 6172 6e73       methodwarns
+00009c30: 7472 203d 2022 2c20 222e 6a6f 696e 2873  tr = ", ".join(s
+00009c40: 656c 6563 7465 645f 6d65 7468 6f64 7329  elected_methods)
+00009c50: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00009c60: 6767 696e 672e 7761 726e 696e 6728 6622  gging.warning(f"
+00009c70: 4d75 6c74 6970 6c65 2063 6f6e 666c 6963  Multiple conflic
+00009c80: 7469 6e67 206f 7665 7264 6973 7065 7273  ting overdispers
+00009c90: 6564 2067 656e 6520 7365 6c65 6374 696f  ed gene selectio
+00009ca0: 6e20 6372 6974 6572 6961 2068 6176 6520  n criteria have 
+00009cb0: 6265 656e 2073 656c 6563 7465 643a 207b  been selected: {
+00009cc0: 6d65 7468 6f64 7761 726e 7374 727d 2e20  methodwarnstr}. 
+00009cd0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00009ce0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00009cf0: 4f6e 6c79 2074 6865 2069 6e74 6572 7365  Only the interse
+00009d00: 6374 696f 6e20 6f66 2074 6865 7365 206d  ction of these m
+00009d10: 6574 686f 6473 2077 696c 6c20 6265 2073  ethods will be s
+00009d20: 656c 6563 7465 642e 2229 0d0a 2020 2020  elected.")..    
+00009d30: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00009d40: 2020 2020 2020 2320 6d69 6e5f 6d65 616e        # min_mean
+00009d50: 2066 696c 7465 720d 0a20 2020 2020 2020   filter..       
+00009d60: 2073 656c 6563 7465 645f 6765 6e65 7320   selected_genes 
+00009d70: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
+00009d80: 5b22 6d65 616e 5f63 6f75 6e74 7322 5d20  ["mean_counts"] 
+00009d90: 3e3d 206d 696e 5f6d 6561 6e0d 0a20 2020  >= min_mean..   
+00009da0: 2020 2020 2023 206d 696e 5f73 636f 7265       # min_score
+00009db0: 2066 696c 7465 720d 0a20 2020 2020 2020   filter..       
+00009dc0: 2069 6620 6d69 6e5f 7363 6f72 6520 6973   if min_score is
+00009dd0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00009de0: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+00009df0: 5f67 656e 6573 203d 2073 656c 6563 7465  _genes = selecte
+00009e00: 645f 6765 6e65 7320 2620 2873 656c 662e  d_genes & (self.
+00009e10: 6164 6174 612e 7661 725b 6f76 6572 6469  adata.var[overdi
+00009e20: 7370 6572 7369 6f6e 5f6d 6574 7269 635d  spersion_metric]
+00009e30: 203e 3d20 6d69 6e5f 7363 6f72 6529 0d0a   >= min_score)..
+00009e40: 2020 2020 2020 2020 2320 746f 705f 6e20          # top_n 
+00009e50: 6669 6c74 6572 0d0a 2020 2020 2020 2020  filter..        
+00009e60: 6966 2074 6f70 5f6e 2069 7320 6e6f 7420  if top_n is not 
+00009e70: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00009e80: 2020 2067 656e 6573 203d 2073 656c 662e     genes = self.
+00009e90: 6164 6174 612e 7661 725b 6f76 6572 6469  adata.var[overdi
+00009ea0: 7370 6572 7369 6f6e 5f6d 6574 7269 635d  spersion_metric]
+00009eb0: 2e73 6f72 745f 7661 6c75 6573 2861 7363  .sort_values(asc
+00009ec0: 656e 6469 6e67 3d46 616c 7365 292e 6865  ending=False).he
+00009ed0: 6164 2869 6e74 2874 6f70 5f6e 2929 2e69  ad(int(top_n)).i
+00009ee0: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
+00009ef0: 2020 7365 6c65 6374 6564 5f67 656e 6573    selected_genes
+00009f00: 203d 2073 656c 6563 7465 645f 6765 6e65   = selected_gene
+00009f10: 7320 2620 7365 6c66 2e61 6461 7461 2e76  s & self.adata.v
+00009f20: 6172 2e69 6e64 6578 2e69 7369 6e28 6765  ar.index.isin(ge
+00009f30: 6e65 7329 0d0a 2020 2020 2020 2020 2320  nes)..        # 
+00009f40: 7175 616e 7469 6c65 2066 696c 7465 720d  quantile filter.
+00009f50: 0a20 2020 2020 2020 2069 6620 7175 616e  .        if quan
+00009f60: 7469 6c65 2069 7320 6e6f 7420 4e6f 6e65  tile is not None
+00009f70: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
+00009f80: 5f74 6f74 616c 5f67 656e 6573 203d 2073  _total_genes = s
+00009f90: 656c 662e 6164 6174 612e 7661 725b 6f76  elf.adata.var[ov
+00009fa0: 6572 6469 7370 6572 7369 6f6e 5f6d 6574  erdispersion_met
+00009fb0: 7269 635d 2e6e 6f74 6e75 6c6c 2829 2e73  ric].notnull().s
+00009fc0: 756d 2829 0d0a 2020 2020 2020 2020 2020  um()..          
+00009fd0: 2020 6765 6e65 7320 3d20 7365 6c66 2e61    genes = self.a
+00009fe0: 6461 7461 2e76 6172 5b6f 7665 7264 6973  data.var[overdis
+00009ff0: 7065 7273 696f 6e5f 6d65 7472 6963 5d2e  persion_metric].
+0000a000: 736f 7274 5f76 616c 7565 7328 6173 6365  sort_values(asce
+0000a010: 6e64 696e 673d 4661 6c73 6529 2e68 6561  nding=False).hea
+0000a020: 6428 696e 7428 7175 616e 7469 6c65 202a  d(int(quantile *
+0000a030: 206e 5f74 6f74 616c 5f67 656e 6573 2929   n_total_genes))
+0000a040: 2e69 6e64 6578 0d0a 2020 2020 2020 2020  .index..        
+0000a050: 2020 2020 7365 6c65 6374 6564 5f67 656e      selected_gen
+0000a060: 6573 203d 2073 656c 6563 7465 645f 6765  es = selected_ge
+0000a070: 6e65 7320 2620 7365 6c66 2e61 6461 7461  nes & self.adata
+0000a080: 2e76 6172 2e69 6e64 6578 2e69 7369 6e28  .var.index.isin(
+0000a090: 6765 6e65 7329 0d0a 0d0a 2020 2020 2020  genes)....      
+0000a0a0: 2020 6e5f 7365 6c65 6374 6564 5f67 656e    n_selected_gen
+0000a0b0: 6573 203d 2073 656c 6563 7465 645f 6765  es = selected_ge
+0000a0c0: 6e65 732e 7375 6d28 290d 0a20 2020 2020  nes.sum()..     
+0000a0d0: 2020 206c 6f67 6769 6e67 2e69 6e66 6f28     logging.info(
+0000a0e0: 6622 7b6e 5f73 656c 6563 7465 645f 6765  f"{n_selected_ge
+0000a0f0: 6e65 737d 2067 656e 6573 2073 656c 6563  nes} genes selec
+0000a100: 7465 6420 666f 7220 6661 6374 6f72 697a  ted for factoriz
+0000a110: 6174 696f 6e22 290d 0a20 2020 2020 2020  ation")..       
+0000a120: 200d 0a20 2020 2020 2020 2023 206d 616b   ..        # mak
+0000a130: 6520 6368 616e 6765 7320 746f 2044 6174  e changes to Dat
+0000a140: 6173 6574 206f 626a 6563 740d 0a20 2020  aset object..   
+0000a150: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+0000a160: 7661 725b 2273 656c 6563 7465 6422 5d20  var["selected"] 
+0000a170: 3d20 7365 6c65 6374 6564 5f67 656e 6573  = selected_genes
+0000a180: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+0000a190: 6461 7461 2e6f 6273 5b22 6876 675f 616c  data.obs["hvg_al
+0000a1a0: 6c5f 3022 5d20 3d20 2873 656c 662e 746f  l_0"] = (self.to
+0000a1b0: 5f64 6628 6e6f 726d 616c 697a 6564 3d54  _df(normalized=T
+0000a1c0: 7275 6529 2e6c 6f63 5b3a 2c20 7365 6c65  rue).loc[:, sele
+0000a1d0: 6374 6564 5f67 656e 6573 5d2e 7375 6d28  cted_genes].sum(
+0000a1e0: 6178 6973 3d31 2920 3d3d 2030 292e 6173  axis=1) == 0).as
+0000a1f0: 7479 7065 2822 7374 7222 292e 6173 7479  type("str").asty
+0000a200: 7065 2822 6361 7465 676f 7279 2229 0d0a  pe("category")..
+0000a210: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+0000a220: 7461 2e75 6e73 5b22 6f64 6722 5d5b 226f  ta.uns["odg"]["o
+0000a230: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
+0000a240: 7472 6963 225d 203d 206f 7665 7264 6973  tric"] = overdis
+0000a250: 7065 7273 696f 6e5f 6d65 7472 6963 0d0a  persion_metric..
+0000a260: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+0000a270: 7461 2e75 6e73 5b22 6f64 6722 5d5b 226d  ta.uns["odg"]["m
+0000a280: 696e 5f6d 6561 6e22 5d20 3d20 6d69 6e5f  in_mean"] = min_
+0000a290: 6d65 616e 0d0a 2020 2020 2020 2020 7365  mean..        se
+0000a2a0: 6c66 2e61 6461 7461 2e75 6e73 5b22 6f64  lf.adata.uns["od
+0000a2b0: 6722 5d5b 226d 696e 5f73 636f 7265 225d  g"]["min_score"]
+0000a2c0: 203d 206d 696e 5f73 636f 7265 2069 6620   = min_score if 
+0000a2d0: 6d69 6e5f 7363 6f72 6520 6973 206e 6f74  min_score is not
+0000a2e0: 204e 6f6e 6520 656c 7365 2022 220d 0a20   None else "".. 
+0000a2f0: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+0000a300: 612e 756e 735b 226f 6467 225d 5b22 746f  a.uns["odg"]["to
+0000a310: 705f 6e22 5d20 3d20 746f 705f 6e20 6966  p_n"] = top_n if
+0000a320: 2074 6f70 5f6e 2069 7320 6e6f 7420 4e6f   top_n is not No
+0000a330: 6e65 2065 6c73 6520 2222 0d0a 2020 2020  ne else ""..    
+0000a340: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
+0000a350: 6e73 5b22 6f64 6722 5d5b 2271 7561 6e74  ns["odg"]["quant
+0000a360: 696c 6522 5d20 3d20 7175 616e 7469 6c65  ile"] = quantile
+0000a370: 2069 6620 7175 616e 7469 6c65 2069 7320   if quantile is 
+0000a380: 6e6f 7420 4e6f 6e65 2065 6c73 6520 2222  not None else ""
+0000a390: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+0000a3a0: 7070 656e 645f 746f 5f68 6973 746f 7279  ppend_to_history
+0000a3b0: 2822 4f76 6572 6469 7370 6572 7365 6420  ("Overdispersed 
+0000a3c0: 6765 6e65 7320 7365 6c65 6374 6564 2229  genes selected")
+0000a3d0: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+0000a3e0: 696e 6974 6961 6c69 7a65 5f63 6e6d 6628  initialize_cnmf(
+0000a3f0: 7365 6c66 2c20 636e 6d66 5f6f 7574 7075  self, cnmf_outpu
+0000a400: 745f 6469 723a 2073 7472 2c0d 0a20 2020  t_dir: str,..   
 0000a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a420: 2020 2020 636e 6d66 5f6e 616d 653a 2073      cnmf_name: s
-0000a430: 7472 2c0d 0a20 2020 2020 2020 2020 2020  tr,..           
-0000a440: 2020 2020 2020 2020 2020 2020 206b 7661               kva
-0000a450: 6c73 3a20 436f 6c6c 6563 7469 6f6e 203d  ls: Collection =
-0000a460: 2072 616e 6765 2832 2c20 3631 292c 0d0a   range(2, 61),..
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a480: 2020 2020 2020 2020 6e5f 6974 6572 3a20          n_iter: 
-0000a490: 696e 7420 3d20 3230 302c 0d0a 2020 2020  int = 200,..    
+0000a420: 2020 2020 2063 6e6d 665f 6e61 6d65 3a20       cnmf_name: 
+0000a430: 7374 722c 0d0a 2020 2020 2020 2020 2020  str,..          
+0000a440: 2020 2020 2020 2020 2020 2020 2020 6b76                kv
+0000a450: 616c 733a 2043 6f6c 6c65 6374 696f 6e20  als: Collection 
+0000a460: 3d20 7261 6e67 6528 322c 2036 3129 2c0d  = range(2, 61),.
+0000a470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a480: 2020 2020 2020 2020 206e 5f69 7465 723a           n_iter:
+0000a490: 2069 6e74 203d 2032 3030 2c0d 0a20 2020   int = 200,..   
 0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4b0: 2020 2020 6265 7461 5f6c 6f73 733a 2073      beta_loss: s
-0000a4c0: 7472 203d 2022 6b75 6c6c 6261 636b 2d6c  tr = "kullback-l
-0000a4d0: 6569 626c 6572 222c 0d0a 2020 2020 2020  eibler",..      
+0000a4b0: 2020 2020 2062 6574 615f 6c6f 7373 3a20       beta_loss: 
+0000a4c0: 7374 7220 3d20 226b 756c 6c62 6163 6b2d  str = "kullback-
+0000a4d0: 6c65 6962 6c65 7222 2c0d 0a20 2020 2020  leibler",..     
 0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4f0: 2020 7365 6564 3a20 4f70 7469 6f6e 616c    seed: Optional
-0000a500: 5b69 6e74 5d20 3d20 4e6f 6e65 2920 2d3e  [int] = None) ->
-0000a510: 2063 6e6d 662e 634e 4d46 3a0d 0a20 2020   cnmf.cNMF:..   
-0000a520: 2020 2020 2022 2222 496e 6974 6961 6c69       """Initiali
-0000a530: 7a65 2061 2063 4e4d 4620 7275 6e20 666f  ze a cNMF run fo
-0000a540: 7220 7375 6273 6571 7565 6e74 2066 6163  r subsequent fac
-0000a550: 746f 7269 7a61 7469 6f6e 2e0d 0a0d 0a20  torization..... 
-0000a560: 2020 2020 2020 203a 7061 7261 6d20 636e         :param cn
-0000a570: 6d66 5f6f 7574 7075 745f 6469 723a 204f  mf_output_dir: O
-0000a580: 7574 7075 7420 6469 7265 6374 6f72 7920  utput directory 
-0000a590: 666f 7220 634e 4d46 2072 6573 756c 7473  for cNMF results
-0000a5a0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-0000a5b0: 636e 6d66 5f6f 7574 7075 745f 6469 723a  cnmf_output_dir:
-0000a5c0: 2073 7472 0d0a 2020 2020 2020 2020 3a70   str..        :p
-0000a5d0: 6172 616d 2063 6e6d 665f 6e61 6d65 3a20  aram cnmf_name: 
-0000a5e0: 4e61 6d65 206f 6620 7468 6520 634e 4d46  Name of the cNMF
-0000a5f0: 2072 6573 756c 7473 2e20 4669 6c65 7320   results. Files 
-0000a600: 7769 6c6c 2062 6520 6f75 7470 7574 2074  will be output t
-0000a610: 6f20 5b63 6e6d 665f 6f75 7470 7574 5f64  o [cnmf_output_d
-0000a620: 6972 5d2f 5b63 6e6d 665f 6e61 6d65 5d2f  ir]/[cnmf_name]/
-0000a630: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-0000a640: 636e 6d66 5f6e 616d 653a 2073 7472 0d0a  cnmf_name: str..
-0000a650: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
-0000a660: 7661 6c73 3a20 5261 6e6b 7320 666f 7220  vals: Ranks for 
-0000a670: 634e 4d46 2066 6163 746f 7269 7a61 7469  cNMF factorizati
-0000a680: 6f6e 2c20 6465 6661 756c 7473 2074 6f20  on, defaults to 
-0000a690: 7261 6e67 6528 322c 2036 3129 0d0a 2020  range(2, 61)..  
-0000a6a0: 2020 2020 2020 3a74 7970 6520 6b76 616c        :type kval
-0000a6b0: 733a 2043 6f6c 6c65 6374 696f 6e2c 206f  s: Collection, o
-0000a6c0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-0000a6d0: 203a 7061 7261 6d20 6e5f 6974 6572 3a20   :param n_iter: 
-0000a6e0: 4e75 6d62 6572 206f 6620 6974 6572 6174  Number of iterat
-0000a6f0: 696f 6e73 2066 726f 6d20 7768 6963 6820  ions from which 
-0000a700: 746f 2062 7569 6c64 2061 2063 6f6e 7365  to build a conse
-0000a710: 6e73 7573 2073 6f6c 7574 696f 6e2c 2064  nsus solution, d
-0000a720: 6566 6175 6c74 7320 746f 2032 3030 0d0a  efaults to 200..
-0000a730: 2020 2020 2020 2020 3a74 7970 6520 6e5f          :type n_
-0000a740: 6974 6572 3a20 696e 742c 206f 7074 696f  iter: int, optio
-0000a750: 6e61 6c0d 0a20 2020 2020 2020 203a 7061  nal..        :pa
-0000a760: 7261 6d20 6265 7461 5f6c 6f73 733a 2062  ram beta_loss: b
-0000a770: 6574 612d 6c6f 7373 2066 756e 6374 696f  eta-loss functio
-0000a780: 6e2c 2065 6974 6865 7220 226b 756c 6c62  n, either "kullb
-0000a790: 6163 6b2d 6c65 6962 6c65 7222 206f 7220  ack-leibler" or 
-0000a7a0: 2266 726f 6265 6e69 7573 222e 2044 6566  "frobenius". Def
-0000a7b0: 6175 6c74 7320 746f 2022 6b75 6c6c 6261  aults to "kullba
-0000a7c0: 636b 2d6c 6569 626c 6572 220d 0a20 2020  ck-leibler"..   
-0000a7d0: 2020 2020 203a 7479 7065 2062 6574 615f       :type beta_
-0000a7e0: 6c6f 7373 3a20 7374 722c 206f 7074 696f  loss: str, optio
-0000a7f0: 6e61 6c0d 0a20 2020 2020 2020 203a 7061  nal..        :pa
-0000a800: 7261 6d20 7365 6564 3a20 5261 6e64 6f6d  ram seed: Random
-0000a810: 2073 6565 6420 666f 7220 7265 7072 6f64   seed for reprod
-0000a820: 7563 6962 696c 6974 792c 2064 6566 6175  ucibility, defau
-0000a830: 6c74 7320 746f 204e 6f6e 650d 0a20 2020  lts to None..   
-0000a840: 2020 2020 203a 7479 7065 2073 6565 643a       :type seed:
-0000a850: 204f 7074 696f 6e61 6c5b 696e 745d 2c20   Optional[int], 
-0000a860: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-0000a870: 2020 3a72 6574 7572 6e3a 2063 4e4d 4620    :return: cNMF 
-0000a880: 6f62 6a65 6374 0d0a 2020 2020 2020 2020  object..        
-0000a890: 3a72 7479 7065 3a20 3a63 6c61 7373 3a60  :rtype: :class:`
-0000a8a0: 6d6f 7361 6963 6d70 692e 636e 6d66 2e63  mosaicmpi.cnmf.c
-0000a8b0: 4e4d 4660 0d0a 2020 2020 2020 2020 2222  NMF`..        ""
-0000a8c0: 220d 0a20 2020 2020 2020 2063 6e6d 665f  "..        cnmf_
-0000a8d0: 6f62 6a20 3d20 636e 6d66 2e63 4e4d 4628  obj = cnmf.cNMF(
-0000a8e0: 6f75 7470 7574 5f64 6972 3d63 6e6d 665f  output_dir=cnmf_
-0000a8f0: 6f75 7470 7574 5f64 6972 2c20 6e61 6d65  output_dir, name
-0000a900: 3d63 6e6d 665f 6e61 6d65 290d 0a20 2020  =cnmf_name)..   
-0000a910: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
-0000a920: 2077 7269 7465 2054 504d 2028 6e6f 726d   write TPM (norm
-0000a930: 616c 697a 6564 2920 6461 7461 0d0a 2020  alized) data..  
-0000a940: 2020 2020 2020 7470 6d20 3d20 6164 2e41        tpm = ad.A
-0000a950: 6e6e 4461 7461 2873 656c 662e 746f 5f64  nnData(self.to_d
-0000a960: 6628 6e6f 726d 616c 697a 6564 3d54 7275  f(normalized=Tru
-0000a970: 6529 290d 0a20 2020 2020 2020 2074 706d  e))..        tpm
-0000a980: 2e77 7269 7465 5f68 3561 6428 636e 6d66  .write_h5ad(cnmf
-0000a990: 5f6f 626a 2e70 6174 6873 5b22 7470 6d22  _obj.paths["tpm"
-0000a9a0: 5d29 0d0a 0d0a 2020 2020 2020 2020 6765  ])....        ge
-0000a9b0: 6e65 5f74 706d 5f6d 6561 6e20 3d20 6e70  ne_tpm_mean = np
-0000a9c0: 2e61 7272 6179 2874 706d 2e58 2e6d 6561  .array(tpm.X.mea
-0000a9d0: 6e28 6178 6973 3d30 2929 2e72 6573 6861  n(axis=0)).resha
-0000a9e0: 7065 282d 3129 0d0a 2020 2020 2020 2020  pe(-1)..        
-0000a9f0: 6765 6e65 5f74 706d 5f73 7464 6465 7620  gene_tpm_stddev 
-0000aa00: 3d20 6e70 2e61 7272 6179 2874 706d 2e58  = np.array(tpm.X
-0000aa10: 2e73 7464 2861 7869 733d 302c 2064 646f  .std(axis=0, ddo
-0000aa20: 663d 3029 292e 7265 7368 6170 6528 2d31  f=0)).reshape(-1
-0000aa30: 290d 0a20 2020 2020 2020 2069 6e70 7574  )..        input
-0000aa40: 5f74 706d 5f73 7461 7473 203d 2070 642e  _tpm_stats = pd.
-0000aa50: 4461 7461 4672 616d 6528 5b67 656e 655f  DataFrame([gene_
-0000aa60: 7470 6d5f 6d65 616e 2c20 6765 6e65 5f74  tpm_mean, gene_t
-0000aa70: 706d 5f73 7464 6465 765d 2c20 696e 6465  pm_stddev], inde
-0000aa80: 7820 3d20 5b27 5f5f 6d65 616e 272c 2027  x = ['__mean', '
-0000aa90: 5f5f 7374 6427 5d29 2e54 0d0a 2020 2020  __std']).T..    
-0000aaa0: 2020 2020 7574 696c 732e 7361 7665 5f64      utils.save_d
-0000aab0: 665f 746f 5f6e 707a 2869 6e70 7574 5f74  f_to_npz(input_t
-0000aac0: 706d 5f73 7461 7473 2c20 636e 6d66 5f6f  pm_stats, cnmf_o
-0000aad0: 626a 2e70 6174 6873 5b27 7470 6d5f 7374  bj.paths['tpm_st
-0000aae0: 6174 7327 5d29 0d0a 2020 2020 2020 2020  ats'])..        
-0000aaf0: 6f76 6572 6469 7370 6572 7365 645f 6765  overdispersed_ge
-0000ab00: 6e65 7320 3d20 7365 6c66 2e61 6461 7461  nes = self.adata
-0000ab10: 2e76 6172 5b22 7365 6c65 6374 6564 225d  .var["selected"]
-0000ab20: 5b73 656c 662e 6164 6174 612e 7661 725b  [self.adata.var[
-0000ab30: 2273 656c 6563 7465 6422 5d5d 2e69 6e64  "selected"]].ind
-0000ab40: 6578 0d0a 0d0a 2020 2020 2020 2020 2320  ex....        # 
-0000ab50: 5375 6273 6574 206f 7574 2068 6967 682d  Subset out high-
-0000ab60: 7661 7269 616e 6365 2067 656e 6573 0d0a  variance genes..
-0000ab70: 2020 2020 2020 2020 6e6f 726d 5f63 6f75          norm_cou
-0000ab80: 6e74 7320 3d20 7365 6c66 2e61 6461 7461  nts = self.adata
-0000ab90: 5b3a 2c20 6f76 6572 6469 7370 6572 7365  [:, overdisperse
-0000aba0: 645f 6765 6e65 735d 0d0a 2020 2020 2020  d_genes]..      
-0000abb0: 2020 2323 2053 6361 6c65 2067 656e 6573    ## Scale genes
-0000abc0: 2074 6f20 756e 6974 2076 6172 6961 6e63   to unit varianc
-0000abd0: 650d 0a20 2020 2020 2020 2069 6620 7370  e..        if sp
-0000abe0: 2e69 7373 7061 7273 6528 7470 6d2e 5829  .issparse(tpm.X)
-0000abf0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-0000ac00: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
-0000ac10: 7465 6445 7272 6f72 2822 416e 6e44 6174  tedError("AnnDat
-0000ac20: 6173 2077 6974 6820 7370 6172 7365 206d  as with sparse m
-0000ac30: 6174 7269 6365 7320 6172 6520 6e6f 7420  atrices are not 
-0000ac40: 7375 7070 6f72 7465 6420 6279 206d 6f73  supported by mos
-0000ac50: 6169 634d 5049 2079 6574 2e22 290d 0a20  aicMPI yet.").. 
-0000ac60: 2020 2020 2020 2020 2020 2023 2073 632e             # sc.
-0000ac70: 7070 2e73 6361 6c65 286e 6f72 6d5f 636f  pp.scale(norm_co
-0000ac80: 756e 7473 2c20 7a65 726f 5f63 656e 7465  unts, zero_cente
-0000ac90: 723d 4661 6c73 6529 0d0a 2020 2020 2020  r=False)..      
-0000aca0: 2020 2020 2020 2320 6966 206e 702e 6973        # if np.is
-0000acb0: 6e61 6e28 6e6f 726d 5f63 6f75 6e74 732e  nan(norm_counts.
-0000acc0: 582e 6461 7461 292e 7375 6d28 2920 3e20  X.data).sum() > 
-0000acd0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-0000ace0: 2320 2020 2020 7261 6973 6520 5661 6c75  #     raise Valu
-0000acf0: 6545 7272 6f72 2827 4e61 4e73 2069 6e20  eError('NaNs in 
-0000ad00: 6e6f 726d 616c 697a 6564 2063 6f75 6e74  normalized count
-0000ad10: 7320 6d61 7472 6978 2729 2020 2020 2020  s matrix')      
+0000a4f0: 2020 2073 6565 643a 204f 7074 696f 6e61     seed: Optiona
+0000a500: 6c5b 696e 745d 203d 204e 6f6e 6529 202d  l[int] = None) -
+0000a510: 3e20 636e 6d66 2e63 4e4d 463a 0d0a 2020  > cnmf.cNMF:..  
+0000a520: 2020 2020 2020 2222 2249 6e69 7469 616c        """Initial
+0000a530: 697a 6520 6120 634e 4d46 2072 756e 2066  ize a cNMF run f
+0000a540: 6f72 2073 7562 7365 7175 656e 7420 6661  or subsequent fa
+0000a550: 6374 6f72 697a 6174 696f 6e2e 0d0a 0d0a  ctorization.....
+0000a560: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
+0000a570: 6e6d 665f 6f75 7470 7574 5f64 6972 3a20  nmf_output_dir: 
+0000a580: 4f75 7470 7574 2064 6972 6563 746f 7279  Output directory
+0000a590: 2066 6f72 2063 4e4d 4620 7265 7375 6c74   for cNMF result
+0000a5a0: 730d 0a20 2020 2020 2020 203a 7479 7065  s..        :type
+0000a5b0: 2063 6e6d 665f 6f75 7470 7574 5f64 6972   cnmf_output_dir
+0000a5c0: 3a20 7374 720d 0a20 2020 2020 2020 203a  : str..        :
+0000a5d0: 7061 7261 6d20 636e 6d66 5f6e 616d 653a  param cnmf_name:
+0000a5e0: 204e 616d 6520 6f66 2074 6865 2063 4e4d   Name of the cNM
+0000a5f0: 4620 7265 7375 6c74 732e 2046 696c 6573  F results. Files
+0000a600: 2077 696c 6c20 6265 206f 7574 7075 7420   will be output 
+0000a610: 746f 205b 636e 6d66 5f6f 7574 7075 745f  to [cnmf_output_
+0000a620: 6469 725d 2f5b 636e 6d66 5f6e 616d 655d  dir]/[cnmf_name]
+0000a630: 2f0d 0a20 2020 2020 2020 203a 7479 7065  /..        :type
+0000a640: 2063 6e6d 665f 6e61 6d65 3a20 7374 720d   cnmf_name: str.
+0000a650: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000a660: 6b76 616c 733a 2052 616e 6b73 2066 6f72  kvals: Ranks for
+0000a670: 2063 4e4d 4620 6661 6374 6f72 697a 6174   cNMF factorizat
+0000a680: 696f 6e2c 2064 6566 6175 6c74 7320 746f  ion, defaults to
+0000a690: 2072 616e 6765 2832 2c20 3631 290d 0a20   range(2, 61).. 
+0000a6a0: 2020 2020 2020 203a 7479 7065 206b 7661         :type kva
+0000a6b0: 6c73 3a20 436f 6c6c 6563 7469 6f6e 2c20  ls: Collection, 
+0000a6c0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+0000a6d0: 2020 3a70 6172 616d 206e 5f69 7465 723a    :param n_iter:
+0000a6e0: 204e 756d 6265 7220 6f66 2069 7465 7261   Number of itera
+0000a6f0: 7469 6f6e 7320 6672 6f6d 2077 6869 6368  tions from which
+0000a700: 2074 6f20 6275 696c 6420 6120 636f 6e73   to build a cons
+0000a710: 656e 7375 7320 736f 6c75 7469 6f6e 2c20  ensus solution, 
+0000a720: 6465 6661 756c 7473 2074 6f20 3230 300d  defaults to 200.
+0000a730: 0a20 2020 2020 2020 203a 7479 7065 206e  .        :type n
+0000a740: 5f69 7465 723a 2069 6e74 2c20 6f70 7469  _iter: int, opti
+0000a750: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
+0000a760: 6172 616d 2062 6574 615f 6c6f 7373 3a20  aram beta_loss: 
+0000a770: 6265 7461 2d6c 6f73 7320 6675 6e63 7469  beta-loss functi
+0000a780: 6f6e 2c20 6569 7468 6572 2022 6b75 6c6c  on, either "kull
+0000a790: 6261 636b 2d6c 6569 626c 6572 2220 6f72  back-leibler" or
+0000a7a0: 2022 6672 6f62 656e 6975 7322 2e20 4465   "frobenius". De
+0000a7b0: 6661 756c 7473 2074 6f20 226b 756c 6c62  faults to "kullb
+0000a7c0: 6163 6b2d 6c65 6962 6c65 7222 0d0a 2020  ack-leibler"..  
+0000a7d0: 2020 2020 2020 3a74 7970 6520 6265 7461        :type beta
+0000a7e0: 5f6c 6f73 733a 2073 7472 2c20 6f70 7469  _loss: str, opti
+0000a7f0: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
+0000a800: 6172 616d 2073 6565 643a 2052 616e 646f  aram seed: Rando
+0000a810: 6d20 7365 6564 2066 6f72 2072 6570 726f  m seed for repro
+0000a820: 6475 6369 6269 6c69 7479 2c20 6465 6661  ducibility, defa
+0000a830: 756c 7473 2074 6f20 4e6f 6e65 0d0a 2020  ults to None..  
+0000a840: 2020 2020 2020 3a74 7970 6520 7365 6564        :type seed
+0000a850: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d2c  : Optional[int],
+0000a860: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+0000a870: 2020 203a 7265 7475 726e 3a20 634e 4d46     :return: cNMF
+0000a880: 206f 626a 6563 740d 0a20 2020 2020 2020   object..       
+0000a890: 203a 7274 7970 653a 203a 636c 6173 733a   :rtype: :class:
+0000a8a0: 606d 6f73 6169 636d 7069 2e63 6e6d 662e  `mosaicmpi.cnmf.
+0000a8b0: 634e 4d46 600d 0a20 2020 2020 2020 2022  cNMF`..        "
+0000a8c0: 2222 0d0a 2020 2020 2020 2020 636e 6d66  ""..        cnmf
+0000a8d0: 5f6f 626a 203d 2063 6e6d 662e 634e 4d46  _obj = cnmf.cNMF
+0000a8e0: 286f 7574 7075 745f 6469 723d 636e 6d66  (output_dir=cnmf
+0000a8f0: 5f6f 7574 7075 745f 6469 722c 206e 616d  _output_dir, nam
+0000a900: 653d 636e 6d66 5f6e 616d 6529 0d0a 2020  e=cnmf_name)..  
+0000a910: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000a920: 2320 7772 6974 6520 5450 4d20 286e 6f72  # write TPM (nor
+0000a930: 6d61 6c69 7a65 6429 2064 6174 610d 0a20  malized) data.. 
+0000a940: 2020 2020 2020 2074 706d 203d 2061 642e         tpm = ad.
+0000a950: 416e 6e44 6174 6128 7365 6c66 2e74 6f5f  AnnData(self.to_
+0000a960: 6466 286e 6f72 6d61 6c69 7a65 643d 5472  df(normalized=Tr
+0000a970: 7565 2929 0d0a 2020 2020 2020 2020 7470  ue))..        tp
+0000a980: 6d2e 7772 6974 655f 6835 6164 2863 6e6d  m.write_h5ad(cnm
+0000a990: 665f 6f62 6a2e 7061 7468 735b 2274 706d  f_obj.paths["tpm
+0000a9a0: 225d 290d 0a0d 0a20 2020 2020 2020 2067  "])....        g
+0000a9b0: 656e 655f 7470 6d5f 6d65 616e 203d 206e  ene_tpm_mean = n
+0000a9c0: 702e 6172 7261 7928 7470 6d2e 582e 6d65  p.array(tpm.X.me
+0000a9d0: 616e 2861 7869 733d 3029 292e 7265 7368  an(axis=0)).resh
+0000a9e0: 6170 6528 2d31 290d 0a20 2020 2020 2020  ape(-1)..       
+0000a9f0: 2067 656e 655f 7470 6d5f 7374 6464 6576   gene_tpm_stddev
+0000aa00: 203d 206e 702e 6172 7261 7928 7470 6d2e   = np.array(tpm.
+0000aa10: 582e 7374 6428 6178 6973 3d30 2c20 6464  X.std(axis=0, dd
+0000aa20: 6f66 3d30 2929 2e72 6573 6861 7065 282d  of=0)).reshape(-
+0000aa30: 3129 0d0a 2020 2020 2020 2020 696e 7075  1)..        inpu
+0000aa40: 745f 7470 6d5f 7374 6174 7320 3d20 7064  t_tpm_stats = pd
+0000aa50: 2e44 6174 6146 7261 6d65 285b 6765 6e65  .DataFrame([gene
+0000aa60: 5f74 706d 5f6d 6561 6e2c 2067 656e 655f  _tpm_mean, gene_
+0000aa70: 7470 6d5f 7374 6464 6576 5d2c 2069 6e64  tpm_stddev], ind
+0000aa80: 6578 203d 205b 275f 5f6d 6561 6e27 2c20  ex = ['__mean', 
+0000aa90: 275f 5f73 7464 275d 292e 540d 0a20 2020  '__std']).T..   
+0000aaa0: 2020 2020 2075 7469 6c73 2e73 6176 655f       utils.save_
+0000aab0: 6466 5f74 6f5f 6e70 7a28 696e 7075 745f  df_to_npz(input_
+0000aac0: 7470 6d5f 7374 6174 732c 2063 6e6d 665f  tpm_stats, cnmf_
+0000aad0: 6f62 6a2e 7061 7468 735b 2774 706d 5f73  obj.paths['tpm_s
+0000aae0: 7461 7473 275d 290d 0a20 2020 2020 2020  tats'])..       
+0000aaf0: 206f 7665 7264 6973 7065 7273 6564 5f67   overdispersed_g
+0000ab00: 656e 6573 203d 2073 656c 662e 6164 6174  enes = self.adat
+0000ab10: 612e 7661 725b 2273 656c 6563 7465 6422  a.var["selected"
+0000ab20: 5d5b 7365 6c66 2e61 6461 7461 2e76 6172  ][self.adata.var
+0000ab30: 5b22 7365 6c65 6374 6564 225d 5d2e 696e  ["selected"]].in
+0000ab40: 6465 780d 0a0d 0a20 2020 2020 2020 2023  dex....        #
+0000ab50: 2053 7562 7365 7420 6f75 7420 6869 6768   Subset out high
+0000ab60: 2d76 6172 6961 6e63 6520 6765 6e65 730d  -variance genes.
+0000ab70: 0a20 2020 2020 2020 206e 6f72 6d5f 636f  .        norm_co
+0000ab80: 756e 7473 203d 2073 656c 662e 6164 6174  unts = self.adat
+0000ab90: 615b 3a2c 206f 7665 7264 6973 7065 7273  a[:, overdispers
+0000aba0: 6564 5f67 656e 6573 5d0d 0a20 2020 2020  ed_genes]..     
+0000abb0: 2020 2023 2320 5363 616c 6520 6765 6e65     ## Scale gene
+0000abc0: 7320 746f 2075 6e69 7420 7661 7269 616e  s to unit varian
+0000abd0: 6365 0d0a 2020 2020 2020 2020 6966 2073  ce..        if s
+0000abe0: 702e 6973 7370 6172 7365 2874 706d 2e58  p.issparse(tpm.X
+0000abf0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000ac00: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+0000ac10: 6e74 6564 4572 726f 7228 2241 6e6e 4461  ntedError("AnnDa
+0000ac20: 7461 7320 7769 7468 2073 7061 7273 6520  tas with sparse 
+0000ac30: 6d61 7472 6963 6573 2061 7265 206e 6f74  matrices are not
+0000ac40: 2073 7570 706f 7274 6564 2062 7920 6d6f   supported by mo
+0000ac50: 7361 6963 4d50 4920 7965 742e 2229 0d0a  saicMPI yet.")..
+0000ac60: 2020 2020 2020 2020 2020 2020 2320 7363              # sc
+0000ac70: 2e70 702e 7363 616c 6528 6e6f 726d 5f63  .pp.scale(norm_c
+0000ac80: 6f75 6e74 732c 207a 6572 6f5f 6365 6e74  ounts, zero_cent
+0000ac90: 6572 3d46 616c 7365 290d 0a20 2020 2020  er=False)..     
+0000aca0: 2020 2020 2020 2023 2069 6620 6e70 2e69         # if np.i
+0000acb0: 736e 616e 286e 6f72 6d5f 636f 756e 7473  snan(norm_counts
+0000acc0: 2e58 2e64 6174 6129 2e73 756d 2829 203e  .X.data).sum() >
+0000acd0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+0000ace0: 2023 2020 2020 2072 6169 7365 2056 616c   #     raise Val
+0000acf0: 7565 4572 726f 7228 274e 614e 7320 696e  ueError('NaNs in
+0000ad00: 206e 6f72 6d61 6c69 7a65 6420 636f 756e   normalized coun
+0000ad10: 7473 206d 6174 7269 7827 2920 2020 2020  ts matrix')     
 0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad30: 200d 0a20 2020 2020 2020 2065 6c73 653a   ..        else:
-0000ad40: 0d0a 2020 2020 2020 2020 2020 2020 6e6f  ..            no
-0000ad50: 726d 5f63 6f75 6e74 732e 5820 2f3d 206e  rm_counts.X /= n
-0000ad60: 6f72 6d5f 636f 756e 7473 2e58 2e73 7464  orm_counts.X.std
-0000ad70: 2861 7869 733d 302c 2064 646f 663d 3129  (axis=0, ddof=1)
-0000ad80: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000ad90: 206e 702e 6973 6e61 6e28 6e6f 726d 5f63   np.isnan(norm_c
-0000ada0: 6f75 6e74 732e 5829 2e73 756d 2829 2e73  ounts.X).sum().s
-0000adb0: 756d 2829 203e 2030 3a0d 0a20 2020 2020  um() > 0:..     
-0000adc0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000add0: 2056 616c 7565 4572 726f 7228 274e 614e   ValueError('NaN
-0000ade0: 7320 696e 206e 6f72 6d61 6c69 7a65 6420  s in normalized 
-0000adf0: 636f 756e 7473 206d 6174 7269 7827 2920  counts matrix') 
+0000ad30: 2020 0d0a 2020 2020 2020 2020 656c 7365    ..        else
+0000ad40: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
+0000ad50: 6f72 6d5f 636f 756e 7473 2e58 202f 3d20  orm_counts.X /= 
+0000ad60: 6e6f 726d 5f63 6f75 6e74 732e 582e 7374  norm_counts.X.st
+0000ad70: 6428 6178 6973 3d30 2c20 6464 6f66 3d31  d(axis=0, ddof=1
+0000ad80: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0000ad90: 6620 6e70 2e69 736e 616e 286e 6f72 6d5f  f np.isnan(norm_
+0000ada0: 636f 756e 7473 2e58 292e 7375 6d28 292e  counts.X).sum().
+0000adb0: 7375 6d28 2920 3e20 303a 0d0a 2020 2020  sum() > 0:..    
+0000adc0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000add0: 6520 5661 6c75 6545 7272 6f72 2827 4e61  e ValueError('Na
+0000ade0: 4e73 2069 6e20 6e6f 726d 616c 697a 6564  Ns in normalized
+0000adf0: 2063 6f75 6e74 7320 6d61 7472 6978 2729   counts matrix')
 0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae10: 2020 200d 0a0d 0a20 2020 2020 2020 2023     ....        #
-0000ae20: 2320 5361 7665 2061 205c 6e2d 6465 6c69  # Save a \n-deli
-0000ae30: 6d69 7465 6420 6c69 7374 206f 6620 7468  mited list of th
-0000ae40: 6520 6869 6768 2d76 6172 6961 6e63 6520  e high-variance 
-0000ae50: 6765 6e65 7320 7573 6564 2066 6f72 2066  genes used for f
-0000ae60: 6163 746f 7269 7a61 7469 6f6e 0d0a 2020  actorization..  
-0000ae70: 2020 2020 2020 6f70 656e 2863 6e6d 665f        open(cnmf_
-0000ae80: 6f62 6a2e 7061 7468 735b 276e 6d66 5f67  obj.paths['nmf_g
-0000ae90: 656e 6573 5f6c 6973 7427 5d2c 2027 7727  enes_list'], 'w'
-0000aea0: 292e 7772 6974 6528 275c 6e27 2e6a 6f69  ).write('\n'.joi
-0000aeb0: 6e28 6f76 6572 6469 7370 6572 7365 645f  n(overdispersed_
-0000aec0: 6765 6e65 7329 290d 0a0d 0a20 2020 2020  genes))....     
-0000aed0: 2020 2069 6620 6e6f 726d 5f63 6f75 6e74     if norm_count
-0000aee0: 732e 582e 6474 7970 6520 213d 206e 702e  s.X.dtype != np.
-0000aef0: 666c 6f61 7436 343a 0d0a 2020 2020 2020  float64:..      
-0000af00: 2020 2020 2020 6e6f 726d 5f63 6f75 6e74        norm_count
-0000af10: 732e 5820 3d20 6e6f 726d 5f63 6f75 6e74  s.X = norm_count
-0000af20: 732e 582e 6173 7479 7065 286e 702e 666c  s.X.astype(np.fl
-0000af30: 6f61 7436 3429 0d0a 0d0a 2020 2020 2020  oat64)....      
-0000af40: 2020 6e6f 726d 5f63 6f75 6e74 732e 7772    norm_counts.wr
-0000af50: 6974 655f 6835 6164 2863 6e6d 665f 6f62  ite_h5ad(cnmf_ob
-0000af60: 6a2e 7061 7468 735b 276e 6f72 6d61 6c69  j.paths['normali
-0000af70: 7a65 645f 636f 756e 7473 275d 290d 0a0d  zed_counts'])...
-0000af80: 0a20 2020 2020 2020 2023 2073 6176 6520  .        # save 
-0000af90: 7061 7261 6d65 7465 7273 2066 6f72 2066  parameters for f
-0000afa0: 6163 746f 7269 7a61 7469 6f6e 2073 7465  actorization ste
-0000afb0: 700d 0a20 2020 2020 2020 2063 6e6d 665f  p..        cnmf_
-0000afc0: 6f62 6a2e 7361 7665 5f6e 6d66 5f69 7465  obj.save_nmf_ite
-0000afd0: 725f 7061 7261 6d73 282a 636e 6d66 5f6f  r_params(*cnmf_o
-0000afe0: 626a 2e67 6574 5f6e 6d66 5f69 7465 725f  bj.get_nmf_iter_
-0000aff0: 7061 7261 6d73 286b 733d 6b76 616c 732c  params(ks=kvals,
-0000b000: 206e 5f69 7465 723d 6e5f 6974 6572 2c20   n_iter=n_iter, 
-0000b010: 7261 6e64 6f6d 5f73 7461 7465 5f73 6565  random_state_see
-0000b020: 643d 7365 6564 2c20 6265 7461 5f6c 6f73  d=seed, beta_los
-0000b030: 733d 6265 7461 5f6c 6f73 7329 290d 0a0d  s=beta_loss))...
-0000b040: 0a20 2020 2020 2020 2023 2073 6176 6520  .        # save 
-0000b050: 7061 7261 6d65 7465 7273 2069 6e20 416e  parameters in An
-0000b060: 6e44 6174 6120 6f62 6a65 6374 0d0a 2020  nData object..  
-0000b070: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
-0000b080: 2e75 6e73 5b22 636e 6d66 225d 203d 2063  .uns["cnmf"] = c
-0000b090: 6e6d 665f 6f62 6a2e 6765 745f 6e6d 665f  nmf_obj.get_nmf_
-0000b0a0: 6974 6572 5f70 6172 616d 7328 6b73 3d6b  iter_params(ks=k
-0000b0b0: 7661 6c73 2c20 6e5f 6974 6572 3d6e 5f69  vals, n_iter=n_i
-0000b0c0: 7465 722c 2072 616e 646f 6d5f 7374 6174  ter, random_stat
-0000b0d0: 655f 7365 6564 3d73 6565 642c 2062 6574  e_seed=seed, bet
-0000b0e0: 615f 6c6f 7373 3d62 6574 615f 6c6f 7373  a_loss=beta_loss
-0000b0f0: 295b 315d 2020 2320 6469 6374 206f 6620  )[1]  # dict of 
-0000b100: 636e 6d66 2070 6172 616d 6574 6572 730d  cnmf parameters.
-0000b110: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-0000b120: 2020 2073 656c 662e 6170 7065 6e64 5f74     self.append_t
-0000b130: 6f5f 6869 7374 6f72 7928 6622 634e 4d46  o_history(f"cNMF
-0000b140: 2070 6172 616d 6574 6572 7320 6164 6465   parameters adde
-0000b150: 642e 2063 4e4d 4620 696e 7075 7473 2069  d. cNMF inputs i
-0000b160: 6e69 7469 616c 697a 6564 2069 6e20 7b63  nitialized in {c
-0000b170: 6e6d 665f 6f75 7470 7574 5f64 6972 7d2f  nmf_output_dir}/
-0000b180: 7b63 6e6d 665f 6e61 6d65 7d22 290d 0a20  {cnmf_name}").. 
-0000b190: 2020 2020 2020 2072 6574 7572 6e20 636e         return cn
-0000b1a0: 6d66 5f6f 626a 0d0a 2020 2020 0d0a 2020  mf_obj..    ..  
-0000b1b0: 2020 6465 6620 6164 645f 636e 6d66 5f72    def add_cnmf_r
-0000b1c0: 6573 756c 7473 2873 656c 662c 2063 6e6d  esults(self, cnm
-0000b1d0: 665f 6f75 7470 7574 5f64 6972 2c20 636e  f_output_dir, cn
-0000b1e0: 6d66 5f6e 616d 652c 206c 6f63 616c 5f64  mf_name, local_d
-0000b1f0: 656e 7369 7479 5f74 6872 6573 686f 6c64  ensity_threshold
-0000b200: 3a20 666c 6f61 7420 3d20 4e6f 6e65 2c20  : float = None, 
-0000b210: 6c6f 6361 6c5f 6e65 6967 6862 6f72 686f  local_neighborho
-0000b220: 6f64 5f73 697a 653a 2066 6c6f 6174 203d  od_size: float =
-0000b230: 204e 6f6e 6529 3a0d 0a20 2020 2020 2020   None):..       
-0000b240: 2022 2222 0d0a 2020 2020 2020 2020 4166   """..        Af
-0000b250: 7465 7220 6661 6374 6f72 697a 6174 696f  ter factorizatio
-0000b260: 6e2c 2061 6464 2063 6f6d 706c 6574 6564  n, add completed
-0000b270: 2063 4e4d 4620 7265 7375 6c74 7320 696e   cNMF results in
-0000b280: 205b 636e 6d66 5f6f 7574 7075 745f 6469   [cnmf_output_di
-0000b290: 725d 2f5b 636e 6d66 5f6e 616d 655d 2074  r]/[cnmf_name] t
-0000b2a0: 6f20 7468 6520 6461 7461 7365 7420 6f62  o the dataset ob
-0000b2b0: 6a65 6374 2e0d 0a0d 0a20 2020 2020 2020  ject.....       
-0000b2c0: 203a 7061 7261 6d20 636e 6d66 5f6f 7574   :param cnmf_out
-0000b2d0: 7075 745f 6469 723a 204f 7574 7075 7420  put_dir: Output 
-0000b2e0: 6469 7265 6374 6f72 7920 666f 7220 634e  directory for cN
-0000b2f0: 4d46 2072 6573 756c 7473 0d0a 2020 2020  MF results..    
-0000b300: 2020 2020 3a74 7970 6520 636e 6d66 5f6f      :type cnmf_o
-0000b310: 7574 7075 745f 6469 723a 2073 7472 0d0a  utput_dir: str..
-0000b320: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-0000b330: 6e6d 665f 6e61 6d65 3a20 4e61 6d65 206f  nmf_name: Name o
-0000b340: 6620 7468 6520 634e 4d46 2072 6573 756c  f the cNMF resul
-0000b350: 7473 2e20 4669 6c65 7320 7769 6c6c 2062  ts. Files will b
-0000b360: 6520 6f75 7470 7574 2074 6f20 5b63 6e6d  e output to [cnm
-0000b370: 665f 6f75 7470 7574 5f64 6972 5d2f 5b63  f_output_dir]/[c
-0000b380: 6e6d 665f 6e61 6d65 5d2f 0d0a 2020 2020  nmf_name]/..    
-0000b390: 2020 2020 3a74 7970 6520 636e 6d66 5f6e      :type cnmf_n
-0000b3a0: 616d 653a 2073 7472 0d0a 2020 2020 2020  ame: str..      
-0000b3b0: 2020 3a70 6172 616d 206c 6f63 616c 5f64    :param local_d
-0000b3c0: 656e 7369 7479 5f74 6872 6573 686f 6c64  ensity_threshold
-0000b3d0: 3a20 5468 7265 7368 6f6c 6420 666f 7220  : Threshold for 
-0000b3e0: 7468 6520 6c6f 6361 6c20 6465 6e73 6974  the local densit
-0000b3f0: 7920 6669 6c74 6572 696e 6720 7072 696f  y filtering prio
-0000b400: 7220 746f 2047 4550 2063 6f6e 7365 6e73  r to GEP consens
-0000b410: 7573 2e20 4163 6365 7074 6162 6c65 2074  us. Acceptable t
-0000b420: 6872 6573 686f 6c64 7320 6172 6520 3e20  hresholds are > 
-0000b430: 3020 616e 6420 3c3d 2032 2028 322e 3020  0 and <= 2 (2.0 
-0000b440: 6973 206e 6f20 6669 6c74 6572 696e 6729  is no filtering)
-0000b450: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-0000b460: 6e65 2e0d 0a20 2020 2020 2020 203a 7479  ne...        :ty
-0000b470: 7065 206c 6f63 616c 5f64 656e 7369 7479  pe local_density
-0000b480: 5f74 6872 6573 686f 6c64 3a20 666c 6f61  _threshold: floa
-0000b490: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-0000b4a0: 2020 2020 203a 7061 7261 6d20 6c6f 6361       :param loca
-0000b4b0: 6c5f 6e65 6967 6862 6f72 686f 6f64 5f73  l_neighborhood_s
-0000b4c0: 697a 653a 2046 7261 6374 696f 6e20 6f66  ize: Fraction of
-0000b4d0: 2074 6865 206e 756d 6265 7220 6f66 2072   the number of r
-0000b4e0: 6570 6c69 6361 7465 7320 746f 2075 7365  eplicates to use
-0000b4f0: 2061 7320 6e65 6172 6573 7420 6e65 6967   as nearest neig
-0000b500: 6862 6f72 7320 666f 7220 6c6f 6361 6c20  hbors for local 
-0000b510: 6465 6e73 6974 7920 6669 6c74 6572 696e  density filterin
-0000b520: 672e 2044 6566 6175 6c74 7320 746f 204e  g. Defaults to N
-0000b530: 6f6e 650d 0a20 2020 2020 2020 203a 7479  one..        :ty
-0000b540: 7065 206c 6f63 616c 5f6e 6569 6768 626f  pe local_neighbo
-0000b550: 7268 6f6f 645f 7369 7a65 3a20 666c 6f61  rhood_size: floa
-0000b560: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-0000b570: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000b580: 2020 7365 6c66 2e61 6461 7461 2e75 6e73    self.adata.uns
-0000b590: 5b22 636e 6d66 5f6e 616d 6522 5d20 3d20  ["cnmf_name"] = 
-0000b5a0: 636e 6d66 5f6e 616d 650d 0a0d 0a20 2020  cnmf_name....   
-0000b5b0: 2020 2020 2023 2069 6e66 6572 2066 726f       # infer fro
-0000b5c0: 6d20 6669 6c65 6e61 6d65 7320 7768 6963  m filenames whic
-0000b5d0: 6820 6c6f 6361 6c20 6465 6e73 6974 7920  h local density 
-0000b5e0: 7468 7265 7368 6f6c 6420 7761 7320 7573  threshold was us
-0000b5f0: 6564 0d0a 2020 2020 2020 2020 7365 6e73  ed..        sens
-0000b600: 6564 5f6c 6474 7320 3d20 7365 7428 290d  ed_ldts = set().
-0000b610: 0a20 2020 2020 2020 2066 6f72 2066 6e20  .        for fn 
-0000b620: 696e 2067 6c6f 6228 6f73 2e70 6174 682e  in glob(os.path.
-0000b630: 6a6f 696e 2863 6e6d 665f 6f75 7470 7574  join(cnmf_output
-0000b640: 5f64 6972 2c20 636e 6d66 5f6e 616d 652c  _dir, cnmf_name,
-0000b650: 2066 227b 636e 6d66 5f6e 616d 657d 2a2e   f"{cnmf_name}*.
-0000b660: 2a73 7065 6374 7261 2a2e 6b5f 2a22 2929  *spectra*.k_*"))
-0000b670: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
-0000b680: 6474 5f73 7472 203d 206f 732e 7061 7468  dt_str = os.path
-0000b690: 2e62 6173 656e 616d 6528 666e 292e 7370  .basename(fn).sp
-0000b6a0: 6c69 7428 222e 2229 5b2d 335d 0d0a 2020  lit(".")[-3]..  
-0000b6b0: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
-0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6d0: 6c64 7420 3d20 666c 6f61 7428 6c64 745f  ldt = float(ldt_
-0000b6e0: 7374 722e 7265 706c 6163 6528 2264 745f  str.replace("dt_
-0000b6f0: 222c 2022 2229 2e72 6570 6c61 6365 2822  ", "").replace("
-0000b700: 5f22 2c20 222e 2229 290d 0a20 2020 2020  _", "."))..     
-0000b710: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
-0000b720: 6c75 6545 7272 6f72 3a0d 0a20 2020 2020  lueError:..     
-0000b730: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
-0000b740: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000b750: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000b760: 2020 2020 7365 6e73 6564 5f6c 6474 732e      sensed_ldts.
-0000b770: 6164 6428 286c 6474 5f73 7472 2c20 6c64  add((ldt_str, ld
-0000b780: 7429 290d 0a20 2020 2020 2020 2069 6620  t))..        if 
-0000b790: 6c6f 6361 6c5f 6465 6e73 6974 795f 7468  local_density_th
-0000b7a0: 7265 7368 6f6c 6420 6973 204e 6f6e 6520  reshold is None 
-0000b7b0: 616e 6420 6c65 6e28 7365 6e73 6564 5f6c  and len(sensed_l
-0000b7c0: 6474 7329 203d 3d20 313a 0d0a 2020 2020  dts) == 1:..    
-0000b7d0: 2020 2020 2020 2020 6c64 745f 7374 722c          ldt_str,
-0000b7e0: 206c 6474 203d 2073 656e 7365 645f 6c64   ldt = sensed_ld
-0000b7f0: 7473 2e70 6f70 2829 0d0a 2020 2020 2020  ts.pop()..      
-0000b800: 2020 656c 6966 206c 6f63 616c 5f64 656e    elif local_den
-0000b810: 7369 7479 5f74 6872 6573 686f 6c64 2069  sity_threshold i
-0000b820: 6e20 286c 6474 5b31 5d20 666f 7220 6c64  n (ldt[1] for ld
-0000b830: 7420 696e 2073 656e 7365 645f 6c64 7473  t in sensed_ldts
-0000b840: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000b850: 6c64 745f 7374 722c 206c 6474 203d 205b  ldt_str, ldt = [
-0000b860: 286c 6474 5f73 7472 2c20 6c64 7429 2066  (ldt_str, ldt) f
-0000b870: 6f72 206c 6474 5f73 7472 2c20 6c64 7420  or ldt_str, ldt 
-0000b880: 696e 2073 656e 7365 645f 6c64 7473 2069  in sensed_ldts i
-0000b890: 6620 6c64 7420 3d3d 206c 6f63 616c 5f64  f ldt == local_d
-0000b8a0: 656e 7369 7479 5f74 6872 6573 686f 6c64  ensity_threshold
-0000b8b0: 5d2e 706f 7028 290d 0a20 2020 2020 2020  ].pop()..       
-0000b8c0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0000b8d0: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
-0000b8e0: 6545 7272 6f72 2866 226c 6f63 616c 5f64  eError(f"local_d
-0000b8f0: 656e 7369 7479 5f74 6872 6573 686f 6c64  ensity_threshold
-0000b900: 206f 6620 7b6c 6f63 616c 5f64 656e 7369   of {local_densi
-0000b910: 7479 5f74 6872 6573 686f 6c64 7d20 646f  ty_threshold} do
-0000b920: 6573 206e 6f74 206d 6174 6368 2077 6861  es not match wha
-0000b930: 7420 6973 2069 6e20 7468 6520 634e 4d46  t is in the cNMF
-0000b940: 2072 6573 756c 7420 6469 7265 6374 6f72   result director
-0000b950: 793a 207b 7365 6e73 6564 5f6c 6474 737d  y: {sensed_ldts}
-0000b960: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-0000b970: 2e61 6461 7461 2e75 6e73 5b22 6c64 7422  .adata.uns["ldt"
-0000b980: 5d20 3d20 6c64 740d 0a20 2020 2020 2020  ] = ldt..       
-0000b990: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-0000b9a0: 226c 6e73 225d 203d 206c 6f63 616c 5f6e  "lns"] = local_n
-0000b9b0: 6569 6768 626f 7268 6f6f 645f 7369 7a65  eighborhood_size
-0000b9c0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0000b9d0: 2020 2020 2020 2020 2320 496d 706f 7274          # Import
-0000b9e0: 2047 4550 730d 0a20 2020 2020 2020 2072   GEPs..        r
-0000b9f0: 6573 756c 745f 7479 7065 7320 3d20 7b0d  esult_types = {.
-0000ba00: 0a20 2020 2020 2020 2020 2020 2022 6765  .            "ge
-0000ba10: 6e65 5f73 7065 6374 7261 5f73 636f 7265  ne_spectra_score
-0000ba20: 223a 2022 636e 6d66 5f67 6570 5f73 636f  ": "cnmf_gep_sco
-0000ba30: 7265 222c 0d0a 2020 2020 2020 2020 2020  re",..          
-0000ba40: 2020 2267 656e 655f 7370 6563 7472 615f    "gene_spectra_
-0000ba50: 7470 6d22 3a20 2263 6e6d 665f 6765 705f  tpm": "cnmf_gep_
-0000ba60: 7470 6d22 2c0d 0a20 2020 2020 2020 2020  tpm",..         
-0000ba70: 2020 2022 7370 6563 7472 6122 3a20 2263     "spectra": "c
-0000ba80: 6e6d 665f 6765 705f 7261 7722 0d0a 2020  nmf_gep_raw"..  
-0000ba90: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-0000baa0: 2020 2020 2066 6f72 206d 6174 6368 7374       for matchst
-0000bab0: 722c 2072 6573 756c 745f 7479 7065 2069  r, result_type i
-0000bac0: 6e20 7265 7375 6c74 5f74 7970 6573 2e69  n result_types.i
-0000bad0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-0000bae0: 2020 2020 206c 6f67 6769 6e67 2e69 6e66       logging.inf
-0000baf0: 6f28 6622 496d 706f 7274 696e 6720 4745  o(f"Importing GE
-0000bb00: 5073 3a20 7b6d 6174 6368 7374 727d 2229  Ps: {matchstr}")
-0000bb10: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000bb20: 6d65 7461 5f77 203d 205b 5d0d 0a20 2020  meta_w = []..   
-0000bb30: 2020 2020 2020 2020 2066 6f72 2066 6e20           for fn 
-0000bb40: 696e 2067 6c6f 6228 6f73 2e70 6174 682e  in glob(os.path.
-0000bb50: 6a6f 696e 2863 6e6d 665f 6f75 7470 7574  join(cnmf_output
-0000bb60: 5f64 6972 2c20 636e 6d66 5f6e 616d 652c  _dir, cnmf_name,
-0000bb70: 2066 227b 636e 6d66 5f6e 616d 657d 2a2e   f"{cnmf_name}*.
-0000bb80: 7b6d 6174 6368 7374 727d 2e6b 5f2a 2e7b  {matchstr}.k_*.{
-0000bb90: 6c64 745f 7374 727d 2e2a 7478 7422 2929  ldt_str}.*txt"))
-0000bba0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000bbb0: 2020 206b 203d 2069 6e74 286f 732e 7061     k = int(os.pa
-0000bbc0: 7468 2e62 6173 656e 616d 6528 666e 292e  th.basename(fn).
-0000bbd0: 7265 6d6f 7665 7072 6566 6978 2866 227b  removeprefix(f"{
-0000bbe0: 636e 6d66 5f6e 616d 657d 2e7b 6d61 7463  cnmf_name}.{matc
-0000bbf0: 6873 7472 7d2e 2229 2e73 706c 6974 2822  hstr}.").split("
-0000bc00: 2e22 295b 305d 2e72 6570 6c61 6365 2822  .")[0].replace("
-0000bc10: 6b5f 222c 2022 2229 290d 0a20 2020 2020  k_", ""))..     
-0000bc20: 2020 2020 2020 2020 2020 2077 203d 2070             w = p
-0000bc30: 642e 7265 6164 5f74 6162 6c65 2866 6e2c  d.read_table(fn,
-0000bc40: 2069 6e64 6578 5f63 6f6c 3d30 290d 0a20   index_col=0).. 
-0000bc50: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000bc60: 2e69 6e64 6578 203d 2073 7472 286b 2920  .index = str(k) 
-0000bc70: 2b20 222e 2220 2b20 772e 696e 6465 782e  + "." + w.index.
-0000bc80: 6173 7479 7065 2873 7472 290d 0a20 2020  astype(str)..   
-0000bc90: 2020 2020 2020 2020 2020 2020 206d 6574               met
-0000bca0: 615f 772e 6170 7065 6e64 2877 290d 0a20  a_w.append(w).. 
-0000bcb0: 2020 2020 2020 2020 2020 206d 6574 615f             meta_
-0000bcc0: 7720 3d20 7064 2e63 6f6e 6361 7428 6d65  w = pd.concat(me
-0000bcd0: 7461 5f77 2c20 6178 6973 3d30 292e 542e  ta_w, axis=0).T.
-0000bce0: 7265 696e 6465 7828 7365 6c66 2e61 6461  reindex(self.ada
-0000bcf0: 7461 2e76 6172 2e69 6e64 6578 292e 7265  ta.var.index).re
-0000bd00: 6e61 6d65 5f61 7869 7328 5b22 6b2e 6765  name_axis(["k.ge
-0000bd10: 7022 5d2c 2061 7869 733d 3129 0d0a 2020  p"], axis=1)..  
-0000bd20: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000bd30: 6461 7461 2e76 6172 6d5b 7265 7375 6c74  data.varm[result
-0000bd40: 5f74 7970 655d 203d 206d 6574 615f 770d  _type] = meta_w.
-0000bd50: 0a0d 0a20 2020 2020 2020 2023 2049 6d70  ...        # Imp
-0000bd60: 6f72 7420 5573 6167 6573 0d0a 2020 2020  ort Usages..    
-0000bd70: 2020 2020 6c6f 6767 696e 672e 696e 666f      logging.info
-0000bd80: 2866 2249 6d70 6f72 7469 6e67 2055 7361  (f"Importing Usa
-0000bd90: 6765 7322 2920 200d 0a20 2020 2020 2020  ges")  ..       
-0000bda0: 2075 7361 6765 203d 205b 5d0d 0a20 2020   usage = []..   
-0000bdb0: 2020 2020 2066 6f72 2066 6e20 696e 2067       for fn in g
-0000bdc0: 6c6f 6228 6f73 2e70 6174 682e 6a6f 696e  lob(os.path.join
-0000bdd0: 2863 6e6d 665f 6f75 7470 7574 5f64 6972  (cnmf_output_dir
-0000bde0: 2c20 636e 6d66 5f6e 616d 652c 2066 227b  , cnmf_name, f"{
-0000bdf0: 636e 6d66 5f6e 616d 657d 2a2e 7573 6167  cnmf_name}*.usag
-0000be00: 6573 2e6b 5f2a 2e7b 6c64 745f 7374 727d  es.k_*.{ldt_str}
-0000be10: 2e2a 7478 7422 2929 3a0d 0a20 2020 2020  .*txt")):..     
-0000be20: 2020 2020 2020 206b 203d 2069 6e74 286f         k = int(o
-0000be30: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-0000be40: 666e 292e 7265 6d6f 7665 7072 6566 6978  fn).removeprefix
-0000be50: 2866 227b 636e 6d66 5f6e 616d 657d 2e75  (f"{cnmf_name}.u
-0000be60: 7361 6765 732e 2229 2e73 706c 6974 2822  sages.").split("
-0000be70: 2e22 295b 305d 2e72 6570 6c61 6365 2822  .")[0].replace("
-0000be80: 6b5f 222c 2022 2229 290d 0a20 2020 2020  k_", ""))..     
-0000be90: 2020 2020 2020 2068 203d 2070 642e 7265         h = pd.re
-0000bea0: 6164 5f74 6162 6c65 2866 6e2c 2069 6e64  ad_table(fn, ind
-0000beb0: 6578 5f63 6f6c 3d30 290d 0a20 2020 2020  ex_col=0)..     
-0000bec0: 2020 2020 2020 2068 2e63 6f6c 756d 6e73         h.columns
-0000bed0: 203d 2073 7472 286b 2920 2b20 222e 2220   = str(k) + "." 
-0000bee0: 2b20 682e 636f 6c75 6d6e 732e 6173 7479  + h.columns.asty
-0000bef0: 7065 2873 7472 290d 0a20 2020 2020 2020  pe(str)..       
-0000bf00: 2020 2020 2075 7361 6765 2e61 7070 656e       usage.appen
-0000bf10: 6428 6829 0d0a 2020 2020 2020 2020 7365  d(h)..        se
-0000bf20: 6c66 2e61 6461 7461 2e6f 6273 6d5b 2263  lf.adata.obsm["c
-0000bf30: 6e6d 665f 7573 6167 6522 5d20 3d20 7064  nmf_usage"] = pd
-0000bf40: 2e63 6f6e 6361 7428 7573 6167 652c 2061  .concat(usage, a
-0000bf50: 7869 733d 3129 2e73 6f72 745f 696e 6465  xis=1).sort_inde
-0000bf60: 7828 6178 6973 3d31 292e 7265 6e61 6d65  x(axis=1).rename
-0000bf70: 5f61 7869 7328 5b22 6b2e 6765 7022 5d2c  _axis(["k.gep"],
-0000bf80: 2061 7869 733d 3129 0d0a 2020 2020 2020   axis=1)..      
-0000bf90: 2020 0d0a 2020 2020 2020 2020 2320 496d    ..        # Im
-0000bfa0: 706f 7274 2067 656e 6520 6c69 7374 2075  port gene list u
-0000bfb0: 7365 6420 666f 7220 6661 6374 6f72 697a  sed for factoriz
-0000bfc0: 6174 696f 6e0d 0a20 2020 2020 2020 2077  ation..        w
-0000bfd0: 6974 6820 6f70 656e 286f 732e 7061 7468  ith open(os.path
-0000bfe0: 2e6a 6f69 6e28 636e 6d66 5f6f 7574 7075  .join(cnmf_outpu
-0000bff0: 745f 6469 722c 2063 6e6d 665f 6e61 6d65  t_dir, cnmf_name
-0000c000: 2c20 6622 7b63 6e6d 665f 6e61 6d65 7d2e  , f"{cnmf_name}.
-0000c010: 6f76 6572 6469 7370 6572 7365 645f 6765  overdispersed_ge
-0000c020: 6e65 732e 7478 7422 2929 2061 7320 663a  nes.txt")) as f:
-0000c030: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000c040: 6c66 2e61 6461 7461 2e75 6e73 5b22 6765  lf.adata.uns["ge
-0000c050: 6e65 5f6c 6973 7422 5d20 3d20 5b6c 696e  ne_list"] = [lin
-0000c060: 652e 7374 7269 7028 2920 666f 7220 6c69  e.strip() for li
-0000c070: 6e65 2069 6e20 662e 7265 6164 6c69 6e65  ne in f.readline
-0000c080: 7328 295d 0d0a 0d0a 2020 2020 2020 2020  s()]....        
-0000c090: 2320 496d 706f 7274 204b 2d73 656c 6563  # Import K-selec
-0000c0a0: 7469 6f6e 2073 7461 7473 0d0a 2020 2020  tion stats..    
-0000c0b0: 2020 2020 6b76 616c 7320 3d20 7064 2e44      kvals = pd.D
-0000c0c0: 6174 6146 7261 6d65 282a 2a6e 702e 6c6f  ataFrame(**np.lo
-0000c0d0: 6164 286f 732e 7061 7468 2e6a 6f69 6e28  ad(os.path.join(
-0000c0e0: 636e 6d66 5f6f 7574 7075 745f 6469 722c  cnmf_output_dir,
-0000c0f0: 2063 6e6d 665f 6e61 6d65 2c20 6622 7b63   cnmf_name, f"{c
-0000c100: 6e6d 665f 6e61 6d65 7d2e 6b5f 7365 6c65  nmf_name}.k_sele
-0000c110: 6374 696f 6e5f 7374 6174 732e 6466 2e6e  ction_stats.df.n
-0000c120: 707a 2229 2c20 616c 6c6f 775f 7069 636b  pz"), allow_pick
-0000c130: 6c65 3d54 7275 6529 292e 7365 745f 696e  le=True)).set_in
-0000c140: 6465 7828 226b 2229 5b5b 2273 7461 6269  dex("k")[["stabi
-0000c150: 6c69 7479 222c 2022 7072 6564 6963 7469  lity", "predicti
-0000c160: 6f6e 5f65 7272 6f72 225d 5d0d 0a20 2020  on_error"]]..   
-0000c170: 2020 2020 206b 7661 6c73 2e69 6e64 6578       kvals.index
-0000c180: 203d 206b 7661 6c73 2e69 6e64 6578 2e61   = kvals.index.a
-0000c190: 7374 7970 6528 696e 7429 0d0a 2020 2020  stype(int)..    
-0000c1a0: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
-0000c1b0: 6e73 5b22 6b76 616c 7322 5d20 3d20 6b76  ns["kvals"] = kv
-0000c1c0: 616c 730d 0a20 2020 2020 2020 2073 656c  als..        sel
-0000c1d0: 662e 6170 7065 6e64 5f74 6f5f 6869 7374  f.append_to_hist
-0000c1e0: 6f72 7928 2263 4e4d 4620 7265 7375 6c74  ory("cNMF result
-0000c1f0: 7320 6164 6465 6420 6672 6f6d 206f 7574  s added from out
-0000c200: 7075 7420 6469 7265 6374 6f72 7920 7b63  put directory {c
-0000c210: 6e6d 665f 6f75 7470 7574 5f64 6972 7d2f  nmf_output_dir}/
-0000c220: 7b63 6e6d 665f 6e61 6d65 7d22 290d 0a0d  {cnmf_name}")...
-0000c230: 0a20 2020 2064 6566 2072 656d 6f76 655f  .    def remove_
-0000c240: 636e 6d66 5f72 6573 756c 7473 2873 656c  cnmf_results(sel
-0000c250: 6629 3a0d 0a20 2020 2020 2020 2066 6f72  f):..        for
-0000c260: 2072 6573 756c 745f 7479 7065 2069 6e20   result_type in 
-0000c270: 2822 636e 6d66 5f67 6570 5f73 636f 7265  ("cnmf_gep_score
-0000c280: 222c 2022 636e 6d66 5f67 6570 5f74 706d  ", "cnmf_gep_tpm
-0000c290: 222c 2022 636e 6d66 5f67 6570 5f72 6177  ", "cnmf_gep_raw
-0000c2a0: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-0000c2b0: 2073 656c 662e 6164 6174 612e 7661 726d   self.adata.varm
-0000c2c0: 2e70 6f70 2872 6573 756c 745f 7479 7065  .pop(result_type
-0000c2d0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000c2e0: 6164 6174 612e 6f62 736d 2e70 6f70 2822  adata.obsm.pop("
-0000c2f0: 636e 6d66 5f75 7361 6765 2229 0d0a 2020  cnmf_usage")..  
-0000c300: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
-0000c310: 2e75 6e73 2e70 6f70 2822 6765 6e65 5f6c  .uns.pop("gene_l
-0000c320: 6973 7422 290d 0a20 2020 2020 2020 2073  ist")..        s
-0000c330: 656c 662e 6164 6174 612e 756e 732e 706f  elf.adata.uns.po
-0000c340: 7028 226b 7661 6c73 2229 0d0a 2020 2020  p("kvals")..    
-0000c350: 2020 2020 7365 6c66 2e61 7070 656e 645f      self.append_
-0000c360: 746f 5f68 6973 746f 7279 2822 634e 4d46  to_history("cNMF
-0000c370: 2072 6573 756c 7473 2072 656d 6f76 6564   results removed
-0000c380: 2e22 290d 0a0d 0a0d 0a20 2020 2064 6566  .")......    def
-0000c390: 2067 6574 5f75 7361 6765 7328 7365 6c66   get_usages(self
-0000c3a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000c3b0: 2020 2020 2020 6b3a 2055 6e69 6f6e 5b69        k: Union[i
-0000c3c0: 6e74 2c20 4974 6572 6162 6c65 5d20 3d20  nt, Iterable] = 
-0000c3d0: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
-0000c3e0: 2020 2020 2020 2020 2020 6469 7363 7265            discre
-0000c3f0: 7469 7a65 3a20 626f 6f6c 203d 2046 616c  tize: bool = Fal
-0000c400: 7365 2c0d 0a20 2020 2020 2020 2020 2020  se,..           
-0000c410: 2020 2020 2020 2020 6e6f 726d 616c 697a          normaliz
-0000c420: 653a 2062 6f6f 6c20 3d20 4661 6c73 650d  e: bool = False.
-0000c430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c440: 2020 2020 2920 2d3e 2070 642e 4461 7461      ) -> pd.Data
-0000c450: 4672 616d 653a 0d0a 2020 2020 2020 2020  Frame:..        
-0000c460: 2222 220d 0a20 2020 2020 2020 2043 616c  """..        Cal
-0000c470: 6375 6c61 7465 2075 7361 6765 206f 6620  culate usage of 
-0000c480: 6561 6368 2047 4550 2069 6e20 6561 6368  each GEP in each
-0000c490: 2073 616d 706c 652f 6f62 7365 7276 6174   sample/observat
-0000c4a0: 696f 6e2e 0d0a 0d0a 2020 2020 2020 2020  ion.....        
-0000c4b0: 3a70 6172 616d 206b 3a20 4966 2061 6e20  :param k: If an 
-0000c4c0: 696e 7465 6765 7220 6f72 206c 6973 7420  integer or list 
-0000c4d0: 6f66 2069 6e74 6567 6572 732c 2072 6574  of integers, ret
-0000c4e0: 7572 6e73 2075 7361 6765 7320 6f6e 6c79  urns usages only
-0000c4f0: 2066 6f72 2073 7065 6369 6669 6564 2072   for specified r
-0000c500: 616e 6b73 2e20 4f74 6865 7277 6973 652c  anks. Otherwise,
-0000c510: 2072 6574 7572 6e73 2075 7361 6765 206f   returns usage o
-0000c520: 6620 616c 6c20 4745 5073 2061 6372 6f73  f all GEPs acros
-0000c530: 7320 7261 6e6b 732e 2044 6566 6175 6c74  s ranks. Default
-0000c540: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
-0000c550: 2020 203a 7479 7065 206b 3a20 696e 742c     :type k: int,
-0000c560: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-0000c570: 2020 203a 7061 7261 6d20 6469 7363 7265     :param discre
-0000c580: 7469 7a65 3a20 4469 7363 7265 7469 7a65  tize: Discretize
-0000c590: 7320 7468 6520 7573 6167 6520 6d61 7472  s the usage matr
-0000c5a0: 6978 2073 7563 6820 7468 6174 2066 6f72  ix such that for
-0000c5b0: 2065 6163 6820 7661 6c75 6520 6f66 206b   each value of k
-0000c5c0: 2c20 6561 6368 2073 616d 706c 6520 6861  , each sample ha
-0000c5d0: 7320 7573 6167 6520 6f66 206f 6e6c 7920  s usage of only 
-0000c5e0: 3120 4745 5020 2874 6865 206f 6e65 2077  1 GEP (the one w
-0000c5f0: 6974 6820 7468 6520 6d61 7869 6d75 6d20  ith the maximum 
-0000c600: 7573 6167 6529 2e20 4465 6661 756c 7473  usage). Defaults
-0000c610: 2074 6f20 4661 6c73 650d 0a20 2020 2020   to False..     
-0000c620: 2020 203a 7479 7065 2064 6973 6372 6574     :type discret
-0000c630: 697a 653a 2062 6f6f 6c2c 206f 7074 696f  ize: bool, optio
-0000c640: 6e61 6c0d 0a20 2020 2020 2020 203a 7061  nal..        :pa
-0000c650: 7261 6d20 6e6f 726d 616c 697a 653a 204e  ram normalize: N
-0000c660: 6f72 6d61 6c69 7a65 2074 6865 2047 4550  ormalize the GEP
-0000c670: 2075 7361 6765 206d 6174 7269 7820 7375   usage matrix su
-0000c680: 6368 2074 6861 7420 666f 7220 6561 6368  ch that for each
-0000c690: 2076 616c 7565 206f 6620 6b2c 2075 7361   value of k, usa
-0000c6a0: 6765 206f 6620 616c 6c20 4745 5073 2073  ge of all GEPs s
-0000c6b0: 756d 7320 746f 2031 2e20 4465 6661 756c  ums to 1. Defaul
-0000c6c0: 7473 2074 6f20 4661 6c73 650d 0a20 2020  ts to False..   
-0000c6d0: 2020 2020 203a 7479 7065 206e 6f72 6d61       :type norma
-0000c6e0: 6c69 7a65 3a20 626f 6f6c 2c20 6f70 7469  lize: bool, opti
-0000c6f0: 6f6e 616c 0d0a 2020 2020 2020 2020 3a72  onal..        :r
-0000c700: 6574 7572 6e3a 206f 6273 6572 7661 7469  eturn: observati
-0000c710: 6f6e 20c3 9720 4745 5020 6d61 7472 6978  on .. GEP matrix
-0000c720: 0d0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-0000c730: 3a20 7064 2e44 6174 6146 7261 6d65 0d0a  : pd.DataFrame..
-0000c740: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-0000c750: 2020 2020 2064 6620 3d20 7365 6c66 2e61       df = self.a
-0000c760: 6461 7461 2e6f 6273 6d5b 2263 6e6d 665f  data.obsm["cnmf_
-0000c770: 7573 6167 6522 5d2e 636f 7079 2829 0d0a  usage"].copy()..
-0000c780: 2020 2020 2020 2020 6466 2e63 6f6c 756d          df.colum
-0000c790: 6e73 203d 2070 642e 4d75 6c74 6949 6e64  ns = pd.MultiInd
-0000c7a0: 6578 2e66 726f 6d5f 7475 706c 6573 2864  ex.from_tuples(d
-0000c7b0: 662e 636f 6c75 6d6e 732e 7374 722e 7370  f.columns.str.sp
-0000c7c0: 6c69 7428 222e 2229 2e74 6f5f 6c69 7374  lit(".").to_list
-0000c7d0: 2829 290d 0a20 2020 2020 2020 2064 662e  ())..        df.
-0000c7e0: 636f 6c75 6d6e 7320 3d20 6466 2e63 6f6c  columns = df.col
-0000c7f0: 756d 6e73 2e73 6574 5f6c 6576 656c 7328  umns.set_levels(
-0000c800: 5b6c 2e61 7374 7970 6528 2269 6e74 2229  [l.astype("int")
-0000c810: 2066 6f72 206c 2069 6e20 6466 2e63 6f6c   for l in df.col
-0000c820: 756d 6e73 2e6c 6576 656c 735d 290d 0a20  umns.levels]).. 
-0000c830: 2020 2020 2020 2069 6620 6e6f 726d 616c         if normal
-0000c840: 697a 653a 0d0a 2020 2020 2020 2020 2020  ize:..          
-0000c850: 2020 6e6f 726d 616c 697a 6564 203d 205b    normalized = [
-0000c860: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
-0000c870: 6f72 205f 2c20 7375 6264 6620 696e 2064  or _, subdf in d
-0000c880: 662e 542e 6772 6f75 7062 7928 6c65 7665  f.T.groupby(leve
-0000c890: 6c3d 3029 3a0d 0a20 2020 2020 2020 2020  l=0):..         
-0000c8a0: 2020 2020 2020 206e 6f72 6d61 6c69 7a65         normalize
-0000c8b0: 642e 6170 7065 6e64 2873 7562 6466 2e64  d.append(subdf.d
-0000c8c0: 6976 2873 7562 6466 2e73 756d 2829 2929  iv(subdf.sum()))
-0000c8d0: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
-0000c8e0: 203d 2070 642e 636f 6e63 6174 286e 6f72   = pd.concat(nor
-0000c8f0: 6d61 6c69 7a65 6429 2e54 0d0a 2020 2020  malized).T..    
-0000c900: 2020 2020 6966 2064 6973 6372 6574 697a      if discretiz
-0000c910: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000c920: 6469 7363 7265 7469 7a65 6420 3d20 5b5d  discretized = []
-0000c930: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-0000c940: 7220 5f2c 2073 7562 6466 2069 6e20 6466  r _, subdf in df
-0000c950: 2e54 2e67 726f 7570 6279 286c 6576 656c  .T.groupby(level
-0000c960: 3d30 293a 0d0a 2020 2020 2020 2020 2020  =0):..          
-0000c970: 2020 2020 2020 6469 7363 7265 7469 7a65        discretize
-0000c980: 642e 6170 7065 6e64 2873 7562 6466 2e65  d.append(subdf.e
-0000c990: 7128 7375 6264 662e 6d61 7828 2929 2e61  q(subdf.max()).a
-0000c9a0: 7374 7970 6528 696e 7429 290d 0a20 2020  stype(int))..   
-0000c9b0: 2020 2020 2020 2020 2064 6620 3d20 7064           df = pd
-0000c9c0: 2e63 6f6e 6361 7428 6469 7363 7265 7469  .concat(discreti
-0000c9d0: 7a65 6429 2e54 2020 2020 2020 2020 0d0a  zed).T        ..
-0000c9e0: 2020 2020 2020 2020 6966 206b 2069 7320          if k is 
-0000c9f0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-0000ca00: 2020 2020 2020 2064 6620 3d20 6466 2e6c         df = df.l
-0000ca10: 6f63 5b3a 2c20 6b5d 0d0a 2020 2020 2020  oc[:, k]..      
-0000ca20: 2020 6466 203d 2064 662e 736f 7274 5f69    df = df.sort_i
-0000ca30: 6e64 6578 2861 7869 733d 3129 2020 200d  ndex(axis=1)   .
-0000ca40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000ca50: 6466 0d0a 0d0a 2020 2020 6465 6620 6765  df....    def ge
-0000ca60: 745f 7072 6f67 7261 6d73 2873 656c 662c  t_programs(self,
-0000ca70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ca80: 2020 206b 3a20 556e 696f 6e5b 696e 742c     k: Union[int,
-0000ca90: 2049 7465 7261 626c 655d 203d 204e 6f6e   Iterable] = Non
-0000caa0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0000cab0: 2020 2020 2074 7970 653d 2263 6e6d 665f       type="cnmf_
-0000cac0: 6765 705f 7363 6f72 6522 0d0a 2020 2020  gep_score"..    
-0000cad0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-0000cae0: 3e20 7064 2e44 6174 6146 7261 6d65 3a0d  > pd.DataFrame:.
-0000caf0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000cb00: 2020 2020 2020 4765 7420 6665 6174 7572        Get featur
-0000cb10: 6520 7363 6f72 6573 2066 6f72 2070 726f  e scores for pro
-0000cb20: 6772 616d 732e 0d0a 0d0a 2020 2020 2020  grams.....      
-0000cb30: 2020 3a70 6172 616d 206b 3a20 4966 2061    :param k: If a
-0000cb40: 6e20 696e 7465 6765 7220 6f72 206c 6973  n integer or lis
-0000cb50: 7420 6f66 2069 6e74 6567 6572 732c 2072  t of integers, r
-0000cb60: 6574 7572 6e73 2047 4550 7320 6f6e 6c79  eturns GEPs only
-0000cb70: 2066 6f72 2073 7065 6369 6669 6564 2072   for specified r
-0000cb80: 616e 6b73 2e20 4f74 6865 7277 6973 652c  anks. Otherwise,
-0000cb90: 2072 6574 7572 6e73 2047 4550 7320 6672   returns GEPs fr
-0000cba0: 6f6d 2061 6c6c 2072 616e 6b73 2e20 4465  om all ranks. De
-0000cbb0: 6661 756c 7473 2074 6f20 4e6f 6e65 0d0a  faults to None..
-0000cbc0: 2020 2020 2020 2020 3a74 7970 6520 6b3a          :type k:
-0000cbd0: 2055 6e69 6f6e 5b69 6e74 2c20 4974 6572   Union[int, Iter
-0000cbe0: 6162 6c65 5d2c 206f 7074 696f 6e61 6c0d  able], optional.
-0000cbf0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000cc00: 7479 7065 3a20 2263 6e6d 665f 6765 705f  type: "cnmf_gep_
-0000cc10: 7363 6f72 6522 206f 7220 2263 6e6d 665f  score" or "cnmf_
-0000cc20: 6765 705f 7470 6d22 2c20 6465 6661 756c  gep_tpm", defaul
-0000cc30: 7473 2074 6f20 2263 6e6d 665f 6765 705f  ts to "cnmf_gep_
-0000cc40: 7363 6f72 6522 0d0a 2020 2020 2020 2020  score"..        
-0000cc50: 3a74 7970 6520 7479 7065 3a20 7374 722c  :type type: str,
-0000cc60: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-0000cc70: 2020 203a 7265 7475 726e 3a20 6665 6174     :return: feat
-0000cc80: 7572 6573 20c3 9720 4745 5020 6d61 7472  ures .. GEP matr
-0000cc90: 6978 0d0a 2020 2020 2020 2020 3a72 7479  ix..        :rty
-0000cca0: 7065 3a20 7064 2e44 6174 6146 7261 6d65  pe: pd.DataFrame
-0000ccb0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000ccc0: 2020 2020 2020 2064 6620 3d20 7365 6c66         df = self
-0000ccd0: 2e61 6461 7461 2e76 6172 6d5b 7479 7065  .adata.varm[type
-0000cce0: 5d2e 636f 7079 2829 0d0a 2020 2020 2020  ].copy()..      
-0000ccf0: 2020 6466 2e63 6f6c 756d 6e73 203d 2070    df.columns = p
-0000cd00: 642e 4d75 6c74 6949 6e64 6578 2e66 726f  d.MultiIndex.fro
-0000cd10: 6d5f 7475 706c 6573 2864 662e 636f 6c75  m_tuples(df.colu
-0000cd20: 6d6e 732e 7374 722e 7370 6c69 7428 222e  mns.str.split(".
-0000cd30: 2229 2e74 6f5f 6c69 7374 2829 290d 0a20  ").to_list()).. 
-0000cd40: 2020 2020 2020 2064 662e 636f 6c75 6d6e         df.column
-0000cd50: 7320 3d20 6466 2e63 6f6c 756d 6e73 2e73  s = df.columns.s
-0000cd60: 6574 5f6c 6576 656c 7328 5b6c 2e61 7374  et_levels([l.ast
-0000cd70: 7970 6528 2269 6e74 2229 2066 6f72 206c  ype("int") for l
-0000cd80: 2069 6e20 6466 2e63 6f6c 756d 6e73 2e6c   in df.columns.l
-0000cd90: 6576 656c 735d 290d 0a20 2020 2020 2020  evels])..       
-0000cda0: 2069 6620 6973 696e 7374 616e 6365 286b   if isinstance(k
-0000cdb0: 2c20 696e 7429 3a0d 0a20 2020 2020 2020  , int):..       
-0000cdc0: 2020 2020 2064 6620 3d20 6466 2e6c 6f63       df = df.loc
-0000cdd0: 5b3a 2c20 6b5d 0d0a 2020 2020 2020 2020  [:, k]..        
-0000cde0: 2020 2020 6466 203d 2064 662e 7265 6e61      df = df.rena
-0000cdf0: 6d65 5f61 7869 7328 636f 6c75 6d6e 733d  me_axis(columns=
-0000ce00: 5b22 7072 6f67 7261 6d22 5d29 2e73 6f72  ["program"]).sor
-0000ce10: 745f 696e 6465 7828 6178 6973 3d31 290d  t_index(axis=1).
-0000ce20: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-0000ce30: 696e 7374 616e 6365 286b 2c20 4974 6572  instance(k, Iter
-0000ce40: 6162 6c65 293a 0d0a 2020 2020 2020 2020  able):..        
-0000ce50: 2020 2020 6466 203d 2064 662e 6c6f 635b      df = df.loc[
-0000ce60: 3a2c 206b 5d0d 0a20 2020 2020 2020 2020  :, k]..         
-0000ce70: 2020 2064 6620 3d20 6466 2e72 656e 616d     df = df.renam
-0000ce80: 655f 6178 6973 2863 6f6c 756d 6e73 3d5b  e_axis(columns=[
-0000ce90: 226b 222c 2022 7072 6f67 7261 6d22 5d29  "k", "program"])
-0000cea0: 2e73 6f72 745f 696e 6465 7828 6178 6973  .sort_index(axis
-0000ceb0: 3d31 290d 0a20 2020 2020 2020 2072 6574  =1)..        ret
-0000cec0: 7572 6e20 6466 0d0a 2020 2020 0d0a 2020  urn df..    ..  
-0000ced0: 2020 6465 6620 6765 745f 6d65 7461 6461    def get_metada
-0000cee0: 7461 5f64 6628 7365 6c66 2c0d 0a20 2020  ta_df(self,..   
-0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf00: 2020 2020 2069 6e63 6c75 6465 5f63 6174       include_cat
-0000cf10: 6567 6f72 6963 616c 3a20 626f 6f6c 203d  egorical: bool =
-0000cf20: 2054 7275 652c 0d0a 2020 2020 2020 2020   True,..        
-0000cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf40: 696e 636c 7564 655f 6e75 6d65 7269 6361  include_numerica
-0000cf50: 6c3a 2062 6f6f 6c20 3d20 5472 7565 0d0a  l: bool = True..
+0000ae10: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0000ae20: 2323 2053 6176 6520 6120 5c6e 2d64 656c  ## Save a \n-del
+0000ae30: 696d 6974 6564 206c 6973 7420 6f66 2074  imited list of t
+0000ae40: 6865 2068 6967 682d 7661 7269 616e 6365  he high-variance
+0000ae50: 2067 656e 6573 2075 7365 6420 666f 7220   genes used for 
+0000ae60: 6661 6374 6f72 697a 6174 696f 6e0d 0a20  factorization.. 
+0000ae70: 2020 2020 2020 206f 7065 6e28 636e 6d66         open(cnmf
+0000ae80: 5f6f 626a 2e70 6174 6873 5b27 6e6d 665f  _obj.paths['nmf_
+0000ae90: 6765 6e65 735f 6c69 7374 275d 2c20 2777  genes_list'], 'w
+0000aea0: 2729 2e77 7269 7465 2827 5c6e 272e 6a6f  ').write('\n'.jo
+0000aeb0: 696e 286f 7665 7264 6973 7065 7273 6564  in(overdispersed
+0000aec0: 5f67 656e 6573 2929 0d0a 0d0a 2020 2020  _genes))....    
+0000aed0: 2020 2020 6966 206e 6f72 6d5f 636f 756e      if norm_coun
+0000aee0: 7473 2e58 2e64 7479 7065 2021 3d20 6e70  ts.X.dtype != np
+0000aef0: 2e66 6c6f 6174 3634 3a0d 0a20 2020 2020  .float64:..     
+0000af00: 2020 2020 2020 206e 6f72 6d5f 636f 756e         norm_coun
+0000af10: 7473 2e58 203d 206e 6f72 6d5f 636f 756e  ts.X = norm_coun
+0000af20: 7473 2e58 2e61 7374 7970 6528 6e70 2e66  ts.X.astype(np.f
+0000af30: 6c6f 6174 3634 290d 0a0d 0a20 2020 2020  loat64)....     
+0000af40: 2020 206e 6f72 6d5f 636f 756e 7473 2e77     norm_counts.w
+0000af50: 7269 7465 5f68 3561 6428 636e 6d66 5f6f  rite_h5ad(cnmf_o
+0000af60: 626a 2e70 6174 6873 5b27 6e6f 726d 616c  bj.paths['normal
+0000af70: 697a 6564 5f63 6f75 6e74 7327 5d29 0d0a  ized_counts'])..
+0000af80: 0d0a 2020 2020 2020 2020 2320 7361 7665  ..        # save
+0000af90: 2070 6172 616d 6574 6572 7320 666f 7220   parameters for 
+0000afa0: 6661 6374 6f72 697a 6174 696f 6e20 7374  factorization st
+0000afb0: 6570 0d0a 2020 2020 2020 2020 636e 6d66  ep..        cnmf
+0000afc0: 5f6f 626a 2e73 6176 655f 6e6d 665f 6974  _obj.save_nmf_it
+0000afd0: 6572 5f70 6172 616d 7328 2a63 6e6d 665f  er_params(*cnmf_
+0000afe0: 6f62 6a2e 6765 745f 6e6d 665f 6974 6572  obj.get_nmf_iter
+0000aff0: 5f70 6172 616d 7328 6b73 3d6b 7661 6c73  _params(ks=kvals
+0000b000: 2c20 6e5f 6974 6572 3d6e 5f69 7465 722c  , n_iter=n_iter,
+0000b010: 2072 616e 646f 6d5f 7374 6174 655f 7365   random_state_se
+0000b020: 6564 3d73 6565 642c 2062 6574 615f 6c6f  ed=seed, beta_lo
+0000b030: 7373 3d62 6574 615f 6c6f 7373 2929 0d0a  ss=beta_loss))..
+0000b040: 0d0a 2020 2020 2020 2020 2320 7361 7665  ..        # save
+0000b050: 2070 6172 616d 6574 6572 7320 696e 2041   parameters in A
+0000b060: 6e6e 4461 7461 206f 626a 6563 740d 0a20  nnData object.. 
+0000b070: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+0000b080: 612e 756e 735b 2263 6e6d 6622 5d20 3d20  a.uns["cnmf"] = 
+0000b090: 636e 6d66 5f6f 626a 2e67 6574 5f6e 6d66  cnmf_obj.get_nmf
+0000b0a0: 5f69 7465 725f 7061 7261 6d73 286b 733d  _iter_params(ks=
+0000b0b0: 6b76 616c 732c 206e 5f69 7465 723d 6e5f  kvals, n_iter=n_
+0000b0c0: 6974 6572 2c20 7261 6e64 6f6d 5f73 7461  iter, random_sta
+0000b0d0: 7465 5f73 6565 643d 7365 6564 2c20 6265  te_seed=seed, be
+0000b0e0: 7461 5f6c 6f73 733d 6265 7461 5f6c 6f73  ta_loss=beta_los
+0000b0f0: 7329 5b31 5d20 2023 2064 6963 7420 6f66  s)[1]  # dict of
+0000b100: 2063 6e6d 6620 7061 7261 6d65 7465 7273   cnmf parameters
+0000b110: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0000b120: 2020 2020 7365 6c66 2e61 7070 656e 645f      self.append_
+0000b130: 746f 5f68 6973 746f 7279 2866 2263 4e4d  to_history(f"cNM
+0000b140: 4620 7061 7261 6d65 7465 7273 2061 6464  F parameters add
+0000b150: 6564 2e20 634e 4d46 2069 6e70 7574 7320  ed. cNMF inputs 
+0000b160: 696e 6974 6961 6c69 7a65 6420 696e 207b  initialized in {
+0000b170: 636e 6d66 5f6f 7574 7075 745f 6469 727d  cnmf_output_dir}
+0000b180: 2f7b 636e 6d66 5f6e 616d 657d 2229 0d0a  /{cnmf_name}")..
+0000b190: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+0000b1a0: 6e6d 665f 6f62 6a0d 0a20 2020 200d 0a20  nmf_obj..    .. 
+0000b1b0: 2020 2064 6566 2061 6464 5f63 6e6d 665f     def add_cnmf_
+0000b1c0: 7265 7375 6c74 7328 7365 6c66 2c20 636e  results(self, cn
+0000b1d0: 6d66 5f6f 7574 7075 745f 6469 722c 2063  mf_output_dir, c
+0000b1e0: 6e6d 665f 6e61 6d65 2c20 6c6f 6361 6c5f  nmf_name, local_
+0000b1f0: 6465 6e73 6974 795f 7468 7265 7368 6f6c  density_threshol
+0000b200: 643a 2066 6c6f 6174 203d 204e 6f6e 652c  d: float = None,
+0000b210: 206c 6f63 616c 5f6e 6569 6768 626f 7268   local_neighborh
+0000b220: 6f6f 645f 7369 7a65 3a20 666c 6f61 7420  ood_size: float 
+0000b230: 3d20 4e6f 6e65 293a 0d0a 2020 2020 2020  = None):..      
+0000b240: 2020 2222 220d 0a20 2020 2020 2020 2041    """..        A
+0000b250: 6674 6572 2066 6163 746f 7269 7a61 7469  fter factorizati
+0000b260: 6f6e 2c20 6164 6420 636f 6d70 6c65 7465  on, add complete
+0000b270: 6420 634e 4d46 2072 6573 756c 7473 2069  d cNMF results i
+0000b280: 6e20 5b63 6e6d 665f 6f75 7470 7574 5f64  n [cnmf_output_d
+0000b290: 6972 5d2f 5b63 6e6d 665f 6e61 6d65 5d20  ir]/[cnmf_name] 
+0000b2a0: 746f 2074 6865 2064 6174 6173 6574 206f  to the dataset o
+0000b2b0: 626a 6563 742e 0d0a 0d0a 2020 2020 2020  bject.....      
+0000b2c0: 2020 3a70 6172 616d 2063 6e6d 665f 6f75    :param cnmf_ou
+0000b2d0: 7470 7574 5f64 6972 3a20 4f75 7470 7574  tput_dir: Output
+0000b2e0: 2064 6972 6563 746f 7279 2066 6f72 2063   directory for c
+0000b2f0: 4e4d 4620 7265 7375 6c74 730d 0a20 2020  NMF results..   
+0000b300: 2020 2020 203a 7479 7065 2063 6e6d 665f       :type cnmf_
+0000b310: 6f75 7470 7574 5f64 6972 3a20 7374 720d  output_dir: str.
+0000b320: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000b330: 636e 6d66 5f6e 616d 653a 204e 616d 6520  cnmf_name: Name 
+0000b340: 6f66 2074 6865 2063 4e4d 4620 7265 7375  of the cNMF resu
+0000b350: 6c74 732e 2046 696c 6573 2077 696c 6c20  lts. Files will 
+0000b360: 6265 206f 7574 7075 7420 746f 205b 636e  be output to [cn
+0000b370: 6d66 5f6f 7574 7075 745f 6469 725d 2f5b  mf_output_dir]/[
+0000b380: 636e 6d66 5f6e 616d 655d 2f0d 0a20 2020  cnmf_name]/..   
+0000b390: 2020 2020 203a 7479 7065 2063 6e6d 665f       :type cnmf_
+0000b3a0: 6e61 6d65 3a20 7374 720d 0a20 2020 2020  name: str..     
+0000b3b0: 2020 203a 7061 7261 6d20 6c6f 6361 6c5f     :param local_
+0000b3c0: 6465 6e73 6974 795f 7468 7265 7368 6f6c  density_threshol
+0000b3d0: 643a 2054 6872 6573 686f 6c64 2066 6f72  d: Threshold for
+0000b3e0: 2074 6865 206c 6f63 616c 2064 656e 7369   the local densi
+0000b3f0: 7479 2066 696c 7465 7269 6e67 2070 7269  ty filtering pri
+0000b400: 6f72 2074 6f20 4745 5020 636f 6e73 656e  or to GEP consen
+0000b410: 7375 732e 2041 6363 6570 7461 626c 6520  sus. Acceptable 
+0000b420: 7468 7265 7368 6f6c 6473 2061 7265 203e  thresholds are >
+0000b430: 2030 2061 6e64 203c 3d20 3220 2832 2e30   0 and <= 2 (2.0
+0000b440: 2069 7320 6e6f 2066 696c 7465 7269 6e67   is no filtering
+0000b450: 292e 2044 6566 6175 6c74 7320 746f 204e  ). Defaults to N
+0000b460: 6f6e 652e 0d0a 2020 2020 2020 2020 3a74  one...        :t
+0000b470: 7970 6520 6c6f 6361 6c5f 6465 6e73 6974  ype local_densit
+0000b480: 795f 7468 7265 7368 6f6c 643a 2066 6c6f  y_threshold: flo
+0000b490: 6174 2c20 6f70 7469 6f6e 616c 0d0a 2020  at, optional..  
+0000b4a0: 2020 2020 2020 3a70 6172 616d 206c 6f63        :param loc
+0000b4b0: 616c 5f6e 6569 6768 626f 7268 6f6f 645f  al_neighborhood_
+0000b4c0: 7369 7a65 3a20 4672 6163 7469 6f6e 206f  size: Fraction o
+0000b4d0: 6620 7468 6520 6e75 6d62 6572 206f 6620  f the number of 
+0000b4e0: 7265 706c 6963 6174 6573 2074 6f20 7573  replicates to us
+0000b4f0: 6520 6173 206e 6561 7265 7374 206e 6569  e as nearest nei
+0000b500: 6768 626f 7273 2066 6f72 206c 6f63 616c  ghbors for local
+0000b510: 2064 656e 7369 7479 2066 696c 7465 7269   density filteri
+0000b520: 6e67 2e20 4465 6661 756c 7473 2074 6f20  ng. Defaults to 
+0000b530: 4e6f 6e65 0d0a 2020 2020 2020 2020 3a74  None..        :t
+0000b540: 7970 6520 6c6f 6361 6c5f 6e65 6967 6862  ype local_neighb
+0000b550: 6f72 686f 6f64 5f73 697a 653a 2066 6c6f  orhood_size: flo
+0000b560: 6174 2c20 6f70 7469 6f6e 616c 0d0a 2020  at, optional..  
+0000b570: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+0000b580: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
+0000b590: 735b 2263 6e6d 665f 6e61 6d65 225d 203d  s["cnmf_name"] =
+0000b5a0: 2063 6e6d 665f 6e61 6d65 0d0a 0d0a 2020   cnmf_name....  
+0000b5b0: 2020 2020 2020 2320 696e 6665 7220 6672        # infer fr
+0000b5c0: 6f6d 2066 696c 656e 616d 6573 2077 6869  om filenames whi
+0000b5d0: 6368 206c 6f63 616c 2064 656e 7369 7479  ch local density
+0000b5e0: 2074 6872 6573 686f 6c64 2077 6173 2075   threshold was u
+0000b5f0: 7365 640d 0a20 2020 2020 2020 2073 656e  sed..        sen
+0000b600: 7365 645f 6c64 7473 203d 2073 6574 2829  sed_ldts = set()
+0000b610: 0d0a 2020 2020 2020 2020 666f 7220 666e  ..        for fn
+0000b620: 2069 6e20 676c 6f62 286f 732e 7061 7468   in glob(os.path
+0000b630: 2e6a 6f69 6e28 636e 6d66 5f6f 7574 7075  .join(cnmf_outpu
+0000b640: 745f 6469 722c 2063 6e6d 665f 6e61 6d65  t_dir, cnmf_name
+0000b650: 2c20 6622 7b63 6e6d 665f 6e61 6d65 7d2a  , f"{cnmf_name}*
+0000b660: 2e2a 7370 6563 7472 612a 2e6b 5f2a 2229  .*spectra*.k_*")
+0000b670: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000b680: 6c64 745f 7374 7220 3d20 6f73 2e70 6174  ldt_str = os.pat
+0000b690: 682e 6261 7365 6e61 6d65 2866 6e29 2e73  h.basename(fn).s
+0000b6a0: 706c 6974 2822 2e22 295b 2d33 5d0d 0a20  plit(".")[-3].. 
+0000b6b0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+0000b6c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b6d0: 206c 6474 203d 2066 6c6f 6174 286c 6474   ldt = float(ldt
+0000b6e0: 5f73 7472 2e72 6570 6c61 6365 2822 6474  _str.replace("dt
+0000b6f0: 5f22 2c20 2222 292e 7265 706c 6163 6528  _", "").replace(
+0000b700: 225f 222c 2022 2e22 2929 0d0a 2020 2020  "_", "."))..    
+0000b710: 2020 2020 2020 2020 6578 6365 7074 2056          except V
+0000b720: 616c 7565 4572 726f 723a 0d0a 2020 2020  alueError:..    
+0000b730: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+0000b740: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0000b750: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000b760: 2020 2020 2073 656e 7365 645f 6c64 7473       sensed_ldts
+0000b770: 2e61 6464 2828 6c64 745f 7374 722c 206c  .add((ldt_str, l
+0000b780: 6474 2929 0d0a 2020 2020 2020 2020 6966  dt))..        if
+0000b790: 206c 6f63 616c 5f64 656e 7369 7479 5f74   local_density_t
+0000b7a0: 6872 6573 686f 6c64 2069 7320 4e6f 6e65  hreshold is None
+0000b7b0: 2061 6e64 206c 656e 2873 656e 7365 645f   and len(sensed_
+0000b7c0: 6c64 7473 2920 3d3d 2031 3a0d 0a20 2020  ldts) == 1:..   
+0000b7d0: 2020 2020 2020 2020 206c 6474 5f73 7472           ldt_str
+0000b7e0: 2c20 6c64 7420 3d20 7365 6e73 6564 5f6c  , ldt = sensed_l
+0000b7f0: 6474 732e 706f 7028 290d 0a20 2020 2020  dts.pop()..     
+0000b800: 2020 2065 6c69 6620 6c6f 6361 6c5f 6465     elif local_de
+0000b810: 6e73 6974 795f 7468 7265 7368 6f6c 6420  nsity_threshold 
+0000b820: 696e 2028 6c64 745b 315d 2066 6f72 206c  in (ldt[1] for l
+0000b830: 6474 2069 6e20 7365 6e73 6564 5f6c 6474  dt in sensed_ldt
+0000b840: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
+0000b850: 206c 6474 5f73 7472 2c20 6c64 7420 3d20   ldt_str, ldt = 
+0000b860: 5b28 6c64 745f 7374 722c 206c 6474 2920  [(ldt_str, ldt) 
+0000b870: 666f 7220 6c64 745f 7374 722c 206c 6474  for ldt_str, ldt
+0000b880: 2069 6e20 7365 6e73 6564 5f6c 6474 7320   in sensed_ldts 
+0000b890: 6966 206c 6474 203d 3d20 6c6f 6361 6c5f  if ldt == local_
+0000b8a0: 6465 6e73 6974 795f 7468 7265 7368 6f6c  density_threshol
+0000b8b0: 645d 2e70 6f70 2829 0d0a 2020 2020 2020  d].pop()..      
+0000b8c0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0000b8d0: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
+0000b8e0: 6d65 4572 726f 7228 6622 6c6f 6361 6c5f  meError(f"local_
+0000b8f0: 6465 6e73 6974 795f 7468 7265 7368 6f6c  density_threshol
+0000b900: 6420 6f66 207b 6c6f 6361 6c5f 6465 6e73  d of {local_dens
+0000b910: 6974 795f 7468 7265 7368 6f6c 647d 2064  ity_threshold} d
+0000b920: 6f65 7320 6e6f 7420 6d61 7463 6820 7768  oes not match wh
+0000b930: 6174 2069 7320 696e 2074 6865 2063 4e4d  at is in the cNM
+0000b940: 4620 7265 7375 6c74 2064 6972 6563 746f  F result directo
+0000b950: 7279 3a20 7b73 656e 7365 645f 6c64 7473  ry: {sensed_ldts
+0000b960: 7d22 290d 0a20 2020 2020 2020 2073 656c  }")..        sel
+0000b970: 662e 6164 6174 612e 756e 735b 226c 6474  f.adata.uns["ldt
+0000b980: 225d 203d 206c 6474 0d0a 2020 2020 2020  "] = ldt..      
+0000b990: 2020 7365 6c66 2e61 6461 7461 2e75 6e73    self.adata.uns
+0000b9a0: 5b22 6c6e 7322 5d20 3d20 6c6f 6361 6c5f  ["lns"] = local_
+0000b9b0: 6e65 6967 6862 6f72 686f 6f64 5f73 697a  neighborhood_siz
+0000b9c0: 650d 0a20 2020 2020 2020 2020 2020 200d  e..            .
+0000b9d0: 0a20 2020 2020 2020 2023 2049 6d70 6f72  .        # Impor
+0000b9e0: 7420 4745 5073 0d0a 2020 2020 2020 2020  t GEPs..        
+0000b9f0: 7265 7375 6c74 5f74 7970 6573 203d 207b  result_types = {
+0000ba00: 0d0a 2020 2020 2020 2020 2020 2020 2267  ..            "g
+0000ba10: 656e 655f 7370 6563 7472 615f 7363 6f72  ene_spectra_scor
+0000ba20: 6522 3a20 2263 6e6d 665f 6765 705f 7363  e": "cnmf_gep_sc
+0000ba30: 6f72 6522 2c0d 0a20 2020 2020 2020 2020  ore",..         
+0000ba40: 2020 2022 6765 6e65 5f73 7065 6374 7261     "gene_spectra
+0000ba50: 5f74 706d 223a 2022 636e 6d66 5f67 6570  _tpm": "cnmf_gep
+0000ba60: 5f74 706d 222c 0d0a 2020 2020 2020 2020  _tpm",..        
+0000ba70: 2020 2020 2273 7065 6374 7261 223a 2022      "spectra": "
+0000ba80: 636e 6d66 5f67 6570 5f72 6177 220d 0a20  cnmf_gep_raw".. 
+0000ba90: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+0000baa0: 2020 2020 2020 666f 7220 6d61 7463 6873        for matchs
+0000bab0: 7472 2c20 7265 7375 6c74 5f74 7970 6520  tr, result_type 
+0000bac0: 696e 2072 6573 756c 745f 7479 7065 732e  in result_types.
+0000bad0: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
+0000bae0: 2020 2020 2020 6c6f 6767 696e 672e 696e        logging.in
+0000baf0: 666f 2866 2249 6d70 6f72 7469 6e67 2047  fo(f"Importing G
+0000bb00: 4550 733a 207b 6d61 7463 6873 7472 7d22  EPs: {matchstr}"
+0000bb10: 2920 200d 0a20 2020 2020 2020 2020 2020  )  ..           
+0000bb20: 206d 6574 615f 7720 3d20 5b5d 0d0a 2020   meta_w = []..  
+0000bb30: 2020 2020 2020 2020 2020 666f 7220 666e            for fn
+0000bb40: 2069 6e20 676c 6f62 286f 732e 7061 7468   in glob(os.path
+0000bb50: 2e6a 6f69 6e28 636e 6d66 5f6f 7574 7075  .join(cnmf_outpu
+0000bb60: 745f 6469 722c 2063 6e6d 665f 6e61 6d65  t_dir, cnmf_name
+0000bb70: 2c20 6622 7b63 6e6d 665f 6e61 6d65 7d2a  , f"{cnmf_name}*
+0000bb80: 2e7b 6d61 7463 6873 7472 7d2e 6b5f 2a2e  .{matchstr}.k_*.
+0000bb90: 7b6c 6474 5f73 7472 7d2e 2a74 7874 2229  {ldt_str}.*txt")
+0000bba0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000bbb0: 2020 2020 6b20 3d20 696e 7428 6f73 2e70      k = int(os.p
+0000bbc0: 6174 682e 6261 7365 6e61 6d65 2866 6e29  ath.basename(fn)
+0000bbd0: 2e72 656d 6f76 6570 7265 6669 7828 6622  .removeprefix(f"
+0000bbe0: 7b63 6e6d 665f 6e61 6d65 7d2e 7b6d 6174  {cnmf_name}.{mat
+0000bbf0: 6368 7374 727d 2e22 292e 7370 6c69 7428  chstr}.").split(
+0000bc00: 222e 2229 5b30 5d2e 7265 706c 6163 6528  ".")[0].replace(
+0000bc10: 226b 5f22 2c20 2222 2929 0d0a 2020 2020  "k_", ""))..    
+0000bc20: 2020 2020 2020 2020 2020 2020 7720 3d20              w = 
+0000bc30: 7064 2e72 6561 645f 7461 626c 6528 666e  pd.read_table(fn
+0000bc40: 2c20 696e 6465 785f 636f 6c3d 3029 0d0a  , index_col=0)..
+0000bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc60: 772e 696e 6465 7820 3d20 7374 7228 6b29  w.index = str(k)
+0000bc70: 202b 2022 2e22 202b 2077 2e69 6e64 6578   + "." + w.index
+0000bc80: 2e61 7374 7970 6528 7374 7229 0d0a 2020  .astype(str)..  
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0000bca0: 7461 5f77 2e61 7070 656e 6428 7729 0d0a  ta_w.append(w)..
+0000bcb0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+0000bcc0: 5f77 203d 2070 642e 636f 6e63 6174 286d  _w = pd.concat(m
+0000bcd0: 6574 615f 772c 2061 7869 733d 3029 2e54  eta_w, axis=0).T
+0000bce0: 2e72 6569 6e64 6578 2873 656c 662e 6164  .reindex(self.ad
+0000bcf0: 6174 612e 7661 722e 696e 6465 7829 2e72  ata.var.index).r
+0000bd00: 656e 616d 655f 6178 6973 285b 226b 2e67  ename_axis(["k.g
+0000bd10: 6570 225d 2c20 6178 6973 3d31 290d 0a20  ep"], axis=1).. 
+0000bd20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000bd30: 6164 6174 612e 7661 726d 5b72 6573 756c  adata.varm[resul
+0000bd40: 745f 7479 7065 5d20 3d20 6d65 7461 5f77  t_type] = meta_w
+0000bd50: 0d0a 0d0a 2020 2020 2020 2020 2320 496d  ....        # Im
+0000bd60: 706f 7274 2055 7361 6765 730d 0a20 2020  port Usages..   
+0000bd70: 2020 2020 206c 6f67 6769 6e67 2e69 6e66       logging.inf
+0000bd80: 6f28 6622 496d 706f 7274 696e 6720 5573  o(f"Importing Us
+0000bd90: 6167 6573 2229 2020 0d0a 2020 2020 2020  ages")  ..      
+0000bda0: 2020 7573 6167 6520 3d20 5b5d 0d0a 2020    usage = []..  
+0000bdb0: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
+0000bdc0: 676c 6f62 286f 732e 7061 7468 2e6a 6f69  glob(os.path.joi
+0000bdd0: 6e28 636e 6d66 5f6f 7574 7075 745f 6469  n(cnmf_output_di
+0000bde0: 722c 2063 6e6d 665f 6e61 6d65 2c20 6622  r, cnmf_name, f"
+0000bdf0: 7b63 6e6d 665f 6e61 6d65 7d2a 2e75 7361  {cnmf_name}*.usa
+0000be00: 6765 732e 6b5f 2a2e 7b6c 6474 5f73 7472  ges.k_*.{ldt_str
+0000be10: 7d2e 2a74 7874 2229 293a 0d0a 2020 2020  }.*txt")):..    
+0000be20: 2020 2020 2020 2020 6b20 3d20 696e 7428          k = int(
+0000be30: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
+0000be40: 2866 6e29 2e72 656d 6f76 6570 7265 6669  (fn).removeprefi
+0000be50: 7828 6622 7b63 6e6d 665f 6e61 6d65 7d2e  x(f"{cnmf_name}.
+0000be60: 7573 6167 6573 2e22 292e 7370 6c69 7428  usages.").split(
+0000be70: 222e 2229 5b30 5d2e 7265 706c 6163 6528  ".")[0].replace(
+0000be80: 226b 5f22 2c20 2222 2929 0d0a 2020 2020  "k_", ""))..    
+0000be90: 2020 2020 2020 2020 6820 3d20 7064 2e72          h = pd.r
+0000bea0: 6561 645f 7461 626c 6528 666e 2c20 696e  ead_table(fn, in
+0000beb0: 6465 785f 636f 6c3d 3029 0d0a 2020 2020  dex_col=0)..    
+0000bec0: 2020 2020 2020 2020 682e 636f 6c75 6d6e          h.column
+0000bed0: 7320 3d20 7374 7228 6b29 202b 2022 2e22  s = str(k) + "."
+0000bee0: 202b 2068 2e63 6f6c 756d 6e73 2e61 7374   + h.columns.ast
+0000bef0: 7970 6528 7374 7229 0d0a 2020 2020 2020  ype(str)..      
+0000bf00: 2020 2020 2020 7573 6167 652e 6170 7065        usage.appe
+0000bf10: 6e64 2868 290d 0a20 2020 2020 2020 2073  nd(h)..        s
+0000bf20: 656c 662e 6164 6174 612e 6f62 736d 5b22  elf.adata.obsm["
+0000bf30: 636e 6d66 5f75 7361 6765 225d 203d 2070  cnmf_usage"] = p
+0000bf40: 642e 636f 6e63 6174 2875 7361 6765 2c20  d.concat(usage, 
+0000bf50: 6178 6973 3d31 292e 736f 7274 5f69 6e64  axis=1).sort_ind
+0000bf60: 6578 2861 7869 733d 3129 2e72 656e 616d  ex(axis=1).renam
+0000bf70: 655f 6178 6973 285b 226b 2e67 6570 225d  e_axis(["k.gep"]
+0000bf80: 2c20 6178 6973 3d31 290d 0a20 2020 2020  , axis=1)..     
+0000bf90: 2020 200d 0a20 2020 2020 2020 2023 2049     ..        # I
+0000bfa0: 6d70 6f72 7420 6765 6e65 206c 6973 7420  mport gene list 
+0000bfb0: 7573 6564 2066 6f72 2066 6163 746f 7269  used for factori
+0000bfc0: 7a61 7469 6f6e 0d0a 2020 2020 2020 2020  zation..        
+0000bfd0: 7769 7468 206f 7065 6e28 6f73 2e70 6174  with open(os.pat
+0000bfe0: 682e 6a6f 696e 2863 6e6d 665f 6f75 7470  h.join(cnmf_outp
+0000bff0: 7574 5f64 6972 2c20 636e 6d66 5f6e 616d  ut_dir, cnmf_nam
+0000c000: 652c 2066 227b 636e 6d66 5f6e 616d 657d  e, f"{cnmf_name}
+0000c010: 2e6f 7665 7264 6973 7065 7273 6564 5f67  .overdispersed_g
+0000c020: 656e 6573 2e74 7874 2229 2920 6173 2066  enes.txt")) as f
+0000c030: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+0000c040: 656c 662e 6164 6174 612e 756e 735b 2267  elf.adata.uns["g
+0000c050: 656e 655f 6c69 7374 225d 203d 205b 6c69  ene_list"] = [li
+0000c060: 6e65 2e73 7472 6970 2829 2066 6f72 206c  ne.strip() for l
+0000c070: 696e 6520 696e 2066 2e72 6561 646c 696e  ine in f.readlin
+0000c080: 6573 2829 5d0d 0a0d 0a20 2020 2020 2020  es()]....       
+0000c090: 2023 2049 6d70 6f72 7420 4b2d 7365 6c65   # Import K-sele
+0000c0a0: 6374 696f 6e20 7374 6174 730d 0a20 2020  ction stats..   
+0000c0b0: 2020 2020 206b 7661 6c73 203d 2070 642e       kvals = pd.
+0000c0c0: 4461 7461 4672 616d 6528 2a2a 6e70 2e6c  DataFrame(**np.l
+0000c0d0: 6f61 6428 6f73 2e70 6174 682e 6a6f 696e  oad(os.path.join
+0000c0e0: 2863 6e6d 665f 6f75 7470 7574 5f64 6972  (cnmf_output_dir
+0000c0f0: 2c20 636e 6d66 5f6e 616d 652c 2066 227b  , cnmf_name, f"{
+0000c100: 636e 6d66 5f6e 616d 657d 2e6b 5f73 656c  cnmf_name}.k_sel
+0000c110: 6563 7469 6f6e 5f73 7461 7473 2e64 662e  ection_stats.df.
+0000c120: 6e70 7a22 292c 2061 6c6c 6f77 5f70 6963  npz"), allow_pic
+0000c130: 6b6c 653d 5472 7565 2929 2e73 6574 5f69  kle=True)).set_i
+0000c140: 6e64 6578 2822 6b22 295b 5b22 7374 6162  ndex("k")[["stab
+0000c150: 696c 6974 7922 2c20 2270 7265 6469 6374  ility", "predict
+0000c160: 696f 6e5f 6572 726f 7222 5d5d 0d0a 2020  ion_error"]]..  
+0000c170: 2020 2020 2020 6b76 616c 732e 696e 6465        kvals.inde
+0000c180: 7820 3d20 6b76 616c 732e 696e 6465 782e  x = kvals.index.
+0000c190: 6173 7479 7065 2869 6e74 290d 0a20 2020  astype(int)..   
+0000c1a0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+0000c1b0: 756e 735b 226b 7661 6c73 225d 203d 206b  uns["kvals"] = k
+0000c1c0: 7661 6c73 0d0a 2020 2020 2020 2020 7365  vals..        se
+0000c1d0: 6c66 2e61 7070 656e 645f 746f 5f68 6973  lf.append_to_his
+0000c1e0: 746f 7279 2822 634e 4d46 2072 6573 756c  tory("cNMF resul
+0000c1f0: 7473 2061 6464 6564 2066 726f 6d20 6f75  ts added from ou
+0000c200: 7470 7574 2064 6972 6563 746f 7279 207b  tput directory {
+0000c210: 636e 6d66 5f6f 7574 7075 745f 6469 727d  cnmf_output_dir}
+0000c220: 2f7b 636e 6d66 5f6e 616d 657d 2229 0d0a  /{cnmf_name}")..
+0000c230: 0d0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
+0000c240: 5f63 6e6d 665f 7265 7375 6c74 7328 7365  _cnmf_results(se
+0000c250: 6c66 293a 0d0a 2020 2020 2020 2020 666f  lf):..        fo
+0000c260: 7220 7265 7375 6c74 5f74 7970 6520 696e  r result_type in
+0000c270: 2028 2263 6e6d 665f 6765 705f 7363 6f72   ("cnmf_gep_scor
+0000c280: 6522 2c20 2263 6e6d 665f 6765 705f 7470  e", "cnmf_gep_tp
+0000c290: 6d22 2c20 2263 6e6d 665f 6765 705f 7261  m", "cnmf_gep_ra
+0000c2a0: 7722 293a 0d0a 2020 2020 2020 2020 2020  w"):..          
+0000c2b0: 2020 7365 6c66 2e61 6461 7461 2e76 6172    self.adata.var
+0000c2c0: 6d2e 706f 7028 7265 7375 6c74 5f74 7970  m.pop(result_typ
+0000c2d0: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
+0000c2e0: 2e61 6461 7461 2e6f 6273 6d2e 706f 7028  .adata.obsm.pop(
+0000c2f0: 2263 6e6d 665f 7573 6167 6522 290d 0a20  "cnmf_usage").. 
+0000c300: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+0000c310: 612e 756e 732e 706f 7028 2267 656e 655f  a.uns.pop("gene_
+0000c320: 6c69 7374 2229 0d0a 2020 2020 2020 2020  list")..        
+0000c330: 7365 6c66 2e61 6461 7461 2e75 6e73 2e70  self.adata.uns.p
+0000c340: 6f70 2822 6b76 616c 7322 290d 0a20 2020  op("kvals")..   
+0000c350: 2020 2020 2073 656c 662e 6170 7065 6e64       self.append
+0000c360: 5f74 6f5f 6869 7374 6f72 7928 2263 4e4d  _to_history("cNM
+0000c370: 4620 7265 7375 6c74 7320 7265 6d6f 7665  F results remove
+0000c380: 642e 2229 0d0a 0d0a 0d0a 2020 2020 6465  d.")......    de
+0000c390: 6620 6765 745f 7573 6167 6573 2873 656c  f get_usages(sel
+0000c3a0: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
+0000c3b0: 2020 2020 2020 206b 3a20 556e 696f 6e5b         k: Union[
+0000c3c0: 696e 742c 2049 7465 7261 626c 655d 203d  int, Iterable] =
+0000c3d0: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
+0000c3e0: 2020 2020 2020 2020 2020 2064 6973 6372             discr
+0000c3f0: 6574 697a 653a 2062 6f6f 6c20 3d20 4661  etize: bool = Fa
+0000c400: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+0000c410: 2020 2020 2020 2020 206e 6f72 6d61 6c69           normali
+0000c420: 7a65 3a20 626f 6f6c 203d 2046 616c 7365  ze: bool = False
+0000c430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c440: 2020 2020 2029 202d 3e20 7064 2e44 6174       ) -> pd.Dat
+0000c450: 6146 7261 6d65 3a0d 0a20 2020 2020 2020  aFrame:..       
+0000c460: 2022 2222 0d0a 2020 2020 2020 2020 4361   """..        Ca
+0000c470: 6c63 756c 6174 6520 7573 6167 6520 6f66  lculate usage of
+0000c480: 2065 6163 6820 4745 5020 696e 2065 6163   each GEP in eac
+0000c490: 6820 7361 6d70 6c65 2f6f 6273 6572 7661  h sample/observa
+0000c4a0: 7469 6f6e 2e0d 0a0d 0a20 2020 2020 2020  tion.....       
+0000c4b0: 203a 7061 7261 6d20 6b3a 2049 6620 616e   :param k: If an
+0000c4c0: 2069 6e74 6567 6572 206f 7220 6c69 7374   integer or list
+0000c4d0: 206f 6620 696e 7465 6765 7273 2c20 7265   of integers, re
+0000c4e0: 7475 726e 7320 7573 6167 6573 206f 6e6c  turns usages onl
+0000c4f0: 7920 666f 7220 7370 6563 6966 6965 6420  y for specified 
+0000c500: 7261 6e6b 732e 204f 7468 6572 7769 7365  ranks. Otherwise
+0000c510: 2c20 7265 7475 726e 7320 7573 6167 6520  , returns usage 
+0000c520: 6f66 2061 6c6c 2047 4550 7320 6163 726f  of all GEPs acro
+0000c530: 7373 2072 616e 6b73 2e20 4465 6661 756c  ss ranks. Defaul
+0000c540: 7473 2074 6f20 4e6f 6e65 0d0a 2020 2020  ts to None..    
+0000c550: 2020 2020 3a74 7970 6520 6b3a 2069 6e74      :type k: int
+0000c560: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+0000c570: 2020 2020 3a70 6172 616d 2064 6973 6372      :param discr
+0000c580: 6574 697a 653a 2044 6973 6372 6574 697a  etize: Discretiz
+0000c590: 6573 2074 6865 2075 7361 6765 206d 6174  es the usage mat
+0000c5a0: 7269 7820 7375 6368 2074 6861 7420 666f  rix such that fo
+0000c5b0: 7220 6561 6368 2076 616c 7565 206f 6620  r each value of 
+0000c5c0: 6b2c 2065 6163 6820 7361 6d70 6c65 2068  k, each sample h
+0000c5d0: 6173 2075 7361 6765 206f 6620 6f6e 6c79  as usage of only
+0000c5e0: 2031 2047 4550 2028 7468 6520 6f6e 6520   1 GEP (the one 
+0000c5f0: 7769 7468 2074 6865 206d 6178 696d 756d  with the maximum
+0000c600: 2075 7361 6765 292e 2044 6566 6175 6c74   usage). Default
+0000c610: 7320 746f 2046 616c 7365 0d0a 2020 2020  s to False..    
+0000c620: 2020 2020 3a74 7970 6520 6469 7363 7265      :type discre
+0000c630: 7469 7a65 3a20 626f 6f6c 2c20 6f70 7469  tize: bool, opti
+0000c640: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
+0000c650: 6172 616d 206e 6f72 6d61 6c69 7a65 3a20  aram normalize: 
+0000c660: 4e6f 726d 616c 697a 6520 7468 6520 4745  Normalize the GE
+0000c670: 5020 7573 6167 6520 6d61 7472 6978 2073  P usage matrix s
+0000c680: 7563 6820 7468 6174 2066 6f72 2065 6163  uch that for eac
+0000c690: 6820 7661 6c75 6520 6f66 206b 2c20 7573  h value of k, us
+0000c6a0: 6167 6520 6f66 2061 6c6c 2047 4550 7320  age of all GEPs 
+0000c6b0: 7375 6d73 2074 6f20 312e 2044 6566 6175  sums to 1. Defau
+0000c6c0: 6c74 7320 746f 2046 616c 7365 0d0a 2020  lts to False..  
+0000c6d0: 2020 2020 2020 3a74 7970 6520 6e6f 726d        :type norm
+0000c6e0: 616c 697a 653a 2062 6f6f 6c2c 206f 7074  alize: bool, opt
+0000c6f0: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
+0000c700: 7265 7475 726e 3a20 6f62 7365 7276 6174  return: observat
+0000c710: 696f 6e20 c397 2047 4550 206d 6174 7269  ion .. GEP matri
+0000c720: 780d 0a20 2020 2020 2020 203a 7274 7970  x..        :rtyp
+0000c730: 653a 2070 642e 4461 7461 4672 616d 650d  e: pd.DataFrame.
+0000c740: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+0000c750: 2020 2020 2020 6466 203d 2073 656c 662e        df = self.
+0000c760: 6164 6174 612e 6f62 736d 5b22 636e 6d66  adata.obsm["cnmf
+0000c770: 5f75 7361 6765 225d 2e63 6f70 7928 290d  _usage"].copy().
+0000c780: 0a20 2020 2020 2020 2064 662e 636f 6c75  .        df.colu
+0000c790: 6d6e 7320 3d20 7064 2e4d 756c 7469 496e  mns = pd.MultiIn
+0000c7a0: 6465 782e 6672 6f6d 5f74 7570 6c65 7328  dex.from_tuples(
+0000c7b0: 6466 2e63 6f6c 756d 6e73 2e73 7472 2e73  df.columns.str.s
+0000c7c0: 706c 6974 2822 2e22 292e 746f 5f6c 6973  plit(".").to_lis
+0000c7d0: 7428 2929 0d0a 2020 2020 2020 2020 6466  t())..        df
+0000c7e0: 2e63 6f6c 756d 6e73 203d 2064 662e 636f  .columns = df.co
+0000c7f0: 6c75 6d6e 732e 7365 745f 6c65 7665 6c73  lumns.set_levels
+0000c800: 285b 6c2e 6173 7479 7065 2822 696e 7422  ([l.astype("int"
+0000c810: 2920 666f 7220 6c20 696e 2064 662e 636f  ) for l in df.co
+0000c820: 6c75 6d6e 732e 6c65 7665 6c73 5d29 0d0a  lumns.levels])..
+0000c830: 2020 2020 2020 2020 6966 206e 6f72 6d61          if norma
+0000c840: 6c69 7a65 3a0d 0a20 2020 2020 2020 2020  lize:..         
+0000c850: 2020 206e 6f72 6d61 6c69 7a65 6420 3d20     normalized = 
+0000c860: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+0000c870: 666f 7220 5f2c 2073 7562 6466 2069 6e20  for _, subdf in 
+0000c880: 6466 2e54 2e67 726f 7570 6279 286c 6576  df.T.groupby(lev
+0000c890: 656c 3d30 293a 0d0a 2020 2020 2020 2020  el=0):..        
+0000c8a0: 2020 2020 2020 2020 6e6f 726d 616c 697a          normaliz
+0000c8b0: 6564 2e61 7070 656e 6428 7375 6264 662e  ed.append(subdf.
+0000c8c0: 6469 7628 7375 6264 662e 7375 6d28 2929  div(subdf.sum())
+0000c8d0: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
+0000c8e0: 6620 3d20 7064 2e63 6f6e 6361 7428 6e6f  f = pd.concat(no
+0000c8f0: 726d 616c 697a 6564 292e 540d 0a20 2020  rmalized).T..   
+0000c900: 2020 2020 2069 6620 6469 7363 7265 7469       if discreti
+0000c910: 7a65 3a0d 0a20 2020 2020 2020 2020 2020  ze:..           
+0000c920: 2064 6973 6372 6574 697a 6564 203d 205b   discretized = [
+0000c930: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
+0000c940: 6f72 205f 2c20 7375 6264 6620 696e 2064  or _, subdf in d
+0000c950: 662e 542e 6772 6f75 7062 7928 6c65 7665  f.T.groupby(leve
+0000c960: 6c3d 3029 3a0d 0a20 2020 2020 2020 2020  l=0):..         
+0000c970: 2020 2020 2020 2064 6973 6372 6574 697a         discretiz
+0000c980: 6564 2e61 7070 656e 6428 7375 6264 662e  ed.append(subdf.
+0000c990: 6571 2873 7562 6466 2e6d 6178 2829 292e  eq(subdf.max()).
+0000c9a0: 6173 7479 7065 2869 6e74 2929 0d0a 2020  astype(int))..  
+0000c9b0: 2020 2020 2020 2020 2020 6466 203d 2070            df = p
+0000c9c0: 642e 636f 6e63 6174 2864 6973 6372 6574  d.concat(discret
+0000c9d0: 697a 6564 292e 5420 2020 2020 2020 200d  ized).T        .
+0000c9e0: 0a20 2020 2020 2020 2069 6620 6b20 6973  .        if k is
+0000c9f0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+0000ca00: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
+0000ca10: 6c6f 635b 3a2c 206b 5d0d 0a20 2020 2020  loc[:, k]..     
+0000ca20: 2020 2064 6620 3d20 6466 2e73 6f72 745f     df = df.sort_
+0000ca30: 696e 6465 7828 6178 6973 3d31 2920 2020  index(axis=1)   
+0000ca40: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000ca50: 2064 660d 0a0d 0a20 2020 2064 6566 2067   df....    def g
+0000ca60: 6574 5f70 726f 6772 616d 7328 7365 6c66  et_programs(self
+0000ca70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000ca80: 2020 2020 6b3a 2055 6e69 6f6e 5b69 6e74      k: Union[int
+0000ca90: 2c20 4974 6572 6162 6c65 5d20 3d20 4e6f  , Iterable] = No
+0000caa0: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+0000cab0: 2020 2020 2020 7479 7065 3d22 636e 6d66        type="cnmf
+0000cac0: 5f67 6570 5f73 636f 7265 220d 0a20 2020  _gep_score"..   
+0000cad0: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+0000cae0: 2d3e 2070 642e 4461 7461 4672 616d 653a  -> pd.DataFrame:
+0000caf0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+0000cb00: 2020 2020 2020 2047 6574 2066 6561 7475         Get featu
+0000cb10: 7265 2073 636f 7265 7320 666f 7220 7072  re scores for pr
+0000cb20: 6f67 7261 6d73 2e0d 0a0d 0a20 2020 2020  ograms.....     
+0000cb30: 2020 203a 7061 7261 6d20 6b3a 2049 6620     :param k: If 
+0000cb40: 616e 2069 6e74 6567 6572 206f 7220 6c69  an integer or li
+0000cb50: 7374 206f 6620 696e 7465 6765 7273 2c20  st of integers, 
+0000cb60: 7265 7475 726e 7320 4745 5073 206f 6e6c  returns GEPs onl
+0000cb70: 7920 666f 7220 7370 6563 6966 6965 6420  y for specified 
+0000cb80: 7261 6e6b 732e 204f 7468 6572 7769 7365  ranks. Otherwise
+0000cb90: 2c20 7265 7475 726e 7320 4745 5073 2066  , returns GEPs f
+0000cba0: 726f 6d20 616c 6c20 7261 6e6b 732e 2044  rom all ranks. D
+0000cbb0: 6566 6175 6c74 7320 746f 204e 6f6e 650d  efaults to None.
+0000cbc0: 0a20 2020 2020 2020 203a 7479 7065 206b  .        :type k
+0000cbd0: 3a20 556e 696f 6e5b 696e 742c 2049 7465  : Union[int, Ite
+0000cbe0: 7261 626c 655d 2c20 6f70 7469 6f6e 616c  rable], optional
+0000cbf0: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000cc00: 2074 7970 653a 2022 636e 6d66 5f67 6570   type: "cnmf_gep
+0000cc10: 5f73 636f 7265 2220 6f72 2022 636e 6d66  _score" or "cnmf
+0000cc20: 5f67 6570 5f74 706d 222c 2064 6566 6175  _gep_tpm", defau
+0000cc30: 6c74 7320 746f 2022 636e 6d66 5f67 6570  lts to "cnmf_gep
+0000cc40: 5f73 636f 7265 220d 0a20 2020 2020 2020  _score"..       
+0000cc50: 203a 7479 7065 2074 7970 653a 2073 7472   :type type: str
+0000cc60: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+0000cc70: 2020 2020 3a72 6574 7572 6e3a 2066 6561      :return: fea
+0000cc80: 7475 7265 7320 c397 2047 4550 206d 6174  tures .. GEP mat
+0000cc90: 7269 780d 0a20 2020 2020 2020 203a 7274  rix..        :rt
+0000cca0: 7970 653a 2070 642e 4461 7461 4672 616d  ype: pd.DataFram
+0000ccb0: 650d 0a20 2020 2020 2020 2022 2222 0d0a  e..        """..
+0000ccc0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+0000ccd0: 656c 662e 6861 735f 636e 6d66 5f72 6573  elf.has_cnmf_res
+0000cce0: 756c 7473 0d0a 2020 2020 2020 2020 6466  ults..        df
+0000ccf0: 203d 2073 656c 662e 6164 6174 612e 7661   = self.adata.va
+0000cd00: 726d 5b74 7970 655d 2e63 6f70 7928 290d  rm[type].copy().
+0000cd10: 0a20 2020 2020 2020 2064 662e 636f 6c75  .        df.colu
+0000cd20: 6d6e 7320 3d20 7064 2e4d 756c 7469 496e  mns = pd.MultiIn
+0000cd30: 6465 782e 6672 6f6d 5f74 7570 6c65 7328  dex.from_tuples(
+0000cd40: 6466 2e63 6f6c 756d 6e73 2e73 7472 2e73  df.columns.str.s
+0000cd50: 706c 6974 2822 2e22 292e 746f 5f6c 6973  plit(".").to_lis
+0000cd60: 7428 2929 0d0a 2020 2020 2020 2020 6466  t())..        df
+0000cd70: 2e63 6f6c 756d 6e73 203d 2064 662e 636f  .columns = df.co
+0000cd80: 6c75 6d6e 732e 7365 745f 6c65 7665 6c73  lumns.set_levels
+0000cd90: 285b 6c2e 6173 7479 7065 2822 696e 7422  ([l.astype("int"
+0000cda0: 2920 666f 7220 6c20 696e 2064 662e 636f  ) for l in df.co
+0000cdb0: 6c75 6d6e 732e 6c65 7665 6c73 5d29 0d0a  lumns.levels])..
+0000cdc0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+0000cdd0: 7461 6e63 6528 6b2c 2028 696e 742c 206e  tance(k, (int, n
+0000cde0: 702e 696e 7465 6765 7229 293a 0d0a 2020  p.integer)):..  
+0000cdf0: 2020 2020 2020 2020 2020 6466 203d 2064            df = d
+0000ce00: 662e 6c6f 635b 3a2c 206b 5d0d 0a20 2020  f.loc[:, k]..   
+0000ce10: 2020 2020 2020 2020 2064 6620 3d20 6466           df = df
+0000ce20: 2e72 656e 616d 655f 6178 6973 2863 6f6c  .rename_axis(col
+0000ce30: 756d 6e73 3d5b 2270 726f 6772 616d 225d  umns=["program"]
+0000ce40: 292e 736f 7274 5f69 6e64 6578 2861 7869  ).sort_index(axi
+0000ce50: 733d 3129 0d0a 2020 2020 2020 2020 656c  s=1)..        el
+0000ce60: 6966 2069 7369 6e73 7461 6e63 6528 6b2c  if isinstance(k,
+0000ce70: 2049 7465 7261 626c 6529 3a0d 0a20 2020   Iterable):..   
+0000ce80: 2020 2020 2020 2020 2064 6620 3d20 6466           df = df
+0000ce90: 2e6c 6f63 5b3a 2c20 6b5d 0d0a 2020 2020  .loc[:, k]..    
+0000cea0: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
+0000ceb0: 7265 6e61 6d65 5f61 7869 7328 636f 6c75  rename_axis(colu
+0000cec0: 6d6e 733d 5b22 6b22 2c20 2270 726f 6772  mns=["k", "progr
+0000ced0: 616d 225d 292e 736f 7274 5f69 6e64 6578  am"]).sort_index
+0000cee0: 2861 7869 733d 3129 0d0a 2020 2020 2020  (axis=1)..      
+0000cef0: 2020 7265 7475 726e 2064 660d 0a20 2020    return df..   
+0000cf00: 200d 0a20 2020 2064 6566 2067 6574 5f61   ..    def get_a
+0000cf10: 7070 726f 7869 6d61 7469 6f6e 2873 656c  pproximation(sel
+0000cf20: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
+0000cf30: 2020 2020 2020 2020 2020 2020 2020 6b3a                k:
+0000cf40: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+0000cf50: 204e 6f6e 652c 0d0a 2020 2020 2020 2020   None,..        
 0000cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf70: 2020 2020 2020 2020 2920 2d3e 2070 642e          ) -> pd.
-0000cf80: 4461 7461 4672 616d 653a 0d0a 2020 2020  DataFrame:..    
-0000cf90: 2020 2020 2222 2247 6574 2073 616d 706c      """Get sampl
-0000cfa0: 652f 6f62 7365 7276 6174 696f 6e20 6d65  e/observation me
-0000cfb0: 7461 6461 7461 2e0d 0a0d 0a20 2020 2020  tadata.....     
-0000cfc0: 2020 203a 7061 7261 6d20 696e 636c 7564     :param includ
-0000cfd0: 655f 6361 7465 676f 7269 6361 6c3a 2049  e_categorical: I
-0000cfe0: 6e63 6c75 6465 2063 6174 6567 6f72 6963  nclude categoric
-0000cff0: 616c 206d 6574 6164 6174 6120 6c61 7965  al metadata laye
-0000d000: 7273 2c20 6465 6661 756c 7473 2074 6f20  rs, defaults to 
-0000d010: 5472 7565 0d0a 2020 2020 2020 2020 3a74  True..        :t
-0000d020: 7970 6520 696e 636c 7564 655f 6361 7465  ype include_cate
-0000d030: 676f 7269 6361 6c3a 2062 6f6f 6c2c 206f  gorical: bool, o
-0000d040: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-0000d050: 203a 7061 7261 6d20 696e 636c 7564 655f   :param include_
-0000d060: 6e75 6d65 7269 6361 6c3a 2049 6e63 6c75  numerical: Inclu
-0000d070: 6465 206e 756d 6572 6963 616c 206d 6574  de numerical met
-0000d080: 6164 6174 6120 6c61 7965 7273 2c20 6465  adata layers, de
-0000d090: 6661 756c 7473 2074 6f20 5472 7565 0d0a  faults to True..
-0000d0a0: 2020 2020 2020 2020 3a74 7970 6520 696e          :type in
-0000d0b0: 636c 7564 655f 6e75 6d65 7269 6361 6c3a  clude_numerical:
-0000d0c0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
-0000d0d0: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
-0000d0e0: 2056 616c 7565 4572 726f 723a 2045 7272   ValueError: Err
-0000d0f0: 6f72 2069 6620 6d65 7461 6461 7461 2074  or if metadata t
-0000d100: 7970 6573 2061 7265 206e 6f74 2072 6563  ypes are not rec
-0000d110: 6f67 6e69 7a65 640d 0a20 2020 2020 2020  ognized..       
-0000d120: 203a 7265 7475 726e 3a20 6f62 7365 7276   :return: observ
-0000d130: 6174 696f 6e73 20c3 9720 6d65 7461 6461  ations .. metada
-0000d140: 7461 206d 6174 7269 780d 0a20 2020 2020  ta matrix..     
-0000d150: 2020 203a 7274 7970 653a 2070 642e 4461     :rtype: pd.Da
-0000d160: 7461 4672 616d 650d 0a20 2020 2020 2020  taFrame..       
-0000d170: 2022 2222 0d0a 2020 2020 2020 2020 6474   """..        dt
-0000d180: 7970 6573 203d 205b 5d0d 0a20 2020 2020  ypes = []..     
-0000d190: 2020 2069 6620 696e 636c 7564 655f 6361     if include_ca
-0000d1a0: 7465 676f 7269 6361 6c3a 0d0a 2020 2020  tegorical:..    
-0000d1b0: 2020 2020 2020 2020 6474 7970 6573 2e61          dtypes.a
-0000d1c0: 7070 656e 6428 2263 6174 6567 6f72 7922  ppend("category"
-0000d1d0: 290d 0a20 2020 2020 2020 2069 6620 696e  )..        if in
-0000d1e0: 636c 7564 655f 6e75 6d65 7269 6361 6c3a  clude_numerical:
-0000d1f0: 0d0a 2020 2020 2020 2020 2020 2020 6474  ..            dt
-0000d200: 7970 6573 202b 3d20 5b22 666c 6f61 7422  ypes += ["float"
-0000d210: 2c20 2269 6e74 225d 0d0a 2020 2020 2020  , "int"]..      
-0000d220: 2020 756e 6578 706c 6169 6e65 645f 636f    unexplained_co
-0000d230: 6c73 203d 2073 656c 662e 6164 6174 612e  ls = self.adata.
-0000d240: 6f62 732e 7365 6c65 6374 5f64 7479 7065  obs.select_dtype
-0000d250: 7328 6578 636c 7564 653d 2822 6361 7465  s(exclude=("cate
-0000d260: 676f 7279 222c 2022 666c 6f61 7422 2c20  gory", "float", 
-0000d270: 2269 6e74 2229 292e 636f 6c75 6d6e 730d  "int")).columns.
-0000d280: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0000d290: 756e 6578 706c 6169 6e65 645f 636f 6c73  unexplained_cols
-0000d2a0: 2920 3e20 303a 0d0a 2020 2020 2020 2020  ) > 0:..        
-0000d2b0: 2020 2020 756e 6578 706c 6169 6e65 645f      unexplained_
-0000d2c0: 636f 6c5f 7374 7220 3d20 222c 2022 2e6a  col_str = ", ".j
-0000d2d0: 6f69 6e28 756e 6578 706c 6169 6e65 645f  oin(unexplained_
-0000d2e0: 636f 6c73 290d 0a20 2020 2020 2020 2020  cols)..         
-0000d2f0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000d300: 726f 7228 6622 7b75 6e65 7870 6c61 696e  ror(f"{unexplain
-0000d310: 6564 5f63 6f6c 5f73 7472 7d20 6d65 7461  ed_col_str} meta
-0000d320: 6461 7461 2063 6f6c 756d 6e73 2068 6176  data columns hav
-0000d330: 6520 756e 7265 636f 676e 697a 6564 2064  e unrecognized d
-0000d340: 7479 7065 732e 2229 0d0a 2020 2020 2020  types.")..      
-0000d350: 2020 6466 203d 2073 656c 662e 6164 6174    df = self.adat
-0000d360: 612e 6f62 732e 7365 6c65 6374 5f64 7479  a.obs.select_dty
-0000d370: 7065 7328 696e 636c 7564 653d 6474 7970  pes(include=dtyp
-0000d380: 6573 290d 0a20 2020 2020 2020 2064 6620  es)..        df 
-0000d390: 3d20 6466 2e64 726f 706e 6128 6178 6973  = df.dropna(axis
-0000d3a0: 3d31 2c20 686f 773d 2261 6c6c 2229 0d0a  =1, how="all")..
-0000d3b0: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
-0000d3c0: 7265 706c 6163 6528 226e 616e 222c 206e  replace("nan", n
-0000d3d0: 702e 4e61 4e29 2020 2354 4f44 4f3a 2041  p.NaN)  #TODO: A
-0000d3e0: 6464 7265 7373 2065 7272 6f72 3a20 2f68  ddress error: /h
-0000d3f0: 6f6d 652f 7462 7665 7268 6579 2f6d 696e  ome/tbverhey/min
-0000d400: 6963 6f6e 6461 332f 656e 7673 2f6d 6f73  iconda3/envs/mos
-0000d410: 6169 636d 7069 2f6c 6962 2f70 7974 686f  aicmpi/lib/pytho
-0000d420: 6e33 2e31 312f 7369 7465 2d70 6163 6b61  n3.11/site-packa
-0000d430: 6765 732f 6d6f 7361 6963 6d70 692f 6461  ges/mosaicmpi/da
-0000d440: 7461 7365 742e 7079 3a31 3032 313a 2046  taset.py:1021: F
-0000d450: 7574 7572 6557 6172 6e69 6e67 3a20 5468  utureWarning: Th
-0000d460: 6520 6265 6861 7669 6f72 206f 6620 5365  e behavior of Se
-0000d470: 7269 6573 2e72 6570 6c61 6365 2028 616e  ries.replace (an
-0000d480: 6420 4461 7461 4672 616d 652e 7265 706c  d DataFrame.repl
-0000d490: 6163 6529 2077 6974 6820 4361 7465 676f  ace) with Catego
-0000d4a0: 7269 6361 6c44 7479 7065 2069 7320 6465  ricalDtype is de
-0000d4b0: 7072 6563 6174 6564 2e20 496e 2061 2066  precated. In a f
-0000d4c0: 7574 7572 6520 7665 7273 696f 6e2c 2072  uture version, r
-0000d4d0: 6570 6c61 6365 2077 696c 6c20 6f6e 6c79  eplace will only
-0000d4e0: 2062 6520 7573 6564 2066 6f72 2063 6173   be used for cas
-0000d4f0: 6573 2074 6861 7420 7072 6573 6572 7665  es that preserve
-0000d500: 2074 6865 2063 6174 6567 6f72 6965 732e   the categories.
-0000d510: 2054 6f20 6368 616e 6765 2074 6865 2063   To change the c
-0000d520: 6174 6567 6f72 6965 732c 2075 7365 2073  ategories, use s
-0000d530: 6572 2e63 6174 2e72 656e 616d 655f 6361  er.cat.rename_ca
-0000d540: 7465 676f 7269 6573 2069 6e73 7465 6164  tegories instead
-0000d550: 2e0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-0000d560: 6e20 6466 0d0a 2020 2020 0d0a 2020 2020  n df..    ..    
-0000d570: 6465 6620 6765 745f 6361 7465 676f 7279  def get_category
-0000d580: 5f6f 7665 7272 6570 7265 7365 6e74 6174  _overrepresentat
-0000d590: 696f 6e28 7365 6c66 2c0d 0a20 2020 2020  ion(self,..     
-0000d5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5c0: 2020 206c 6179 6572 3a20 7374 722c 0d0a     layer: str,..
-0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5f0: 2020 2020 2020 2020 7472 756e 6361 7465          truncate
-0000d600: 5f6e 6567 6174 6976 653a 2062 6f6f 6c20  _negative: bool 
-0000d610: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
-0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d640: 2073 7562 7365 745f 6361 7465 676f 7269   subset_categori
-0000d650: 6573 3a20 436f 6c6c 6563 7469 6f6e 5b73  es: Collection[s
-0000d660: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
-0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d690: 2020 2020 2920 2d3e 2070 642e 4461 7461      ) -> pd.Data
-0000d6a0: 4672 616d 653a 0d0a 2020 2020 2020 2020  Frame:..        
-0000d6b0: 2222 2243 616c 6375 6c61 7465 2050 6561  """Calculate Pea
-0000d6c0: 7273 6f6e 2072 6573 6964 7561 6c20 6f66  rson residual of
-0000d6d0: 2063 6869 2d73 7175 6172 6564 2074 6573   chi-squared tes
-0000d6e0: 742c 2061 7373 6f63 6961 7469 6e67 2070  t, associating p
-0000d6f0: 726f 6772 616d 7320 666f 7220 6561 6368  rograms for each
-0000d700: 2072 616e 6b20 286b 2920 746f 2063 6174   rank (k) to cat
-0000d710: 6567 6f72 6965 7320 6f66 2073 616d 706c  egories of sampl
-0000d720: 6573 2f6f 6273 6572 7661 7469 6f6e 732e  es/observations.
-0000d730: 2042 7920 6465 6661 756c 742c 2074 7275   By default, tru
-0000d740: 6e63 6174 6573 206e 6567 6174 6976 6520  ncates negative 
-0000d750: 7661 6c75 6573 2e0d 0a0d 0a20 2020 2020  values.....     
-0000d760: 2020 203a 7061 7261 6d20 6c61 7965 723a     :param layer:
-0000d770: 206e 616d 6520 6f66 2063 6174 6567 6f72   name of categor
-0000d780: 6963 616c 2064 6174 6120 6c61 7965 720d  ical data layer.
-0000d790: 0a20 2020 2020 2020 203a 7479 7065 206c  .        :type l
-0000d7a0: 6179 6572 3a20 7374 720d 0a20 2020 2020  ayer: str..     
-0000d7b0: 2020 203a 7061 7261 6d20 7472 756e 6361     :param trunca
-0000d7c0: 7465 5f6e 6567 6174 6976 653a 2054 7275  te_negative: Tru
-0000d7d0: 6e63 6174 6520 6e65 6761 7469 7665 2072  ncate negative r
-0000d7e0: 6573 6964 7561 6c73 2074 6f20 302c 2064  esiduals to 0, d
-0000d7f0: 6566 6175 6c74 7320 746f 2054 7275 650d  efaults to True.
-0000d800: 0a20 2020 2020 2020 203a 7479 7065 2074  .        :type t
-0000d810: 7275 6e63 6174 655f 6e65 6761 7469 7665  runcate_negative
-0000d820: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
-0000d830: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000d840: 2073 7562 7365 745f 6361 7465 676f 7269   subset_categori
-0000d850: 6573 3a20 5072 6f76 6964 6520 6120 7375  es: Provide a su
-0000d860: 6273 6574 206f 6620 6361 7465 676f 7269  bset of categori
-0000d870: 6573 2066 6f72 2063 616c 6375 6c61 7469  es for calculati
-0000d880: 6e67 206f 7665 7272 6570 7265 7365 6e74  ng overrepresent
-0000d890: 6174 696f 6e0d 0a20 2020 2020 2020 203a  ation..        :
-0000d8a0: 7479 7065 2073 7562 7365 745f 6361 7465  type subset_cate
-0000d8b0: 676f 7269 6573 3a20 436f 6c6c 6563 7469  gories: Collecti
-0000d8c0: 6f6e 5b73 7472 5d0d 0a20 2020 2020 2020  on[str]..       
-0000d8d0: 203a 7265 7475 726e 3a20 6361 7465 676f   :return: catego
-0000d8e0: 7279 20c3 9720 7072 6f67 7261 6d20 6d61  ry .. program ma
-0000d8f0: 7472 6978 206f 6620 6f76 6572 7265 7072  trix of overrepr
-0000d900: 6573 656e 7461 7469 6f6e 2076 616c 7565  esentation value
-0000d910: 730d 0a20 2020 2020 2020 203a 7274 7970  s..        :rtyp
-0000d920: 653a 2070 642e 4461 7461 4672 616d 650d  e: pd.DataFrame.
-0000d930: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-0000d940: 2020 2020 2020 7573 6167 6520 3d20 7365        usage = se
-0000d950: 6c66 2e67 6574 5f75 7361 6765 7328 6e6f  lf.get_usages(no
-0000d960: 726d 616c 697a 653d 5472 7565 292e 636f  rmalize=True).co
-0000d970: 7079 2829 0d0a 2020 2020 2020 2020 7361  py()..        sa
-0000d980: 6d70 6c65 5f74 6f5f 636c 6173 7320 3d20  mple_to_class = 
-0000d990: 7365 6c66 2e67 6574 5f6d 6574 6164 6174  self.get_metadat
-0000d9a0: 615f 6466 2829 5b6c 6179 6572 5d0d 0a20  a_df()[layer].. 
-0000d9b0: 2020 2020 2020 2069 6620 7375 6273 6574         if subset
-0000d9c0: 5f63 6174 6567 6f72 6965 7320 6973 206e  _categories is n
-0000d9d0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000d9e0: 2020 2020 2020 7361 6d70 6c65 5f74 6f5f        sample_to_
-0000d9f0: 636c 6173 735b 7e73 616d 706c 655f 746f  class[~sample_to
-0000da00: 5f63 6c61 7373 2e69 7369 6e28 7375 6273  _class.isin(subs
-0000da10: 6574 5f63 6174 6567 6f72 6965 7329 5d20  et_categories)] 
-0000da20: 3d20 6e70 2e4e 614e 0d0a 2020 2020 2020  = np.NaN..      
-0000da30: 2020 7573 6167 652e 696e 6465 7820 3d20    usage.index = 
-0000da40: 7573 6167 652e 696e 6465 782e 6d61 7028  usage.index.map(
-0000da50: 7361 6d70 6c65 5f74 6f5f 636c 6173 7329  sample_to_class)
-0000da60: 0d0a 2020 2020 2020 2020 6f62 7365 7276  ..        observ
-0000da70: 6564 203d 2075 7361 6765 2e67 726f 7570  ed = usage.group
-0000da80: 6279 286c 6576 656c 3d30 2c20 6f62 7365  by(level=0, obse
-0000da90: 7276 6564 3d54 7275 6529 2e73 756d 2829  rved=True).sum()
-0000daa0: 0d0a 2020 2020 2020 2020 6f62 7365 7276  ..        observ
-0000dab0: 6564 203d 206f 6273 6572 7665 645b 6f62  ed = observed[ob
-0000dac0: 7365 7276 6564 2e73 756d 2861 7869 733d  served.sum(axis=
-0000dad0: 3129 203e 2030 5d0d 0a20 2020 2020 2020  1) > 0]..       
-0000dae0: 206e 5f63 6174 6567 6f72 6965 7320 3d20   n_categories = 
-0000daf0: 6f62 7365 7276 6564 2e73 6861 7065 5b30  observed.shape[0
-0000db00: 5d0d 0a20 2020 2020 2020 2069 6620 6e5f  ]..        if n_
-0000db10: 6361 7465 676f 7269 6573 203c 2032 3a0d  categories < 2:.
-0000db20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000db30: 6c61 7965 7220 213d 2022 6876 675f 616c  layer != "hvg_al
-0000db40: 6c5f 3022 3a0d 0a20 2020 2020 2020 2020  l_0":..         
-0000db50: 2020 2020 2020 206c 6f67 6769 6e67 2e77         logging.w
-0000db60: 6172 6e69 6e67 2866 224f 7665 7272 6570  arning(f"Overrep
-0000db70: 7265 7365 6e74 6174 696f 6e20 636f 756c  resentation coul
-0000db80: 6420 6e6f 7420 6265 2063 616c 6375 6c61  d not be calcula
-0000db90: 7465 6420 666f 7220 6c61 7965 7220 277b  ted for layer '{
-0000dba0: 6c61 7965 727d 272c 2061 7320 6f6e 6c79  layer}', as only
-0000dbb0: 207b 6e5f 6361 7465 676f 7269 6573 7d20   {n_categories} 
-0000dbc0: 6361 7465 676f 7269 6573 2077 6572 6520  categories were 
-0000dbd0: 666f 756e 6420 696e 2074 6865 2064 6174  found in the dat
-0000dbe0: 612e 2022 0d0a 2020 2020 2020 2020 2020  a. "..          
-0000dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc00: 2020 2020 2020 6622 4e6f 7465 2074 6861        f"Note tha
-0000dc10: 7420 656d 7074 7920 7661 6c75 6573 2069  t empty values i
-0000dc20: 6e20 7468 6520 6d65 7461 6461 7461 2061  n the metadata a
-0000dc30: 7265 206e 6f74 2063 6f6e 7369 6465 7265  re not considere
-0000dc40: 6420 6120 6361 7465 676f 7279 2e20 220d  d a category. ".
-0000dc50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc70: 2066 224f 7665 7272 6570 7265 7365 6e74   f"Overrepresent
-0000dc80: 6174 696f 6e20 6361 6e6e 6f74 2062 6520  ation cannot be 
-0000dc90: 6361 6c63 756c 6174 6564 2077 6974 6820  calculated with 
-0000dca0: 6665 7765 7220 7468 616e 2032 2063 6174  fewer than 2 cat
-0000dcb0: 6567 6f72 6965 7320 666f 7220 6561 6368  egories for each
-0000dcc0: 206c 6179 6572 2e20 2229 0d0a 2020 2020   layer. ")..    
-0000dcd0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-0000dce0: 642e 4461 7461 4672 616d 6528 6e70 2e4e  d.DataFrame(np.N
-0000dcf0: 614e 2c20 696e 6465 7820 3d20 6f62 7365  aN, index = obse
-0000dd00: 7276 6564 2e69 6e64 6578 2c20 636f 6c75  rved.index, colu
-0000dd10: 6d6e 733d 6f62 7365 7276 6564 2e63 6f6c  mns=observed.col
-0000dd20: 756d 6e73 290d 0a20 2020 2020 2020 2065  umns)..        e
-0000dd30: 7870 6563 7465 6420 3d20 5b5d 0d0a 2020  xpected = []..  
-0000dd40: 2020 2020 2020 666f 7220 6b2c 206f 6273        for k, obs
-0000dd50: 5f6b 2069 6e20 6f62 7365 7276 6564 2e54  _k in observed.T
-0000dd60: 2e67 726f 7570 6279 286c 6576 656c 3d31  .groupby(level=1
-0000dd70: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000dd80: 6578 705f 6b20 3d20 7064 2e44 6174 6146  exp_k = pd.DataF
-0000dd90: 7261 6d65 286f 6273 5f6b 2e73 756d 2861  rame(obs_k.sum(a
-0000dda0: 7869 733d 3129 2920 4020 7064 2e44 6174  xis=1)) @ pd.Dat
-0000ddb0: 6146 7261 6d65 286f 6273 5f6b 2e73 756d  aFrame(obs_k.sum
-0000ddc0: 2861 7869 733d 3029 292e 5420 2f20 6f62  (axis=0)).T / ob
-0000ddd0: 735f 6b2e 7375 6d28 292e 7375 6d28 290d  s_k.sum().sum().
-0000dde0: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-0000ddf0: 6563 7465 642e 6170 7065 6e64 2865 7870  ected.append(exp
-0000de00: 5f6b 290d 0a20 2020 2020 2020 2065 7870  _k)..        exp
-0000de10: 6563 7465 6420 3d20 7064 2e63 6f6e 6361  ected = pd.conca
-0000de20: 7428 6578 7065 6374 6564 292e 540d 0a20  t(expected).T.. 
-0000de30: 2020 2020 2020 2063 6869 7371 5f72 6573         chisq_res
-0000de40: 6964 203d 2028 6f62 7365 7276 6564 202d  id = (observed -
-0000de50: 2065 7870 6563 7465 6429 202f 206e 702e   expected) / np.
-0000de60: 7371 7274 2865 7870 6563 7465 6429 2020  sqrt(expected)  
-0000de70: 2320 7065 6172 736f 6e20 7265 7369 6475  # pearson residu
-0000de80: 616c 206f 6620 6368 692d 7371 7561 7265  al of chi-square
-0000de90: 6420 7465 7374 206f 6620 636f 6e74 696e  d test of contin
-0000dea0: 6765 6e63 7920 7461 626c 650d 0a20 2020  gency table..   
-0000deb0: 2020 2020 2069 6620 7472 756e 6361 7465       if truncate
-0000dec0: 5f6e 6567 6174 6976 653a 0d0a 2020 2020  _negative:..    
-0000ded0: 2020 2020 2020 2020 6368 6973 715f 7265          chisq_re
-0000dee0: 7369 6420 3d20 6368 6973 715f 7265 7369  sid = chisq_resi
-0000def0: 642e 636c 6970 286c 6f77 6572 3d30 290d  d.clip(lower=0).
-0000df00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000df10: 6368 6973 715f 7265 7369 640d 0a20 2020  chisq_resid..   
-0000df20: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-0000df30: 2064 6566 2067 6574 5f6d 6574 6164 6174   def get_metadat
-0000df40: 615f 636f 7272 656c 6174 696f 6e28 7365  a_correlation(se
-0000df50: 6c66 2c20 0d0a 2020 2020 2020 2020 2020  lf, ..          
-0000df60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df70: 2020 2020 2020 206c 6179 6572 3a20 7374         layer: st
-0000df80: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-0000df90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfa0: 2020 2020 206d 6574 686f 643a 2073 7472       method: str
-0000dfb0: 203d 2022 7065 6172 736f 6e22 0d0a 2020   = "pearson"..  
-0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfd0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000dfe0: 202d 3e20 7064 2e53 6572 6965 733a 0d0a   -> pd.Series:..
-0000dff0: 2020 2020 2020 2020 2222 2243 616c 6375          """Calcu
-0000e000: 6c61 7465 2050 6561 7273 6f6e 2063 6f72  late Pearson cor
-0000e010: 7265 6c61 7469 6f6e 206f 6620 4745 5020  relation of GEP 
-0000e020: 7573 6167 6520 746f 206e 756d 6572 6963  usage to numeric
-0000e030: 616c 206d 6574 6164 6174 6120 6163 726f  al metadata acro
-0000e040: 7373 2073 616d 706c 6573 2f6f 6273 6572  ss samples/obser
-0000e050: 7661 7469 6f6e 732e 0d0a 0d0a 2020 2020  vations.....    
-0000e060: 2020 2020 3a70 6172 616d 206c 6179 6572      :param layer
-0000e070: 3a20 6e61 6d65 206f 6620 6e75 6d65 7269  : name of numeri
-0000e080: 6361 6c20 6461 7461 206c 6179 6572 0d0a  cal data layer..
-0000e090: 2020 2020 2020 2020 3a74 7970 6520 6c61          :type la
-0000e0a0: 7965 723a 2073 7472 0d0a 2020 2020 2020  yer: str..      
-0000e0b0: 2020 3a70 6172 616d 206d 6574 686f 643a    :param method:
-0000e0c0: 2043 6f72 7265 6c61 7469 6f6e 206d 6574   Correlation met
-0000e0d0: 686f 643a 2022 7065 6172 736f 6e22 2c20  hod: "pearson", 
-0000e0e0: 2273 7065 6172 6d61 6e22 2c20 6f72 2022  "spearman", or "
-0000e0f0: 6b65 6e64 616c 6c22 2e20 4465 6661 756c  kendall". Defaul
-0000e100: 7473 2074 6f20 2270 6561 7273 6f6e 220d  ts to "pearson".
-0000e110: 0a20 2020 2020 2020 203a 7479 7065 206d  .        :type m
-0000e120: 6574 686f 643a 2073 7472 2c20 6f70 7469  ethod: str, opti
-0000e130: 6f6e 616c 0d0a 2020 2020 2020 2020 3a72  onal..        :r
-0000e140: 6574 7572 6e3a 2063 6f72 7265 6c61 7469  eturn: correlati
-0000e150: 6f6e 206f 6620 4745 5020 746f 206d 6574  on of GEP to met
-0000e160: 6164 6174 610d 0a20 2020 2020 2020 203a  adata..        :
-0000e170: 7274 7970 653a 2070 642e 5365 7269 6573  rtype: pd.Series
-0000e180: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-0000e190: 2020 2020 2020 2075 7361 6765 203d 2073         usage = s
-0000e1a0: 656c 662e 6765 745f 7573 6167 6573 2829  elf.get_usages()
-0000e1b0: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-0000e1c0: 206d 6574 6164 6174 6120 3d20 7365 6c66   metadata = self
-0000e1d0: 2e67 6574 5f6d 6574 6164 6174 615f 6466  .get_metadata_df
-0000e1e0: 2829 5b6c 6179 6572 5d0d 0a20 2020 2020  ()[layer]..     
-0000e1f0: 2020 206d 645f 636f 7272 203d 2075 7361     md_corr = usa
-0000e200: 6765 2e63 6f72 7277 6974 6828 6d65 7461  ge.corrwith(meta
-0000e210: 6461 7461 2c20 6d65 7468 6f64 3d6d 6574  data, method=met
-0000e220: 686f 6429 0d0a 2020 2020 2020 2020 7265  hod)..        re
-0000e230: 7475 726e 206d 645f 636f 7272 0d0a 2020  turn md_corr..  
-0000e240: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
-0000e250: 6170 7065 6e64 5f74 6f5f 6869 7374 6f72  append_to_histor
-0000e260: 7928 7365 6c66 2c20 656e 7472 7929 3a0d  y(self, entry):.
-0000e270: 0a20 2020 2020 2020 2022 2222 4164 6420  .        """Add 
-0000e280: 656e 7472 7920 746f 2044 6174 6173 6574  entry to Dataset
-0000e290: 2068 6973 746f 7279 2e0d 0a0d 0a20 2020   history.....   
-0000e2a0: 2020 2020 203a 7061 7261 6d20 656e 7472       :param entr
-0000e2b0: 793a 2044 6573 6372 6970 7469 6f6e 206f  y: Description o
-0000e2c0: 6620 6576 656e 7420 746f 2072 6563 6f72  f event to recor
-0000e2d0: 6420 696e 2074 6865 2068 6973 746f 7279  d in the history
-0000e2e0: 2e0d 0a20 2020 2020 2020 203a 7479 7065  ...        :type
-0000e2f0: 2065 6e74 7279 3a20 7374 720d 0a20 2020   entry: str..   
-0000e300: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-0000e310: 2020 7365 6c66 2e61 6461 7461 2e75 6e73    self.adata.uns
-0000e320: 5b22 6869 7374 6f72 7922 5d5b 6461 7465  ["history"][date
-0000e330: 7469 6d65 2e75 7463 6e6f 7728 292e 6973  time.utcnow().is
-0000e340: 6f66 6f72 6d61 7428 295d 203d 2065 6e74  oformat()] = ent
-0000e350: 7279 0d0a 2020 2020 2020 2020 0d0a 2020  ry..        ..  
-0000e360: 2020 6465 6620 6765 745f 6869 7374 6f72    def get_histor
-0000e370: 7928 7365 6c66 293a 0d0a 2020 2020 2020  y(self):..      
-0000e380: 2020 2222 2252 6574 7572 6e73 2074 696d    """Returns tim
-0000e390: 6573 7461 6d70 6564 2068 6973 746f 7279  estamped history
-0000e3a0: 206f 6620 4461 7461 7365 7420 6f62 6a65   of Dataset obje
-0000e3b0: 6374 2e0d 0a0d 0a20 2020 2020 2020 203a  ct.....        :
-0000e3c0: 7265 7475 726e 3a20 6869 7374 6f72 790d  return: history.
-0000e3d0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-0000e3e0: 2064 6963 740d 0a20 2020 2020 2020 2022   dict..        "
-0000e3f0: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-0000e400: 726e 2073 656c 662e 6164 6174 612e 756e  rn self.adata.un
-0000e410: 735b 2268 6973 746f 7279 225d            s["history"]
+0000cf70: 2020 7072 6f67 7261 6d5f 7479 7065 3a20    program_type: 
+0000cf80: 4c69 7465 7261 6c5b 2263 6e6d 665f 6765  Literal["cnmf_ge
+0000cf90: 705f 7470 6d22 2c20 2263 6e6d 665f 6765  p_tpm", "cnmf_ge
+0000cfa0: 705f 7261 7722 5d20 3d20 2263 6e6d 665f  p_raw"] = "cnmf_
+0000cfb0: 6765 705f 7470 6d22 0d0a 2020 2020 2020  gep_tpm"..      
+0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfd0: 2020 2029 202d 3e20 7064 2e44 6174 6146     ) -> pd.DataF
+0000cfe0: 7261 6d65 3a0d 0a20 2020 2020 2020 2022  rame:..        "
+0000cff0: 2222 5265 7475 726e 2074 6865 2061 7070  ""Return the app
+0000d000: 726f 7869 6d61 7465 6420 6461 7461 2062  roximated data b
+0000d010: 7920 6d75 6c74 6970 6c79 696e 6720 7468  y multiplying th
+0000d020: 6520 7072 6f67 7261 6d73 2061 6e64 2075  e programs and u
+0000d030: 7361 6765 206d 6174 7269 6365 7320 666f  sage matrices fo
+0000d040: 7220 6120 6769 7665 6e20 7261 6e6b 2028  r a given rank (
+0000d050: 6b29 2e20 4465 6661 756c 7473 2074 6f20  k). Defaults to 
+0000d060: 7468 6520 6869 6768 6573 7420 7261 6e6b  the highest rank
+0000d070: 2061 7661 696c 6162 6c65 2e0d 0a0d 0a20   available..... 
+0000d080: 2020 2020 2020 203a 7061 7261 6d20 6b3a         :param k:
+0000d090: 2072 616e 6b2c 2064 6566 6175 6c74 7320   rank, defaults 
+0000d0a0: 746f 204e 6f6e 650d 0a20 2020 2020 2020  to None..       
+0000d0b0: 203a 7479 7065 206b 3a20 696e 742c 206f   :type k: int, o
+0000d0c0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+0000d0d0: 203a 7265 7475 726e 3a20 4170 7072 6f78   :return: Approx
+0000d0e0: 696d 6174 696f 6e20 6f66 2064 6174 6173  imation of datas
+0000d0f0: 6574 2062 6173 6564 206f 6e20 7072 6f67  et based on prog
+0000d100: 7261 6d73 2061 6e64 2075 7361 6765 730d  rams and usages.
+0000d110: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+0000d120: 2070 642e 4461 7461 4672 616d 650d 0a20   pd.DataFrame.. 
+0000d130: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0000d140: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
+0000d150: 6861 735f 636e 6d66 5f72 6573 756c 7473  has_cnmf_results
+0000d160: 0d0a 2020 2020 2020 2020 6966 206b 2069  ..        if k i
+0000d170: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+0000d180: 2020 2020 206b 203d 2073 656c 662e 6164       k = self.ad
+0000d190: 6174 612e 756e 735b 226b 7661 6c73 225d  ata.uns["kvals"]
+0000d1a0: 2e69 6e64 6578 2e6d 6178 2829 0d0a 2020  .index.max()..  
+0000d1b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000d1c0: 6170 7072 6f78 696d 6174 696f 6e20 3d20  approximation = 
+0000d1d0: 2873 656c 662e 6765 745f 7573 6167 6573  (self.get_usages
+0000d1e0: 286b 3d6b 2920 2040 2073 656c 662e 6765  (k=k)  @ self.ge
+0000d1f0: 745f 7072 6f67 7261 6d73 2874 7970 653d  t_programs(type=
+0000d200: 7072 6f67 7261 6d5f 7479 7065 2c20 6b3d  program_type, k=
+0000d210: 6b29 2e54 290d 0a0d 0a20 2020 2020 2020  k).T)....       
+0000d220: 2072 6574 7572 6e20 6170 7072 6f78 696d   return approxim
+0000d230: 6174 696f 6e0d 0a20 2020 2020 2020 200d  ation..        .
+0000d240: 0a20 2020 2064 6566 2063 616c 6375 6c61  .    def calcula
+0000d250: 7465 5f63 6e6d 665f 7072 6564 6963 7469  te_cnmf_predicti
+0000d260: 6f6e 5f65 7272 6f72 2873 656c 662c 0d0a  on_error(self,..
+0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d290: 2020 2020 2020 206b 3a20 4f70 7469 6f6e         k: Option
+0000d2a0: 616c 5b55 6e69 6f6e 5b69 6e74 2c20 4974  al[Union[int, It
+0000d2b0: 6572 6162 6c65 5d5d 203d 204e 6f6e 6529  erable]] = None)
+0000d2c0: 3a0d 0a20 2020 2020 2020 200d 0a0d 0a20  :..        .... 
+0000d2d0: 2020 2020 2020 2066 726f 6d20 736b 6c65         from skle
+0000d2e0: 6172 6e2e 6465 636f 6d70 6f73 6974 696f  arn.decompositio
+0000d2f0: 6e20 696d 706f 7274 206e 6f6e 5f6e 6567  n import non_neg
+0000d300: 6174 6976 655f 6661 6374 6f72 697a 6174  ative_factorizat
+0000d310: 696f 6e0d 0a0d 0a0d 0a20 2020 2020 2020  ion......       
+0000d320: 2069 6620 6b20 6973 204e 6f6e 653a 0d0a   if k is None:..
+0000d330: 2020 2020 2020 2020 2020 2020 6b76 616c              kval
+0000d340: 7320 3d20 7365 6c66 2e61 6461 7461 2e75  s = self.adata.u
+0000d350: 6e73 5b22 6b76 616c 7322 5d2e 696e 6465  ns["kvals"].inde
+0000d360: 780d 0a20 2020 2020 2020 2065 6c69 6620  x..        elif 
+0000d370: 6973 696e 7374 616e 6365 286b 2c20 4974  isinstance(k, It
+0000d380: 6572 6162 6c65 293a 0d0a 2020 2020 2020  erable):..      
+0000d390: 2020 2020 2020 6b76 616c 7320 3d20 6b0d        kvals = k.
+0000d3a0: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+0000d3b0: 696e 7374 616e 6365 286b 2c20 2869 6e74  instance(k, (int
+0000d3c0: 2c20 6e70 2e69 6e74 6567 6572 2929 3a0d  , np.integer)):.
+0000d3d0: 0a20 2020 2020 2020 2020 2020 206b 7661  .            kva
+0000d3e0: 6c73 203d 205b 6b5d 0d0a 2020 2020 2020  ls = [k]..      
+0000d3f0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0000d400: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0000d410: 4572 726f 720d 0a20 2020 2020 2020 200d  Error..        .
+0000d420: 0a20 2020 2020 2020 206e 6f72 6d5f 636f  .        norm_co
+0000d430: 756e 7473 203d 2073 656c 662e 6164 6174  unts = self.adat
+0000d440: 612e 746f 5f64 6628 292e 6c6f 635b 3a2c  a.to_df().loc[:,
+0000d450: 2073 656c 662e 6164 6174 612e 7661 725b   self.adata.var[
+0000d460: 2273 656c 6563 7465 6422 5d5d 0d0a 2020  "selected"]]..  
+0000d470: 2020 2020 2020 6e6f 726d 5f63 6f75 6e74        norm_count
+0000d480: 7320 2f3d 206e 6f72 6d5f 636f 756e 7473  s /= norm_counts
+0000d490: 2e73 7464 2861 7869 733d 302c 2064 646f  .std(axis=0, ddo
+0000d4a0: 663d 3129 0d0a 0d0a 2020 2020 2020 2020  f=1)....        
+0000d4b0: 7072 6564 5f65 7272 6f72 203d 2070 642e  pred_error = pd.
+0000d4c0: 5365 7269 6573 2869 6e64 6578 3d6b 7661  Series(index=kva
+0000d4d0: 6c73 2c20 6e61 6d65 3d22 634e 4d46 2070  ls, name="cNMF p
+0000d4e0: 7265 6469 6374 696f 6e5f 6572 726f 7222  rediction_error"
+0000d4f0: 290d 0a20 2020 2020 2020 2066 6f72 206b  )..        for k
+0000d500: 7661 6c20 696e 206b 7661 6c73 3a0d 0a20  val in kvals:.. 
+0000d510: 2020 2020 2020 2020 2020 2023 206f 6274             # obt
+0000d520: 6169 6e20 7265 636f 6e73 7472 7563 7465  ain reconstructe
+0000d530: 6420 6e6f 726d 616c 697a 6564 2063 6f75  d normalized cou
+0000d540: 6e74 7320 6d61 7472 6978 2062 7920 7265  nts matrix by re
+0000d550: 2d66 6974 7469 6e67 2075 7361 6765 2061  -fitting usage a
+0000d560: 6e64 2063 6f6d 7075 7469 6e67 2064 6f74  nd computing dot
+0000d570: 2070 726f 6475 6374 3a20 7573 6167 652e   product: usage.
+0000d580: 646f 7428 7370 6563 7472 6129 0d0a 2020  dot(spectra)..  
+0000d590: 2020 2020 2020 2020 2020 6d65 6469 616e            median
+0000d5a0: 5f73 7065 6374 7261 203d 2073 656c 662e  _spectra = self.
+0000d5b0: 6765 745f 7072 6f67 7261 6d73 286b 3d6b  get_programs(k=k
+0000d5c0: 7661 6c2c 2074 7970 653d 2263 6e6d 665f  val, type="cnmf_
+0000d5d0: 6765 705f 7261 7722 292e 6472 6f70 6e61  gep_raw").dropna
+0000d5e0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+0000d5f0: 7266 5f75 7361 6765 732c 2072 665f 7370  rf_usages, rf_sp
+0000d600: 6563 7472 612c 206e 6974 6572 203d 206e  ectra, niter = n
+0000d610: 6f6e 5f6e 6567 6174 6976 655f 6661 6374  on_negative_fact
+0000d620: 6f72 697a 6174 696f 6e28 583d 6e6f 726d  orization(X=norm
+0000d630: 5f63 6f75 6e74 732e 7661 6c75 6573 2c0d  _counts.values,.
+0000d640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d670: 2020 2020 2061 6c70 6861 5f48 3d30 2e30       alpha_H=0.0
+0000d680: 2c20 616c 7068 615f 573d 302e 302c 2062  , alpha_W=0.0, b
+0000d690: 6574 615f 6c6f 7373 3d22 6b75 6c6c 6261  eta_loss="kullba
+0000d6a0: 636b 2d6c 6569 626c 6572 222c 2069 6e69  ck-leibler", ini
+0000d6b0: 743d 2272 616e 646f 6d22 2c0d 0a20 2020  t="random",..   
+0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6f0: 206c 315f 7261 7469 6f3d 302e 302c 206d   l1_ratio=0.0, m
+0000d700: 6178 5f69 7465 723d 3130 3030 2c20 736f  ax_iter=1000, so
+0000d710: 6c76 6572 3d22 6d75 222c 2074 6f6c 3d30  lver="mu", tol=0
+0000d720: 2e30 3030 312c 206e 5f63 6f6d 706f 6e65  .0001, n_compone
+0000d730: 6e74 733d 6b76 616c 2c20 483d 6d65 6469  nts=kval, H=medi
+0000d740: 616e 5f73 7065 6374 7261 2e54 2e76 616c  an_spectra.T.val
+0000d750: 7565 732c 2075 7064 6174 655f 483d 4661  ues, update_H=Fa
+0000d760: 6c73 6529 0d0a 0d0a 2020 2020 2020 2020  lse)....        
+0000d770: 2020 2020 7266 5f75 7361 6765 7320 3d20      rf_usages = 
+0000d780: 7064 2e44 6174 6146 7261 6d65 2872 665f  pd.DataFrame(rf_
+0000d790: 7573 6167 6573 2c20 696e 6465 783d 6e6f  usages, index=no
+0000d7a0: 726d 5f63 6f75 6e74 732e 696e 6465 782c  rm_counts.index,
+0000d7b0: 2063 6f6c 756d 6e73 3d6d 6564 6961 6e5f   columns=median_
+0000d7c0: 7370 6563 7472 612e 542e 696e 6465 7829  spectra.T.index)
+0000d7d0: 0d0a 2020 2020 2020 2020 2020 2020 7266  ..            rf
+0000d7e0: 5f70 7265 645f 6e6f 726d 5f63 6f75 6e74  _pred_norm_count
+0000d7f0: 7320 3d20 7266 5f75 7361 6765 732e 646f  s = rf_usages.do
+0000d800: 7428 6d65 6469 616e 5f73 7065 6374 7261  t(median_spectra
+0000d810: 2e54 290d 0a20 2020 2020 2020 2020 2020  .T)..           
+0000d820: 2070 7265 645f 6572 726f 725b 6b76 616c   pred_error[kval
+0000d830: 5d20 3d20 2828 6e6f 726d 5f63 6f75 6e74  ] = ((norm_count
+0000d840: 7320 2d20 7266 5f70 7265 645f 6e6f 726d  s - rf_pred_norm
+0000d850: 5f63 6f75 6e74 7329 2a2a 3229 2e73 756d  _counts)**2).sum
+0000d860: 2829 2e73 756d 2829 0d0a 0d0a 2020 2020  ().sum()....    
+0000d870: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0000d880: 6528 6b2c 2028 696e 742c 206e 702e 696e  e(k, (int, np.in
+0000d890: 7465 6765 7229 293a 0d0a 2020 2020 2020  teger)):..      
+0000d8a0: 2020 2020 2020 7265 7475 726e 2070 7265        return pre
+0000d8b0: 645f 6572 726f 725b 6b5d 0d0a 2020 2020  d_error[k]..    
+0000d8c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0000d8d0: 2020 2020 2020 2072 6574 7572 6e20 7072         return pr
+0000d8e0: 6564 5f65 7272 6f72 0d0a 0d0a 2020 2020  ed_error....    
+0000d8f0: 6465 6620 7661 6c69 6461 7465 5f63 6e6d  def validate_cnm
+0000d900: 665f 7072 6564 6963 7469 6f6e 5f65 7272  f_prediction_err
+0000d910: 6f72 7328 7365 6c66 2c20 746f 6c65 7261  ors(self, tolera
+0000d920: 6e63 653a 2066 6c6f 6174 203d 2031 652d  nce: float = 1e-
+0000d930: 3829 202d 3e20 7064 2e44 6174 6146 7261  8) -> pd.DataFra
+0000d940: 6d65 3a0d 0a20 2020 2020 2020 2022 2222  me:..        """
+0000d950: 5661 6c69 6461 7465 2074 6865 2064 6174  Validate the dat
+0000d960: 6173 6574 2061 6e64 2063 4e4d 4620 736f  aset and cNMF so
+0000d970: 6c75 7469 6f6e 7320 666f 7220 6561 6368  lutions for each
+0000d980: 2072 616e 6b20 6279 2063 6f6d 7061 7269   rank by compari
+0000d990: 6e67 2074 6865 0d0a 2020 2020 2020 2020  ng the..        
+0000d9a0: 7072 6564 6963 7469 6f6e 2065 7272 6f72  prediction error
+0000d9b0: 2076 616c 7565 7320 7374 6f72 6564 2069   values stored i
+0000d9c0: 6e20 7468 6520 6f62 6a65 6374 205b 7365  n the object [se
+0000d9d0: 6c66 2e61 6461 7461 2e75 6e73 2e6b 7661  lf.adata.uns.kva
+0000d9e0: 6c73 5d20 746f 2074 686f 7365 2063 616c  ls] to those cal
+0000d9f0: 6375 6c61 7465 6420 6672 6f6d 2074 6865  culated from the
+0000da00: 0d0a 2020 2020 2020 2020 6461 7461 7365  ..        datase
+0000da10: 7427 7320 6461 7461 206d 6174 7269 6365  t's data matrice
+0000da20: 7320 5b62 6173 6564 206f 6e20 7365 6c66  s [based on self
+0000da30: 2e61 6461 7461 2e58 2061 6e64 2073 656c  .adata.X and sel
+0000da40: 662e 6164 6174 612e 7661 726d 5b27 636e  f.adata.varm['cn
+0000da50: 6d66 5f67 6570 5f72 6177 275d 5d2e 2054  mf_gep_raw']]. T
+0000da60: 6869 7320 6361 6e20 6265 2061 2071 7569  his can be a qui
+0000da70: 636b 2061 6e64 2073 656e 7369 7469 7665  ck and sensitive
+0000da80: 2077 6179 2074 6f20 6173 7365 7373 0d0a   way to assess..
+0000da90: 2020 2020 2020 2020 7468 6174 2074 6865          that the
+0000daa0: 2064 6174 6173 6574 2061 6e64 2074 6865   dataset and the
+0000dab0: 2063 4e4d 4620 736f 6c75 7469 6f6e 7320   cNMF solutions 
+0000dac0: 6861 7665 206e 6f74 2062 6565 6e20 616c  have not been al
+0000dad0: 7465 7265 642e 0d0a 0d0a 2020 2020 2020  tered.....      
+0000dae0: 2020 3a70 6172 616d 2074 6f6c 6572 616e    :param toleran
+0000daf0: 6365 3a20 6d61 7869 6d75 6d20 7265 6c61  ce: maximum rela
+0000db00: 7469 7665 2065 7272 6f72 2066 6f72 2061  tive error for a
+0000db10: 6e79 206b 2077 6865 6e20 636f 6d70 7574  ny k when comput
+0000db20: 696e 6720 7468 6520 7072 6564 6963 7469  ing the predicti
+0000db30: 6f6e 2065 7272 6f72 2c20 6465 6661 756c  on error, defaul
+0000db40: 7473 2074 6f20 302e 3030 3031 0d0a 2020  ts to 0.0001..  
+0000db50: 2020 2020 2020 3a74 7970 6520 746f 6c65        :type tole
+0000db60: 7261 6e63 653a 2066 6c6f 6174 2c20 6f70  rance: float, op
+0000db70: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+0000db80: 3a72 6169 7365 7320 5661 6c75 6545 7272  :raises ValueErr
+0000db90: 6f72 3a20 6966 2074 6865 206d 6178 696d  or: if the maxim
+0000dba0: 756d 2072 656c 6174 6976 6520 6572 726f  um relative erro
+0000dbb0: 7220 6578 6365 6564 7320 7468 6520 746f  r exceeds the to
+0000dbc0: 6c65 7261 6e63 650d 0a20 2020 2020 2020  lerance..       
+0000dbd0: 203a 7265 7475 726e 3a20 4461 7461 4672   :return: DataFr
+0000dbe0: 616d 6520 7769 7468 2073 746f 7265 6420  ame with stored 
+0000dbf0: 616e 6420 636f 6d70 7574 6564 2070 7265  and computed pre
+0000dc00: 6469 6374 696f 6e20 6572 726f 722c 2061  diction error, a
+0000dc10: 6e64 2072 656c 6174 6976 6520 6572 726f  nd relative erro
+0000dc20: 7220 666f 7220 6561 6368 2072 616e 6b0d  r for each rank.
+0000dc30: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+0000dc40: 2070 642e 4461 7461 4672 616d 650d 0a20   pd.DataFrame.. 
+0000dc50: 2020 2020 2020 2022 2222 0d0a 200d 0a20         """.. .. 
+0000dc60: 2020 2020 2020 2070 7265 645f 6572 726f         pred_erro
+0000dc70: 7220 3d20 7064 2e53 6572 6965 7328 290d  r = pd.Series().
+0000dc80: 0a20 2020 2020 2020 2066 6f72 206b 2069  .        for k i
+0000dc90: 6e20 7365 6c66 2e61 6461 7461 2e75 6e73  n self.adata.uns
+0000dca0: 5b27 6b76 616c 7327 5d2e 696e 6465 783a  ['kvals'].index:
+0000dcb0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0000dcc0: 6564 5f65 7272 6f72 5b6b 5d20 3d20 7365  ed_error[k] = se
+0000dcd0: 6c66 2e63 616c 6375 6c61 7465 5f63 6e6d  lf.calculate_cnm
+0000dce0: 665f 7072 6564 6963 7469 6f6e 5f65 7272  f_prediction_err
+0000dcf0: 6f72 286b 3d6b 290d 0a20 2020 2020 2020  or(k=k)..       
+0000dd00: 2023 2076 616c 6964 6174 6520 6572 726f   # validate erro
+0000dd10: 7220 6f66 2074 6865 2073 6f6c 7574 696f  r of the solutio
+0000dd20: 6e73 206d 6174 6368 6573 2063 4e4d 4627  ns matches cNMF'
+0000dd30: 7320 7374 6f72 6564 2065 7272 6f72 2076  s stored error v
+0000dd40: 616c 7565 730d 0a20 2020 2020 2020 2064  alues..        d
+0000dd50: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
+0000dd60: 287b 2273 746f 7265 6422 3a20 7365 6c66  ({"stored": self
+0000dd70: 2e61 6461 7461 2e75 6e73 5b27 6b76 616c  .adata.uns['kval
+0000dd80: 7327 5d5b 2270 7265 6469 6374 696f 6e5f  s']["prediction_
+0000dd90: 6572 726f 7222 5d2c 0d0a 2020 2020 2020  error"],..      
+0000dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddb0: 2020 2020 2022 636f 6d70 7574 6564 223a       "computed":
+0000ddc0: 2070 7265 645f 6572 726f 727d 290d 0a20   pred_error}).. 
+0000ddd0: 2020 2020 2020 2064 665b 2272 656c 6174         df["relat
+0000dde0: 6976 655f 6572 726f 7222 5d20 3d20 2864  ive_error"] = (d
+0000ddf0: 665b 2263 6f6d 7075 7465 6422 5d20 2d20  f["computed"] - 
+0000de00: 6466 5b22 7374 6f72 6564 225d 292e 6162  df["stored"]).ab
+0000de10: 7328 2920 2f20 6466 5b22 7374 6f72 6564  s() / df["stored
+0000de20: 225d 0d0a 2020 2020 2020 2020 0d0a 2020  "]..        ..  
+0000de30: 2020 2020 2020 6966 2028 6466 5b22 7265        if (df["re
+0000de40: 6c61 7469 7665 5f65 7272 6f72 225d 203e  lative_error"] >
+0000de50: 2074 6f6c 6572 616e 6365 292e 616e 7928   tolerance).any(
+0000de60: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000de70: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000de80: 2866 2244 6174 6173 6574 2076 616c 6964  (f"Dataset valid
+0000de90: 6174 696f 6e20 6661 696c 6564 2075 7369  ation failed usi
+0000dea0: 6e67 2063 4e4d 4620 7072 6564 6963 7469  ng cNMF predicti
+0000deb0: 6f6e 2065 7272 6f72 2074 6f6c 6572 616e  on error toleran
+0000dec0: 6365 206f 6620 7b74 6f6c 6572 616e 6365  ce of {tolerance
+0000ded0: 7d2e 2022 0d0a 2020 2020 2020 2020 2020  }. "..          
+0000dee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000def0: 2020 2022 5468 6973 2063 616e 206f 6363     "This can occ
+0000df00: 7572 2077 6865 6e20 6461 7461 7365 7420  ur when dataset 
+0000df10: 6f62 6a65 6374 7320 6172 6520 756e 696e  objects are unin
+0000df20: 7465 6e74 696f 6e61 6c6c 7920 616c 7465  tentionally alte
+0000df30: 7265 6420 616e 6420 7468 6520 6d61 7472  red and the matr
+0000df40: 6963 6573 2022 0d0a 2020 2020 2020 2020  ices "..        
+0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df60: 2020 2020 2022 6172 6520 6e6f 7420 636f       "are not co
+0000df70: 6e73 6973 7465 6e74 2077 6974 6820 7468  nsistent with th
+0000df80: 6520 6f72 6967 696e 616c 206f 6e65 7320  e original ones 
+0000df90: 7573 6564 2066 6f72 2066 6163 746f 7269  used for factori
+0000dfa0: 7a61 7469 6f6e 2e22 290d 0a0d 0a20 2020  zation.")....   
+0000dfb0: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
+0000dfc0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+0000dfd0: 6465 6620 6765 745f 6d65 7461 6461 7461  def get_metadata
+0000dfe0: 5f64 6628 7365 6c66 2c0d 0a20 2020 2020  _df(self,..     
+0000dff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e000: 2020 2069 6e63 6c75 6465 5f63 6174 6567     include_categ
+0000e010: 6f72 6963 616c 3a20 626f 6f6c 203d 2054  orical: bool = T
+0000e020: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+0000e030: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000e040: 636c 7564 655f 6e75 6d65 7269 6361 6c3a  clude_numerical:
+0000e050: 2062 6f6f 6c20 3d20 5472 7565 0d0a 2020   bool = True..  
+0000e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e070: 2020 2020 2020 2920 2d3e 2070 642e 4461        ) -> pd.Da
+0000e080: 7461 4672 616d 653a 0d0a 2020 2020 2020  taFrame:..      
+0000e090: 2020 2222 2247 6574 2073 616d 706c 652f    """Get sample/
+0000e0a0: 6f62 7365 7276 6174 696f 6e20 6d65 7461  observation meta
+0000e0b0: 6461 7461 2e0d 0a0d 0a20 2020 2020 2020  data.....       
+0000e0c0: 203a 7061 7261 6d20 696e 636c 7564 655f   :param include_
+0000e0d0: 6361 7465 676f 7269 6361 6c3a 2049 6e63  categorical: Inc
+0000e0e0: 6c75 6465 2063 6174 6567 6f72 6963 616c  lude categorical
+0000e0f0: 206d 6574 6164 6174 6120 6c61 7965 7273   metadata layers
+0000e100: 2c20 6465 6661 756c 7473 2074 6f20 5472  , defaults to Tr
+0000e110: 7565 0d0a 2020 2020 2020 2020 3a74 7970  ue..        :typ
+0000e120: 6520 696e 636c 7564 655f 6361 7465 676f  e include_catego
+0000e130: 7269 6361 6c3a 2062 6f6f 6c2c 206f 7074  rical: bool, opt
+0000e140: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
+0000e150: 7061 7261 6d20 696e 636c 7564 655f 6e75  param include_nu
+0000e160: 6d65 7269 6361 6c3a 2049 6e63 6c75 6465  merical: Include
+0000e170: 206e 756d 6572 6963 616c 206d 6574 6164   numerical metad
+0000e180: 6174 6120 6c61 7965 7273 2c20 6465 6661  ata layers, defa
+0000e190: 756c 7473 2074 6f20 5472 7565 0d0a 2020  ults to True..  
+0000e1a0: 2020 2020 2020 3a74 7970 6520 696e 636c        :type incl
+0000e1b0: 7564 655f 6e75 6d65 7269 6361 6c3a 2062  ude_numerical: b
+0000e1c0: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a20  ool, optional.. 
+0000e1d0: 2020 2020 2020 203a 7261 6973 6573 2056         :raises V
+0000e1e0: 616c 7565 4572 726f 723a 2045 7272 6f72  alueError: Error
+0000e1f0: 2069 6620 6d65 7461 6461 7461 2074 7970   if metadata typ
+0000e200: 6573 2061 7265 206e 6f74 2072 6563 6f67  es are not recog
+0000e210: 6e69 7a65 640d 0a20 2020 2020 2020 203a  nized..        :
+0000e220: 7265 7475 726e 3a20 6f62 7365 7276 6174  return: observat
+0000e230: 696f 6e73 20c3 9720 6d65 7461 6461 7461  ions .. metadata
+0000e240: 206d 6174 7269 780d 0a20 2020 2020 2020   matrix..       
+0000e250: 203a 7274 7970 653a 2070 642e 4461 7461   :rtype: pd.Data
+0000e260: 4672 616d 650d 0a20 2020 2020 2020 2022  Frame..        "
+0000e270: 2222 0d0a 2020 2020 2020 2020 6474 7970  ""..        dtyp
+0000e280: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
+0000e290: 2069 6620 696e 636c 7564 655f 6361 7465   if include_cate
+0000e2a0: 676f 7269 6361 6c3a 0d0a 2020 2020 2020  gorical:..      
+0000e2b0: 2020 2020 2020 6474 7970 6573 2e61 7070        dtypes.app
+0000e2c0: 656e 6428 2263 6174 6567 6f72 7922 290d  end("category").
+0000e2d0: 0a20 2020 2020 2020 2069 6620 696e 636c  .        if incl
+0000e2e0: 7564 655f 6e75 6d65 7269 6361 6c3a 0d0a  ude_numerical:..
+0000e2f0: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
+0000e300: 6573 202b 3d20 5b22 666c 6f61 7422 2c20  es += ["float", 
+0000e310: 2269 6e74 225d 0d0a 2020 2020 2020 2020  "int"]..        
+0000e320: 756e 6578 706c 6169 6e65 645f 636f 6c73  unexplained_cols
+0000e330: 203d 2073 656c 662e 6164 6174 612e 6f62   = self.adata.ob
+0000e340: 732e 7365 6c65 6374 5f64 7479 7065 7328  s.select_dtypes(
+0000e350: 6578 636c 7564 653d 2822 6361 7465 676f  exclude=("catego
+0000e360: 7279 222c 2022 666c 6f61 7422 2c20 2269  ry", "float", "i
+0000e370: 6e74 2229 292e 636f 6c75 6d6e 730d 0a20  nt")).columns.. 
+0000e380: 2020 2020 2020 2069 6620 6c65 6e28 756e         if len(un
+0000e390: 6578 706c 6169 6e65 645f 636f 6c73 2920  explained_cols) 
+0000e3a0: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
+0000e3b0: 2020 756e 6578 706c 6169 6e65 645f 636f    unexplained_co
+0000e3c0: 6c5f 7374 7220 3d20 222c 2022 2e6a 6f69  l_str = ", ".joi
+0000e3d0: 6e28 756e 6578 706c 6169 6e65 645f 636f  n(unexplained_co
+0000e3e0: 6c73 290d 0a20 2020 2020 2020 2020 2020  ls)..           
+0000e3f0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0000e400: 7228 6622 7b75 6e65 7870 6c61 696e 6564  r(f"{unexplained
+0000e410: 5f63 6f6c 5f73 7472 7d20 6d65 7461 6461  _col_str} metada
+0000e420: 7461 2063 6f6c 756d 6e73 2068 6176 6520  ta columns have 
+0000e430: 756e 7265 636f 676e 697a 6564 2064 7479  unrecognized dty
+0000e440: 7065 732e 2229 0d0a 2020 2020 2020 2020  pes.")..        
+0000e450: 6466 203d 2073 656c 662e 6164 6174 612e  df = self.adata.
+0000e460: 6f62 732e 7365 6c65 6374 5f64 7479 7065  obs.select_dtype
+0000e470: 7328 696e 636c 7564 653d 6474 7970 6573  s(include=dtypes
+0000e480: 290d 0a20 2020 2020 2020 2064 6620 3d20  )..        df = 
+0000e490: 6466 2e64 726f 706e 6128 6178 6973 3d31  df.dropna(axis=1
+0000e4a0: 2c20 686f 773d 2261 6c6c 2229 0d0a 2020  , how="all")..  
+0000e4b0: 2020 2020 2020 6466 203d 2064 662e 7265        df = df.re
+0000e4c0: 706c 6163 6528 226e 616e 222c 206e 702e  place("nan", np.
+0000e4d0: 4e61 4e29 2020 2354 4f44 4f3a 2041 6464  NaN)  #TODO: Add
+0000e4e0: 7265 7373 2065 7272 6f72 3a20 2f68 6f6d  ress error: /hom
+0000e4f0: 652f 7462 7665 7268 6579 2f6d 696e 6963  e/tbverhey/minic
+0000e500: 6f6e 6461 332f 656e 7673 2f6d 6f73 6169  onda3/envs/mosai
+0000e510: 636d 7069 2f6c 6962 2f70 7974 686f 6e33  cmpi/lib/python3
+0000e520: 2e31 312f 7369 7465 2d70 6163 6b61 6765  .11/site-package
+0000e530: 732f 6d6f 7361 6963 6d70 692f 6461 7461  s/mosaicmpi/data
+0000e540: 7365 742e 7079 3a31 3032 313a 2046 7574  set.py:1021: Fut
+0000e550: 7572 6557 6172 6e69 6e67 3a20 5468 6520  ureWarning: The 
+0000e560: 6265 6861 7669 6f72 206f 6620 5365 7269  behavior of Seri
+0000e570: 6573 2e72 6570 6c61 6365 2028 616e 6420  es.replace (and 
+0000e580: 4461 7461 4672 616d 652e 7265 706c 6163  DataFrame.replac
+0000e590: 6529 2077 6974 6820 4361 7465 676f 7269  e) with Categori
+0000e5a0: 6361 6c44 7479 7065 2069 7320 6465 7072  calDtype is depr
+0000e5b0: 6563 6174 6564 2e20 496e 2061 2066 7574  ecated. In a fut
+0000e5c0: 7572 6520 7665 7273 696f 6e2c 2072 6570  ure version, rep
+0000e5d0: 6c61 6365 2077 696c 6c20 6f6e 6c79 2062  lace will only b
+0000e5e0: 6520 7573 6564 2066 6f72 2063 6173 6573  e used for cases
+0000e5f0: 2074 6861 7420 7072 6573 6572 7665 2074   that preserve t
+0000e600: 6865 2063 6174 6567 6f72 6965 732e 2054  he categories. T
+0000e610: 6f20 6368 616e 6765 2074 6865 2063 6174  o change the cat
+0000e620: 6567 6f72 6965 732c 2075 7365 2073 6572  egories, use ser
+0000e630: 2e63 6174 2e72 656e 616d 655f 6361 7465  .cat.rename_cate
+0000e640: 676f 7269 6573 2069 6e73 7465 6164 2e0d  gories instead..
+0000e650: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000e660: 6466 0d0a 2020 2020 0d0a 2020 2020 6465  df..    ..    de
+0000e670: 6620 6765 745f 6361 7465 676f 7279 5f6f  f get_category_o
+0000e680: 7665 7272 6570 7265 7365 6e74 6174 696f  verrepresentatio
+0000e690: 6e28 7365 6c66 2c0d 0a20 2020 2020 2020  n(self,..       
+0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6c0: 206c 6179 6572 3a20 7374 722c 0d0a 2020   layer: str,..  
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6f0: 2020 2020 2020 7472 756e 6361 7465 5f6e        truncate_n
+0000e700: 6567 6174 6976 653a 2062 6f6f 6c20 3d20  egative: bool = 
+0000e710: 5472 7565 2c0d 0a20 2020 2020 2020 2020  True,..         
+0000e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e730: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e740: 7562 7365 745f 6361 7465 676f 7269 6573  ubset_categories
+0000e750: 3a20 436f 6c6c 6563 7469 6f6e 5b73 7472  : Collection[str
+0000e760: 5d20 3d20 4e6f 6e65 0d0a 2020 2020 2020  ] = None..      
+0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e790: 2020 2920 2d3e 2070 642e 4461 7461 4672    ) -> pd.DataFr
+0000e7a0: 616d 653a 0d0a 2020 2020 2020 2020 2222  ame:..        ""
+0000e7b0: 2243 616c 6375 6c61 7465 2050 6561 7273  "Calculate Pears
+0000e7c0: 6f6e 2072 6573 6964 7561 6c20 6f66 2063  on residual of c
+0000e7d0: 6869 2d73 7175 6172 6564 2074 6573 742c  hi-squared test,
+0000e7e0: 2061 7373 6f63 6961 7469 6e67 2070 726f   associating pro
+0000e7f0: 6772 616d 7320 666f 7220 6561 6368 2072  grams for each r
+0000e800: 616e 6b20 286b 2920 746f 2063 6174 6567  ank (k) to categ
+0000e810: 6f72 6965 7320 6f66 2073 616d 706c 6573  ories of samples
+0000e820: 2f6f 6273 6572 7661 7469 6f6e 732e 2042  /observations. B
+0000e830: 7920 6465 6661 756c 742c 2074 7275 6e63  y default, trunc
+0000e840: 6174 6573 206e 6567 6174 6976 6520 7661  ates negative va
+0000e850: 6c75 6573 2e0d 0a0d 0a20 2020 2020 2020  lues.....       
+0000e860: 203a 7061 7261 6d20 6c61 7965 723a 206e   :param layer: n
+0000e870: 616d 6520 6f66 2063 6174 6567 6f72 6963  ame of categoric
+0000e880: 616c 2064 6174 6120 6c61 7965 720d 0a20  al data layer.. 
+0000e890: 2020 2020 2020 203a 7479 7065 206c 6179         :type lay
+0000e8a0: 6572 3a20 7374 720d 0a20 2020 2020 2020  er: str..       
+0000e8b0: 203a 7061 7261 6d20 7472 756e 6361 7465   :param truncate
+0000e8c0: 5f6e 6567 6174 6976 653a 2054 7275 6e63  _negative: Trunc
+0000e8d0: 6174 6520 6e65 6761 7469 7665 2072 6573  ate negative res
+0000e8e0: 6964 7561 6c73 2074 6f20 302c 2064 6566  iduals to 0, def
+0000e8f0: 6175 6c74 7320 746f 2054 7275 650d 0a20  aults to True.. 
+0000e900: 2020 2020 2020 203a 7479 7065 2074 7275         :type tru
+0000e910: 6e63 6174 655f 6e65 6761 7469 7665 3a20  ncate_negative: 
+0000e920: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0d0a  bool, optional..
+0000e930: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+0000e940: 7562 7365 745f 6361 7465 676f 7269 6573  ubset_categories
+0000e950: 3a20 5072 6f76 6964 6520 6120 7375 6273  : Provide a subs
+0000e960: 6574 206f 6620 6361 7465 676f 7269 6573  et of categories
+0000e970: 2066 6f72 2063 616c 6375 6c61 7469 6e67   for calculating
+0000e980: 206f 7665 7272 6570 7265 7365 6e74 6174   overrepresentat
+0000e990: 696f 6e0d 0a20 2020 2020 2020 203a 7479  ion..        :ty
+0000e9a0: 7065 2073 7562 7365 745f 6361 7465 676f  pe subset_catego
+0000e9b0: 7269 6573 3a20 436f 6c6c 6563 7469 6f6e  ries: Collection
+0000e9c0: 5b73 7472 5d0d 0a20 2020 2020 2020 203a  [str]..        :
+0000e9d0: 7265 7475 726e 3a20 6361 7465 676f 7279  return: category
+0000e9e0: 20c3 9720 7072 6f67 7261 6d20 6d61 7472   .. program matr
+0000e9f0: 6978 206f 6620 6f76 6572 7265 7072 6573  ix of overrepres
+0000ea00: 656e 7461 7469 6f6e 2076 616c 7565 730d  entation values.
+0000ea10: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+0000ea20: 2070 642e 4461 7461 4672 616d 650d 0a20   pd.DataFrame.. 
+0000ea30: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+0000ea40: 2020 2020 7573 6167 6520 3d20 7365 6c66      usage = self
+0000ea50: 2e67 6574 5f75 7361 6765 7328 6e6f 726d  .get_usages(norm
+0000ea60: 616c 697a 653d 5472 7565 292e 636f 7079  alize=True).copy
+0000ea70: 2829 0d0a 2020 2020 2020 2020 7361 6d70  ()..        samp
+0000ea80: 6c65 5f74 6f5f 636c 6173 7320 3d20 7365  le_to_class = se
+0000ea90: 6c66 2e67 6574 5f6d 6574 6164 6174 615f  lf.get_metadata_
+0000eaa0: 6466 2829 5b6c 6179 6572 5d0d 0a20 2020  df()[layer]..   
+0000eab0: 2020 2020 2069 6620 7375 6273 6574 5f63       if subset_c
+0000eac0: 6174 6567 6f72 6965 7320 6973 206e 6f74  ategories is not
+0000ead0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0000eae0: 2020 2020 7361 6d70 6c65 5f74 6f5f 636c      sample_to_cl
+0000eaf0: 6173 735b 7e73 616d 706c 655f 746f 5f63  ass[~sample_to_c
+0000eb00: 6c61 7373 2e69 7369 6e28 7375 6273 6574  lass.isin(subset
+0000eb10: 5f63 6174 6567 6f72 6965 7329 5d20 3d20  _categories)] = 
+0000eb20: 6e70 2e4e 614e 0d0a 2020 2020 2020 2020  np.NaN..        
+0000eb30: 7573 6167 652e 696e 6465 7820 3d20 7573  usage.index = us
+0000eb40: 6167 652e 696e 6465 782e 6d61 7028 7361  age.index.map(sa
+0000eb50: 6d70 6c65 5f74 6f5f 636c 6173 7329 0d0a  mple_to_class)..
+0000eb60: 2020 2020 2020 2020 6f62 7365 7276 6564          observed
+0000eb70: 203d 2075 7361 6765 2e67 726f 7570 6279   = usage.groupby
+0000eb80: 286c 6576 656c 3d30 2c20 6f62 7365 7276  (level=0, observ
+0000eb90: 6564 3d54 7275 6529 2e73 756d 2829 0d0a  ed=True).sum()..
+0000eba0: 2020 2020 2020 2020 6f62 7365 7276 6564          observed
+0000ebb0: 203d 206f 6273 6572 7665 645b 6f62 7365   = observed[obse
+0000ebc0: 7276 6564 2e73 756d 2861 7869 733d 3129  rved.sum(axis=1)
+0000ebd0: 203e 2030 5d0d 0a20 2020 2020 2020 206e   > 0]..        n
+0000ebe0: 5f63 6174 6567 6f72 6965 7320 3d20 6f62  _categories = ob
+0000ebf0: 7365 7276 6564 2e73 6861 7065 5b30 5d0d  served.shape[0].
+0000ec00: 0a20 2020 2020 2020 2069 6620 6e5f 6361  .        if n_ca
+0000ec10: 7465 676f 7269 6573 203c 2032 3a0d 0a20  tegories < 2:.. 
+0000ec20: 2020 2020 2020 2020 2020 2069 6620 6c61             if la
+0000ec30: 7965 7220 213d 2022 6876 675f 616c 6c5f  yer != "hvg_all_
+0000ec40: 3022 3a0d 0a20 2020 2020 2020 2020 2020  0":..           
+0000ec50: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
+0000ec60: 6e69 6e67 2866 224f 7665 7272 6570 7265  ning(f"Overrepre
+0000ec70: 7365 6e74 6174 696f 6e20 636f 756c 6420  sentation could 
+0000ec80: 6e6f 7420 6265 2063 616c 6375 6c61 7465  not be calculate
+0000ec90: 6420 666f 7220 6c61 7965 7220 277b 6c61  d for layer '{la
+0000eca0: 7965 727d 272c 2061 7320 6f6e 6c79 207b  yer}', as only {
+0000ecb0: 6e5f 6361 7465 676f 7269 6573 7d20 6361  n_categories} ca
+0000ecc0: 7465 676f 7269 6573 2077 6572 6520 666f  tegories were fo
+0000ecd0: 756e 6420 696e 2074 6865 2064 6174 612e  und in the data.
+0000ece0: 2022 0d0a 2020 2020 2020 2020 2020 2020   "..            
+0000ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed00: 2020 2020 6622 4e6f 7465 2074 6861 7420      f"Note that 
+0000ed10: 656d 7074 7920 7661 6c75 6573 2069 6e20  empty values in 
+0000ed20: 7468 6520 6d65 7461 6461 7461 2061 7265  the metadata are
+0000ed30: 206e 6f74 2063 6f6e 7369 6465 7265 6420   not considered 
+0000ed40: 6120 6361 7465 676f 7279 2e20 220d 0a20  a category. ".. 
+0000ed50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000ed70: 224f 7665 7272 6570 7265 7365 6e74 6174  "Overrepresentat
+0000ed80: 696f 6e20 6361 6e6e 6f74 2062 6520 6361  ion cannot be ca
+0000ed90: 6c63 756c 6174 6564 2077 6974 6820 6665  lculated with fe
+0000eda0: 7765 7220 7468 616e 2032 2063 6174 6567  wer than 2 categ
+0000edb0: 6f72 6965 7320 666f 7220 6561 6368 206c  ories for each l
+0000edc0: 6179 6572 2e20 2229 0d0a 2020 2020 2020  ayer. ")..      
+0000edd0: 2020 2020 2020 7265 7475 726e 2070 642e        return pd.
+0000ede0: 4461 7461 4672 616d 6528 6e70 2e4e 614e  DataFrame(np.NaN
+0000edf0: 2c20 696e 6465 7820 3d20 6f62 7365 7276  , index = observ
+0000ee00: 6564 2e69 6e64 6578 2c20 636f 6c75 6d6e  ed.index, column
+0000ee10: 733d 6f62 7365 7276 6564 2e63 6f6c 756d  s=observed.colum
+0000ee20: 6e73 290d 0a20 2020 2020 2020 2065 7870  ns)..        exp
+0000ee30: 6563 7465 6420 3d20 5b5d 0d0a 2020 2020  ected = []..    
+0000ee40: 2020 2020 666f 7220 6b2c 206f 6273 5f6b      for k, obs_k
+0000ee50: 2069 6e20 6f62 7365 7276 6564 2e54 2e67   in observed.T.g
+0000ee60: 726f 7570 6279 286c 6576 656c 3d31 293a  roupby(level=1):
+0000ee70: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+0000ee80: 705f 6b20 3d20 7064 2e44 6174 6146 7261  p_k = pd.DataFra
+0000ee90: 6d65 286f 6273 5f6b 2e73 756d 2861 7869  me(obs_k.sum(axi
+0000eea0: 733d 3129 2920 4020 7064 2e44 6174 6146  s=1)) @ pd.DataF
+0000eeb0: 7261 6d65 286f 6273 5f6b 2e73 756d 2861  rame(obs_k.sum(a
+0000eec0: 7869 733d 3029 292e 5420 2f20 6f62 735f  xis=0)).T / obs_
+0000eed0: 6b2e 7375 6d28 292e 7375 6d28 290d 0a20  k.sum().sum().. 
+0000eee0: 2020 2020 2020 2020 2020 2065 7870 6563             expec
+0000eef0: 7465 642e 6170 7065 6e64 2865 7870 5f6b  ted.append(exp_k
+0000ef00: 290d 0a20 2020 2020 2020 2065 7870 6563  )..        expec
+0000ef10: 7465 6420 3d20 7064 2e63 6f6e 6361 7428  ted = pd.concat(
+0000ef20: 6578 7065 6374 6564 292e 540d 0a20 2020  expected).T..   
+0000ef30: 2020 2020 2063 6869 7371 5f72 6573 6964       chisq_resid
+0000ef40: 203d 2028 6f62 7365 7276 6564 202d 2065   = (observed - e
+0000ef50: 7870 6563 7465 6429 202f 206e 702e 7371  xpected) / np.sq
+0000ef60: 7274 2865 7870 6563 7465 6429 2020 2320  rt(expected)  # 
+0000ef70: 7065 6172 736f 6e20 7265 7369 6475 616c  pearson residual
+0000ef80: 206f 6620 6368 692d 7371 7561 7265 6420   of chi-squared 
+0000ef90: 7465 7374 206f 6620 636f 6e74 696e 6765  test of continge
+0000efa0: 6e63 7920 7461 626c 650d 0a20 2020 2020  ncy table..     
+0000efb0: 2020 2069 6620 7472 756e 6361 7465 5f6e     if truncate_n
+0000efc0: 6567 6174 6976 653a 0d0a 2020 2020 2020  egative:..      
+0000efd0: 2020 2020 2020 6368 6973 715f 7265 7369        chisq_resi
+0000efe0: 6420 3d20 6368 6973 715f 7265 7369 642e  d = chisq_resid.
+0000eff0: 636c 6970 286c 6f77 6572 3d30 290d 0a20  clip(lower=0).. 
+0000f000: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
+0000f010: 6973 715f 7265 7369 640d 0a20 2020 200d  isq_resid..    .
+0000f020: 0a20 2020 2020 2020 200d 0a20 2020 2064  .        ..    d
+0000f030: 6566 2067 6574 5f6d 6574 6164 6174 615f  ef get_metadata_
+0000f040: 636f 7272 656c 6174 696f 6e28 7365 6c66  correlation(self
+0000f050: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+0000f060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f070: 2020 2020 206c 6179 6572 3a20 7374 722c       layer: str,
+0000f080: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0a0: 2020 206d 6574 686f 643a 2073 7472 203d     method: str =
+0000f0b0: 2022 7065 6172 736f 6e22 0d0a 2020 2020   "pearson"..    
+0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0d0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+0000f0e0: 3e20 7064 2e53 6572 6965 733a 0d0a 2020  > pd.Series:..  
+0000f0f0: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+0000f100: 7465 2050 6561 7273 6f6e 2063 6f72 7265  te Pearson corre
+0000f110: 6c61 7469 6f6e 206f 6620 4745 5020 7573  lation of GEP us
+0000f120: 6167 6520 746f 206e 756d 6572 6963 616c  age to numerical
+0000f130: 206d 6574 6164 6174 6120 6163 726f 7373   metadata across
+0000f140: 2073 616d 706c 6573 2f6f 6273 6572 7661   samples/observa
+0000f150: 7469 6f6e 732e 0d0a 0d0a 2020 2020 2020  tions.....      
+0000f160: 2020 3a70 6172 616d 206c 6179 6572 3a20    :param layer: 
+0000f170: 6e61 6d65 206f 6620 6e75 6d65 7269 6361  name of numerica
+0000f180: 6c20 6461 7461 206c 6179 6572 0d0a 2020  l data layer..  
+0000f190: 2020 2020 2020 3a74 7970 6520 6c61 7965        :type laye
+0000f1a0: 723a 2073 7472 0d0a 2020 2020 2020 2020  r: str..        
+0000f1b0: 3a70 6172 616d 206d 6574 686f 643a 2043  :param method: C
+0000f1c0: 6f72 7265 6c61 7469 6f6e 206d 6574 686f  orrelation metho
+0000f1d0: 643a 2022 7065 6172 736f 6e22 2c20 2273  d: "pearson", "s
+0000f1e0: 7065 6172 6d61 6e22 2c20 6f72 2022 6b65  pearman", or "ke
+0000f1f0: 6e64 616c 6c22 2e20 4465 6661 756c 7473  ndall". Defaults
+0000f200: 2074 6f20 2270 6561 7273 6f6e 220d 0a20   to "pearson".. 
+0000f210: 2020 2020 2020 203a 7479 7065 206d 6574         :type met
+0000f220: 686f 643a 2073 7472 2c20 6f70 7469 6f6e  hod: str, option
+0000f230: 616c 0d0a 2020 2020 2020 2020 3a72 6574  al..        :ret
+0000f240: 7572 6e3a 2063 6f72 7265 6c61 7469 6f6e  urn: correlation
+0000f250: 206f 6620 4745 5020 746f 206d 6574 6164   of GEP to metad
+0000f260: 6174 610d 0a20 2020 2020 2020 203a 7274  ata..        :rt
+0000f270: 7970 653a 2070 642e 5365 7269 6573 0d0a  ype: pd.Series..
+0000f280: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+0000f290: 2020 2020 2075 7361 6765 203d 2073 656c       usage = sel
+0000f2a0: 662e 6765 745f 7573 6167 6573 2829 2e63  f.get_usages().c
+0000f2b0: 6f70 7928 290d 0a20 2020 2020 2020 206d  opy()..        m
+0000f2c0: 6574 6164 6174 6120 3d20 7365 6c66 2e67  etadata = self.g
+0000f2d0: 6574 5f6d 6574 6164 6174 615f 6466 2829  et_metadata_df()
+0000f2e0: 5b6c 6179 6572 5d0d 0a20 2020 2020 2020  [layer]..       
+0000f2f0: 206d 645f 636f 7272 203d 2075 7361 6765   md_corr = usage
+0000f300: 2e63 6f72 7277 6974 6828 6d65 7461 6461  .corrwith(metada
+0000f310: 7461 2c20 6d65 7468 6f64 3d6d 6574 686f  ta, method=metho
+0000f320: 6429 0d0a 2020 2020 2020 2020 7265 7475  d)..        retu
+0000f330: 726e 206d 645f 636f 7272 0d0a 2020 2020  rn md_corr..    
+0000f340: 2020 2020 0d0a 2020 2020 6465 6620 6170      ..    def ap
+0000f350: 7065 6e64 5f74 6f5f 6869 7374 6f72 7928  pend_to_history(
+0000f360: 7365 6c66 2c20 656e 7472 7929 3a0d 0a20  self, entry):.. 
+0000f370: 2020 2020 2020 2022 2222 4164 6420 656e         """Add en
+0000f380: 7472 7920 746f 2044 6174 6173 6574 2068  try to Dataset h
+0000f390: 6973 746f 7279 2e0d 0a0d 0a20 2020 2020  istory.....     
+0000f3a0: 2020 203a 7061 7261 6d20 656e 7472 793a     :param entry:
+0000f3b0: 2044 6573 6372 6970 7469 6f6e 206f 6620   Description of 
+0000f3c0: 6576 656e 7420 746f 2072 6563 6f72 6420  event to record 
+0000f3d0: 696e 2074 6865 2068 6973 746f 7279 2e0d  in the history..
+0000f3e0: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
+0000f3f0: 6e74 7279 3a20 7374 720d 0a20 2020 2020  ntry: str..     
+0000f400: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+0000f410: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
+0000f420: 6869 7374 6f72 7922 5d5b 6461 7465 7469  history"][dateti
+0000f430: 6d65 2e75 7463 6e6f 7728 292e 6973 6f66  me.utcnow().isof
+0000f440: 6f72 6d61 7428 295d 203d 2065 6e74 7279  ormat()] = entry
+0000f450: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0000f460: 6465 6620 6765 745f 6869 7374 6f72 7928  def get_history(
+0000f470: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+0000f480: 2222 2252 6574 7572 6e73 2074 696d 6573  """Returns times
+0000f490: 7461 6d70 6564 2068 6973 746f 7279 206f  tamped history o
+0000f4a0: 6620 4461 7461 7365 7420 6f62 6a65 6374  f Dataset object
+0000f4b0: 2e0d 0a0d 0a20 2020 2020 2020 203a 7265  .....        :re
+0000f4c0: 7475 726e 3a20 6869 7374 6f72 790d 0a20  turn: history.. 
+0000f4d0: 2020 2020 2020 203a 7274 7970 653a 2064         :rtype: d
+0000f4e0: 6963 740d 0a20 2020 2020 2020 2022 2222  ict..        """
+0000f4f0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000f500: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+0000f510: 2268 6973 746f 7279 225d                 "history"]
```

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/gprofiler.py` & `mosaicmpi-2.5.0/src/mosaicmpi/gprofiler.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/integration.py` & `mosaicmpi-2.5.0/src/mosaicmpi/integration.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/nancorrmp.py` & `mosaicmpi-2.5.0/src/mosaicmpi/nancorrmp.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/network.py` & `mosaicmpi-2.5.0/src/mosaicmpi/network.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/orphan.py` & `mosaicmpi-2.5.0/src/mosaicmpi/orphan.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/plots.py` & `mosaicmpi-2.5.0/src/mosaicmpi/plots.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi/utils.py` & `mosaicmpi-2.5.0/src/mosaicmpi/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi.egg-info/PKG-INFO` & `mosaicmpi-2.5.0/src/mosaicmpi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicmpi
-Version: 2.4.9
+Version: 2.5.0
 Summary: mosaicMPI: Mosaic Multi-resolution Program Integration
 Home-page: https://github.com/MorrissyLab/mosaicMPI
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/mosaicMPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,54 +30,54 @@
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
 Requires-Dist: fastcluster
 Requires-Dist: tqdm
 
 ![mosaicMPI logo](https://github.com/MorrissyLab/mosaicMPI/blob/main/docs/source/_static/img/logo.png?raw=True)
 
-# mosaicMPI: mosaic multi-resolution program integration
+# mosaicMPI: Mosaic Multi-resolution Program Integration
 
-![version badge](https://img.shields.io/badge/version-2.4.9-blue)
+![version badge](https://img.shields.io/badge/version-2.5.0-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mosaicmpi.svg)](https://pypi.org/project/mosaicmpi/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/mosaicmpi)](https://anaconda.org/conda-forge/mosaicmpi/)
 [![Documentation status](https://readthedocs.org/projects/mosaicmpi/badge/?version=latest&style=flat)](https://mosaicmpi.readthedocs.io)
 [![Downloads](https://static.pepy.tech/badge/mosaicmpi)](https://pepy.tech/project/mosaicmpi)
 [![Stars](https://img.shields.io/github/stars/MorrissyLab/mosaicMPI?logo=GitHub&color=yellow)](https://github.com/MorrissyLab/mosaicMPI/stargazers)
 [![License](https://img.shields.io/pypi/l/mosaicmpi.svg)](https://github.com/MorrissyLab/mosaicMPI/blob/main/LICENSE)
 [![DOI:10.1101/2023.08.18.553919](http://img.shields.io/badge/DOI-10.1101/2023.08.18.553919-B31B1B.svg)](https://doi.org/10.1101/2023.08.18.553919)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Sorana Morrissy](https://github.com/ancasorana)
 
 Contributors: Hyojin Song, Aaron Gillmor, Gurveer Gill, Courtney Hall
 
-**mosaicMPI** is a Python package enabling mosaic integration of bulk, single-cell, and spatial expression data through program-level integration.
-Programs are first discovered using consensus non-negative matrix factorization and then integrated using a flexible network-based approach to
-group similar programs together across resolutions and datasets. Program communities are then interpreted using sample/cell metadata and gene set analyses. Integrative program communities enable metadata transfer across datasets.
+**mosaicMPI** is a Python package for enabling mosaic integration of bulk, single-cell, and spatial expression data through program-level integration. Programs are first discovered using unsupervised deconvolution (consensus non-negative matrix factorization, cNMF) across multiple ranks separately for each dataset. A flexible network-based approach groups similar programs together across resolutions and datasets. Program communities are then interpreted using sample/cell metadata and gene set analyses. Integrative program communities enable metadata transfer across datasets.
 
 ## ⚡Main Features
 
 Here are just a few of the things that mosaicMPI does well:
 
 - Identifies interpretable, non-negative programs at multiple resolutions
 - Mosaic integration does not require subsetting features/genes to
   a shared or overdispersed subset
 - Multi-omics integration without shared sample IDs
-- Ideal for incremental integration (adding datasets one at a time) since
+- Incremental integration (adding datasets one at a time) since
   deconvolution is performed independently on each dataset
-- Integration performs well even when the datasets have mismatched features
-  (eg. Microarray, RNA-Seq, Proteomics) or sparsity (eg single-cell vs bulk RNA-Seq and ATAC-Seq)
+- High performance integration of of datasets with mismatched features
+  (eg. Microarray, RNA-Seq, Proteomics) or sparsity (eg. single-cell vs. bulk)
 - Metadata transfer across datasets
-- Command-line interface for rapid data exploration and python
-  interface for extensibility and flexibility
+
+mosaicMPI is usable via:
+- command-line interface for rapid data exploration and integration
+- python interface for extensibility and flexibility
 
 ## 🔧 Install
 
 ### 🧰 System Requirements
 
-- Compatible with and tested on OS X, Windows and Linux systems
+- Compatible with OS X, Windows and Linux systems
 - Memory usage depends on size and number of datasets
 
 ### ✨ Latest Release
 Install the package with `conda`:
 ```bash
 # create an environment called mosaic and install
 conda create -n mosaic -c conda-forge mosaicmpi
@@ -95,8 +95,8 @@
 
 ## 📖 Documentation
 
 Read the [documentation](https://mosaicmpi.readthedocs.io/).
 
 ## 💭 Getting Help
 
-For errors arising during use of mosaicMPI, create and browse issues in the [GitHub "issues" tab](https://github.com/MorrissyLab/mosaicMPI/issues).
+For questions arising during use of mosaicMPI, create and browse issues in the [GitHub "issues" tab](https://github.com/MorrissyLab/mosaicMPI/issues).
```

### Comparing `mosaicmpi-2.4.9/src/mosaicmpi.egg-info/SOURCES.txt` & `mosaicmpi-2.5.0/src/mosaicmpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

