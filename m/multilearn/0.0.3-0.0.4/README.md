# Comparing `tmp/multilearn-0.0.3.tar.gz` & `tmp/multilearn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multilearn-0.0.3.tar", last modified: Mon Apr 22 19:52:20 2024, max compression
+gzip compressed data, was "multilearn-0.0.4.tar", last modified: Tue May  7 01:39:37 2024, max compression
```

## Comparing `multilearn-0.0.3.tar` & `multilearn-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:52:20.469278 multilearn-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-22 19:52:16.000000 multilearn-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-22 19:52:20.469278 multilearn-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-22 19:52:16.000000 multilearn-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:52:20.469278 multilearn-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-22 19:52:16.000000 multilearn-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:52:20.445277 multilearn-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:52:20.449277 multilearn-0.0.3/src/multilearn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:52:16.000000 multilearn-0.0.3/src/multilearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:52:20.461278 multilearn-0.0.3/src/multilearn/data/
--rw-r--r--   0 runner    (1001) docker     (127)   844293 2024-04-22 19:52:16.000000 multilearn-0.0.3/src/multilearn/data/asr.csv
--rw-r--r--   0 runner    (1001) docker     (127)  7966155 2024-04-22 19:52:16.000000 multilearn-0.0.3/src/multilearn/data/opband.csv
--rw-r--r--   0 runner    (1001) docker     (127)  7788414 2024-04-22 19:52:16.000000 multilearn-0.0.3/src/multilearn/data/stability.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-22 19:52:16.000000 multilearn-0.0.3/src/multilearn/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-22 19:52:16.000000 multilearn-0.0.3/src/multilearn/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-22 19:52:16.000000 multilearn-0.0.3/src/multilearn/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-22 19:52:16.000000 multilearn-0.0.3/src/multilearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:52:20.469278 multilearn-0.0.3/src/multilearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-22 19:52:20.000000 multilearn-0.0.3/src/multilearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 19:52:20.000000 multilearn-0.0.3/src/multilearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:52:20.000000 multilearn-0.0.3/src/multilearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 19:52:20.000000 multilearn-0.0.3/src/multilearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 19:52:20.000000 multilearn-0.0.3/src/multilearn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:52:20.469278 multilearn-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-22 19:52:16.000000 multilearn-0.0.3/tests/test_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:39:37.584017 multilearn-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-07 01:39:34.000000 multilearn-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-07 01:39:37.580017 multilearn-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-07 01:39:34.000000 multilearn-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:39:37.584017 multilearn-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-07 01:39:34.000000 multilearn-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:39:37.556017 multilearn-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:39:37.556017 multilearn-0.0.4/src/multilearn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:39:34.000000 multilearn-0.0.4/src/multilearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:39:37.572017 multilearn-0.0.4/src/multilearn/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   844293 2024-05-07 01:39:34.000000 multilearn-0.0.4/src/multilearn/data/asr.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  7966155 2024-05-07 01:39:34.000000 multilearn-0.0.4/src/multilearn/data/opband.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  7788414 2024-05-07 01:39:34.000000 multilearn-0.0.4/src/multilearn/data/stability.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-07 01:39:34.000000 multilearn-0.0.4/src/multilearn/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-07 01:39:34.000000 multilearn-0.0.4/src/multilearn/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-05-07 01:39:34.000000 multilearn-0.0.4/src/multilearn/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-05-07 01:39:34.000000 multilearn-0.0.4/src/multilearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:39:37.580017 multilearn-0.0.4/src/multilearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-07 01:39:37.000000 multilearn-0.0.4/src/multilearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 01:39:37.000000 multilearn-0.0.4/src/multilearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:39:37.000000 multilearn-0.0.4/src/multilearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 01:39:37.000000 multilearn-0.0.4/src/multilearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 01:39:37.000000 multilearn-0.0.4/src/multilearn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:39:37.580017 multilearn-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-07 01:39:34.000000 multilearn-0.0.4/tests/test_fit.py
```

### Comparing `multilearn-0.0.3/LICENSE` & `multilearn-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multilearn-0.0.3/PKG-INFO` & `multilearn-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilearn
-Version: 0.0.3
+Version: 0.0.4
 Summary: Multi-task learning with Pytorch.
 Home-page: https://github.com/leschultz/multilearn
 Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_nltzniz2_/tmpllulpxs9_TarContainer/0/2", line 43, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multilearn Version: 0.0.3 Summary: Multi-task
