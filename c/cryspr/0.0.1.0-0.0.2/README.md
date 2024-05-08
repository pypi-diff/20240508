# Comparing `tmp/cryspr-0.0.1.0.tar.gz` & `tmp/cryspr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryspr-0.0.1.0.tar", last modified: Sun May  5 22:56:18 2024, max compression
+gzip compressed data, was "cryspr-0.0.2.tar", last modified: Wed May  8 11:22:48 2024, max compression
```

## Comparing `cryspr-0.0.1.0.tar` & `cryspr-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 22:56:18.763671 cryspr-0.0.1.0/
--rw-rw-rw-   0        0        0     1123 2024-05-02 17:12:05.000000 cryspr-0.0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4572 2024-05-05 22:56:18.763671 cryspr-0.0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2306 2024-05-05 22:35:06.000000 cryspr-0.0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 22:56:18.750672 cryspr-0.0.1.0/cryspr/
--rw-rw-rw-   0        0        0      497 2024-04-24 10:08:46.000000 cryspr-0.0.1.0/cryspr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:56:18.756672 cryspr-0.0.1.0/cryspr/calculators/
--rw-rw-rw-   0        0        0     1423 2024-05-03 23:23:14.000000 cryspr-0.0.1.0/cryspr/calculators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:56:18.758671 cryspr-0.0.1.0/cryspr/optimization/
--rw-rw-rw-   0        0        0       32 2024-05-05 21:33:39.000000 cryspr-0.0.1.0/cryspr/optimization/__init__.py
--rw-rw-rw-   0        0        0     2022 2024-05-03 14:31:21.000000 cryspr-0.0.1.0/cryspr/optimization/global.py
--rw-rw-rw-   0        0        0    11853 2024-05-05 17:33:06.000000 cryspr-0.0.1.0/cryspr/optimization/local.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:56:18.761670 cryspr-0.0.1.0/cryspr/utils/
--rw-rw-rw-   0        0        0        0 2024-04-24 19:10:27.000000 cryspr-0.0.1.0/cryspr/utils/__init__.py
--rw-rw-rw-   0        0        0      237 2024-05-03 19:55:08.000000 cryspr-0.0.1.0/cryspr/utils/analysis.py
--rw-rw-rw-   0        0        0      121 2024-05-02 23:01:33.000000 cryspr-0.0.1.0/cryspr/utils/log.py
--rw-rw-rw-   0        0        0    11739 2024-05-05 20:16:27.000000 cryspr-0.0.1.0/cryspr/utils/predict.py
--rw-rw-rw-   0        0        0     6741 2024-05-05 17:04:15.000000 cryspr-0.0.1.0/cryspr/utils/struct.py
--rw-rw-rw-   0        0        0     2263 2024-05-02 23:19:48.000000 cryspr-0.0.1.0/cryspr/wyckoffgene.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:56:18.762670 cryspr-0.0.1.0/cryspr.egg-info/
--rw-rw-rw-   0        0        0     4572 2024-05-05 22:56:18.000000 cryspr-0.0.1.0/cryspr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-05-05 22:56:18.000000 cryspr-0.0.1.0/cryspr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 22:56:18.000000 cryspr-0.0.1.0/cryspr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-05 22:56:18.000000 cryspr-0.0.1.0/cryspr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-05 22:56:18.000000 cryspr-0.0.1.0/cryspr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1238 2024-05-05 22:56:01.000000 cryspr-0.0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 22:56:18.764671 cryspr-0.0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 11:22:48.551861 cryspr-0.0.2/
+-rw-rw-rw-   0        0        0     1123 2024-05-02 17:12:05.000000 cryspr-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5037 2024-05-08 11:22:48.551861 cryspr-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2773 2024-05-08 11:12:42.000000 cryspr-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 11:22:48.538857 cryspr-0.0.2/cryspr/
+-rw-rw-rw-   0        0        0      497 2024-04-24 10:08:46.000000 cryspr-0.0.2/cryspr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:22:48.543856 cryspr-0.0.2/cryspr/calculators/
+-rw-rw-rw-   0        0        0     1423 2024-05-03 23:23:14.000000 cryspr-0.0.2/cryspr/calculators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:22:48.545861 cryspr-0.0.2/cryspr/optimization/
+-rw-rw-rw-   0        0        0       32 2024-05-05 21:33:39.000000 cryspr-0.0.2/cryspr/optimization/__init__.py
+-rw-rw-rw-   0        0        0     2022 2024-05-03 14:31:21.000000 cryspr-0.0.2/cryspr/optimization/global.py
+-rw-rw-rw-   0        0        0    11853 2024-05-05 17:33:06.000000 cryspr-0.0.2/cryspr/optimization/local.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:22:48.549862 cryspr-0.0.2/cryspr/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-24 19:10:27.000000 cryspr-0.0.2/cryspr/utils/__init__.py
+-rw-rw-rw-   0        0        0      237 2024-05-03 19:55:08.000000 cryspr-0.0.2/cryspr/utils/analysis.py
+-rw-rw-rw-   0        0        0      121 2024-05-02 23:01:33.000000 cryspr-0.0.2/cryspr/utils/log.py
+-rw-rw-rw-   0        0        0    11739 2024-05-05 20:16:27.000000 cryspr-0.0.2/cryspr/utils/predict.py
+-rw-rw-rw-   0        0        0     6741 2024-05-05 17:04:15.000000 cryspr-0.0.2/cryspr/utils/struct.py
+-rw-rw-rw-   0        0        0     2263 2024-05-02 23:19:48.000000 cryspr-0.0.2/cryspr/wyckoffgene.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:22:48.550862 cryspr-0.0.2/cryspr.egg-info/
+-rw-rw-rw-   0        0        0     5037 2024-05-08 11:22:48.000000 cryspr-0.0.2/cryspr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-05-08 11:22:48.000000 cryspr-0.0.2/cryspr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 11:22:48.000000 cryspr-0.0.2/cryspr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-08 11:22:48.000000 cryspr-0.0.2/cryspr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 11:22:48.000000 cryspr-0.0.2/cryspr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1236 2024-05-08 11:19:15.000000 cryspr-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 11:22:48.551861 cryspr-0.0.2/setup.cfg
```

### Comparing `cryspr-0.0.1.0/LICENSE` & `cryspr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryspr-0.0.1.0/PKG-INFO` & `cryspr-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryspr
-Version: 0.0.1.0
+Version: 0.0.2
 Summary: Python implementation of crystal structure pre-relaxation and predcition (CrySPR).
 Author-email: Wei Nong <nw2y47@outlook.com>, Ruiming Zhu <raymond_zhurm@outlook.com>, Kedar Hippalgaonkar <kedar@ntu.edu.sg>
 Maintainer-email: Wei Nong <nw2y47@outlook.com>, Ruiming Zhu <raymond_zhurm@outlook.com>
 License: MIT License
         
         Copyright (c) 2024 Kedar Hippalgaonkar's Materials by Design Lab
         
