# Comparing `tmp/panelsplit-0.2.0.tar.gz` & `tmp/panelsplit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panelsplit-0.2.0.tar", last modified: Tue Mar 26 16:59:40 2024, max compression
+gzip compressed data, was "panelsplit-0.3.0.tar", last modified: Wed May  8 20:48:20 2024, max compression
```

## Comparing `panelsplit-0.2.0.tar` & `panelsplit-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-03-26 16:59:40.206817 panelsplit-0.2.0/
--rw-r--r--   0 ericfrey   (501) staff       (20)      412 2024-03-26 16:58:07.000000 panelsplit-0.2.0/CITATION.cff
--rw-r--r--   0 ericfrey   (501) staff       (20)     1081 2024-03-26 16:58:07.000000 panelsplit-0.2.0/LICENSE
--rw-r--r--   0 ericfrey   (501) staff       (20)     8094 2024-03-26 16:59:40.206119 panelsplit-0.2.0/PKG-INFO
--rw-r--r--   0 ericfrey   (501) staff       (20)     7644 2024-03-26 16:58:07.000000 panelsplit-0.2.0/README.md
-drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-03-26 16:59:40.196311 panelsplit-0.2.0/examples/
--rw-r--r--   0 ericfrey   (501) staff       (20)   108532 2024-03-26 16:58:07.000000 panelsplit-0.2.0/examples/An introduction to PanelSplit.ipynb
-drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-03-26 16:59:40.199732 panelsplit-0.2.0/panelsplit/
--rw-r--r--   0 ericfrey   (501) staff       (20)       35 2024-02-19 10:30:46.000000 panelsplit-0.2.0/panelsplit/__init__.py
--rw-r--r--   0 ericfrey   (501) staff       (20)    17476 2024-03-26 16:58:07.000000 panelsplit-0.2.0/panelsplit/panelsplit.py
-drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-03-26 16:59:40.205213 panelsplit-0.2.0/panelsplit.egg-info/
--rw-r--r--   0 ericfrey   (501) staff       (20)     8094 2024-03-26 16:59:39.000000 panelsplit-0.2.0/panelsplit.egg-info/PKG-INFO
--rw-r--r--   0 ericfrey   (501) staff       (20)      301 2024-03-26 16:59:40.000000 panelsplit-0.2.0/panelsplit.egg-info/SOURCES.txt
--rw-r--r--   0 ericfrey   (501) staff       (20)        1 2024-03-26 16:59:39.000000 panelsplit-0.2.0/panelsplit.egg-info/dependency_links.txt
--rw-r--r--   0 ericfrey   (501) staff       (20)       49 2024-03-26 16:59:39.000000 panelsplit-0.2.0/panelsplit.egg-info/requires.txt
--rw-r--r--   0 ericfrey   (501) staff       (20)       11 2024-03-26 16:59:39.000000 panelsplit-0.2.0/panelsplit.egg-info/top_level.txt
--rw-r--r--   0 ericfrey   (501) staff       (20)       38 2024-03-26 16:59:40.207062 panelsplit-0.2.0/setup.cfg
--rw-r--r--   0 ericfrey   (501) staff       (20)     1268 2024-03-26 16:58:07.000000 panelsplit-0.2.0/setup.py
+drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:48:20.273117 panelsplit-0.3.0/
+-rw-r--r--   0 ericfrey   (501) staff       (20)      411 2024-05-08 20:39:25.000000 panelsplit-0.3.0/CITATION.cff
+-rw-r--r--   0 ericfrey   (501) staff       (20)     1081 2024-03-26 16:58:07.000000 panelsplit-0.3.0/LICENSE
+-rw-r--r--   0 ericfrey   (501) staff       (20)     8094 2024-05-08 20:48:20.272018 panelsplit-0.3.0/PKG-INFO
+-rw-r--r--   0 ericfrey   (501) staff       (20)     7644 2024-03-26 16:58:07.000000 panelsplit-0.3.0/README.md
+drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:48:20.261206 panelsplit-0.3.0/examples/
+-rw-r--r--   0 ericfrey   (501) staff       (20)   108532 2024-03-26 16:58:07.000000 panelsplit-0.3.0/examples/An introduction to PanelSplit.ipynb
+drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:48:20.264761 panelsplit-0.3.0/panelsplit/
+-rw-r--r--   0 ericfrey   (501) staff       (20)       35 2024-02-19 10:30:46.000000 panelsplit-0.3.0/panelsplit/__init__.py
+-rw-r--r--   0 ericfrey   (501) staff       (20)    18101 2024-05-08 20:00:30.000000 panelsplit-0.3.0/panelsplit/panelsplit.py
+drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:48:20.268916 panelsplit-0.3.0/panelsplit.egg-info/
+-rw-r--r--   0 ericfrey   (501) staff       (20)     8094 2024-05-08 20:48:19.000000 panelsplit-0.3.0/panelsplit.egg-info/PKG-INFO
+-rw-r--r--   0 ericfrey   (501) staff       (20)      344 2024-05-08 20:48:20.000000 panelsplit-0.3.0/panelsplit.egg-info/SOURCES.txt
+-rw-r--r--   0 ericfrey   (501) staff       (20)        1 2024-05-08 20:48:19.000000 panelsplit-0.3.0/panelsplit.egg-info/dependency_links.txt
+-rw-r--r--   0 ericfrey   (501) staff       (20)       49 2024-05-08 20:48:19.000000 panelsplit-0.3.0/panelsplit.egg-info/requires.txt
+-rw-r--r--   0 ericfrey   (501) staff       (20)       11 2024-05-08 20:48:19.000000 panelsplit-0.3.0/panelsplit.egg-info/top_level.txt
+-rw-r--r--   0 ericfrey   (501) staff       (20)       38 2024-05-08 20:48:20.273360 panelsplit-0.3.0/setup.cfg
+-rw-r--r--   0 ericfrey   (501) staff       (20)     1219 2024-05-08 20:35:39.000000 panelsplit-0.3.0/setup.py
+drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:48:20.269904 panelsplit-0.3.0/tests/
+-rw-r--r--   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:04:00.000000 panelsplit-0.3.0/tests/__init__.py
+-rw-r--r--   0 ericfrey   (501) staff       (20)     1649 2024-05-08 20:30:49.000000 panelsplit-0.3.0/tests/test_PanelSplit.py
```

### Comparing `panelsplit-0.2.0/LICENSE` & `panelsplit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panelsplit-0.2.0/PKG-INFO` & `panelsplit-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panelsplit
-Version: 0.2.0
+Version: 0.3.0
 Summary: A tool for panel data analysis.
 Home-page: https://github.com/4Freye/panelsplit
 Author: Eric Frey, Ben Seimon
 Author-email: eric.frey@bse.eu, benjamin.seimon@bse.eu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panelsplit-0.2.0/README.md` & `panelsplit-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `panelsplit-0.2.0/examples/An introduction to PanelSplit.ipynb` & `panelsplit-0.3.0/examples/An introduction to PanelSplit.ipynb`

 * *Files identical despite different names*

