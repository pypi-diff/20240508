# Comparing `tmp/Garfield-0.1.0.tar.gz` & `tmp/Garfield-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Garfield-0.1.0.tar", last modified: Wed May  8 07:38:12 2024, max compression
+gzip compressed data, was "Garfield-0.1.1.tar", last modified: Wed May  8 10:16:27 2024, max compression
```

## Comparing `Garfield-0.1.0.tar` & `Garfield-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 07:38:12.743060 Garfield-0.1.0/
-drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 07:38:12.735060 Garfield-0.1.0/Garfield/
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)      320 2024-05-08 06:58:29.000000 Garfield-0.1.0/Garfield/__init__.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     8091 2024-05-08 06:58:28.000000 Garfield-0.1.0/Garfield/_settings.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)       50 2024-05-08 06:58:29.000000 Garfield-0.1.0/Garfield/_version.py
-drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 07:38:12.731059 Garfield-0.1.0/Garfield/data/
-drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 07:38:12.739060 Garfield-0.1.0/Garfield/data/gene_anno/
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)   811724 2024-05-08 06:58:24.000000 Garfield-0.1.0/Garfield/data/gene_anno/hg19_genes.bed
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)  1365384 2024-05-08 06:58:25.000000 Garfield-0.1.0/Garfield/data/gene_anno/hg38_genes.bed
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)  1215424 2024-05-08 06:58:25.000000 Garfield-0.1.0/Garfield/data/gene_anno/mm10_genes.bed
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)  1258181 2024-05-08 06:58:26.000000 Garfield-0.1.0/Garfield/data/gene_anno/mm9_genes.bed
-drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 07:38:12.743060 Garfield-0.1.0/Garfield/model/
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    15537 2024-05-08 06:58:26.000000 Garfield-0.1.0/Garfield/model/GarfieldTrainer.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     3149 2024-05-08 06:58:26.000000 Garfield-0.1.0/Garfield/model/Garfield_net.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)      599 2024-05-08 06:58:27.000000 Garfield-0.1.0/Garfield/model/__init__.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    28466 2024-05-08 06:58:26.000000 Garfield-0.1.0/Garfield/model/_layers.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     5301 2024-05-08 06:58:27.000000 Garfield-0.1.0/Garfield/model/_loss.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     3809 2024-05-08 06:58:27.000000 Garfield-0.1.0/Garfield/model/_tools.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     2235 2024-05-08 06:58:27.000000 Garfield-0.1.0/Garfield/model/_utils.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     4184 2024-05-08 06:58:26.000000 Garfield-0.1.0/Garfield/model/metrics.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    20924 2024-05-08 06:58:26.000000 Garfield-0.1.0/Garfield/model/prepare_Data.py
-drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 07:38:12.743060 Garfield-0.1.0/Garfield/preprocessing/
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)      657 2024-05-08 06:58:28.000000 Garfield-0.1.0/Garfield/preprocessing/__init__.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     8789 2024-05-08 06:58:28.000000 Garfield-0.1.0/Garfield/preprocessing/_graph.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     5498 2024-05-08 06:58:28.000000 Garfield-0.1.0/Garfield/preprocessing/_pca.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    10655 2024-05-08 06:58:28.000000 Garfield-0.1.0/Garfield/preprocessing/_qc.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    21610 2024-05-08 06:58:28.000000 Garfield-0.1.0/Garfield/preprocessing/_utils.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    13540 2024-05-08 06:58:27.000000 Garfield-0.1.0/Garfield/preprocessing/preprocess.py
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     5316 2024-05-08 06:58:27.000000 Garfield-0.1.0/Garfield/preprocessing/read_adata.py
-drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 07:38:12.735060 Garfield-0.1.0/Garfield.egg-info/
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     5196 2024-05-08 07:38:12.000000 Garfield-0.1.0/Garfield.egg-info/PKG-INFO
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)      889 2024-05-08 07:38:12.000000 Garfield-0.1.0/Garfield.egg-info/SOURCES.txt
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)        1 2024-05-08 07:38:12.000000 Garfield-0.1.0/Garfield.egg-info/dependency_links.txt
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)      274 2024-05-08 07:38:12.000000 Garfield-0.1.0/Garfield.egg-info/requires.txt
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)        9 2024-05-08 07:38:12.000000 Garfield-0.1.0/Garfield.egg-info/top_level.txt
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     1498 2024-05-08 06:58:29.000000 Garfield-0.1.0/LICENSE
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     5196 2024-05-08 07:38:12.743060 Garfield-0.1.0/PKG-INFO
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     4710 2024-05-08 06:58:29.000000 Garfield-0.1.0/README.md
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)       38 2024-05-08 07:38:12.743060 Garfield-0.1.0/setup.cfg
--rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     1087 2024-05-08 07:37:04.000000 Garfield-0.1.0/setup.py
+drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 10:16:27.336049 Garfield-0.1.1/
+drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 10:16:27.324049 Garfield-0.1.1/Garfield/
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)      320 2024-05-08 06:58:29.000000 Garfield-0.1.1/Garfield/__init__.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     8091 2024-05-08 06:58:28.000000 Garfield-0.1.1/Garfield/_settings.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)       50 2024-05-08 10:14:03.000000 Garfield-0.1.1/Garfield/_version.py
+drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 10:16:27.324049 Garfield-0.1.1/Garfield/data/
+drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 10:16:27.332049 Garfield-0.1.1/Garfield/data/gene_anno/
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)   811724 2024-05-08 06:58:24.000000 Garfield-0.1.1/Garfield/data/gene_anno/hg19_genes.bed
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)  1365384 2024-05-08 06:58:25.000000 Garfield-0.1.1/Garfield/data/gene_anno/hg38_genes.bed
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)  1215424 2024-05-08 06:58:25.000000 Garfield-0.1.1/Garfield/data/gene_anno/mm10_genes.bed
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)  1258181 2024-05-08 06:58:26.000000 Garfield-0.1.1/Garfield/data/gene_anno/mm9_genes.bed
+drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 10:16:27.332049 Garfield-0.1.1/Garfield/model/
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    15537 2024-05-08 06:58:26.000000 Garfield-0.1.1/Garfield/model/GarfieldTrainer.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     3149 2024-05-08 06:58:26.000000 Garfield-0.1.1/Garfield/model/Garfield_net.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)      599 2024-05-08 06:58:27.000000 Garfield-0.1.1/Garfield/model/__init__.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    28466 2024-05-08 06:58:26.000000 Garfield-0.1.1/Garfield/model/_layers.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     5301 2024-05-08 06:58:27.000000 Garfield-0.1.1/Garfield/model/_loss.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     3809 2024-05-08 06:58:27.000000 Garfield-0.1.1/Garfield/model/_tools.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     2235 2024-05-08 06:58:27.000000 Garfield-0.1.1/Garfield/model/_utils.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     4184 2024-05-08 06:58:26.000000 Garfield-0.1.1/Garfield/model/metrics.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    20924 2024-05-08 06:58:26.000000 Garfield-0.1.1/Garfield/model/prepare_Data.py
+drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 10:16:27.336049 Garfield-0.1.1/Garfield/preprocessing/
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)      657 2024-05-08 06:58:28.000000 Garfield-0.1.1/Garfield/preprocessing/__init__.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     8789 2024-05-08 06:58:28.000000 Garfield-0.1.1/Garfield/preprocessing/_graph.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     5498 2024-05-08 06:58:28.000000 Garfield-0.1.1/Garfield/preprocessing/_pca.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    10655 2024-05-08 06:58:28.000000 Garfield-0.1.1/Garfield/preprocessing/_qc.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    21610 2024-05-08 06:58:28.000000 Garfield-0.1.1/Garfield/preprocessing/_utils.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)    13540 2024-05-08 06:58:27.000000 Garfield-0.1.1/Garfield/preprocessing/preprocess.py
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     5316 2024-05-08 06:58:27.000000 Garfield-0.1.1/Garfield/preprocessing/read_adata.py
+drwxrwxr-x   0 zhouweige  (1003) zhouweige  (1004)        0 2024-05-08 10:16:27.324049 Garfield-0.1.1/Garfield.egg-info/
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     5196 2024-05-08 10:16:27.000000 Garfield-0.1.1/Garfield.egg-info/PKG-INFO
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)      889 2024-05-08 10:16:27.000000 Garfield-0.1.1/Garfield.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)        1 2024-05-08 10:16:27.000000 Garfield-0.1.1/Garfield.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)      274 2024-05-08 10:16:27.000000 Garfield-0.1.1/Garfield.egg-info/requires.txt
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)        9 2024-05-08 10:16:27.000000 Garfield-0.1.1/Garfield.egg-info/top_level.txt
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     1498 2024-05-08 06:58:29.000000 Garfield-0.1.1/LICENSE
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     5196 2024-05-08 10:16:27.336049 Garfield-0.1.1/PKG-INFO
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     4710 2024-05-08 07:40:02.000000 Garfield-0.1.1/README.md
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)       38 2024-05-08 10:16:27.336049 Garfield-0.1.1/setup.cfg
+-rw-rw-r--   0 zhouweige  (1003) zhouweige  (1004)     1078 2024-05-08 10:13:24.000000 Garfield-0.1.1/setup.py
```

### Comparing `Garfield-0.1.0/Garfield/_settings.py` & `Garfield-0.1.1/Garfield/_settings.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/data/gene_anno/hg19_genes.bed` & `Garfield-0.1.1/Garfield/data/gene_anno/hg19_genes.bed`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/data/gene_anno/hg38_genes.bed` & `Garfield-0.1.1/Garfield/data/gene_anno/hg38_genes.bed`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/data/gene_anno/mm10_genes.bed` & `Garfield-0.1.1/Garfield/data/gene_anno/mm10_genes.bed`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/data/gene_anno/mm9_genes.bed` & `Garfield-0.1.1/Garfield/data/gene_anno/mm9_genes.bed`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/model/GarfieldTrainer.py` & `Garfield-0.1.1/Garfield/model/GarfieldTrainer.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/model/Garfield_net.py` & `Garfield-0.1.1/Garfield/model/Garfield_net.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/model/__init__.py` & `Garfield-0.1.1/Garfield/model/__init__.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/model/_layers.py` & `Garfield-0.1.1/Garfield/model/_layers.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/model/_loss.py` & `Garfield-0.1.1/Garfield/model/_loss.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/model/_tools.py` & `Garfield-0.1.1/Garfield/model/_tools.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/model/_utils.py` & `Garfield-0.1.1/Garfield/model/_utils.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/model/metrics.py` & `Garfield-0.1.1/Garfield/model/metrics.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/model/prepare_Data.py` & `Garfield-0.1.1/Garfield/model/prepare_Data.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/preprocessing/__init__.py` & `Garfield-0.1.1/Garfield/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/preprocessing/_graph.py` & `Garfield-0.1.1/Garfield/preprocessing/_graph.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/preprocessing/_pca.py` & `Garfield-0.1.1/Garfield/preprocessing/_pca.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/preprocessing/_qc.py` & `Garfield-0.1.1/Garfield/preprocessing/_qc.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/preprocessing/_utils.py` & `Garfield-0.1.1/Garfield/preprocessing/_utils.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/preprocessing/preprocess.py` & `Garfield-0.1.1/Garfield/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield/preprocessing/read_adata.py` & `Garfield-0.1.1/Garfield/preprocessing/read_adata.py`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/Garfield.egg-info/PKG-INFO` & `Garfield-0.1.1/Garfield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Garfield
-Version: 0.1.0
+Version: 0.1.1
 Summary: Garfield: Graph-based Contrastive Learning enable Fast Single-Cell Embedding
 Home-page: https://github.com/zhou-1314/Garfield
 Author: Weige Zhou
 Author-email: zhouwg1314@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -55,15 +55,15 @@
 ├── requirements.txt
 └── setup.py
 ```
 
 ## Installation
 Please install `Garfield` from pypi with:
 ```bash
-pip install garfield
+pip install Garfield
 ```
 
 install from Github:
 
 ```
 pip install git+https://github.com/zhou-1314/Garfield.git
 ```
