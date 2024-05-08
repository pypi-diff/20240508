# Comparing `tmp/pulse_coupled_nn-0.0.4.tar.gz` & `tmp/pulse_coupled_nn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pulse_coupled_nn-0.0.4.tar", last modified: Wed May  8 05:02:10 2024, max compression
+gzip compressed data, was "dist\pulse_coupled_nn-0.0.5.tar", last modified: Wed May  8 05:06:38 2024, max compression
```

## Comparing `pulse_coupled_nn-0.0.4.tar` & `pulse_coupled_nn-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 05:02:10.000000 pulse_coupled_nn-0.0.4/
--rw-rw-rw-   0        0        0     2342 2024-05-08 05:02:10.000000 pulse_coupled_nn-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2024-05-07 09:55:09.000000 pulse_coupled_nn-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 05:02:10.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/
--rw-rw-rw-   0        0        0      313 2024-05-08 04:55:29.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/__init__.py
--rw-rw-rw-   0        0        0     1534 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/classic_model.py
--rw-rw-rw-   0        0        0     1285 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/flm_model.py
--rw-rw-rw-   0        0        0     6845 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/general_model.py
--rw-rw-rw-   0        0        0     1200 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/icm_model.py
--rw-rw-rw-   0        0        0      803 2024-05-07 09:14:40.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/kernels.py
--rw-rw-rw-   0        0        0     2345 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/mlm_model.py
--rw-rw-rw-   0        0        0     1319 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/scm_model.py
--rw-rw-rw-   0        0        0     1473 2024-05-07 09:14:40.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/simulator.py
--rw-rw-rw-   0        0        0     1385 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/slm_model.py
--rw-rw-rw-   0        0        0     2354 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn/test_run.py
-drwxrwxrwx   0        0        0        0 2024-05-08 05:02:10.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn.egg-info/
--rw-rw-rw-   0        0        0     2342 2024-05-08 05:02:10.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2024-05-08 05:02:10.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 05:02:10.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-08 05:02:10.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-08 05:02:10.000000 pulse_coupled_nn-0.0.4/pulse_coupled_nn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 05:02:10.000000 pulse_coupled_nn-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      876 2024-05-08 05:02:03.000000 pulse_coupled_nn-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:06:38.000000 pulse_coupled_nn-0.0.5/
+-rw-rw-rw-   0        0        0     2342 2024-05-08 05:06:38.000000 pulse_coupled_nn-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2024-05-07 09:55:09.000000 pulse_coupled_nn-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 05:06:38.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/
+-rw-rw-rw-   0        0        0      322 2024-05-08 05:05:50.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/__init__.py
+-rw-rw-rw-   0        0        0     1534 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/classic_model.py
+-rw-rw-rw-   0        0        0     1285 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/flm_model.py
+-rw-rw-rw-   0        0        0     6845 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/general_model.py
+-rw-rw-rw-   0        0        0     1200 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/icm_model.py
+-rw-rw-rw-   0        0        0      803 2024-05-07 09:14:40.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/kernels.py
+-rw-rw-rw-   0        0        0     2345 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/mlm_model.py
+-rw-rw-rw-   0        0        0     1319 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/scm_model.py
+-rw-rw-rw-   0        0        0     1473 2024-05-07 09:14:40.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/simulator.py
+-rw-rw-rw-   0        0        0     1385 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/slm_model.py
+-rw-rw-rw-   0        0        0     2354 2024-05-07 09:36:35.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn/test_run.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:06:38.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn.egg-info/
+-rw-rw-rw-   0        0        0     2342 2024-05-08 05:06:38.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2024-05-08 05:06:38.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 05:06:38.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-08 05:06:38.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-08 05:06:38.000000 pulse_coupled_nn-0.0.5/pulse_coupled_nn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 05:06:38.000000 pulse_coupled_nn-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-05-08 05:06:32.000000 pulse_coupled_nn-0.0.5/setup.py
```

### Comparing `pulse_coupled_nn-0.0.4/PKG-INFO` & `pulse_coupled_nn-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulse_coupled_nn
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python implementation of the Pulse Coupled Neural Network (PCNN)
 Home-page: https://github.com/ArdeleanRichard/PCNN
 Author: Eugen-Richard Ardelean
 Author-email: ardeleaneugenrichard@gmail.com
 License: MIT
 Description: # PCNN
         Python implementation of the Pulse Coupled Neural Network (PCNN) alongside multiple variations:
```

### Comparing `pulse_coupled_nn-0.0.4/README.md` & `pulse_coupled_nn-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn/classic_model.py` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn/classic_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn/flm_model.py` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn/flm_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn/general_model.py` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn/general_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn/icm_model.py` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn/icm_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn/kernels.py` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn/kernels.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn/mlm_model.py` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn/mlm_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn/scm_model.py` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn/scm_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn/simulator.py` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn/simulator.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn/slm_model.py` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn/slm_model.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn/test_run.py` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn/test_run.py`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn.egg-info/PKG-INFO` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulse-coupled-nn
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python implementation of the Pulse Coupled Neural Network (PCNN)
 Home-page: https://github.com/ArdeleanRichard/PCNN
 Author: Eugen-Richard Ardelean
 Author-email: ardeleaneugenrichard@gmail.com
 License: MIT
 Description: # PCNN
         Python implementation of the Pulse Coupled Neural Network (PCNN) alongside multiple variations:
```

### Comparing `pulse_coupled_nn-0.0.4/pulse_coupled_nn.egg-info/SOURCES.txt` & `pulse_coupled_nn-0.0.5/pulse_coupled_nn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulse_coupled_nn-0.0.4/setup.py` & `pulse_coupled_nn-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("pulse_coupled_nn/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pulse_coupled_nn",
-    version="0.0.4",
+    version="0.0.5",
     description="Python implementation of the Pulse Coupled Neural Network (PCNN)",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ArdeleanRichard/PCNN",
     author="Eugen-Richard Ardelean",
     author_email="ardeleaneugenrichard@gmail.com",
```