### Comparing `panelsplit-0.2.0/panelsplit/panelsplit.py` & `panelsplit-0.3.0/panelsplit/panelsplit.py`

 * *Files 5% similar despite different names*

```diff
@@ -220,36 +220,45 @@
         - X: pandas DataFrame. The input features for the predictor.
         - labels: Optional pandas DataFrame. Labels to identify the predictions, if provided will be returned along with predictions.
         - prediction_method: Optional str (default='predict'). The prediction method to use. It can be 'predict', 'predict_proba', or 'predict_log_proba'.
         - n_jobs: Optional int (default=1). The number of jobs to run in parallel.
         - return_train_preds: Optional bool (default=False). If True, return predictions for the training set as well.
 
         Returns:
-        pd.DataFrame: Concatenated DataFrame containing predictions made by the model during cross-validation. It includes the original labels joined with the predicted values.
+        - test_preds: NumPy array containing test predictions made by the model during cross-validation. If return_train_preds is True, train predictions will also be returned.
+        - train_preds: NumPy array containing train predictions made by the model during cross-validation.
         """
+
+        def prediction_order_to_original_order(indices): 
+            """
+            To convert the concatenated predictions back to original order provided
+            """
+            indices = np.concatenate([np.where(indices_)[0] for indices_ in indices])
+            return np.argsort(indices)
+
         def predict_split(model, test_indices):
             X_test = X.loc[test_indices]
             return self._predict_split(model, X_test, prediction_method)
 
-        predictions = Parallel(n_jobs=n_jobs)(
+        test_indices = prediction_order_to_original_order([split[1] for split in self.split()])
+
+        test_preds = Parallel(n_jobs=n_jobs)(
             delayed(predict_split)(fitted_estimators[i], test_indices)
             for i, (_, test_indices) in enumerate(self.split())
         )
 
         if return_train_preds:
             train_preds = Parallel(n_jobs=n_jobs)(
                 delayed(predict_split)(fitted_estimators[i], train_indices)
                 for i, (train_indices, _) in enumerate(self.split())
             )
-            return np.concatenate(predictions, axis = 0), np.concatenate(train_preds, axis = 0)
-        
+            train_indices = prediction_order_to_original_order([split[0] for split in self.split()])
+            return np.concatenate(test_preds, axis = 0)[test_indices], np.concatenate(train_preds, axis = 0)[train_indices]
         else:
-            return np.concatenate(predictions, axis = 0)
-
-        
+            return np.concatenate(test_preds, axis=0)[test_indices]
 
     def cross_val_fit_predict(self, estimator, X, y, prediction_method='predict', sample_weight=None, n_jobs=1, return_train_preds=False):
         """
         Fit the estimator using cross-validation and then make predictions.
 
         Parameters:
         - estimator: The machine learning model to be fitted.
```

### Comparing `panelsplit-0.2.0/panelsplit.egg-info/PKG-INFO` & `panelsplit-0.3.0/panelsplit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panelsplit
-Version: 0.2.0
+Version: 0.3.0
 Summary: A tool for panel data analysis.
 Home-page: https://github.com/4Freye/panelsplit
 Author: Eric Frey, Ben Seimon
 Author-email: eric.frey@bse.eu, benjamin.seimon@bse.eu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panelsplit-0.2.0/setup.py` & `panelsplit-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 # Read the contents of the README file
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
-    name='panelsplit',  # Replace with the desired name of your package
-    version='0.2.0',
+    name='panelsplit',
+    version='0.3.0',
     packages=find_packages(include=['panelsplit', 'panelsplit.*']),  # Include only packages within the "panelsplit" folder
 
     # Metadata
     author='Eric Frey, Ben Seimon',
     author_email='eric.frey@bse.eu, benjamin.seimon@bse.eu',
     description='A tool for panel data analysis.',
     url='https://github.com/4Freye/panelsplit',  # URL to your GitHub repository
```

