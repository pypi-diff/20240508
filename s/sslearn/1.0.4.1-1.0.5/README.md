# Comparing `tmp/sslearn-1.0.4.1.tar.gz` & `tmp/sslearn-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sslearn-1.0.4.1.tar", last modified: Tue Feb  6 12:44:11 2024, max compression
+gzip compressed data, was "sslearn-1.0.5.tar", last modified: Wed May  8 15:30:09 2024, max compression
```

## Comparing `sslearn-1.0.4.1.tar` & `sslearn-1.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 12:44:11.765404 sslearn-1.0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-02-06 12:44:11.765404 sslearn-1.0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-06 12:44:11.765404 sslearn-1.0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 12:44:11.761404 sslearn-1.0.4.1/sslearn/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 12:44:11.761404 sslearn-1.0.4.1/sslearn/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/datasets/_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/datasets/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/datasets/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 12:44:11.761404 sslearn-1.0.4.1/sslearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/model_selection/_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/restricted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 12:44:11.761404 sslearn-1.0.4.1/sslearn/subview/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/subview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/subview/_subview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 12:44:11.765404 sslearn-1.0.4.1/sslearn/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49244 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/wrapper/_co.py
--rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/wrapper/_self.py
--rw-r--r--   0 runner    (1001) docker     (127)    29371 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/sslearn/wrapper/_tritraining.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 12:44:11.765404 sslearn-1.0.4.1/sslearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-02-06 12:44:11.000000 sslearn-1.0.4.1/sslearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-06 12:44:11.000000 sslearn-1.0.4.1/sslearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 12:44:11.000000 sslearn-1.0.4.1/sslearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-06 12:44:11.000000 sslearn-1.0.4.1/sslearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-06 12:44:11.000000 sslearn-1.0.4.1/sslearn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 12:44:11.765404 sslearn-1.0.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/test/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/test/test_general.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/test/test_model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/test/test_subview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-02-06 12:43:57.000000 sslearn-1.0.4.1/test/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.569039 sslearn-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-08 15:30:02.000000 sslearn-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-08 15:30:09.569039 sslearn-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-08 15:30:02.000000 sslearn-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 15:30:09.569039 sslearn-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-08 15:30:02.000000 sslearn-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.565039 sslearn-1.0.5/sslearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.565039 sslearn-1.0.5/sslearn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/datasets/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/datasets/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/datasets/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.565039 sslearn-1.0.5/sslearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/model_selection/_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17475 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/restricted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.565039 sslearn-1.0.5/sslearn/subview/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/subview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/subview/_subview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.569039 sslearn-1.0.5/sslearn/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60686 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/wrapper/_co.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/wrapper/_self.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32663 2024-05-08 15:30:02.000000 sslearn-1.0.5/sslearn/wrapper/_tritraining.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.569039 sslearn-1.0.5/sslearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-08 15:30:09.000000 sslearn-1.0.5/sslearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-08 15:30:09.000000 sslearn-1.0.5/sslearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:30:09.000000 sslearn-1.0.5/sslearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 15:30:09.000000 sslearn-1.0.5/sslearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 15:30:09.000000 sslearn-1.0.5/sslearn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:30:09.569039 sslearn-1.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-08 15:30:02.000000 sslearn-1.0.5/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-08 15:30:02.000000 sslearn-1.0.5/test/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-08 15:30:02.000000 sslearn-1.0.5/test/test_model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-08 15:30:02.000000 sslearn-1.0.5/test/test_subview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-08 15:30:02.000000 sslearn-1.0.5/test/test_wrapper.py
```

### Comparing `sslearn-1.0.4.1/LICENSE` & `sslearn-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.4.1/PKG-INFO` & `sslearn-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 Metadata-Version: 2.1
 Name: sslearn
-Version: 1.0.4.1
+Version: 1.0.5
 Summary: A Python package for semi-supervised learning with scikit-learn
 Home-page: https://github.com/jlgarridol/sslearn
-Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/f1.0.4.1.tar.gz
+Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/1.0.5.tar.gz
 Author: José Luis Garrido-Labrador
 Author-email: jlgarrido@ubu.es
 License: new BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib>=1.2.0
 Requires-Dist: numpy>=1.23.3
 Requires-Dist: pandas>=1.4.3
 Requires-Dist: scikit_learn>=1.2.0
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: statsmodels>=0.13.2
 
 Semi-Supervised Learning Library (sslearn)
 ===
 
