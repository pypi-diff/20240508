# Comparing `tmp/adtoolbox-0.1.0.tar.gz` & `tmp/adtoolbox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adtoolbox-0.1.0.tar", max compression
+gzip compressed data, was "adtoolbox-0.2.0.tar", max compression
```

## Comparing `adtoolbox-0.1.0.tar` & `adtoolbox-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      602 2024-05-07 21:44:54.922798 adtoolbox-0.1.0/README.md
--rw-r--r--   0        0        0    10244 2024-04-30 20:19:14.071995 adtoolbox-0.1.0/adtoolbox/.DS_Store
--rw-r--r--   0        0        0     1157 2024-05-03 20:27:38.209459 adtoolbox-0.1.0/adtoolbox/__init__.py
--rw-r--r--   0        0        0      104 2023-02-15 22:46:03.557748 adtoolbox-0.1.0/adtoolbox/__main__.py
--rw-r--r--   0        0        0   128056 2024-05-07 05:53:37.443565 adtoolbox-0.1.0/adtoolbox/adm.py
--rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.1.0/adtoolbox/bio_struct.py
--rwxr-xr-x   0        0        0    29971 2024-05-07 18:50:52.363455 adtoolbox-0.1.0/adtoolbox/cli.py
--rw-r--r--   0        0        0    16774 2024-05-07 04:58:30.708719 adtoolbox-0.1.0/adtoolbox/configs.py
--rw-r--r--   0        0        0   108577 2024-05-02 21:59:44.885729 adtoolbox-0.1.0/adtoolbox/core.py
--rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.1.0/adtoolbox/metagenomics_report.py
--rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.1.0/adtoolbox/optimize.py
--rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.1.0/adtoolbox/pipeline.py
--rw-r--r--   0        0        0     6148 2024-04-30 20:21:01.993885 adtoolbox-0.1.0/adtoolbox/pkg_data/.DS_Store
--rw-r--r--   0        0        0       57 2024-05-07 18:50:54.656200 adtoolbox-0.1.0/adtoolbox/pkg_data/ADToolbox_Configs.json
--rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.1.0/adtoolbox/pkg_data/Modified_ADM_Map.json
--rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.1.0/adtoolbox/pkg_data/Modified_ADM_Model.json
--rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.1.0/adtoolbox/pkg_data/README.md
--rw-r--r--   0        0        0     1123 2024-05-01 22:24:41.310110 adtoolbox-0.1.0/adtoolbox/pkg_data/qiime_template_paired.txt
--rw-r--r--   0        0        0     1090 2023-01-24 23:43:30.618643 adtoolbox-0.1.0/adtoolbox/pkg_data/qiime_template_single.txt
--rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.1.0/adtoolbox/pkg_data/slurm_template.txt
--rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.1.0/adtoolbox/stats.py
--rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.1.0/adtoolbox/tables.py
--rw-r--r--   0        0        0    15931 2024-02-01 18:57:40.645825 adtoolbox-0.1.0/adtoolbox/utils.py
--rw-r--r--   0        0        0      748 2023-02-18 19:25:07.601647 adtoolbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1773 2024-05-08 16:53:19.057012 adtoolbox-0.1.0/setup.py
--rw-r--r--   0        0        0     1575 2024-05-08 16:53:19.057225 adtoolbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      602 2024-05-07 21:44:54.922798 adtoolbox-0.2.0/README.md
+-rw-r--r--   0        0        0    10244 2024-04-30 20:19:14.071995 adtoolbox-0.2.0/adtoolbox/.DS_Store
+-rw-r--r--   0        0        0     1157 2024-05-03 20:27:38.209459 adtoolbox-0.2.0/adtoolbox/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.2.0/adtoolbox/__main__.py
+-rw-r--r--   0        0        0   128057 2024-05-08 17:13:08.818845 adtoolbox-0.2.0/adtoolbox/adm.py
+-rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.2.0/adtoolbox/bio_struct.py
+-rwxr-xr-x   0        0        0    29972 2024-05-08 17:23:18.629590 adtoolbox-0.2.0/adtoolbox/cli.py
+-rw-r--r--   0        0        0    16774 2024-05-07 04:58:30.708719 adtoolbox-0.2.0/adtoolbox/configs.py
+-rw-r--r--   0        0        0   108577 2024-05-02 21:59:44.885729 adtoolbox-0.2.0/adtoolbox/core.py
+-rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.2.0/adtoolbox/metagenomics_report.py
+-rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.2.0/adtoolbox/optimize.py
+-rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.2.0/adtoolbox/pipeline.py
+-rw-r--r--   0        0        0     6148 2024-04-30 20:21:01.993885 adtoolbox-0.2.0/adtoolbox/pkg_data/.DS_Store
+-rw-r--r--   0        0        0       16 2024-05-08 17:26:06.999520 adtoolbox-0.2.0/adtoolbox/pkg_data/ADToolbox_Configs.json
+-rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.2.0/adtoolbox/pkg_data/Modified_ADM_Map.json
+-rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.2.0/adtoolbox/pkg_data/Modified_ADM_Model.json
+-rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.2.0/adtoolbox/pkg_data/README.md
+-rw-r--r--   0        0        0     1123 2024-05-01 22:24:41.310110 adtoolbox-0.2.0/adtoolbox/pkg_data/qiime_template_paired.txt
+-rw-r--r--   0        0        0     1090 2023-01-24 23:43:30.618643 adtoolbox-0.2.0/adtoolbox/pkg_data/qiime_template_single.txt
+-rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.2.0/adtoolbox/pkg_data/slurm_template.txt
+-rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.2.0/adtoolbox/stats.py
+-rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.2.0/adtoolbox/tables.py
+-rw-r--r--   0        0        0    15931 2024-02-01 18:57:40.645825 adtoolbox-0.2.0/adtoolbox/utils.py
+-rw-r--r--   0        0        0      748 2024-05-08 17:28:38.270406 adtoolbox-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1773 2024-05-08 17:28:45.063110 adtoolbox-0.2.0/setup.py
+-rw-r--r--   0        0        0     1575 2024-05-08 17:28:45.063294 adtoolbox-0.2.0/PKG-INFO
```

### Comparing `adtoolbox-0.1.0/README.md` & `adtoolbox-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/.DS_Store` & `adtoolbox-0.2.0/adtoolbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/__init__.py` & `adtoolbox-0.2.0/adtoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/adm.py` & `adtoolbox-0.2.0/adtoolbox/adm.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from dash import Dash, dcc, html, Input, Output,dash_table
 from core import Database as Database
 from core import SeedDB as SeedDB
 from core import Feed
 import pandas as pd
 import dash_bootstrap_components as dbc
 import utils
