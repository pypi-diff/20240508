# Comparing `tmp/sklearn_viz-0.4.9.tar.gz` & `tmp/sklearn_viz-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_viz-0.4.9.tar", max compression
+gzip compressed data, was "sklearn_viz-0.5.0.tar", max compression
```

## Comparing `sklearn_viz-0.4.9.tar` & `sklearn_viz-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1069 2024-05-05 10:04:24.273292 sklearn_viz-0.4.9/LICENSE
--rw-r--r--   0        0        0      354 2024-05-05 10:04:24.273292 sklearn_viz-0.4.9/README.md
--rw-r--r--   0        0        0        0 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/components/__init__.py
--rw-r--r--   0        0        0     4385 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/components/estimators.py
--rw-r--r--   0        0        0      811 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/components/kfold.py
--rw-r--r--   0        0        0      329 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/__init__.py
--rw-r--r--   0        0        0     8306 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/importance.py
--rw-r--r--   0        0        0     4633 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/outlier_detection.py
--rw-r--r--   0        0        0     2403 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/parallel_coordinates.py
--rw-r--r--   0        0        0    16590 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/principal_components.py
--rw-r--r--   0        0        0      643 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/features/scatter_matrix.py
--rw-r--r--   0        0        0      129 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/__init__.py
--rw-r--r--   0        0        0     6079 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/learning_curve.py
--rw-r--r--   0        0        0     1572 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/metrics.py
--rw-r--r--   0        0        0    21547 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/model_selection.py
--rw-r--r--   0        0        0     2497 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/models.py
--rw-r--r--   0        0        0      508 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/scorers.py
--rw-r--r--   0        0        0       21 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/residuals/__init__.py
--rw-r--r--   0        0        0     2058 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/residuals/error.py
--rw-r--r--   0        0        0       28 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/utils/__init__.py
--rw-r--r--   0        0        0     3111 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/elphick/sklearn_viz/utils/timer.py
--rw-r--r--   0        0        0      740 2024-05-05 10:04:24.277292 sklearn_viz-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-08 12:37:45.071231 sklearn_viz-0.5.0/LICENSE
+-rw-r--r--   0        0        0      354 2024-05-08 12:37:45.071231 sklearn_viz-0.5.0/README.md
+-rw-r--r--   0        0        0      165 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/components/__init__.py
+-rw-r--r--   0        0        0     4385 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/components/estimators.py
+-rw-r--r--   0        0        0      811 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/components/kfold.py
+-rw-r--r--   0        0        0      329 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/__init__.py
+-rw-r--r--   0        0        0     8306 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/importance.py
+-rw-r--r--   0        0        0     4633 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/outlier_detection.py
+-rw-r--r--   0        0        0     2403 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/parallel_coordinates.py
+-rw-r--r--   0        0        0    16590 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/principal_components.py
+-rw-r--r--   0        0        0      643 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/features/scatter_matrix.py
+-rw-r--r--   0        0        0      129 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/__init__.py
+-rw-r--r--   0        0        0     6079 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/learning_curve.py
+-rw-r--r--   0        0        0     1572 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/metrics.py
+-rw-r--r--   0        0        0    21547 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/model_selection.py
+-rw-r--r--   0        0        0     2497 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/models.py
+-rw-r--r--   0        0        0      508 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/scorers.py
+-rw-r--r--   0        0        0       21 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/residuals/__init__.py
+-rw-r--r--   0        0        0     2058 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/residuals/error.py
+-rw-r--r--   0        0        0       28 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/utils/__init__.py
+-rw-r--r--   0        0        0      544 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/utils/file.py
+-rw-r--r--   0        0        0     3033 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/utils/plotly.py
+-rw-r--r--   0        0        0     3111 2024-05-08 12:37:45.075231 sklearn_viz-0.5.0/elphick/sklearn_viz/utils/timer.py
+-rw-r--r--   0        0        0      978 2024-05-08 12:37:45.079231 sklearn_viz-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.5.0/PKG-INFO
```

### Comparing `sklearn_viz-0.4.9/LICENSE` & `sklearn_viz-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/components/estimators.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/components/estimators.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/components/kfold.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/components/kfold.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/features/importance.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/features/importance.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/features/outlier_detection.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/features/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/features/parallel_coordinates.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/features/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/features/principal_components.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/features/principal_components.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/features/scatter_matrix.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/features/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/learning_curve.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/learning_curve.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/metrics.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/metrics.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/model_selection.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/model_selection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/model_selection/models.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/model_selection/models.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/residuals/error.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/residuals/error.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/elphick/sklearn_viz/utils/timer.py` & `sklearn_viz-0.5.0/elphick/sklearn_viz/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.4.9/pyproject.toml` & `sklearn_viz-0.5.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 [tool.poetry]
 name = "sklearn-viz"
-version = "0.4.9"
+version = "0.5.0"
 description = ""
 authors = ["Greg <11791585+elphick@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "elphick/sklearn_viz" }]
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
+[tool.poetry.scripts]
+bump_version = "scripts.bump_version:main"
+
+[tool.towncrier]
+package = "elphick.sklearn_viz"
+package_dir = "elphick/sklearn_viz"
+filename = "HISTORY.rst"
+directory = "towncrier/newsfragments"
+
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 scikit-learn = ">=1.2.0"
 pandas = ">=1.3.0"
 matplotlib = "^3.7.2"
 plotly = "^5.15.0"
 statsmodels = "^0.14.0"
@@ -22,11 +31,12 @@
 pytest = "^7.1.3"
 sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-gallery = "^0.11.1"
 sphinx-autodoc-typehints = "^1.18.3"
 myst-parser = "^0.18.0"
 kaleido = "0.2.1"  # For plotly thumbnails
+towncrier = "^23.11.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sklearn_viz-0.4.9/PKG-INFO` & `sklearn_viz-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-viz
-Version: 0.4.9
+Version: 0.5.0
 Summary: 
 Author: Greg
 Author-email: 11791585+elphick@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

