# Comparing `tmp/ood_detectors-0.0.7.tar.gz` & `tmp/ood_detectors-0.0.8.tar.gz`

## Comparing `ood_detectors-0.0.7.tar` & `ood_detectors-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/docki.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/requirements.txt
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/requirements_dev.txt
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/__about__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/__init__.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/ema.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/eval_utils.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/likelihood.py
--rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/losses.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/models.py
--rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/ood_utils.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/ops_utils.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/plot_utils.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/residual.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/sde.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/src/ood_detectors/train.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/tests/init_test.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/LICENSE
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/README.md
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 ood_detectors-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/docki.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/requirements_dev.txt
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/__about__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/__init__.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/ema.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/eval_utils.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/likelihood.py
+-rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/losses.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/models.py
+-rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/ood_utils.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/ops_utils.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/plot_utils.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/residual.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/sde.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/train.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/tests/init_test.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/README.md
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/PKG-INFO
```

### Comparing `ood_detectors-0.0.7/docki.yaml` & `ood_detectors-0.0.8/docki.yaml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/.github/workflows/publish.yml` & `ood_detectors-0.0.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/src/ood_detectors/ema.py` & `ood_detectors-0.0.8/src/ood_detectors/ema.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/src/ood_detectors/eval_utils.py` & `ood_detectors-0.0.8/src/ood_detectors/eval_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/src/ood_detectors/likelihood.py` & `ood_detectors-0.0.8/src/ood_detectors/likelihood.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/src/ood_detectors/losses.py` & `ood_detectors-0.0.8/src/ood_detectors/losses.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/src/ood_detectors/models.py` & `ood_detectors-0.0.8/src/ood_detectors/models.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/src/ood_detectors/ood_utils.py` & `ood_detectors-0.0.8/src/ood_detectors/ood_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/src/ood_detectors/ops_utils.py` & `ood_detectors-0.0.8/src/ood_detectors/ops_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/src/ood_detectors/plot_utils.py` & `ood_detectors-0.0.8/src/ood_detectors/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/src/ood_detectors/residual.py` & `ood_detectors-0.0.8/src/ood_detectors/residual.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/src/ood_detectors/sde.py` & `ood_detectors-0.0.8/src/ood_detectors/sde.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/src/ood_detectors/train.py` & `ood_detectors-0.0.8/src/ood_detectors/train.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/LICENSE` & `ood_detectors-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/README.md` & `ood_detectors-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,20 @@
     warmup=warmup,
     grad_clip=grad_clip,
     continuous=continuous,
     reduce_mean=reduce_mean,
     likelihood_weighting=likelihood_weighting,
     )
 
-train_loss = ood_detector.fit(train_data, update_fn, batch_size)
+train_loss = ood_detector.fit(
+    train_data,  
+    n_epochs=n_epochs,
+    batch_size=batch_size,
+    update_fn=update_fn,
+    )
 ```
 
 ## Create a custom component
 
 You can create a custom component by doing the same thing as the library does. Good luck!
```

### Comparing `ood_detectors-0.0.7/pyproject.toml` & `ood_detectors-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.7/PKG-INFO` & `ood_detectors-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ood_detectors
-Version: 0.0.7
+Version: 0.0.8
 Project-URL: Documentation, https://github.com/Arty-Facts/ood_detectors#readme
 Project-URL: Issues, https://github.com/Arty-Facts/ood_detectors/issues
 Project-URL: Source, https://github.com/Arty-Facts/ood_detectors
 Author-email: Arturas Aleksandraus <arturas@aleksandraus.se>, Yifan Ding <yifan.ding@liu.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -121,15 +121,20 @@
     warmup=warmup,
     grad_clip=grad_clip,
     continuous=continuous,
     reduce_mean=reduce_mean,
     likelihood_weighting=likelihood_weighting,
     )
 
-train_loss = ood_detector.fit(train_data, update_fn, batch_size)
+train_loss = ood_detector.fit(
+    train_data,  
+    n_epochs=n_epochs,
+    batch_size=batch_size,
+    update_fn=update_fn,
+    )
 ```
 
 ## Create a custom component
 
 You can create a custom component by doing the same thing as the library does. Good luck!
```