```

### Comparing `Garfield-0.1.0/Garfield.egg-info/SOURCES.txt` & `Garfield-0.1.1/Garfield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/LICENSE` & `Garfield-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Garfield-0.1.0/PKG-INFO` & `Garfield-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Garfield
-Version: 0.1.0
+Version: 0.1.1
 Summary: Garfield: Graph-based Contrastive Learning enable Fast Single-Cell Embedding
 Home-page: https://github.com/zhou-1314/Garfield
 Author: Weige Zhou
 Author-email: zhouwg1314@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -55,15 +55,15 @@
 ├── requirements.txt
 └── setup.py
 ```
 
 ## Installation
 Please install `Garfield` from pypi with:
 ```bash
-pip install garfield
+pip install Garfield
 ```
 
 install from Github:
 
 ```
 pip install git+https://github.com/zhou-1314/Garfield.git
 ```
```

### Comparing `Garfield-0.1.0/README.md` & `Garfield-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ├── requirements.txt
 └── setup.py
 ```
 
 ## Installation
 Please install `Garfield` from pypi with:
 ```bash
-pip install garfield
+pip install Garfield
 ```
 
 install from Github:
 
 ```
 pip install git+https://github.com/zhou-1314/Garfield.git
 ```
```

### Comparing `Garfield-0.1.0/setup.py` & `Garfield-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 version = {}
 with open("Garfield/_version.py") as fp:
     exec(fp.read(), version)
 
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
 setup(
     name='Garfield',
     version=version['__version__'],
     author='Weige Zhou',
     author_email='zhouwg1314@gmail.com',
     license='BSD',
     description='Garfield: Graph-based Contrastive Learning enable Fast Single-Cell Embedding',
@@ -23,14 +26,11 @@
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
-    install_requires=[
-        x.strip() for x in
-        Path('requirements.txt').read_text('utf-8').splitlines()
-    ],
+    install_requires=requirements,
     include_package_data=True,
     package_data={"Garfield": ["data/gene_anno/*.bed"]}
 )
```