-from __init__ import Main_Dir,PKG_DATA
+from .__init__ import Main_Dir,PKG_DATA
 import dash_escher
 import configs
 import time
 
 ### Note ###
 # The following code is a modified version of the code from the PyADM1 package
 # It is extensively based on PyADM1, and I would like to thank the author of PyADM1 for this work
```

### Comparing `adtoolbox-0.1.0/adtoolbox/bio_struct.py` & `adtoolbox-0.2.0/adtoolbox/bio_struct.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/cli.py` & `adtoolbox-0.2.0/adtoolbox/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 from re import M
 import configs
 import metagenomics_report
 import core
-from __init__ import __version__,Main_Dir
+from adtoolbox import __version__,Main_Dir
 from rich.console import Console
 import rich
 import adm
 from rich.table import Table
 from rich.prompt import Prompt
 from rich import markdown
 import json
```

### Comparing `adtoolbox-0.1.0/adtoolbox/configs.py` & `adtoolbox-0.2.0/adtoolbox/configs.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/core.py` & `adtoolbox-0.2.0/adtoolbox/core.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/metagenomics_report.py` & `adtoolbox-0.2.0/adtoolbox/metagenomics_report.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/optimize.py` & `adtoolbox-0.2.0/adtoolbox/optimize.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/pipeline.py` & `adtoolbox-0.2.0/adtoolbox/pipeline.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/pkg_data/.DS_Store` & `adtoolbox-0.2.0/adtoolbox/pkg_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/pkg_data/Modified_ADM_Map.json` & `adtoolbox-0.2.0/adtoolbox/pkg_data/Modified_ADM_Map.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/pkg_data/Modified_ADM_Model.json` & `adtoolbox-0.2.0/adtoolbox/pkg_data/Modified_ADM_Model.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/pkg_data/README.md` & `adtoolbox-0.2.0/adtoolbox/pkg_data/README.md`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/pkg_data/qiime_template_paired.txt` & `adtoolbox-0.2.0/adtoolbox/pkg_data/qiime_template_paired.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/pkg_data/qiime_template_single.txt` & `adtoolbox-0.2.0/adtoolbox/pkg_data/qiime_template_single.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/stats.py` & `adtoolbox-0.2.0/adtoolbox/stats.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/tables.py` & `adtoolbox-0.2.0/adtoolbox/tables.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/adtoolbox/utils.py` & `adtoolbox-0.2.0/adtoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.1.0/pyproject.toml` & `adtoolbox-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adtoolbox"
-version = "0.1.0"
+version = "0.2.0"
 description = "A tool for modeling and optimization of anaerobic digestion process."
 authors = ["ParsaGhadermazi <54489047+ParsaGhadermazi@users.noreply.github.com>"]
 readme= "README.md"
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 bs4 = "^0.0.1"
 dash = "^2.4.1"
```

### Comparing `adtoolbox-0.1.0/setup.py` & `adtoolbox-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'sympy>=1.10.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ADToolbox = adtoolbox.__main__:main']}
 
 setup_kwargs = {
     'name': 'adtoolbox',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'A tool for modeling and optimization of anaerobic digestion process.',
     'long_description': '# Toolbox Overview\nParsa Ghadermazi \nparsa96@colostate.edu\n\nAD Toolbox is developed in Chan Lab at Colorado State University. The main goal of this toolbox is to provide the tools that are useful for modeling and optimization of anaerobic digestion process.\n\nInterested in trying ADToolbox? Run the notebooks on Binder:\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)\n\nADToolbox comes with a detailed documentation website. You can access this website using the link below:\n\n** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **\n\n\n',
     'author': 'ParsaGhadermazi',
     'author_email': '54489047+ParsaGhadermazi@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `adtoolbox-0.1.0/PKG-INFO` & `adtoolbox-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adtoolbox
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool for modeling and optimization of anaerobic digestion process.
 Author: ParsaGhadermazi
 Author-email: 54489047+ParsaGhadermazi@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

