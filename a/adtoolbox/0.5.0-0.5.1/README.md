# Comparing `tmp/adtoolbox-0.5.0.tar.gz` & `tmp/adtoolbox-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adtoolbox-0.5.0.tar", max compression
+gzip compressed data, was "adtoolbox-0.5.1.tar", max compression
```

## Comparing `adtoolbox-0.5.0.tar` & `adtoolbox-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      815 2024-05-08 17:32:14.704061 adtoolbox-0.5.0/README.md
--rw-r--r--   0        0        0    10244 2024-05-08 17:37:32.568953 adtoolbox-0.5.0/adtoolbox/.DS_Store
--rw-r--r--   0        0        0     1419 2024-05-08 19:32:25.727517 adtoolbox-0.5.0/adtoolbox/__init__.py
--rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.5.0/adtoolbox/__main__.py
--rw-r--r--   0        0        0   128039 2024-05-08 17:48:13.221816 adtoolbox-0.5.0/adtoolbox/adm.py
--rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.5.0/adtoolbox/bio_struct.py
--rwxr-xr-x   0        0        0    29972 2024-05-08 17:23:18.629590 adtoolbox-0.5.0/adtoolbox/cli.py
--rw-r--r--   0        0        0    16774 2024-05-07 04:58:30.708719 adtoolbox-0.5.0/adtoolbox/configs.py
--rw-r--r--   0        0        0   108577 2024-05-02 21:59:44.885729 adtoolbox-0.5.0/adtoolbox/core.py
--rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.5.0/adtoolbox/metagenomics_report.py
--rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.5.0/adtoolbox/optimize.py
--rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.5.0/adtoolbox/pipeline.py
--rw-r--r--   0        0        0     6148 2024-05-08 17:42:50.899853 adtoolbox-0.5.0/adtoolbox/pkg_data/.DS_Store
--rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.5.0/adtoolbox/pkg_data/Modified_ADM_Map.json
--rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.5.0/adtoolbox/pkg_data/Modified_ADM_Model.json
--rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.5.0/adtoolbox/pkg_data/README.md
--rw-r--r--   0        0        0     1123 2024-05-01 22:24:41.310110 adtoolbox-0.5.0/adtoolbox/pkg_data/qiime_template_paired.txt
--rw-r--r--   0        0        0     1090 2023-01-24 23:43:30.618643 adtoolbox-0.5.0/adtoolbox/pkg_data/qiime_template_single.txt
--rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.5.0/adtoolbox/pkg_data/slurm_template.txt
--rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.5.0/adtoolbox/stats.py
--rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.5.0/adtoolbox/tables.py
--rw-r--r--   0        0        0    15931 2024-02-01 18:57:40.645825 adtoolbox-0.5.0/adtoolbox/utils.py
--rw-r--r--   0        0        0      748 2024-05-08 19:32:39.129625 adtoolbox-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4243 2024-05-08 19:32:43.324141 adtoolbox-0.5.0/setup.py
--rw-r--r--   0        0        0     1788 2024-05-08 19:32:43.324336 adtoolbox-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      815 2024-05-08 17:32:14.704061 adtoolbox-0.5.1/README.md
+-rw-r--r--   0        0        0    10244 2024-05-08 17:37:32.568953 adtoolbox-0.5.1/adtoolbox/.DS_Store
+-rw-r--r--   0        0        0     1441 2024-05-08 19:34:33.066301 adtoolbox-0.5.1/adtoolbox/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.5.1/adtoolbox/__main__.py
+-rw-r--r--   0        0        0   128039 2024-05-08 17:48:13.221816 adtoolbox-0.5.1/adtoolbox/adm.py
+-rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.5.1/adtoolbox/bio_struct.py
+-rwxr-xr-x   0        0        0    29972 2024-05-08 17:23:18.629590 adtoolbox-0.5.1/adtoolbox/cli.py
+-rw-r--r--   0        0        0    16774 2024-05-07 04:58:30.708719 adtoolbox-0.5.1/adtoolbox/configs.py
+-rw-r--r--   0        0        0   108577 2024-05-02 21:59:44.885729 adtoolbox-0.5.1/adtoolbox/core.py
+-rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.5.1/adtoolbox/metagenomics_report.py
+-rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.5.1/adtoolbox/optimize.py
+-rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.5.1/adtoolbox/pipeline.py
+-rw-r--r--   0        0        0     6148 2024-05-08 17:42:50.899853 adtoolbox-0.5.1/adtoolbox/pkg_data/.DS_Store
+-rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.5.1/adtoolbox/pkg_data/Modified_ADM_Map.json
+-rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.5.1/adtoolbox/pkg_data/Modified_ADM_Model.json
+-rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.5.1/adtoolbox/pkg_data/README.md
+-rw-r--r--   0        0        0     1123 2024-05-01 22:24:41.310110 adtoolbox-0.5.1/adtoolbox/pkg_data/qiime_template_paired.txt
+-rw-r--r--   0        0        0     1090 2023-01-24 23:43:30.618643 adtoolbox-0.5.1/adtoolbox/pkg_data/qiime_template_single.txt
+-rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.5.1/adtoolbox/pkg_data/slurm_template.txt
+-rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.5.1/adtoolbox/stats.py
+-rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.5.1/adtoolbox/tables.py
+-rw-r--r--   0        0        0    15931 2024-02-01 18:57:40.645825 adtoolbox-0.5.1/adtoolbox/utils.py
+-rw-r--r--   0        0        0      748 2024-05-08 19:34:42.607929 adtoolbox-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4243 2024-05-08 19:34:45.696186 adtoolbox-0.5.1/setup.py
+-rw-r--r--   0        0        0     1788 2024-05-08 19:34:45.696380 adtoolbox-0.5.1/PKG-INFO
```

### Comparing `adtoolbox-0.5.0/README.md` & `adtoolbox-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/.DS_Store` & `adtoolbox-0.5.1/adtoolbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/__init__.py` & `adtoolbox-0.5.1/adtoolbox/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import rich
 from rich.prompt import Prompt
 import sys
 
 """Project Setup for ADToolBox."""
 
 __version__ = "1.0.0"