@@ -76,14 +76,19 @@
 
 ### PyPI distribution
 
 ```bash
 $ pip install cryspr
 ```
 
+Note on the installation of `matgl (1.0.0)` library:
+
+- **Windows OS**: `pip install cryspr` will normally install all related dependencies, and the `matgl ` works for latest version of torch (as-of-date is 2.3.0)
+- **Linux OS**: the `matgl` requires `torch<=2.2.1` and additionally  `pydantic`, which is not well handled by pip. The two dependencies have to be manually installed using `pip`, or to install `matgl` using other package manager, like, `conda`. 
+
 ### Source code (GitHub)
 
 1. Download the repo or git clone.
 
 2. Add the CrySPR project into the system PYTHONPATH either by, e.g., on Linux/Mac OS
 
 ```bash
```

### Comparing `cryspr-0.0.1.0/README.md` & `cryspr-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,19 @@
 
 ### PyPI distribution
 
 ```bash
 $ pip install cryspr
 ```
 
+Note on the installation of `matgl (1.0.0)` library:
+
+- **Windows OS**: `pip install cryspr` will normally install all related dependencies, and the `matgl ` works for latest version of torch (as-of-date is 2.3.0)
+- **Linux OS**: the `matgl` requires `torch<=2.2.1` and additionally  `pydantic`, which is not well handled by pip. The two dependencies have to be manually installed using `pip`, or to install `matgl` using other package manager, like, `conda`. 
+
 ### Source code (GitHub)
 
 1. Download the repo or git clone.
 
 2. Add the CrySPR project into the system PYTHONPATH either by, e.g., on Linux/Mac OS
 
 ```bash
```