+Metadata-Version: 2.1 Name: multilearn Version: 0.0.4 Summary: Multi-task
 learning with Pytorch. Home-page: https://github.com/leschultz/multilearn
 Author: Lane E. Schultz Author-email: laneenriqueschultz@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 torch Requires-Dist: scikit-learn Requires-Dist: lightning Requires-Dist:
 pandas Requires-Dist: matplotlib Requires-Dist: dill Requires-Dist: pytest #
```

### Comparing `multilearn-0.0.3/README.md` & `multilearn-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `multilearn-0.0.3/setup.py` & `multilearn-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 # Package information
 name = 'multilearn'
-version = '0.0.3'  # Need to increment every time to push to PyPI
+version = '0.0.4'  # Need to increment every time to push to PyPI
 description = 'Multi-task learning with Pytorch.'
 url = 'https://github.com/leschultz/multilearn'
 author = 'Lane E. Schultz'
 author_email = 'laneenriqueschultz@gmail.com'
 python_requires = '>=3.10'
 classifiers = ['Programming Language :: Python :: 3',
                'License :: OSI Approved :: MIT License',
```

### Comparing `multilearn-0.0.3/src/multilearn/data/asr.csv` & `multilearn-0.0.4/src/multilearn/data/asr.csv`

 * *Files identical despite different names*

### Comparing `multilearn-0.0.3/src/multilearn/data/opband.csv` & `multilearn-0.0.4/src/multilearn/data/opband.csv`

 * *Files identical despite different names*

### Comparing `multilearn-0.0.3/src/multilearn/data/stability.csv` & `multilearn-0.0.4/src/multilearn/data/stability.csv`

 * *Files identical despite different names*

### Comparing `multilearn-0.0.3/src/multilearn/datasets.py` & `multilearn-0.0.4/src/multilearn/datasets.py`

 * *Files identical despite different names*

### Comparing `multilearn-0.0.3/src/multilearn/models.py` & `multilearn-0.0.4/src/multilearn/models.py`

 * *Files identical despite different names*

### Comparing `multilearn-0.0.3/src/multilearn/plots.py` & `multilearn-0.0.4/src/multilearn/plots.py`

 * *Files identical despite different names*

### Comparing `multilearn-0.0.3/src/multilearn/utils.py` & `multilearn-0.0.4/src/multilearn/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,19 @@
                 dill.dump(
                           v,
                           open(os.path.join(new_dir, 'loss.pkl'), 'wb'),
                           )
 
             elif ('X_' in k) or ('y_' in k):
 
-                if 'X_' in k:
-                    v = v.cpu().detach()
+                v = v.cpu()
+                if isinstance(v, torch.Tensor):
+                    v = v.numpy()
+                else:
+                    v = v.detach()
 
                 np.savetxt(os.path.join(
                                         new_dir,
                                         f'{k}.csv',
                                         ), v, delimiter=',')
```

### Comparing `multilearn-0.0.3/src/multilearn.egg-info/PKG-INFO` & `multilearn-0.0.4/src/multilearn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilearn
-Version: 0.0.3
+Version: 0.0.4
 Summary: Multi-task learning with Pytorch.
 Home-page: https://github.com/leschultz/multilearn
 Author: Lane E. Schultz
 Author-email: laneenriqueschultz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_nltzniz2_/tmpllulpxs9_TarContainer/0/18", line 43, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multilearn Version: 0.0.3 Summary: Multi-task
+Metadata-Version: 2.1 Name: multilearn Version: 0.0.4 Summary: Multi-task
 learning with Pytorch. Home-page: https://github.com/leschultz/multilearn
 Author: Lane E. Schultz Author-email: laneenriqueschultz@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 torch Requires-Dist: scikit-learn Requires-Dist: lightning Requires-Dist:
 pandas Requires-Dist: matplotlib Requires-Dist: dill Requires-Dist: pytest #
```

### Comparing `multilearn-0.0.3/tests/test_fit.py` & `multilearn-0.0.4/tests/test_fit.py`

 * *Files identical despite different names*