-__all__=["adm","configs","__main__","cli","core","optimize","pipeline","utils"]
+__all__=["adm","configs","__main__","cli","core","optimize","pipeline","utils","Main_Dir","PKG_DATA"]
 
 sys.path.append(os.path.join(os.path.dirname(__file__)))
 
 PKG_DATA=os.path.join(os.path.dirname(os.path.realpath(__file__)),"pkg_data")
 
 if not os.path.exists(os.path.join(PKG_DATA,"ADToolbox_Configs.json")):
     with open(os.path.join(PKG_DATA,"ADToolbox_Configs.json"),"w") as f:
```

### Comparing `adtoolbox-0.5.0/adtoolbox/adm.py` & `adtoolbox-0.5.1/adtoolbox/adm.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/bio_struct.py` & `adtoolbox-0.5.1/adtoolbox/bio_struct.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/cli.py` & `adtoolbox-0.5.1/adtoolbox/cli.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/configs.py` & `adtoolbox-0.5.1/adtoolbox/configs.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/core.py` & `adtoolbox-0.5.1/adtoolbox/core.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/metagenomics_report.py` & `adtoolbox-0.5.1/adtoolbox/metagenomics_report.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/optimize.py` & `adtoolbox-0.5.1/adtoolbox/optimize.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/pipeline.py` & `adtoolbox-0.5.1/adtoolbox/pipeline.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/pkg_data/.DS_Store` & `adtoolbox-0.5.1/adtoolbox/pkg_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/pkg_data/Modified_ADM_Map.json` & `adtoolbox-0.5.1/adtoolbox/pkg_data/Modified_ADM_Map.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/pkg_data/Modified_ADM_Model.json` & `adtoolbox-0.5.1/adtoolbox/pkg_data/Modified_ADM_Model.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/pkg_data/README.md` & `adtoolbox-0.5.1/adtoolbox/pkg_data/README.md`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/pkg_data/qiime_template_paired.txt` & `adtoolbox-0.5.1/adtoolbox/pkg_data/qiime_template_paired.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/pkg_data/qiime_template_single.txt` & `adtoolbox-0.5.1/adtoolbox/pkg_data/qiime_template_single.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/stats.py` & `adtoolbox-0.5.1/adtoolbox/stats.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/tables.py` & `adtoolbox-0.5.1/adtoolbox/tables.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/adtoolbox/utils.py` & `adtoolbox-0.5.1/adtoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.0/pyproject.toml` & `adtoolbox-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adtoolbox"
-version = "0.5.0"
+version = "0.5.1"
 description = "A tool for modeling and optimization of anaerobic digestion process."
 authors = ["ParsaGhadermazi <54489047+ParsaGhadermazi@users.noreply.github.com>"]
 readme= "README.md"
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 bs4 = "^0.0.1"
 dash = "^2.4.1"
```

### Comparing `adtoolbox-0.5.0/setup.py` & `adtoolbox-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
  'sympy>=1.10.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ADToolbox = adtoolbox.__main__:main']}
 
 setup_kwargs = {
     'name': 'adtoolbox',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'A tool for modeling and optimization of anaerobic digestion process.',
     'long_description': '# Toolbox Overview\nParsa Ghadermazi \nparsa96@colostate.edu\n\nAD Toolbox is developed in Chan Lab at Colorado State University. The main goal of this toolbox is to provide the tools that are useful for modeling and optimization of anaerobic digestion process.\n\nInterested in trying ADToolbox? Run the notebooks on Binder or Colab:\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)\n<a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">\n  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\nADToolbox comes with a detailed documentation website. You can access this website using the link below:\n\n** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **\n\n\n',
     'author': 'ParsaGhadermazi',
     'author_email': '54489047+ParsaGhadermazi@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `adtoolbox-0.5.0/PKG-INFO` & `adtoolbox-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adtoolbox
-Version: 0.5.0
+Version: 0.5.1
 Summary: A tool for modeling and optimization of anaerobic digestion process.
 Author: ParsaGhadermazi
 Author-email: 54489047+ParsaGhadermazi@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

