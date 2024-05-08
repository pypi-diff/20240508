# Comparing `tmp/kid_ppg-0.0.1.tar.gz` & `tmp/kid_ppg-0.0.4.tar.gz`

## Comparing `kid_ppg-0.0.1.tar` & `kid_ppg-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0   413734 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/KID_PPG_demo.ipynb
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/requirements.txt
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/src/kid_ppg/__init__.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/src/kid_ppg/adaptive_linear_model.py
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/src/kid_ppg/kid_ppg.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/src/kid_ppg/preprocessing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/src/kid_ppg/demo/__init__.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/src/kid_ppg/demo/demo_utils.py
--rw-r--r--   0        0        0  1766723 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/src/kid_ppg/demo/demo_data/PPGDalia_S6_stairs.pkl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/src/kid_ppg/demo/demo_data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/src/kid_ppg/model_weights/__init__.py
--rw-r--r--   0        0        0  4671496 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/src/kid_ppg/model_weights/kid_ppg_weights.h5
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/LICENSE
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 kid_ppg-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0   413734 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/KID_PPG_demo.ipynb
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/src/kid_ppg/__init__.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/src/kid_ppg/adaptive_linear_model.py
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/src/kid_ppg/kid_ppg.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/src/kid_ppg/preprocessing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/src/kid_ppg/demo/__init__.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/src/kid_ppg/demo/demo_utils.py
+-rw-r--r--   0        0        0  1766723 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/src/kid_ppg/demo/demo_data/PPGDalia_S6_stairs.pkl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/src/kid_ppg/demo/demo_data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/src/kid_ppg/model_weights/__init__.py
+-rw-r--r--   0        0        0  4671496 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/src/kid_ppg/model_weights/kid_ppg_weights.h5
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 kid_ppg-0.0.4/PKG-INFO
```

### Comparing `kid_ppg-0.0.1/KID_PPG_demo.ipynb` & `kid_ppg-0.0.4/KID_PPG_demo.ipynb`

 * *Files identical despite different names*

### Comparing `kid_ppg-0.0.1/.github/workflows/python-publish.yml` & `kid_ppg-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kid_ppg-0.0.1/src/kid_ppg/adaptive_linear_model.py` & `kid_ppg-0.0.4/src/kid_ppg/adaptive_linear_model.py`

 * *Files identical despite different names*

### Comparing `kid_ppg-0.0.1/src/kid_ppg/kid_ppg.py` & `kid_ppg-0.0.4/src/kid_ppg/kid_ppg.py`

 * *Files identical despite different names*

### Comparing `kid_ppg-0.0.1/src/kid_ppg/preprocessing.py` & `kid_ppg-0.0.4/src/kid_ppg/preprocessing.py`

 * *Files identical despite different names*

### Comparing `kid_ppg-0.0.1/src/kid_ppg/demo/demo_utils.py` & `kid_ppg-0.0.4/src/kid_ppg/demo/demo_utils.py`

 * *Files identical despite different names*

### Comparing `kid_ppg-0.0.1/src/kid_ppg/demo/demo_data/PPGDalia_S6_stairs.pkl` & `kid_ppg-0.0.4/src/kid_ppg/demo/demo_data/PPGDalia_S6_stairs.pkl`

 * *Files identical despite different names*

### Comparing `kid_ppg-0.0.1/src/kid_ppg/model_weights/kid_ppg_weights.h5` & `kid_ppg-0.0.4/src/kid_ppg/model_weights/kid_ppg_weights.h5`

 * *Files identical despite different names*

### Comparing `kid_ppg-0.0.1/LICENSE` & `kid_ppg-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kid_ppg-0.0.1/README.md` & `kid_ppg-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # KID-PPG: Knowledge-Informed Deep Learning for Extracting Heart Rate from Photoplethysmography Signals 
 
-KID-PPG is the first ever publicly available pre-trained deep learning model for PPG Heart Rate inference.
+KID-PPG is the first ever publicly available pre-trained deep learning model for PPG Heart Rate inference, proposed [here](https://infoscience.epfl.ch/record/310896?ln=en&v=pdf).
 
 # Installation
 KID-PPG is readily available in pip. 
 
 ### Install from pip
 Install KID-PPG from pip \
 `pip install kid-ppg`
```

### Comparing `kid_ppg-0.0.1/pyproject.toml` & `kid_ppg-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kid_ppg"
-version = "0.0.1"
+version = "0.0.4"
 authors = [
   { name="Christodoulos Kechris", email="christodoulos.kechris@epfl.ch" }
 ]
 description = "A library for performing probabilistic heart rate extraction from photoplehysmography signals."
 readme = "README.md"
 requires-python = "==3.10.8"
 dependencies = [
@@ -16,12 +16,13 @@
   "numpy==1.24.3",
   "tensorflow==2.13.0",
   "tensorflow-probability==0.20.1",
   "scipy==1.12.0"
   ]
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
-[project.urls]
+[project.urls]
+"Homepage" = "https://github.com/esl-epfl/KID-PPG"
```

### Comparing `kid_ppg-0.0.1/PKG-INFO` & `kid_ppg-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.3
 Name: kid_ppg
-Version: 0.0.1
+Version: 0.0.4
 Summary: A library for performing probabilistic heart rate extraction from photoplehysmography signals.
+Project-URL: Homepage, https://github.com/esl-epfl/KID-PPG
 Author-email: Christodoulos Kechris <christodoulos.kechris@epfl.ch>
 License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ==3.10.8
 Requires-Dist: numpy==1.24.3
 Requires-Dist: scipy==1.12.0
 Requires-Dist: silence-tensorflow==1.2.1
 Requires-Dist: tensorflow-probability==0.20.1
 Requires-Dist: tensorflow==2.13.0
 Description-Content-Type: text/markdown
 
 # KID-PPG: Knowledge-Informed Deep Learning for Extracting Heart Rate from Photoplethysmography Signals 
 
-KID-PPG is the first ever publicly available pre-trained deep learning model for PPG Heart Rate inference.
+KID-PPG is the first ever publicly available pre-trained deep learning model for PPG Heart Rate inference, proposed [here](https://infoscience.epfl.ch/record/310896?ln=en&v=pdf).
 
 # Installation
 KID-PPG is readily available in pip. 
 
 ### Install from pip
 Install KID-PPG from pip \
 `pip install kid-ppg`
```