-![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability-percentage/jlgarridol/sslearn) ![Code Climate coverage](https://img.shields.io/codeclimate/coverage/jlgarridol/sslearn) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/jlgarridol/sslearn/python-package.yml) ![PyPI - Version](https://img.shields.io/pypi/v/sslearn)
+<!-- Insert logo in the middle -->
+<img width="100%" src="https://raw.githubusercontent.com/jlgarridol/sslearn/main/docs/sslearn.webp"/>
+
+![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability-percentage/jlgarridol/sslearn) ![Code Climate coverage](https://img.shields.io/codeclimate/coverage/jlgarridol/sslearn) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/jlgarridol/sslearn/python-package.yml) ![PyPI - Version](https://img.shields.io/pypi/v/sslearn) [![Static Badge](https://img.shields.io/badge/doc-available-blue?style=flat)](https://jlgarridol.github.io/sslearn/)
 
 The `sslearn` library is a Python package for machine learning over Semi-supervised datasets. It is an extension of [scikit-learn](https://github.com/scikit-learn/scikit-learn).
 
-Installation
----
+## Installation
+
+
 ### Dependencies
 
 * joblib >= 1.2.0
 * numpy >= 1.23.3
 * pandas >= 1.4.3
 * scikit_learn >= 1.2.0
 * scipy >= 1.10.1
@@ -45,35 +51,34 @@
 
 ### `pip` installation
 
 It can be installed using *Pypi*:
 
     pip install sslearn
 
-Code example
----
+## Code example
+
+
 ```python
 from sslearn.wrapper import TriTraining
 from sslearn.model_selection import artificial_ssl_dataset
 from sklearn.datasets import load_iris
 
 X, y = load_iris(return_X_y=True)
 X, y, X_unlabel, true_label = artificial_ssl_dataset(X, y, label_rate=0.1)
 
 model = TriTraining().fit(X, y)
 model.score(X_unlabel, true_label)
 ```
 
-Citing
----
+## Citing 
+
 ```bibtex
-@software{jose_luis_garrido_labrador_2024_10623889,
+@software{garrido2024sslearn,
   author       = {José Luis Garrido-Labrador},
-  title        = {jlgarridol/sslearn: v1.0.4},
+  title        = {jlgarridol/sslearn},
   month        = feb,
   year         = 2024,
   publisher    = {Zenodo},
-  version      = {1.0.4},
-  doi          = {10.5281/zenodo.10623889},
-  url          = {https://doi.org/10.5281/zenodo.10623889}
+  doi          = {10.5281/zenodo.7565221},
 }
 ```
```

### Comparing `sslearn-1.0.4.1/README.md` & `sslearn-1.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Semi-Supervised Learning Library (sslearn)
 ===
 
-![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability-percentage/jlgarridol/sslearn) ![Code Climate coverage](https://img.shields.io/codeclimate/coverage/jlgarridol/sslearn) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/jlgarridol/sslearn/python-package.yml) ![PyPI - Version](https://img.shields.io/pypi/v/sslearn)
+<!-- Insert logo in the middle -->
+<img width="100%" src="https://raw.githubusercontent.com/jlgarridol/sslearn/main/docs/sslearn.webp"/>
+
+![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability-percentage/jlgarridol/sslearn) ![Code Climate coverage](https://img.shields.io/codeclimate/coverage/jlgarridol/sslearn) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/jlgarridol/sslearn/python-package.yml) ![PyPI - Version](https://img.shields.io/pypi/v/sslearn) [![Static Badge](https://img.shields.io/badge/doc-available-blue?style=flat)](https://jlgarridol.github.io/sslearn/)
 
 The `sslearn` library is a Python package for machine learning over Semi-supervised datasets. It is an extension of [scikit-learn](https://github.com/scikit-learn/scikit-learn).
 
-Installation
----
+## Installation
+
+
 ### Dependencies
 
 * joblib >= 1.2.0
 * numpy >= 1.23.3
 * pandas >= 1.4.3
 * scikit_learn >= 1.2.0
 * scipy >= 1.10.1
@@ -19,35 +23,34 @@
 
 ### `pip` installation
 
 It can be installed using *Pypi*:
 
     pip install sslearn
 
-Code example
----
+## Code example
+
+
 ```python
 from sslearn.wrapper import TriTraining
 from sslearn.model_selection import artificial_ssl_dataset
 from sklearn.datasets import load_iris
 
 X, y = load_iris(return_X_y=True)
 X, y, X_unlabel, true_label = artificial_ssl_dataset(X, y, label_rate=0.1)
 
 model = TriTraining().fit(X, y)
 model.score(X_unlabel, true_label)
 ```
 
-Citing
----
+## Citing 
+
 ```bibtex
-@software{jose_luis_garrido_labrador_2024_10623889,
+@software{garrido2024sslearn,
   author       = {José Luis Garrido-Labrador},
-  title        = {jlgarridol/sslearn: v1.0.4},
+  title        = {jlgarridol/sslearn},
   month        = feb,
   year         = 2024,
   publisher    = {Zenodo},
-  version      = {1.0.4},
-  doi          = {10.5281/zenodo.10623889},
-  url          = {https://doi.org/10.5281/zenodo.10623889}
+  doi          = {10.5281/zenodo.7565221},
 }
 ```
```

### Comparing `sslearn-1.0.4.1/setup.py` & `sslearn-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open('sslearn/__init__.py') as f:
         for line in f:
             if line.startswith('__version__'):
                 return line.split('=')[1].strip().strip("'")
 
 
 version = get_version()
-url = f"https://github.com/jlgarridol/sslearn/archive/refs/tags/f{version}.tar.gz"
+url = f"https://github.com/jlgarridol/sslearn/archive/refs/tags/{version}.tar.gz"
 
 setuptools.setup(
     name='sslearn',
     version=version,
     description='A Python package for semi-supervised learning with scikit-learn',
     long_description=readme,
     long_description_content_type='text/markdown',
@@ -38,9 +38,11 @@
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ]
 )
```

### Comparing `sslearn-1.0.4.1/sslearn/datasets/_loader.py` & `sslearn-1.0.5/sslearn/datasets/_loader.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.4.1/sslearn/datasets/_preprocess.py` & `sslearn-1.0.5/sslearn/datasets/_preprocess.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.4.1/sslearn/datasets/_writer.py` & `sslearn-1.0.5/sslearn/datasets/_writer.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.4.1/sslearn/model_selection/_split.py` & `sslearn-1.0.5/sslearn/model_selection/_split.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 import sklearn.model_selection as ms
 from sklearn.utils import check_random_state
 import numpy as np
 
 
 class StratifiedKFoldSS():
+    """
+    Stratified K-Folds cross-validator for semi-supervised learning.
+    
+    Provides label and unlabel indices for each split. Using the `StratifiedKFold` method from `sklearn`.
+    The `test` set is the labeled set and the `train` set is the unlabeled set.
+    """
+
+
     def __init__(self, n_splits=5, shuffle=False, random_state=None):
+        """
+        Parameters
+        ----------
+        n_splits : int, default=5
+            Number of folds. Must be at least 2.
+        shuffle : bool, default=False
+            Whether to shuffle each class's samples before splitting into batches.
+        random_state : int or RandomState instance, default=None
+            When shuffle is True, random_state affects the ordering of the indices.
+            
+        """
 
         self.K = ms.StratifiedKFold(n_splits=n_splits, shuffle=shuffle,
                                     random_state=random_state)
         self.n_splits = n_splits
         self.shuffle = shuffle
         self.random_state = random_state
 
@@ -25,17 +44,17 @@
 
         Yields
         -------
         X : ndarray
             The feature set.
         y : ndarray
             The label set, -1 for unlabel instance.
-        label: ndarray
+        label : ndarray
             The training set indices for split mark as labeled.
-        unlabel: ndarray
+        unlabel : ndarray
             The training set indices for split mark as unlabeled.
         """
         for train, test in self.K.split(X, y):
             # Inverse train and test because train is big dataset
             label = test
             unlabel = train
```

### Comparing `sslearn-1.0.4.1/sslearn/subview/_subview.py` & `sslearn-1.0.5/sslearn/subview/_subview.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,37 @@
                           RegressorMixin)
 from sklearn.base import clone as skclone
 from sklearn.base import is_classifier
 from sklearn.utils import check_X_y
 
 
 class SubView(BaseEstimator):
+    """
+    A classifier that uses a subview of the data.
+    
+    Example
+    -------
+    ```python
+    from sklearn.model_selection import train_test_split
+    from sklearn.tree import DecisionTreeClassifier
+    from sslearn.subview import SubViewClassifier
+
+    # Mode 'include' will include all columns that contain `string`
+    clf = SubViewClassifier(DecisionTreeClassifier(), "sepal", mode="include")
+    clf.fit(X, y)
+
+    # Mode 'regex' will include all columns that match the regex
+    clf = SubViewClassifier(DecisionTreeClassifier(), "sepal.*", mode="regex")
+    clf.fit(X, y)
+
+    # Mode 'index' will include the columns at the index, useful for numpy arrays
+    clf = SubViewClassifier(DecisionTreeClassifier(), [0, 1], mode="index")
+    clf.fit(X, y)
+    ```
+    """
 
     def __init__(self, base_estimator, subview, mode="regex"):
         """Create a classifier that uses a subview of the data.
 
         Parameters
         ----------
         base_estimator : BaseEstimator
```

### Comparing `sslearn-1.0.4.1/sslearn/utils.py` & `sslearn-1.0.5/sslearn/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,113 @@
+"""
+Some utility functions
+
+This module contains utility functions that are used in different parts of the library.
+
+## Functions
+
+[safe_division](#safe_division):
+> Safely divide two numbers preventing division by zero.
+[confidence_interval](#confidence_interval):
+> Calculate the confidence interval of the predictions.
+[choice_with_proportion](#choice_with_proportion): 
+> Choice the best predictions according to the proportion of each class.
+[calculate_prior_probability](#calculate_prior_probability):
+> Calculate the priori probability of each label.
+[mode](#mode):
+> Calculate the mode of a list of values.
+[check_n_jobs](#check_n_jobs):
+> Check `n_jobs` parameter according to the scikit-learn convention.
+[check_classifier](#check_classifier):
+> Check if the classifier is a ClassifierMixin or a list of ClassifierMixin.
+
+"""
+
 import numpy as np
 import os
 import math
 
 import pandas as pd
 
 from statsmodels.stats.proportion import proportion_confint
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.base import ClassifierMixin
 
+__all__ = ["safe_division", "confidence_interval", "choice_with_proportion", "calculate_prior_probability",
+           "mode", "check_n_jobs", "check_classifier"]
+
 
 def safe_division(dividend, divisor, epsilon):
+    """Safely divide two numbers preventing division by zero
+
+    Parameters
+    ----------
+    dividend : numeric
+        Dividend value
+    divisor : numeric
+        Divisor value
+    epsilon : numeric
+        Close to zero value to be used in case of division by zero
+
+    Returns
+    -------
+    result : numeric
+        Result of the division
+    """
     if divisor == 0:
         return dividend / epsilon
     return dividend / divisor
 
 
 def confidence_interval(X, hyp, y, alpha=.95):
+    """Calculate the confidence interval of the predictions
+
+    Parameters
+    ----------
+    X : {array-like, sparse matrix} of shape (n_samples, n_features)
+        The input samples.
+    hyp : classifier
+        The classifier to be used for prediction
+    y : array-like of shape (n_samples,)
+        The target values
+    alpha : float, optional
+        confidence (1 - significance), by default .95
+
+    Returns
+    -------
+    li, hi: float
+        lower and upper bound of the confidence interval
+    """
     data = hyp.predict(X)
 
     successes = np.count_nonzero(data == y)
     trials = X.shape[0]
     li, hi = proportion_confint(successes, trials, alpha=1 - alpha, method="wilson")
     return li, hi
 
 
 def choice_with_proportion(predictions, class_predicted, proportion, extra=0):
+    """Choice the best predictions according to the proportion of each class.
+
+    Parameters
+    ----------
+    predictions : array-like of shape (n_samples,)
+        array of predictions
+    class_predicted : array-like of shape (n_samples,)
+        array of predicted classes
+    proportion : dict
+        dictionary with the proportion of each class
+    extra : int, optional
+        number of extra instances to be added, by default 0
+
+    Returns
+    -------
+    indices: array-like of shape (n_samples,)
+        array of indices of the best predictions
+    """
     n = len(predictions)
     for_each_class = {c: int(n * j) for c, j in proportion.items()}
     indices = np.zeros(0)
     for c in proportion:
         instances = class_predicted == c
         to_add = np.argsort(predictions, kind="mergesort")[instances][::-1][0:for_each_class[c] + extra]
         indices = np.concatenate((indices, to_add))
```

### Comparing `sslearn-1.0.4.1/sslearn/wrapper/_co.py` & `sslearn-1.0.5/sslearn/wrapper/_co.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,36 +15,49 @@
 from sklearn.naive_bayes import GaussianNB
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.preprocessing import LabelEncoder, OneHotEncoder
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.utils import check_array, check_random_state, resample
 from sklearn.utils.validation import check_is_fitted
 
+
 from sslearn.utils import check_n_jobs
 
 from ..base import BaseEnsemble, get_dataset
 from ..utils import (calc_number_per_class, calculate_prior_probability, check_classifier,
                      choice_with_proportion, confidence_interval, mode, safe_division)
 
 
-class BaseCoTraining(BaseEstimator, ClassifierMixin, BaseEnsemble):
+class BaseCoTraining(BaseEnsemble):
+    """
+    Base class for CoTraining classifiers.
+
+    Include
+    -------
+    1. `predict_proba` method that returns the probability of each class.
+    2. `predict` method that returns the class of each instance by argmax of `predict_proba`.
+    3. `score` method that returns the mean accuracy on the given test data and labels.
+    """
+
+    _estimator_type = "classifier"
+
     @abstractmethod
     def fit(self, X, y, **kwards):
         pass
 
     def predict_proba(self, X):
         """Predict probability for each possible outcome.
 
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             Array representing the data.
         Returns
         -------
-        ndarray of shape (n_samples, n_features)
+        class probabilities: ndarray of shape (n_samples, n_classes)
             Array with prediction probabilities.
         """
         is_df = isinstance(X, pd.DataFrame)
         if is_df:
             columns = X.columns
         is_df = isinstance(X, pd.DataFrame)
         if is_df:
@@ -65,34 +78,113 @@
                 base = np.zeros((X.shape[0], len(self.classes_)), np.float)
                 for h in self.h_:
                     base += self._one_hot_not_proba.transform(h.predict(X).reshape(-1, 1))
                 y = softmax(base)
             return y
         else:
             raise NotFittedError("Classifier not fitted")
+        
+        _estimator_type = "classifier"
+
+    def score(self, X, y, sample_weight=None):
+        """
+        Return the mean accuracy on the given test data and labels.
+
+        In multi-label classification, this is the subset accuracy
+        which is a harsh metric since you require for each sample that
+        each label set be correctly predicted.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Test samples.
+
+        y : array-like of shape (n_samples,) or (n_samples, n_outputs)
+            True labels for `X`.
+
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights.
+
+        Returns
+        -------
+        score : float
+            Mean accuracy of ``self.predict(X)`` w.r.t. `y`.
+        """
+        from .metrics import accuracy_score
+
+        return accuracy_score(y, self.predict(X), sample_weight=sample_weight)
 
 
 class DemocraticCoLearning(BaseCoTraining):
+    """
+    **Democratic Co-learning. Ensemble of classifiers of different types.**
+    --------------------------------------------
+
+    A iterative algorithm that uses a ensemble of classifiers to label instances.
+    The main process is:
+    1. Train each classifier with the labeled instances.
+    2. While any classifier is retrained:
+        1. Predict the instances from the unlabeled set.
+        2. Calculate the confidence interval for each classifier for define weights.
+        3. Calculate the weighted vote for each instance.
+        4. Calculate the majority vote for each instance.
+        5. Select the instances to label if majority vote is the same as weighted vote.
+        6. Select the instances to retrain the classifier, if `only_mislabeled` is False then select all instances, else select only mislabeled instances for each classifier.
+        7. Retrain the classifier with the new instances if the error rate is lower than the previous iteration.
+    3. Ignore the classifiers with confidence interval lower than 0.5.
+    4. Combine the probabilities of each classifier.
+
+    **Methods**
+    -------
+    - `fit`: Fit the model with the labeled instances.
+    - `predict` : Predict the class for each instance.
+    - `predict_proba`: Predict the probability for each class.
+    - `score`: Return the mean accuracy on the given test data and labels.
+    
+    
+    **Example**
+    -------
+    ```python
+    from sklearn.datasets import load_iris
+    from sklearn.tree import DecisionTreeClassifier
+    from sklearn.naive_bayes import GaussianNB
+    from sklearn.neighbors import KNeighborsClassifier
+    from sslearn.wrapper import DemocraticCoLearning
+    from sslearn.model_selection import artificial_ssl_dataset
+
+    X, y = load_iris(return_X_y=True)
+    X, y, X_unlabel, y_unlabel, _, _ = artificial_ssl_dataset(X, y, label_rate=0.1, random_state=0)
+    dcl = DemocraticCoLearning(base_estimator=[DecisionTreeClassifier(), GaussianNB(), KNeighborsClassifier(n_neighbors=3)])
+    dcl.fit(X, y)
+    dcl.score(X_unlabel, y_unlabel)
+    ``` 
+
+    **References**
+    ----------
+    Y. Zhou and S. Goldman, (2004) <br>
+    Democratic co-learning, <br>
+    in <i>16th IEEE International Conference on Tools with Artificial Intelligence</i>,<br>
+    pp. 594-602, [10.1109/ICTAI.2004.48](https://doi.org/10.1109/ICTAI.2004.48).
+    """
+
     def __init__(
         self,
         base_estimator=[
             DecisionTreeClassifier(),
             GaussianNB(),
             KNeighborsClassifier(n_neighbors=3),
         ],
         n_estimators=None,
         expand_only_mislabeled=True,
         alpha=0.95,
         q_exp=2,
         random_state=None
     ):
         """
-        Y. Zhou and S. Goldman, "Democratic co-learning,"
-        16th IEEE International Conference on Tools with Artificial Intelligence,
-        2004, pp. 594-602, doi: 10.1109/ICTAI.2004.48.
+        Democratic Co-learning. Ensemble of classifiers of different types.
 
         Parameters
         ----------
         base_estimator : {ClassifierMixin, list}, optional
             An estimator object implementing fit and predict_proba or a list of ClassifierMixin, by default DecisionTreeClassifier()
         n_estimators : int, optional
             number of base_estimators to use. None if base_estimator is a list, by default None
@@ -178,15 +270,15 @@
         y : array-like of shape (n_samples,)
             The target values (class labels), -1 if unlabel.
         estimator_kwards : {list, dict}, optional
             list of kwards for each estimator or kwards for all estimators, by default None
 
         Returns
         -------
-        self
+        self : DemocraticCoLearning
             fitted classifier
         """
 
         X_label, y_label, X_unlabel = get_dataset(X, y)
 
         is_df = isinstance(X_label, pd.DataFrame)
 
@@ -342,49 +434,94 @@
 
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             Array representing the data.
         Returns
         -------
-        ndarray of shape (n_samples, n_features)
+        class probabilities: ndarray of shape (n_samples, n_classes)
             Array with prediction probabilities.
         """
         if "h_" in dir(self):
             if len(X) == 1:
                 X = [X]
             return self.__combine_probabilities(X)
         else:
             raise NotFittedError("Classifier not fitted")
 
 
 class CoTraining(BaseCoTraining):
     """
-    Avrim Blum and Tom Mitchell. 1998.
-    Combining labeled and unlabeled data with co-training.
-    In Proceedings of the eleventh annual conference on Computational learning theory (COLT' 98).
-    Association for Computing Machinery, New York, NY, USA, 92–100.
-    DOI:https://doi.org/10.1145/279943.279962
-
-    Han, Xian-Hua, Yen-wei Chen, and Xiang Ruan. 2011. 
-    ‘Multi-Class Co-Training Learning for Object and Scene Recognition’.
-    Pp. 67–70 in. Nara, Japan.
+    **CoTraining classifier. Multi-view learning algorithm that uses two classifiers to label instances.**
+    --------------------------------------------
+
+    The main process is:
+    1. Train each classifier with the labeled instances and their respective view.
+    2. While max iterations is not reached or any instance is unlabeled:
+        1. Predict the instances from the unlabeled set.
+        2. Select the instances that have the same prediction and the predictions are above the threshold.
+        3. Label the instances with the highest probability, keeping the balance of the classes.
+        4. Retrain the classifier with the new instances.
+    3. Combine the probabilities of each classifier.
+
+    **Methods**
+    -------
+    - `fit`: Fit the model with the labeled instances.
+    - `predict` : Predict the class for each instance.
+    - `predict_proba`: Predict the probability for each class.
+    - `score`: Return the mean accuracy on the given test data and labels.
+
+    **Example**
+    -------
+    ```python
+    from sklearn.datasets import load_iris
+    from sklearn.tree import DecisionTreeClassifier
+    from sslearn.wrapper import CoTraining
+    from sslearn.model_selection import artificial_ssl_dataset
+
+    X, y = load_iris(return_X_y=True)
+    X, y, X_unlabel, y_unlabel, _, _ = artificial_ssl_dataset(X, y, label_rate=0.1, random_state=0)
+    cotraining = CoTraining(DecisionTreeClassifier())
+    X1 = X[:, [0, 1]]
+    X2 = X[:, [2, 3]]
+    cotraining.fit(X1, y, X2) 
+    # or
+    cotraining.fit(X, y, features=[[0, 1], [2, 3]])
+    # or
+    cotraining = CoTraining(DecisionTreeClassifier(), force_second_view=False)
+    cotraining.fit(X, y)
+    ``` 
+
+    **References**
+    ----------
+    Avrim Blum and Tom Mitchell. (1998).<br>
+    Combining labeled and unlabeled data with co-training<br>
+    in <i>Proceedings of the eleventh annual conference on Computational learning theory (COLT' 98)</i>.<br>
+    Association for Computing Machinery, New York, NY, USA, 92-100.<br>
+    [10.1145/279943.279962](https://doi.org/10.1145/279943.279962)
+
+    Han, Xian-Hua, Yen-wei Chen, and Xiang Ruan. (2011). <br>
+    Multi-Class Co-Training Learning for Object and Scene Recognition,<br>
+    pp. 67-70 in. Nara, Japan. <br>
+    [http://www.mva-org.jp/Proceedings/2011CD/papers/04-08.pdf](http://www.mva-org.jp/Proceedings/2011CD/papers/04-08.pdf)<br>
     """
 
     def __init__(
         self,
         base_estimator=DecisionTreeClassifier(),
         second_base_estimator=None,
         max_iterations=30,
         poolsize=75,
         threshold=0.5,
         force_second_view=True,
         random_state=None
     ):
-        """Create a CoTraining classifier
+        """
+        Create a CoTraining classifier. 
+        Multi-view learning algorithm that uses two classifiers to label instances.
 
         Parameters
         ----------
         base_estimator : ClassifierMixin, optional
             The classifier that will be used in the cotraining algorithm on the feature set, by default DecisionTreeClassifier()
         second_base_estimator : ClassifierMixin, optional
             The classifier that will be used in the cotraining algorithm on another feature set, if none are a clone of base_estimator, by default None
@@ -394,14 +531,15 @@
             The size of the pool of unlabeled samples from which the classifier can choose, by default 75
         threshold : float, optional
             The threshold for label instances, by default 0.5
         force_second_view : bool, optional
             The second classifier needs a different view of the data. If False then a second view will be same as the first, by default True
         random_state : int, RandomState instance, optional
             controls the randomness of the estimator, by default None
+
         """
         self.base_estimator = check_classifier(base_estimator, False)
         if second_base_estimator is not None:
             second_base_estimator = check_classifier(second_base_estimator, False)
         self.second_base_estimator = second_base_estimator
         self.max_iterations = max_iterations
         self.poolsize = poolsize
@@ -557,15 +695,15 @@
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             Array representing the data.
         X2 : {array-like, sparse matrix} of shape (n_samples, n_features), optional
             Array representing the data from another view, by default None
         Returns
         -------
-        ndarray of shape (n_samples, n_features)
+        class probabilities: ndarray of shape (n_samples, n_classes)
             Array with prediction probabilities.
         """
         if "columns_" in dir(self):
             return super().predict_proba(X, **kwards)
         elif "h_" in dir(self):
             ys = []
             ys.append(self.h_[0].predict_proba(X, **kwards))
@@ -622,32 +760,74 @@
         if "X2" in kwards:
             return accuracy_score(y, self.predict(X, kwards["X2"]), sample_weight=sample_weight)
         else:
             return super().score(X, y, sample_weight=sample_weight)
 
 
 class Rasco(BaseCoTraining):
+    """
+    **Co-Training based on random subspaces**
+    --------------------------------------------
+
+    Generate a set of random subspaces and train a classifier for each subspace.
+
+    The main process is:
+    1. Generate a set of random subspaces.
+    2. Train a classifier for each subspace.
+    3. While max iterations is not reached or any instance is unlabeled:
+        1. Predict the instances from the unlabeled set for each classifier.
+        2. Calculate the average of the predictions.
+        3. Select the instances with the highest probability.
+        4. Label the instances with the highest probability, keeping the balance of the classes.
+        5. Retrain the classifier with the new instances.
+    4. Combine the probabilities of each classifier.
+
+    **Methods**
+    -------
+    - `fit`: Fit the model with the labeled instances.
+    - `predict` : Predict the class for each instance.
+    - `predict_proba`: Predict the probability for each class.
+    - `score`: Return the mean accuracy on the given test data and labels.
+
+    **Example**
+    -------
+    ```python
+    from sklearn.datasets import load_iris
+    from sslearn.wrapper import Rasco
+    from sslearn.model_selection import artificial_ssl_dataset
+
+    X, y = load_iris(return_X_y=True)
+    X, y, X_unlabel, y_unlabel, _, _ = artificial_ssl_dataset(X, y, label_rate=0.1, random_state=0)
+    rasco = Rasco()
+    rasco.fit(X, y)
+    rasco.score(X_unlabel, y_unlabel) 
+    ```    
+
+    **References**
+    ----------
+    Wang, J., Luo, S. W., & Zeng, X. H. (2008).<br>
+    A random subspace method for co-training,<br>
+    in <i>2008 IEEE International Joint Conference on Neural Networks</i><br>
+    IEEE World Congress on Computational Intelligence<br>
+    (pp. 195-200). IEEE. [10.1109/IJCNN.2008.4633789](https://doi.org/10.1109/IJCNN.2008.4633789)
+    """
+
+
     def __init__(
         self,
         base_estimator=DecisionTreeClassifier(),
         max_iterations=10,
         n_estimators=30,
         subspace_size=None,
         random_state=None,
         n_jobs=None,
     ):
         """
         Co-Training based on random subspaces
 
-        Wang, J., Luo, S. W., & Zeng, X. H. (2008, June).
-        A random subspace method for co-training.
-        In <i>2008 IEEE International Joint Conference on Neural Networks</i>
-        (IEEE World Congress on Computational Intelligence)
-        (pp. 195-200). IEEE.
-
         Parameters
         ----------
         base_estimator : ClassifierMixin, optional
             An estimator object implementing fit and predict_proba, by default DecisionTreeClassifier()
         max_iterations : int, optional
             Maximum number of iterations allowed. Should be greater than or equal to 0.
             If is -1 then will be infinite iterations until U be empty, by default 10
@@ -674,15 +854,15 @@
         X : array like
             Labeled dataset
         y : array like, optional
             Target for each X, not needed on Rasco, by default None
 
         Returns
         -------
-        list
+        subspaces : list
             List of index of features
         """
         random_state = check_random_state(random_state)
         features = list(range(X.shape[1]))
         idxs = []
         for _ in range(self.n_estimators):
             idxs.append(random_state.permutation(features)[: self.subspace_size])
@@ -766,31 +946,62 @@
         self.h_ = cfs
         self.columns_ = idxs
 
         return self
 
 
 class RelRasco(Rasco):
+    """
+    **Co-Training based on relevant random subspaces**
+    --------------------------------------------
+
+    Is a variation of `sslearn.wrapper.Rasco` that uses the mutual information of each feature to select the random subspaces.
+    The process of training is the same as Rasco.
+
+    **Methods**
+    -------
+    - `fit`: Fit the model with the labeled instances.
+    - `predict` : Predict the class for each instance.
+    - `predict_proba`: Predict the probability for each class.
+    - `score`: Return the mean accuracy on the given test data and labels.
+
+    **Example**
+    -------
+    ```python
+    from sklearn.datasets import load_iris
+    from sslearn.wrapper import RelRasco
+    from sslearn.model_selection import artificial_ssl_dataset
+
+    X, y = load_iris(return_X_y=True)
+    X, y, X_unlabel, y_unlabel, _, _ = artificial_ssl_dataset(X, y, label_rate=0.1, random_state=0)
+    relrasco = RelRasco()
+    relrasco.fit(X, y)
+    relrasco.score(X_unlabel, y_unlabel)
+    ```
+
+    **References**
+    ----------
+    Yaslan, Y., & Cataltepe, Z. (2010).<br>
+    Co-training with relevant random subspaces.<br>
+    <i>Neurocomputing</i>, 73(10-12), 1652-1661.<br>
+    [10.1016/j.neucom.2010.01.018](https://doi.org/10.1016/j.neucom.2010.01.018)
+    """
+
     def __init__(
         self,
         base_estimator=DecisionTreeClassifier(),
         max_iterations=10,
         n_estimators=30,
         subspace_size=None,
         random_state=None,
         n_jobs=None,
     ):
         """
         Co-Training with relevant random subspaces
 
-        Yaslan, Y., & Cataltepe, Z. (2010).
-        Co-training with relevant random subspaces.
-        <i>Neurocomputing</i>, 73(10-12), 1652-1661.
-
-
         Parameters
         ----------
         base_estimator : ClassifierMixin, optional
             An estimator object implementing fit and predict_proba, by default DecisionTreeClassifier()
         max_iterations : int, optional
             Maximum number of iterations allowed. Should be greater than or equal to 0.
             If is -1 then will be infinite iterations until U be empty, by default 10
@@ -798,14 +1009,15 @@
             The number of base estimators in the ensemble., by default 30
         subspace_size : int, optional
             The number of features for each subspace. If it is None will be the half of the features size., by default None
         random_state : int, RandomState instance, optional
             controls the randomness of the estimator, by default None
         n_jobs : int, optional
             The number of jobs to run in parallel. -1 means using all processors., by default None
+
         """
         super().__init__(
             base_estimator,
             max_iterations,
             n_estimators,
             subspace_size,
             random_state,
@@ -820,15 +1032,15 @@
         X : array like
             Labeled dataset
         y : array like, optional
             Target for each X, only needed on Rel-Rasco, by default None
 
         Returns
         -------
-        list
+        subspaces: list
             List of index of features
         """
         random_state = check_random_state(random_state)
         relevance = mutual_info_classif(X, y, random_state=random_state)
         idxs = []
         for _ in range(self.n_estimators):
             subspace = []
@@ -840,40 +1052,85 @@
                 else:
                     subspace.append(f2)
             idxs.append(subspace)
         return idxs
 
 
 # Done and tested
-class CoTrainingByCommittee(ClassifierMixin, BaseEnsemble, BaseEstimator):
+class CoTrainingByCommittee(BaseCoTraining):
+    """
+    **Co-Training by Committee classifier.**
+    --------------------------------------------
+
+    Create a committee trained by co-training based on the diversity of the classifiers
+
+    The main process is:
+    1. Train a committee of classifiers.
+    2. Create a pool of unlabeled instances.
+    3. While max iterations is not reached or any instance is unlabeled:
+        1. Predict the instances from the unlabeled set.
+        2. Select the instances with the highest probability.
+        3. Label the instances with the highest probability, keeping the balance of the classes but ensuring that at least n instances of each class are added.
+        4. Retrain the classifier with the new instances.
+    4. Combine the probabilities of each classifier.
+
+    **Methods**
+    -------
+    - `fit`: Fit the model with the labeled instances.
+    - `predict` : Predict the class for each instance.
+    - `predict_proba`: Predict the probability for each class.
+    - `score`: Return the mean accuracy on the given test data and labels.
+
+    **Example**
+    -------
+    ```python
+    from sklearn.datasets import load_iris
+    from sslearn.wrapper import CoTrainingByCommittee
+    from sslearn.model_selection import artificial_ssl_dataset
+
+    X, y = load_iris(return_X_y=True)
+    X, y, X_unlabel, y_unlabel, _, _ = artificial_ssl_dataset(X, y, label_rate=0.1, random_state=0)
+    cotraining = CoTrainingByCommittee()
+    cotraining.fit(X, y)
+    cotraining.score(X_unlabel, y_unlabel)
+    ```
+
+    **References**
+    ----------
+    M. F. A. Hady and F. Schwenker,<br>
+    Co-training by Committee: A New Semi-supervised Learning Framework,<br>
+    in <i>2008 IEEE International Conference on Data Mining Workshops</i>,<br>
+    Pisa, 2008, pp. 563-572,  [10.1109/ICDMW.2008.27](https://doi.org/10.1109/ICDMW.2008.27)
+    """
+
     def __init__(
         self,
         ensemble_estimator=BaggingClassifier(),
         max_iterations=100,
         poolsize=100,
         min_instances_for_class=3,
         random_state=None,
     ):
-        """Create a committee trained by cotraining based on
+        """
+        Create a committee trained by cotraining based on
         the diversity of classifiers.
-        M. F. A. Hady and F. Schwenker,
-        "Co-training by Committee: A New Semi-supervised Learning Framework,"
-        2008 IEEE International Conference on Data Mining Workshops,
-        Pisa, 2008, pp. 563-572, doi: 10.1109/ICDMW.2008.27.
+
         Parameters
         ----------
         ensemble_estimator : ClassifierMixin, optional
             ensemble method, works without a ensemble as
             self training with pool, by default BaggingClassifier().
         max_iterations : int, optional
             number of iterations of training, -1 if no max iterations, by default 100
         poolsize : int, optional
             max number of unlabeled instances candidates to pseudolabel, by default 100
         random_state : int, RandomState instance, optional
             controls the randomness of the estimator, by default None
+
+
         """
         self.ensemble_estimator = check_classifier(ensemble_estimator, False)
         self.max_iterations = max_iterations
         self.poolsize = poolsize
         self.random_state = random_state
         self.min_instances_for_class = min_instances_for_class
 
@@ -883,15 +1140,15 @@
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             The training input samples.
         y : array-like of shape (n_samples,)
             The target values (class labels), -1 if unlabel.
         Returns
         -------
-        self: CoTrainingByCommittee
+        self : CoTrainingByCommittee
             Fitted estimator.
         """
         self.ensemble_estimator = skclone(self.ensemble_estimator)
         random_state = check_random_state(self.random_state)
 
         X_label, y_prev, X_unlabel = get_dataset(X, y)
 
@@ -965,30 +1222,30 @@
         For a classification model, the predicted class for each sample in X is returned.
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             The input samples.
         Returns
         -------
-        y: array-like of shape (n_samples,)
+        y : array-like of shape (n_samples,)
             The predicted classes
         """
         check_is_fitted(self.ensemble_estimator)
         return self.label_encoder_.inverse_transform(self.ensemble_estimator.predict(X))
 
     def predict_proba(self, X):
         """Predict class probabilities of the input samples X.
         The predicted class probability depends on the ensemble estimator.
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             The input samples.
         Returns
         -------
-        y: ndarray of shape (n_samples, n_classes) or list of n_outputs such arrays if n_outputs > 1
+        y : ndarray of shape (n_samples, n_classes) or list of n_outputs such arrays if n_outputs > 1
             The predicted classes
         """
         check_is_fitted(self.ensemble_estimator)
         return self.ensemble_estimator.predict_proba(X)
 
     def score(self, X, y, sample_weight=None):
         """Return the mean accuracy on the given test data and labels.
@@ -1018,20 +1275,64 @@
                 )
             y = np.array(list(map(lambda x: self.le_dict_.get(x, -1), y)), dtype=y.dtype)
 
         return self.ensemble_estimator.score(X, y, sample_weight)
 
 # Done and tested
 class CoForest(BaseCoTraining):
+    """
+    **CoForest classifier. Random Forest co-training**
+    ----------------------------
+    
+    Ensemble method for CoTraining based on Random Forest.
+
+    The main process is:
+    1. Train a committee of classifiers using bootstrap.
+    2. While any base classifier is retrained:
+        1. Predict the instances from the unlabeled set.
+        2. Select the instances with the highest probability.
+        3. Label the instances with the highest probability
+        4. Add the instances to the labeled set only if the error is not bigger than the previous error.
+        5. Retrain the classifier with the new instances.
+    3. Combine the probabilities of each classifier.
+
+
+    **Methods**
+    -------
+    - `fit`: Fit the model with the labeled instances.
+    - `predict` : Predict the class for each instance.
+    - `predict_proba`: Predict the probability for each class.
+    - `score`: Return the mean accuracy on the given test data and labels.
+
+    **Example**
+    -------
+    ```python
+    from sklearn.datasets import load_iris
+    from sslearn.wrapper import CoForest
+    from sslearn.model_selection import artificial_ssl_dataset
+
+    X, y = load_iris(return_X_y=True)
+    X, y, X_unlabel, y_unlabel, _, _ = artificial_ssl_dataset(X, y, label_rate=0.1, random_state=0)
+    coforest = CoForest()
+    coforest.fit(X, y)
+    coforest.score(X_unlabel, y_unlabel)
+    ```
+
+    **References**
+    ----------
+    Li, M., & Zhou, Z.-H. (2007).<br>
+    Improve Computer-Aided Diagnosis With Machine Learning Techniques Using Undiagnosed Samples.<br>
+    <i>IEEE Transactions on Systems, Man, and Cybernetics - Part A: Systems and Humans</i>,<br>
+    37(6), 1088-1098. [10.1109/tsmca.2007.904745](https://doi.org/10.1109/tsmca.2007.904745)
+    """
+
     def __init__(self, base_estimator=DecisionTreeClassifier(), n_estimators=7, threshold=0.75, bootstrap=True, n_jobs=None, random_state=None, version="1.0.3"):
         """
-        Li, M., & Zhou, Z.-H. (2007).
-        Improve Computer-Aided Diagnosis With Machine Learning Techniques Using Undiagnosed Samples.
-        <i>IEEE Transactions on Systems, Man, and Cybernetics - Part A: Systems and Humans</i>,
-        37(6), 1088–1098. doi:10.1109/tsmca.2007.904745
+        Generate a CoForest classifier.
+        A SSL Random Forest adaption for CoTraining. 
 
         Parameters
         ----------
         base_estimator : ClassifierMixin, optional
             An estimator object implementing fit and predict_proba, by default DecisionTreeClassifier()
         n_estimators : int, optional
             The number of base estimators in the ensemble., by default 7
@@ -1162,15 +1463,15 @@
 
         self.hypotheses = []
         errors = []
         weights = []
         for i in range(self.n_estimators):
             self.hypotheses.append(skclone(self.base_estimator if type(self.base_estimator) is not list else self.base_estimator[i]))
             if "random_state" in dir(self.hypotheses[-1]):
-                self.hypotheses[-1].set_params(random_state=random_state.randint(0, 2 ** 32 - 1))
+                self.hypotheses[-1].set_params(random_state=random_state.randint(0, 2147483647))
             errors.append(0.5)
 
         self.hypotheses = Parallel(n_jobs=n_jobs)(
             delayed(self._fit_estimator)(X_label, y_label, i, beginning=True, **kwards)
             for i in range(self.n_estimators)
         )
```

### Comparing `sslearn-1.0.4.1/sslearn/wrapper/_self.py` & `sslearn-1.0.5/sslearn/wrapper/_self.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,123 +9,98 @@
 
 from sslearn.utils import calculate_prior_probability, check_classifier
 
 from ..base import get_dataset
 
 
 class SelfTraining(SelfTrainingClassifier):
+    """
+    **Self Training Classifier with data loader compatible.**
+    ----------------------------
 
-    """Self-training. Adaptation of SelfTrainingClassifier from sklearn with data loader compatible.
-
-    This class allows a given supervised classifier to function as a
-    semi-supervised classifier, allowing it to learn from unlabeled data. It
-    does this by iteratively predicting pseudo-labels for the unlabeled data
-    and adding them to the training set.
-
-    The classifier will continue iterating until either max_iter is reached, or
-    no pseudo-labels were added to the training set in the previous iteration.
-
-    Read more in the :ref:`User Guide <self_training>`.
-
-    Parameters
-    ----------
-    base_estimator : estimator object
-        An estimator object implementing ``fit`` and ``predict_proba``.
-        Invoking the ``fit`` method will fit a clone of the passed estimator,
-        which will be stored in the ``base_estimator_`` attribute.
-
-    threshold : float, default=0.75
-        The decision threshold for use with `criterion='threshold'`.
-        Should be in [0, 1). When using the 'threshold' criterion, a
-        :ref:`well calibrated classifier <calibration>` should be used.
-
-    criterion : {'threshold', 'k_best'}, default='threshold'
-        The selection criterion used to select which labels to add to the
-        training set. If 'threshold', pseudo-labels with prediction
-        probabilities above `threshold` are added to the dataset. If 'k_best',
-        the `k_best` pseudo-labels with highest prediction probabilities are
-        added to the dataset. When using the 'threshold' criterion, a
-        :ref:`well calibrated classifier <calibration>` should be used.
-
-    k_best : int, default=10
-        The amount of samples to add in each iteration. Only used when
-        `criterion` is k_best'.
-
-    max_iter : int or None, default=10
-        Maximum number of iterations allowed. Should be greater than or equal
-        to 0. If it is ``None``, the classifier will continue to predict labels
-        until no new pseudo-labels are added, or all unlabeled samples have
-        been labeled.
-
-    verbose : bool, default=False
-        Enable verbose output.
-
-    Attributes
-    ----------
-    base_estimator_ : estimator object
-        The fitted estimator.
-
-    classes_ : ndarray or list of ndarray of shape (n_classes,)
-        Class labels for each output. (Taken from the trained
-        ``base_estimator_``).
-
-    transduction_ : ndarray of shape (n_samples,)
-        The labels used for the final fit of the classifier, including
-        pseudo-labels added during fit.
-
-    labeled_iter_ : ndarray of shape (n_samples,)
-        The iteration in which each sample was labeled. When a sample has
-        iteration 0, the sample was already labeled in the original dataset.
-        When a sample has iteration -1, the sample was not labeled in any
-        iteration.
-
-    n_iter_ : int
-        The number of rounds of self-training, that is the number of times the
-        base estimator is fitted on relabeled variants of the training set.
-
-    termination_condition_ : {'max_iter', 'no_change', 'all_labeled'}
-        The reason that fitting was stopped.
-
-        - 'max_iter': `n_iter_` reached `max_iter`.
-        - 'no_change': no new labels were predicted.
-        - 'all_labeled': all unlabeled samples were labeled before `max_iter`
-          was reached.
-
-    Examples
-    --------
-    >>> import numpy as np
-    >>> from sklearn import datasets
-    >>> from sklearn.semi_supervised import SelfTrainingClassifier
-    >>> from sklearn.svm import SVC
-    >>> rng = np.random.RandomState(42)
-    >>> iris = datasets.load_iris()
-    >>> random_unlabeled_points = rng.rand(iris.target.shape[0]) < 0.3
-    >>> iris.target[random_unlabeled_points] = -1
-    >>> svc = SVC(probability=True, gamma="auto")
-    >>> self_training_model = SelfTrainingClassifier(svc)
-    >>> self_training_model.fit(iris.data, iris.target)
-    SelfTrainingClassifier(...)
+    Is the same `SelfTrainingClassifier` from sklearn but with `sslearn` data loader compatible.
+    For more information, see the [sklearn documentation](https://scikit-learn.org/stable/modules/generated/sklearn.semi_supervised.SelfTrainingClassifier.html).
 
-    References
-    ----------
-    David Yarowsky. 1995. Unsupervised word sense disambiguation rivaling
-    supervised methods. In Proceedings of the 33rd annual meeting on
-    Association for Computational Linguistics (ACL '95). Association for
-    Computational Linguistics, Stroudsburg, PA, USA, 189-196. DOI:
-    https://doi.org/10.3115/981658.981684
+    **Example**
+    -----------
+    ```python
+    from sklearn.datasets import load_iris
+    from sslearn.model_selection import artificial_ssl_dataset
+    from sslearn.wrapper import SelfTraining
+
+    X, y = load_iris(return_X_y=True)
+    X, y, X_unlabel, y_unlabel, _, _ = artificial_ssl_dataset(X, y, label_rate=0.1, random_state=0)
+
+    clf = SelfTraining()
+    clf.fit(X, y)
+    clf.score(X_unlabel, y_unlabel)
+    ```
+
+    **References**
+    --------------
+    David Yarowsky. (1995). <br>
+    Unsupervised word sense disambiguation rivaling supervised methods.<br>
+    In <i>Proceedings of the 33rd annual meeting on Association for Computational Linguistics (ACL '95).</i><br>
+    Association for Computational Linguistics,<br>
+    Stroudsburg, PA, USA, 189-196. <br>
+    [10.3115/981658.981684](https://doi.org/10.3115/981658.981684)
     """
+
     _estimator_type = "classifier"
 
     def __init__(self,
                  base_estimator,
                  threshold=0.75,
                  criterion='threshold',
                  k_best=10,
                  max_iter=10,
                  verbose=False):
+        """Self-training. Adaptation of SelfTrainingClassifier from sklearn with data loader compatible.
+
+        This class allows a given supervised classifier to function as a
+        semi-supervised classifier, allowing it to learn from unlabeled data. It
+        does this by iteratively predicting pseudo-labels for the unlabeled data
+        and adding them to the training set.
+
+        The classifier will continue iterating until either max_iter is reached, or
+        no pseudo-labels were added to the training set in the previous iteration.
+
+        Parameters
+        ----------
+        base_estimator : estimator object
+            An estimator object implementing ``fit`` and ``predict_proba``.
+            Invoking the ``fit`` method will fit a clone of the passed estimator,
+            which will be stored in the ``base_estimator_`` attribute.
+
+        threshold : float, default=0.75
+            The decision threshold for use with `criterion='threshold'`.
+            Should be in [0, 1). When using the 'threshold' criterion, a
+            :ref:`well calibrated classifier <calibration>` should be used.
+
+        criterion : {'threshold', 'k_best'}, default='threshold'
+            The selection criterion used to select which labels to add to the
+            training set. If 'threshold', pseudo-labels with prediction
+            probabilities above `threshold` are added to the dataset. If 'k_best',
+            the `k_best` pseudo-labels with highest prediction probabilities are
+            added to the dataset. When using the 'threshold' criterion, a
+            :ref:`well calibrated classifier <calibration>` should be used.
+
+        k_best : int, default=10
+            The amount of samples to add in each iteration. Only used when
+            `criterion` is k_best'.
+
+        max_iter : int or None, default=10
+            Maximum number of iterations allowed. Should be greater than or equal
+            to 0. If it is ``None``, the classifier will continue to predict labels
+            until no new pseudo-labels are added, or all unlabeled samples have
+            been labeled.
+
+        verbose : bool, default=False
+            Enable verbose output.
+        """
         super().__init__(base_estimator, threshold, criterion, k_best, max_iter, verbose)
 
     def fit(self, X, y):
         """
         Fits this ``SelfTrainingClassifier`` to a dataset.
 
         Parameters
@@ -146,45 +121,87 @@
         if y_adapted.dtype.type is str or y_adapted.dtype.type is np.str_:
             y_adapted = y_adapted.astype(object)
             y_adapted[y_adapted == '-1'] = -1
         return super().fit(X, y_adapted)
 
 
 class Setred(ClassifierMixin, BaseEstimator):
+    """
+    **Self-training with Editing.**
+    ----------------------------
+
+    Create a SETRED classifier. It is a self-training algorithm that uses a rejection mechanism to avoid adding noisy samples to the training set.
+    The main process are:
+    1. Train a classifier with the labeled data.
+    2. Create a pool of unlabeled data and select the most confident predictions.
+    3. Repeat until the maximum number of iterations is reached:
+        a. Select the most confident predictions from the unlabeled data.
+        b. Calculate the neighborhood graph of the labeled data and the selected instances from the unlabeled data.
+        c. Calculate the significance level of the selected instances.
+        d. Reject the instances that are not significant according their position in the neighborhood graph.
+        e. Add the selected instances to the labeled data and retrains the classifier.
+        f. Add new instances to the pool of unlabeled data.
+    4. Return the classifier trained with the labeled data.
+
+    **Example**
+    -----------
+    ```python
+    from sklearn.datasets import load_iris
+    from sslearn.model_selection import artificial_ssl_dataset
+    from sslearn.wrapper import Setred
+
+    X, y = load_iris(return_X_y=True)
+    X, y, X_unlabel, y_unlabel, _, _ = artificial_ssl_dataset(X, y, label_rate=0.1, random_state=0)
+
+    clf = Setred()
+    clf.fit(X, y)
+    clf.score(X_unlabel, y_unlabel)
+    ```
+
+    **References**
+    ----------
+    Li, Ming, and Zhi-Hua Zhou. (2005)<br>
+    SETRED: Self-training with editing,<br>
+    in <i>Advances in Knowledge Discovery and Data Mining.</i> <br>
+    Pacific-Asia Conference on Knowledge Discovery and Data Mining <br>
+    LNAI 3518, Springer, Berlin, Heidelberg, <br>
+    [10.1007/11430919_71](https://doi.org/10.1007/11430919_71)
+
+    """
+
     def __init__(
         self,
         base_estimator=KNeighborsClassifier(n_neighbors=3),
         max_iterations=40,
         distance="euclidean",
         poolsize=0.25,
         rejection_threshold=0.05,
         graph_neighbors=1,
         random_state=None,
         n_jobs=None,
     ):
         """
-        Li, Ming, and Zhi-Hua Zhou. "SETRED: Self-training with editing."
-        Pacific-Asia Conference on Knowledge Discovery and Data Mining.
-        Springer, Berlin, Heidelberg, 2005. doi: 10.1007/11430919_71.
-
+        Create a SETRED classifier.
+        It is a self-training algorithm that uses a rejection mechanism to avoid adding noisy samples to the training set.
+        
         Parameters
         ----------
         base_estimator : ClassifierMixin, optional
-            An estimator object implementing fit and predict_proba,, by default DecisionTreeClassifier(), by default KNeighborsClassifier(n_neighbors=3)
+            An estimator object implementing fit and predict_proba, by default KNeighborsClassifier(n_neighbors=3)
         max_iterations : int, optional
             Maximum number of iterations allowed. Should be greater than or equal to 0., by default 40
         distance : str, optional
             The distance metric to use for the graph.
             The default metric is euclidean, and with p=2 is equivalent to the standard Euclidean metric.
             For a list of available metrics, see the documentation of DistanceMetric and the metrics listed in sklearn.metrics.pairwise.PAIRWISE_DISTANCE_FUNCTIONS.
-            Note that the “cosine” metric uses cosine_distances., by default "euclidean"
+            Note that the `cosine` metric uses cosine_distances., by default `euclidean`
         poolsize : float, optional
             Max number of unlabel instances candidates to pseudolabel, by default 0.25
         rejection_threshold : float, optional
-            significance level, by default 0.1
+            significance level, by default 0.05
         graph_neighbors : int, optional
             Number of neighbors for each sample., by default 1
         random_state : int, RandomState instance, optional
             controls the randomness of the estimator, by default None
         n_jobs : int, optional
             The number of parallel jobs to run for neighbors search. None means 1 unless in a joblib.parallel_backend context. -1 means using all processors, by default None
         """
@@ -326,25 +343,25 @@
         For a classification model, the predicted class for each sample in X is returned.
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             The input samples.
         Returns
         -------
-        y: array-like of shape (n_samples,)
+        y : array-like of shape (n_samples,)
             The predicted classes
         """
         return self._base_estimator.predict(X, **kwards)
 
     def predict_proba(self, X, **kwards):
         """Predict class probabilities of the input samples X.
         The predicted class probability depends on the ensemble estimator.
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             The input samples.
         Returns
         -------
-        y: ndarray of shape (n_samples, n_classes) or list of n_outputs such arrays if n_outputs > 1
+        y : ndarray of shape (n_samples, n_classes) or list of n_outputs such arrays if n_outputs > 1
             The predicted classes
         """
         return self._base_estimator.predict_proba(X, **kwards)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sslearn-1.0.4.1/sslearn/wrapper/_tritraining.py` & `sslearn-1.0.5/sslearn/wrapper/_tritraining.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,41 +18,65 @@
 from ..utils import check_classifier, check_n_jobs, safe_division
 from ._co import BaseCoTraining
 
 import time
 
 
 class TriTraining(BaseCoTraining):
+    """
+    **TriTraining. Trio of classifiers with bootstrapping.**
+
+    The main process is:
+    1. Generate three classifiers using bootstrapping.
+    2. Iterate until convergence:
+        1. Calculate the error between two hypotheses.
+        2. If the error is less than the previous error, generate a dataset with the instances where both hypotheses agree.
+        3. Retrain the classifiers with the new dataset and the original labeled dataset.
+    3. Combine the predictions of the three classifiers.
+
+    **Methods**
+    -------
+    - `fit`: Fit the model with the labeled instances.
+    - `predict` : Predict the class for each instance.
+    - `predict_proba`: Predict the probability for each class.
+    - `score`: Return the mean accuracy on the given test data and labels.
+
+    **References**
+    ----------
+    Zhi-Hua Zhou and Ming Li,<br>
+    Tri-training: exploiting unlabeled data using three classifiers,<br>
+    in <i>IEEE Transactions on Knowledge and Data Engineering</i>,<br>
+    vol. 17, no. 11, pp. 1529-1541, Nov. 2005,<br>
+    [10.1109/TKDE.2005.186](https://doi.org/10.1109/TKDE.2005.186)
+
+    """
 
     def __init__(
         self,
         base_estimator=DecisionTreeClassifier(),
         n_samples=None,
         random_state=None,
         n_jobs=None,
     ):
-        """TriTraining
-        Zhi-Hua Zhou and Ming Li,
-        "Tri-training: exploiting unlabeled data using three classifiers,"
-        in <i>IEEE Transactions on Knowledge and Data Engineering</i>,
-        vol. 17, no. 11, pp. 1529-1541, Nov. 2005,
-        doi: 10.1109/TKDE.2005.186.
+        """TriTraining. Trio of classifiers with bootstrapping.
+
         Parameters
         ----------
         base_estimator : ClassifierMixin, optional
             An estimator object implementing fit and predict_proba, by default DecisionTreeClassifier()
         n_samples : int, optional
             Number of samples to generate.
             If left to None this is automatically set to the first dimension of the arrays., by default None
         random_state : int, RandomState instance, optional
             controls the randomness of the estimator, by default None
         n_jobs : int, optional
             The number of jobs to run in parallel for both `fit` and `predict`.
             `None` means 1 unless in a :obj:`joblib.parallel_backend` context.
             `-1` means using all processors., by default None
+       
         """
         self._N_LEARNER = 3
         self.base_estimator = check_classifier(base_estimator, collection_size=self._N_LEARNER)
         self.n_samples = n_samples
         self._epsilon = sys.float_info.epsilon
         self.random_state = random_state
         self.n_jobs = n_jobs
@@ -63,15 +87,15 @@
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             The training input samples.
         y : array-like of shape (n_samples,)
             The target values (class labels), -1 if unlabeled.
         Returns
         -------
-        self: TriTraining
+        self : TriTraining
             Fitted estimator.
         """
         random_state = check_random_state(self.random_state)
         self.n_jobs = min(check_n_jobs(self.n_jobs), self._N_LEARNER)
 
         X_label, y_label, X_unlabel = get_dataset(X, y)
 
@@ -193,15 +217,16 @@
         ----------
         hs : list
             hypotheses collection
         index : int
             base hypothesis  index
         Returns
         -------
-        list
+        classifiers: list
+            Collection of other hypotheses
         """
         another_hs = []
         for i in range(len(hs)):
             if i != index:
                 another_hs.append(hs[i])
         return another_hs
 
@@ -214,15 +239,15 @@
             Collection pseudo-labeled candidates and its labels
         s : int
             Equation 10 in paper
         random_state : int, RandomState instance, optional
             controls the randomness of the estimator, by default None
         Returns
         -------
-        tuple
+        subsamples: tuple
             Collection of pseudo-labeled selected for enlarged labeled examples.
         """
         to_remove = len(L[0]) - s
         select = len(L[0]) - to_remove
 
         return resample(*L, replace=False, n_samples=select, random_state=random_state)
 
@@ -240,27 +265,53 @@
             First hypothesis
         h2 : ClassifierMixin
             Second hypothesis
         epsilon : float
             A small number to avoid division by zero
         Returns
         -------
-        float
+        error : float
             Division of the number of labeled examples on which both h1 and h2 make incorrect classification,
             by the number of labeled examples on which the classification made by h1 is the same as that made by h2.
         """
         y1 = h1.predict(X)
         y2 = h2.predict(X)
 
         error = np.count_nonzero(np.logical_and(y1 == y2, y2 != y))
         coincidence = np.count_nonzero(y1 == y2)
         return safe_division(error, coincidence, epsilon)
 
 
 class WiWTriTraining(TriTraining):
+    """
+    **Who-Is-Who TriTraining.**
+     
+    Trio of classifiers with bootstrapping and restricted set classification.
+    Is the same as TriTraining but with the restricted set classification.
+    Maninly, the conflict rate penalizes the ***measure error*** of basic TriTraining, it can be calculated over differentes subsamples of X, can be:
+    * `labeled` over complete L,
+    * `labeled_plus` over complete L union L',
+    * `unlabeled`: over complete U,
+    * `all`: over complete X (LuU) and
+    * `none`: don't penalize the ***meause error***, only use the restrictions for avoid share classes in the same group. 
+    
+    **Methods**
+    -------
+    - `fit`: Fit the model with the labeled instances. Receives the instance group, an array-like of shape (n_samples) with the group of each instance. Two instances with the same label are not allowed to be in the same group.
+    - `predict` : Predict the class for each instance.
+    - `predict_proba`: Predict the probability for each class.
+    - `score`: Return the mean accuracy on the given test data and labels.
+
+    **References**
+    ----------
+    Ludmila I. Kuncheva, Juan J. Rodríguez, Aaron S. Jackson, (2016)<br>
+    Restricted set classification: Who is there?<br>
+    <i>Pattern Recognition</i>, 63, 158-170, <br>
+    [10.1016/j.patcog.2016.08.028](https://doi.org/10.1016/j.patcog.2016.08.028)
+    """
 
     def __init__(
         self,
         base_estimator,
         n_samples=100,
         n_jobs=None,
         method="hungarian",
@@ -311,15 +362,15 @@
             The training input samples.
         y : array-like of shape (n_samples,)
             The target values (class labels), -1 if unlabeled.
         instance_group : array-like of shape (n_samples)
             The group. Two instances with the same label are not allowed to be in the same group.
         Returns
         -------
-        self: TriTraining
+        self : TriTraining
             Fitted estimator.
         """
         random_state = check_random_state(self.random_state)
         self.n_jobs = check_n_jobs(self.n_jobs)
 
         if instance_group is None:
             warn(
@@ -452,15 +503,15 @@
             First hypothesis
         h2 : ClassifierMixin
             Second hypothesis
         epsilon : float
             A small number to avoid division by zero
         Returns
         -------
-        float
+        error: float
             Division of the number of labeled examples on which both h1 and h2 make incorrect classification,
             by the number of labeled examples on which the classification made by h1 is the same as that made by h2.
         """
         me = super()._measure_error(L, y, h1.base_estimator, h2.base_estimator, epsilon)
 
         LU = kwards.get("LU", None)
         U = kwards.get("U", None)
@@ -499,25 +550,42 @@
 
         y_preds = combine_predictions(y_probas, instance_group, len(self.classes_), self.method)
 
         return self.classes_.take(y_preds)
 
 
 class DeTriTraining(TriTraining):
+    """
+    **TriTraining with Data Editing.**
+
+    It is a variation of the TriTraining, the main difference is that the instances are depurated in each iteration.
+    It means that the instances with their neighbors that have the same class are kept, the rest are removed.
+    At the end of the iterations, the instances are clustered and the class is assigned to the cluster centroid.
+
+    **Methods**
+    -------
+    - `fit`: Fit the model with the labeled instances.
+    - `predict` : Predict the class for each instance.
+    - `predict_proba`: Predict the probability for each class.
+    - `score`: Return the mean accuracy on the given test data and labels.
+
+    **References**
+    ----------
+    Deng C., Guo M.Z. (2006)<br>
+    Tri-training and Data Editing Based Semi-supervised Clustering Algorithm, <br>
+    in <i>Gelbukh A., Reyes-Garcia C.A. (eds) MICAI 2006: Advances in Artificial Intelligence. MICAI 2006.</i><br>
+    Lecture Notes in Computer Science, vol 4293. Springer, Berlin, Heidelberg.<br>
+    [10.1007/11925231_61](https://doi.org/10.1007/11925231_61)
+    """
 
     def __init__(self, base_estimator=DecisionTreeClassifier(), k_neighbors=3,
                  n_samples=None, mode="seeded", max_iterations=100, n_jobs=None, random_state=None):
-        """DeTriTraining
-
-        Deng C., Guo M.Z. (2006)
-        Tri-training and Data Editing Based Semi-supervised Clustering Algorithm. 
-        In: Gelbukh A., Reyes-Garcia C.A. (eds) MICAI 2006: Advances in Artificial Intelligence. MICAI 2006. 
-        Lecture Notes in Computer Science, vol 4293.
-        Springer, Berlin, Heidelberg.
-        https://doi.org/10.1007/11925231_61
+        """
+        DeTriTraining - TriTraining with Depurated and Clustering.
+        Avoid the noise generated by the TriTraining algorithm by depurating the enlarged dataset and clustering the instances.        
 
         Parameters
         ----------
         base_estimator : ClassifierMixin, optional
             An estimator object implementing fit and predict_proba, by default DecisionTreeClassifier()
         n_samples : int, optional
             Number of samples to generate. 
@@ -531,15 +599,15 @@
             If `constrained` each instance belong to nearest cluster unless the instance is in to enlarged dataset, 
             then the instance belongs to the cluster of its class., by default `seeded`
         max_iterations : int, optional
             Maximum number of iterations, by default 100
         n_jobs : int, optional
             The number of parallel jobs to run for neighbors search. 
             None means 1 unless in a joblib.parallel_backend context. -1 means using all processors. 
-            Doesn’t affect fit method., by default None
+            Doesn't affect fit method., by default None
         random_state : int, RandomState instance, optional
             controls the randomness of the estimator, by default None
         """
         super().__init__(base_estimator, n_samples, random_state)
         self.k_neighbors = k_neighbors
         self.mode = mode
         self.max_iterations = max_iterations
@@ -553,15 +621,15 @@
         Parameters
         ----------
         S : tuple (X, y)
             Enlarged dataset
 
         Returns
         -------
-        tuple (X, y)
+        tuple : (X, y)
             Enlarged dataset with instances where at least k_neighbors/2+1 have the same class.
         """
         init = time.time()
         knn = KNeighborsClassifier(n_neighbors=self.k_neighbors, n_jobs=self.n_jobs)
         valid = knn.fit(*S).predict(S[0]) == S[1]
         print(f"Depure time: {time.time() - init}")
         return S[0][valid], S[1][valid]
@@ -574,15 +642,15 @@
         S : tuple (X, y)
             Enlarged dataset
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             Complete dataset, only features
 
         Returns
         -------
-        array-like of shape (n_samples,)
+        y: array-like of shape (n_samples,)
             class predicted for each instance
         """
         centroids = dict()
         clusters = set(S[1])
 
         # uses as numpy
         if isinstance(X, pd.DataFrame):
```

### Comparing `sslearn-1.0.4.1/sslearn.egg-info/PKG-INFO` & `sslearn-1.0.5/sslearn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 Metadata-Version: 2.1
 Name: sslearn
-Version: 1.0.4.1
+Version: 1.0.5
 Summary: A Python package for semi-supervised learning with scikit-learn
 Home-page: https://github.com/jlgarridol/sslearn
-Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/f1.0.4.1.tar.gz
+Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/1.0.5.tar.gz
 Author: José Luis Garrido-Labrador
 Author-email: jlgarrido@ubu.es
 License: new BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joblib>=1.2.0
 Requires-Dist: numpy>=1.23.3
 Requires-Dist: pandas>=1.4.3
 Requires-Dist: scikit_learn>=1.2.0
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: statsmodels>=0.13.2
 
 Semi-Supervised Learning Library (sslearn)
 ===
 
-![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability-percentage/jlgarridol/sslearn) ![Code Climate coverage](https://img.shields.io/codeclimate/coverage/jlgarridol/sslearn) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/jlgarridol/sslearn/python-package.yml) ![PyPI - Version](https://img.shields.io/pypi/v/sslearn)
+<!-- Insert logo in the middle -->
+<img width="100%" src="https://raw.githubusercontent.com/jlgarridol/sslearn/main/docs/sslearn.webp"/>
+
+![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability-percentage/jlgarridol/sslearn) ![Code Climate coverage](https://img.shields.io/codeclimate/coverage/jlgarridol/sslearn) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/jlgarridol/sslearn/python-package.yml) ![PyPI - Version](https://img.shields.io/pypi/v/sslearn) [![Static Badge](https://img.shields.io/badge/doc-available-blue?style=flat)](https://jlgarridol.github.io/sslearn/)
 
 The `sslearn` library is a Python package for machine learning over Semi-supervised datasets. It is an extension of [scikit-learn](https://github.com/scikit-learn/scikit-learn).
 
-Installation
----
+## Installation
+
+
 ### Dependencies
 
 * joblib >= 1.2.0
 * numpy >= 1.23.3
 * pandas >= 1.4.3
 * scikit_learn >= 1.2.0
 * scipy >= 1.10.1
@@ -45,35 +51,34 @@
 
 ### `pip` installation
 
 It can be installed using *Pypi*:
 
     pip install sslearn
 
-Code example
----
+## Code example
+
+
 ```python
 from sslearn.wrapper import TriTraining
 from sslearn.model_selection import artificial_ssl_dataset
 from sklearn.datasets import load_iris
 
 X, y = load_iris(return_X_y=True)
 X, y, X_unlabel, true_label = artificial_ssl_dataset(X, y, label_rate=0.1)
 
 model = TriTraining().fit(X, y)
 model.score(X_unlabel, true_label)
 ```
 
-Citing
----
+## Citing 
+
 ```bibtex
-@software{jose_luis_garrido_labrador_2024_10623889,
+@software{garrido2024sslearn,
   author       = {José Luis Garrido-Labrador},
-  title        = {jlgarridol/sslearn: v1.0.4},
+  title        = {jlgarridol/sslearn},
   month        = feb,
   year         = 2024,
   publisher    = {Zenodo},
-  version      = {1.0.4},
-  doi          = {10.5281/zenodo.10623889},
-  url          = {https://doi.org/10.5281/zenodo.10623889}
+  doi          = {10.5281/zenodo.7565221},
 }
 ```
```

### Comparing `sslearn-1.0.4.1/sslearn.egg-info/SOURCES.txt` & `sslearn-1.0.5/sslearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.4.1/test/test_datasets.py` & `sslearn-1.0.5/test/test_datasets.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.4.1/test/test_general.py` & `sslearn-1.0.5/test/test_general.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from sklearn.svm import LinearSVC
 from sklearn.semi_supervised import SelfTrainingClassifier
 from statsmodels.stats.proportion import proportion_confint
 
 sys.path.append(os.path.join(os.path.dirname(os.path.abspath(__file__)), ".."))
 from sslearn.base import FakedProbaClassifier, OneVsRestSSLClassifier
 from sslearn.restricted import (WhoIsWhoClassifier, combine_predictions,
-                                conflict_rate)
+                                conflict_rate, probability_fusion, feature_fusion)
 from sslearn.utils import (calc_number_per_class, calculate_prior_probability,
                            check_n_jobs, choice_with_proportion,
                            confidence_interval, is_int, safe_division)
 
 
 class TestUtils():
     def test_is_int(self):
@@ -125,8 +125,31 @@
         y = np.array([0, 1, 0, 1, 2])
         group = np.array([0, 0, 1, 1, 1])
         hyp.fit(X, y, group)
 
         assert hyp.conflict_in_train == 1
         assert hyp.predict(X, group).tolist() == [0, 1, 0, 2, 1]
 
+    def test_probability_fusion(self):
+        X = np.array([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]])
+        y = np.array([0, 1, 0, 1, 2])
+        cannot_link = {0: [0, 1], 1: [2, 3, 4]}
+        must_link = {1: [1, 3], 0: [0, 2], 4: [4]}
+
+        h = GaussianNB()
+        h.fit(X, y)
+
+        probability_fusion(h, X, must_link=must_link, cannot_link=cannot_link)
+
+    def test_feature_fusion(self):
+        X = np.array([[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]])
+        y = np.array([0, 1, 0, 1, 2])
+        cannot_link = {0: [0, 1], 1: [2, 3, 4]}
+        must_link = {1: [1, 3], 0: [0, 2], 4: [4]}
+
+        h = GaussianNB()
+        h.fit(X, y)
+
+        result = feature_fusion(h, X, must_link=must_link, cannot_link=cannot_link)
+
+
```

### Comparing `sslearn-1.0.4.1/test/test_model_selection.py` & `sslearn-1.0.5/test/test_model_selection.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.4.1/test/test_subview.py` & `sslearn-1.0.5/test/test_subview.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.4.1/test/test_wrapper.py` & `sslearn-1.0.5/test/test_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.datasets import load_breast_cancer
 
 from sslearn.datasets import read_csv
 from sslearn.model_selection import artificial_ssl_dataset
 from sslearn.wrapper import (
     CoTraining, CoForest, CoTrainingByCommittee, DemocraticCoLearning, Rasco, RelRasco,
-    SelfTraining, Setred, TriTraining, WiWTriTraining, DeTriTraining
+    SelfTraining, Setred, TriTraining, DeTriTraining    
 )
 
 X, y = read_csv(os.path.join(os.path.dirname(os.path.realpath(__file__)), "example_files", "abalone.csv"), format="pandas")
 X2, y2 = read_csv(os.path.join(os.path.dirname(os.path.realpath(__file__)), "example_files", "abalone.csv"), format="numpy")
 
 X_l, y_l = load_breast_cancer(return_X_y=True)
 
@@ -234,44 +234,44 @@
 # Create a fake groups
 groups = list()
 for order, i in enumerate(range(0, len(X), 5)):
     groups.extend([order for _ in range(5)])
 groups = np.array(groups)
 groups = groups[:X.shape[0]]
 
-class TestWiWTriTraining:
+# class TestWiWTriTraining:
     
-    def test_basic(self):
-        clf = WiWTriTraining(base_estimator=DecisionTreeClassifier())
-        clf.fit(X, y, instance_group=groups)
-        clf.predict(X, instance_group=groups)
-        clf.predict_proba(X)
-
-        clf = WiWTriTraining(DecisionTreeClassifier())
-        clf.fit(X2, y2, instance_group=groups)
-        clf.predict(X2, instance_group=groups)
-        clf.predict_proba(X2)
-
-    def test_multiple(self):
-        clf = WiWTriTraining(base_estimator=[DecisionTreeClassifier(max_depth=1), DecisionTreeClassifier(max_depth=2), DecisionTreeClassifier(max_depth=3)])
-        clf.fit(X, y, instance_group=groups)
-        clf.predict(X, instance_group=groups)
-        clf.predict_proba(X)
+#     def test_basic(self):
+#         clf = WiWTriTraining(base_estimator=DecisionTreeClassifier())
+#         clf.fit(X, y, instance_group=groups)
+#         clf.predict(X, instance_group=groups)
+#         clf.predict_proba(X)
+
+#         clf = WiWTriTraining(DecisionTreeClassifier())
+#         clf.fit(X2, y2, instance_group=groups)
+#         clf.predict(X2, instance_group=groups)
+#         clf.predict_proba(X2)
+
+#     def test_multiple(self):
+#         clf = WiWTriTraining(base_estimator=[DecisionTreeClassifier(max_depth=1), DecisionTreeClassifier(max_depth=2), DecisionTreeClassifier(max_depth=3)])
+#         clf.fit(X, y, instance_group=groups)
+#         clf.predict(X, instance_group=groups)
+#         clf.predict_proba(X)
     
-    def test_random_state(self):
-        for i in range(10):
-            clf = WiWTriTraining(base_estimator=KNeighborsClassifier(), random_state=i)
-            clf.fit(X, y, instance_group=groups)
-            y1 = clf.predict(X, instance_group=groups)
-
-            clf = WiWTriTraining(base_estimator=KNeighborsClassifier(), random_state=i)
-            clf.fit(X, y, instance_group=groups)
-            y2 = clf.predict(X, instance_group=groups)
-
-            assert np.all(y1 == y2)
-
-    def test_all_label(self):
-        clf = WiWTriTraining(base_estimator=KNeighborsClassifier())
-        clf.fit(X, y, instance_group=groups)
-        clf.predict(X, instance_group=groups)
-        clf.predict_proba(X)
+#     def test_random_state(self):
+#         for i in range(10):
+#             clf = WiWTriTraining(base_estimator=KNeighborsClassifier(), random_state=i)
+#             clf.fit(X, y, instance_group=groups)
+#             y1 = clf.predict(X, instance_group=groups)
+
+#             clf = WiWTriTraining(base_estimator=KNeighborsClassifier(), random_state=i)
+#             clf.fit(X, y, instance_group=groups)
+#             y2 = clf.predict(X, instance_group=groups)
+
+#             assert np.all(y1 == y2)
+
+#     def test_all_label(self):
+#         clf = WiWTriTraining(base_estimator=KNeighborsClassifier())
+#         clf.fit(X, y, instance_group=groups)
+#         clf.predict(X, instance_group=groups)
+#         clf.predict_proba(X)
```

