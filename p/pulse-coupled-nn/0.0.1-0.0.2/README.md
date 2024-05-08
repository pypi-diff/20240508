# Comparing `tmp/pulse_coupled_nn-0.0.1.tar.gz` & `tmp/pulse_coupled_nn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pulse_coupled_nn-0.0.1.tar", last modified: Tue May  7 09:47:52 2024, max compression
+gzip compressed data, was "dist\pulse_coupled_nn-0.0.2.tar", last modified: Wed May  8 04:53:00 2024, max compression
```

## Comparing `pulse_coupled_nn-0.0.1.tar` & `pulse_coupled_nn-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:47:52.000000 pulse_coupled_nn-0.0.1/
--rw-rw-rw-   0        0        0      892 2024-05-07 09:47:52.000000 pulse_coupled_nn-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1370 2024-05-07 09:47:46.000000 pulse_coupled_nn-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 09:47:52.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:47:52.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/pulse_coupled_nn.egg-info/
--rw-rw-rw-   0        0        0      892 2024-05-07 09:47:52.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/pulse_coupled_nn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      681 2024-05-07 09:47:52.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/pulse_coupled_nn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:47:52.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/pulse_coupled_nn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-07 09:47:52.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/pulse_coupled_nn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-07 09:47:52.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/pulse_coupled_nn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 09:47:52.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/
--rw-rw-rw-   0        0        0        0 2024-05-07 09:13:07.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/__init__.py
--rw-rw-rw-   0        0        0     1534 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/classic_model.py
--rw-rw-rw-   0        0        0     1285 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/flm_model.py
--rw-rw-rw-   0        0        0     6845 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/general_model.py
--rw-rw-rw-   0        0        0     1200 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/icm_model.py
--rw-rw-rw-   0        0        0      803 2024-05-07 09:14:40.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/kernels.py
--rw-rw-rw-   0        0        0     2345 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/mlm_model.py
--rw-rw-rw-   0        0        0     1319 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/scm_model.py
--rw-rw-rw-   0        0        0     1473 2024-05-07 09:14:40.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/simulator.py
--rw-rw-rw-   0        0        0     1385 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/slm_model.py
--rw-rw-rw-   0        0        0     2354 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/test_show.py
--rw-rw-rw-   0        0        0       42 2024-05-07 09:47:52.000000 pulse_coupled_nn-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      942 2024-05-07 09:47:46.000000 pulse_coupled_nn-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:53:00.000000 pulse_coupled_nn-0.0.2/
+-rw-rw-rw-   0        0        0     2342 2024-05-08 04:53:00.000000 pulse_coupled_nn-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2024-05-07 09:55:09.000000 pulse_coupled_nn-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 04:53:00.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/
+-rw-rw-rw-   0        0        0      358 2024-05-07 09:34:45.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/__init__.py
+-rw-rw-rw-   0        0        0     1534 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/classic_model.py
+-rw-rw-rw-   0        0        0     1285 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/flm_model.py
+-rw-rw-rw-   0        0        0     6845 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/general_model.py
+-rw-rw-rw-   0        0        0     1200 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/icm_model.py
+-rw-rw-rw-   0        0        0      803 2024-05-07 09:14:40.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/kernels.py
+-rw-rw-rw-   0        0        0     2345 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/mlm_model.py
+-rw-rw-rw-   0        0        0     1319 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/scm_model.py
+-rw-rw-rw-   0        0        0     1473 2024-05-07 09:14:40.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/simulator.py
+-rw-rw-rw-   0        0        0     1385 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/slm_model.py
+-rw-rw-rw-   0        0        0     2354 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn/test_show.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:53:00.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn.egg-info/
+-rw-rw-rw-   0        0        0     2342 2024-05-08 04:52:59.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-05-08 04:52:59.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 04:52:59.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-08 04:52:59.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-08 04:52:59.000000 pulse_coupled_nn-0.0.2/pulse_coupled_nn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 04:53:00.000000 pulse_coupled_nn-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-05-08 04:52:32.000000 pulse_coupled_nn-0.0.2/setup.py
```

### Comparing `pulse_coupled_nn-0.0.1/README.md` & `pulse_coupled_nn-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 - Intersecting Cortical Model (ICM)
 - Multi Linking Model (MLM)
 - Spiking Cortical Model (SCM)
 - Sigmoidal Linking Model (SLM)
 
 Install:
 ```
-pip install Pulse-Coupled-Neural-Networks
+pip install pulse_coupled_nn
 ```
 
 Usage example:
 ```
 import numpy as np
 import matplotlib.pyplot as plt
```