### Comparing `cryspr-0.0.1.0/cryspr/calculators/__init__.py` & `cryspr-0.0.2/cryspr/calculators/__init__.py`

 * *Files identical despite different names*

### Comparing `cryspr-0.0.1.0/cryspr/optimization/global.py` & `cryspr-0.0.2/cryspr/optimization/global.py`

 * *Files identical despite different names*

### Comparing `cryspr-0.0.1.0/cryspr/optimization/local.py` & `cryspr-0.0.2/cryspr/optimization/local.py`

 * *Files identical despite different names*

### Comparing `cryspr-0.0.1.0/cryspr/utils/predict.py` & `cryspr-0.0.2/cryspr/utils/predict.py`

 * *Files identical despite different names*

### Comparing `cryspr-0.0.1.0/cryspr/utils/struct.py` & `cryspr-0.0.2/cryspr/utils/struct.py`

 * *Files identical despite different names*

### Comparing `cryspr-0.0.1.0/cryspr/wyckoffgene.py` & `cryspr-0.0.2/cryspr/wyckoffgene.py`

 * *Files identical despite different names*

### Comparing `cryspr-0.0.1.0/cryspr.egg-info/PKG-INFO` & `cryspr-0.0.2/cryspr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryspr
-Version: 0.0.1.0
+Version: 0.0.2
 Summary: Python implementation of crystal structure pre-relaxation and predcition (CrySPR).
 Author-email: Wei Nong <nw2y47@outlook.com>, Ruiming Zhu <raymond_zhurm@outlook.com>, Kedar Hippalgaonkar <kedar@ntu.edu.sg>
 Maintainer-email: Wei Nong <nw2y47@outlook.com>, Ruiming Zhu <raymond_zhurm@outlook.com>
 License: MIT License
         
         Copyright (c) 2024 Kedar Hippalgaonkar's Materials by Design Lab
         
@@ -76,14 +76,19 @@
 
 ### PyPI distribution
 
 ```bash
 $ pip install cryspr
 ```
 
+Note on the installation of `matgl (1.0.0)` library:
+
+- **Windows OS**: `pip install cryspr` will normally install all related dependencies, and the `matgl ` works for latest version of torch (as-of-date is 2.3.0)
+- **Linux OS**: the `matgl` requires `torch<=2.2.1` and additionally  `pydantic`, which is not well handled by pip. The two dependencies have to be manually installed using `pip`, or to install `matgl` using other package manager, like, `conda`. 
+
 ### Source code (GitHub)
 
 1. Download the repo or git clone.
 
 2. Add the CrySPR project into the system PYTHONPATH either by, e.g., on Linux/Mac OS
 
 ```bash
```

### Comparing `cryspr-0.0.1.0/pyproject.toml` & `cryspr-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cryspr"
-version = "0.0.1.0"
+version = "0.0.2"
 description = "Python implementation of crystal structure pre-relaxation and predcition (CrySPR)."
 authors = [
     {name = "Wei Nong", email = "nw2y47@outlook.com"},
     {name = "Ruiming Zhu", email = "raymond_zhurm@outlook.com"},
     {name = "Kedar Hippalgaonkar", email = "kedar@ntu.edu.sg"},
 ]
 maintainers = [
```