### Comparing `pulse_coupled_nn-0.0.1/pulse_coupled_nn/pulse_coupled_nn.egg-info/SOURCES.txt` & `pulse_coupled_nn-0.0.2/pulse_coupled_nn.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 README.md
 setup.py
-pulse_coupled_nn/pulse_coupled_nn.egg-info/PKG-INFO
-pulse_coupled_nn/pulse_coupled_nn.egg-info/SOURCES.txt
-pulse_coupled_nn/pulse_coupled_nn.egg-info/dependency_links.txt
-pulse_coupled_nn/pulse_coupled_nn.egg-info/requires.txt
-pulse_coupled_nn/pulse_coupled_nn.egg-info/top_level.txt
-pulse_coupled_nn/src/__init__.py
-pulse_coupled_nn/src/classic_model.py
-pulse_coupled_nn/src/flm_model.py
-pulse_coupled_nn/src/general_model.py
-pulse_coupled_nn/src/icm_model.py
-pulse_coupled_nn/src/kernels.py
-pulse_coupled_nn/src/mlm_model.py
-pulse_coupled_nn/src/scm_model.py
-pulse_coupled_nn/src/simulator.py
-pulse_coupled_nn/src/slm_model.py
-pulse_coupled_nn/src/test_show.py
+pulse_coupled_nn/__init__.py
+pulse_coupled_nn/classic_model.py
+pulse_coupled_nn/flm_model.py
+pulse_coupled_nn/general_model.py
+pulse_coupled_nn/icm_model.py
+pulse_coupled_nn/kernels.py
+pulse_coupled_nn/mlm_model.py
+pulse_coupled_nn/scm_model.py
+pulse_coupled_nn/simulator.py
+pulse_coupled_nn/slm_model.py
+pulse_coupled_nn/test_show.py
+pulse_coupled_nn.egg-info/PKG-INFO
+pulse_coupled_nn.egg-info/SOURCES.txt
+pulse_coupled_nn.egg-info/dependency_links.txt
+pulse_coupled_nn.egg-info/requires.txt
+pulse_coupled_nn.egg-info/top_level.txt
```

### Comparing `pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/classic_model.py` & `pulse_coupled_nn-0.0.2/pulse_coupled_nn/classic_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/flm_model.py` & `pulse_coupled_nn-0.0.2/pulse_coupled_nn/flm_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/general_model.py` & `pulse_coupled_nn-0.0.2/pulse_coupled_nn/general_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/icm_model.py` & `pulse_coupled_nn-0.0.2/pulse_coupled_nn/icm_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/kernels.py` & `pulse_coupled_nn-0.0.2/pulse_coupled_nn/kernels.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/mlm_model.py` & `pulse_coupled_nn-0.0.2/pulse_coupled_nn/mlm_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/scm_model.py` & `pulse_coupled_nn-0.0.2/pulse_coupled_nn/scm_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/simulator.py` & `pulse_coupled_nn-0.0.2/pulse_coupled_nn/simulator.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/slm_model.py` & `pulse_coupled_nn-0.0.2/pulse_coupled_nn/slm_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.1/pulse_coupled_nn/src/test_show.py` & `pulse_coupled_nn-0.0.2/pulse_coupled_nn/test_show.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.1/setup.py` & `pulse_coupled_nn-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import find_packages, setup
 
 with open("pulse_coupled_nn/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pulse_coupled_nn",
-    version="0.0.1",
+    version="0.0.2",
     description="Python implementation of the Pulse Coupled Neural Network (PCNN)",
-    package_dir={"": "pulse_coupled_nn"},
-    packages=find_packages(where="pulse_coupled_nn"),
+    packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ArdeleanRichard/PCNN",
     author="Eugen-Richard Ardelean",
     author_email="ardeleaneugenrichard@gmail.com",
     license="MIT",
     classifiers=[
```

