# Comparing `tmp/jenn-1.0.3.tar.gz` & `tmp/jenn-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenn-1.0.3.tar", last modified: Wed Feb 28 19:19:29 2024, max compression
+gzip compressed data, was "jenn-1.0.4.tar", last modified: Wed May  8 18:55:46 2024, max compression
```

## Comparing `jenn-1.0.3.tar` & `jenn-1.0.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:19:29.579396 jenn-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-28 19:17:43.000000 jenn-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-02-28 19:19:29.579396 jenn-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-02-28 19:17:43.000000 jenn-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-02-28 19:17:43.000000 jenn-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 19:19:29.579396 jenn-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:19:29.571396 jenn-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:19:29.575396 jenn-1.0.3/src/jenn/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:19:29.575396 jenn-1.0.3/src/jenn/core/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/core/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/core/cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12998 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/core/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12383 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10150 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/core/propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/core/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:19:29.575396 jenn-1.0.3/src/jenn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-02-28 19:17:43.000000 jenn-1.0.3/src/jenn/utils/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:19:29.579396 jenn-1.0.3/src/jenn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-02-28 19:19:29.000000 jenn-1.0.3/src/jenn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-28 19:19:29.000000 jenn-1.0.3/src/jenn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 19:19:29.000000 jenn-1.0.3/src/jenn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-28 19:19:29.000000 jenn-1.0.3/src/jenn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-28 19:19:29.000000 jenn-1.0.3/src/jenn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 19:19:29.575396 jenn-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-02-28 19:17:43.000000 jenn-1.0.3/tests/test_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-28 19:17:43.000000 jenn-1.0.3/tests/test_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-02-28 19:17:43.000000 jenn-1.0.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-02-28 19:17:43.000000 jenn-1.0.3/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-28 19:17:43.000000 jenn-1.0.3/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-02-28 19:17:43.000000 jenn-1.0.3/tests/test_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.409620 jenn-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-08 18:53:37.000000 jenn-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-08 18:55:46.409620 jenn-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-08 18:53:37.000000 jenn-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-08 18:53:37.000000 jenn-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:55:46.409620 jenn-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.401620 jenn-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.405620 jenn-1.0.4/src/jenn/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.405620 jenn-1.0.4/src/jenn/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13672 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.409620 jenn-1.0.4/src/jenn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18429 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/utils/rbf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.409620 jenn-1.0.4/src/jenn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-08 18:55:46.000000 jenn-1.0.4/src/jenn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-08 18:55:46.000000 jenn-1.0.4/src/jenn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:55:46.000000 jenn-1.0.4/src/jenn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 18:55:46.000000 jenn-1.0.4/src/jenn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 18:55:46.000000 jenn-1.0.4/src/jenn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.409620 jenn-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_propagation.py
```

### Comparing `jenn-1.0.3/LICENSE` & `jenn-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jenn-1.0.3/PKG-INFO` & `jenn-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jenn
-Version: 1.0.3
+Version: 1.0.4
 Summary: Jacobian-Enhanced Neural Nets (JENN)
 Author-email: "Steven H. Berguin" <stevenberguin@gmail.com>
 Project-URL: Documentation, https://shb84.github.io/JENN/
 Project-URL: Homepage, https://github.com/shb84/JENN
 Project-URL: Issues, https://github.com/shb84/JENN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jenn-1.0.3/README.md` & `jenn-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jenn-1.0.3/pyproject.toml` & `jenn-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jenn"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Steven H. Berguin", email="stevenberguin@gmail.com" },
 ]
 description = "Jacobian-Enhanced Neural Nets (JENN)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -20,14 +20,17 @@
   "orjson>=3.9",
   "numpy>=1.22",
 ]
 
 [project.optional-dependencies]
 viz = ["matplotlib>=3.7"]
 
+[tool.setuptools.package-data]
+jenn = ["*.json"]
+
 [project.urls]
 Documentation = "https://shb84.github.io/JENN/"
 Homepage = "https://github.com/shb84/JENN"
 Issues = "https://github.com/shb84/JENN/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
```

### Comparing `jenn-1.0.3/src/jenn/core/activation.py` & `jenn-1.0.4/src/jenn/core/activation.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         \end{cases}
     """
 
     @classmethod
     def evaluate(
         cls,
         x: np.ndarray,
-        y: np.ndarray = None,
+        y: Union[np.ndarray, None] = None,
     ) -> np.ndarray:  # noqa: D102
         if y is None:
             y = (x > 0) * x
         else:
             y[:] = (x > 0) * x
         return y
 
@@ -200,7 +200,14 @@
         dy: Union[np.ndarray, None] = None,
         ddy: Union[np.ndarray, None] = None,
     ) -> np.ndarray:  # noqa: D102
         if ddy is None:
             return np.zeros(x.shape)
         ddy[:] = 0
         return ddy
+
+
+ACTIVATIONS = dict(
+    relu=Relu,
+    tanh=Tanh,
+    linear=Linear,
+)
```

### Comparing `jenn-1.0.3/src/jenn/core/cache.py` & `jenn-1.0.4/src/jenn/core/cache.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.3/src/jenn/core/cost.py` & `jenn-1.0.4/src/jenn/core/cost.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,141 +5,148 @@
 compute the neural net cost function used for training. 
 It is a modified version of the Least Squared Estimator (LSE), 
 augmented with a penalty function for regularization and another 
 term which accounts for Jacobian prediction error. See
 `paper`_ for details and notation. 
 """  # noqa W291
 
+from typing import Union
+
 import numpy as np
 
 from .data import Dataset
 from .parameters import Parameters
 
 
 class SquaredLoss:
     r"""Least Squares Estimator.
 
     :param Y_true: training data outputs :math:`Y \in \mathbb{R}^{n_y
         \times m}`
+    :param Y_weights: weights by which to prioritize data points (optional)
     """
 
-    def __init__(self, Y_true: np.ndarray):  # noqa: D107
+    def __init__(
+        self, Y_true: np.ndarray, Y_weights: Union[np.ndarray, float] = 1.0
+    ) -> None:
         self.Y_true = Y_true
         self.Y_error = np.zeros(Y_true.shape)  # preallocate to save resources
+        self.Y_weights = np.ones(Y_true.shape) * Y_weights
+        self.n_y, self.m = Y_true.shape
 
     def evaluate(self, Y_pred: np.ndarray) -> np.float64:
         r"""Compute least squares estimator of the states in place.
 
         :param Y_pred: predicted outputs :math:`A^{[L]} \in
             \mathbb{R}^{n_y \times m}`
-        :param indices: only evaluate specified training data indices
-            (used for minibatch)
         """
-        self.Y_error = Y_pred - self.Y_true
-        n_y = self.Y_error.shape[0]
+        self.Y_error[:, :] = Y_pred - self.Y_true
+        self.Y_error *= np.sqrt(self.Y_weights)
         cost = 0
-        for j in range(0, n_y):
+        for j in range(0, self.n_y):
             cost += np.dot(self.Y_error[j], self.Y_error[j].T)
         return np.float64(cost)
 
 
 class GradientEnhancement:
     r"""Least Squares Estimator for partials.
 
     :param J_true: training data jacobian :math:`Y^{\prime} \in
         \mathbb{R}^{n_y \times m}`
+        :param J_weights: weights by which to prioritize partials (optional)
     """
 
-    def __init__(self, J_true: np.ndarray):  # noqa: D107
+    def __init__(
+        self, J_true: np.ndarray, J_weights: Union[np.ndarray, float] = 1.0
+    ) -> None:
         self.J_true = J_true
         self.J_error = np.zeros(J_true.shape)
+        self.J_weights = np.ones(J_true.shape) * J_weights
+        self.n_y, self.n_x, self.m = J_true.shape
 
     def evaluate(self, J_pred: np.ndarray) -> np.float64:
         r"""Compute least squares estimator for the partials.
 
         :param J_pred: predicted Jacobian :math:`A^{\prime[L]} \in
             \mathbb{R}^{n_y \times n_x \times m}`
-        :param indices: only evaluate specified training data indices
-            (used for minibatch)
         """
-        dY_true = self.J_true
-        dY_error = self.J_error
-        n_y, n_x, m = dY_true.shape
+        self.J_error[:, :, :] = self.J_weights * (J_pred - self.J_true)
+        self.J_error *= np.sqrt(self.J_weights)
         cost = 0.0
-        for k in range(0, n_y):
-            for j in range(0, n_x):
-                dY_error[k, j] = J_pred[k, j] - dY_true[k, j]
-                dot_product = np.dot(dY_error[k, j], dY_error[k, j].T)
+        for k in range(0, self.n_y):
+            for j in range(0, self.n_x):
+                dot_product = np.dot(self.J_error[k, j], self.J_error[k, j].T)
                 cost += np.squeeze(dot_product)
         return np.float64(cost)
 
 
 class Regularization:
-    r"""Compute regularization penalty.
+    """Compute regularization penalty."""
 
-    :param weights: neural parameters :math:`W^{[l]} \in
+    def __init__(self, weights: list[np.ndarray], lambd: float = 0.0) -> None:
+        r"""Compute L2 norm penalty.
+
+        :param weights: neural parameters :math:`W^{[l]} \in
         \mathbb{R}^{n^{[l]} \times n^{[l-1]}}` associated with each
         layer
-    """
-
-    def __init__(self, weights: np.ndarray):  # noqa: D107
-        # Preallocate for speed
+        """
         self.weights = weights
-        self._squared_weights = [np.zeros(W.shape) for W in weights]
+        self.lambd = lambd
 
-    def evaluate(self, lambd: float) -> np.float64:
+    def evaluate(
+        self,
+    ) -> float:
         r"""Compute L2 norm penalty.
 
+        :param weights: neural parameters :math:`W^{[l]} \in
+        \mathbb{R}^{n^{[l]} \times n^{[l-1]}}` associated with each
+        layer
         :param lambd: regularization coefficient :math:`\lambda \in
             \mathbb{R}` (hyperparameter to be tuned)
         """
         penalty = 0.0
-        if lambd > 0:
-            for i, weight in enumerate(self.weights):
-                squared_weights = np.square(weight, out=self._squared_weights[i])
-                penalty += np.squeeze(np.sum(squared_weights))
-        return lambd * np.float64(penalty)
+        if self.lambd > 0.0:
+            for W in self.weights:
+                penalty += np.sum(np.square(W)).squeeze()
+            return self.lambd * penalty
+        return 0.0
 
 
 class Cost:
     r"""Neural Network cost function.
 
     :param data: Dataset object containing training data (and associated
         metadata)
     :param parameters: object containing neural net parameters (and
         associated metadata) for each layer
-    :param lambd: regularization coefficient :math:`\lambda \in
-        \mathbb{R}` (hyperparameter to be tuned)
-    :param gamma: jacobian-enhancement coefficient :math:`\gamma \in
-        \mathbb{R}` (hyperparameter to be tuned)
+    :param lambd: regularization coefficient to avoid overfitting
     """
 
     def __init__(
         self,
         data: Dataset,
         parameters: Parameters,
         lambd: float = 0.0,
-        gamma: float = 0.0,
-    ):  # noqa: D107
+    ) -> None:
         self.data = data
         self.parameters = parameters
-        self.lambd = lambd
-        self.gamma = gamma
-        self.squared_loss = SquaredLoss(data.Y)
-        self.regularization = Regularization(parameters.W)
-        if data.J is not None and gamma > 0.0:  # noqa: PLR2004
-            self.gradient_enhancement = GradientEnhancement(data.J)
-
-    def evaluate(self, Y_pred: np.ndarray, J_pred: np.ndarray = None) -> np.float64:
+        self.squared_loss = SquaredLoss(data.Y, data.Y_weights)
+        self.regularization = Regularization(parameters.W, lambd)
+        if data.J is not None:  # noqa: PLR2004
+            self.gradient_enhancement = GradientEnhancement(data.J, data.J_weights)
+
+    def evaluate(
+        self, Y_pred: np.ndarray, J_pred: Union[np.ndarray, None] = None
+    ) -> np.float64:
         r"""Evaluate cost function.
 
         :param Y_pred: predicted outputs :math:`A^{[L]} \in
             \mathbb{R}^{n_x \times m}`
         :param J_pred: predicted Jacobian :math:`A^{\prime[L]} \in
             \mathbb{R}^{n_y \times n_x \times m}`
         """
         cost = self.squared_loss.evaluate(Y_pred)
         if J_pred is not None and hasattr(self, "gradient_enhancement"):
-            cost += self.gradient_enhancement.evaluate(J_pred) * self.gamma
-        cost += self.regularization.evaluate(self.lambd)
+            cost += self.gradient_enhancement.evaluate(J_pred)
+        cost += self.regularization.evaluate()
         cost *= 0.5 / self.data.m
         return cost
```

### Comparing `jenn-1.0.3/src/jenn/core/data.py` & `jenn-1.0.4/src/jenn/core/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,18 +34,15 @@
     batches = []
     m = X.shape[1]
     if not batch_size:
         batch_size = m
     batch_size = min(batch_size, m)
 
     # Step 1: Shuffle the indices
-    if shuffle:
-        indices = list(rng.permutation(m))
-    else:
-        indices = np.arange(m)
+    indices: list[int] = list(rng.permutation(m)) if shuffle else np.arange(m).tolist()
 
     # Step 2: Partition (shuffled_X, shuffled_Y). Minus the end case.
     num_complete_minibatches = int(math.floor(m / batch_size))
     k = 0
     for _ in range(num_complete_minibatches):
         mini_batch = indices[k * batch_size : (k + 1) * batch_size]
         if mini_batch:
@@ -75,15 +72,17 @@
 
     :param array: array of shape (-1, m)
     :return: column array corresponding to std dev of each row
     """
     return np.std(array, axis=1).reshape((-1, 1))
 
 
-def _safe_divide(value: np.ndarray, eps: float = np.finfo(float).eps) -> np.ndarray:
+def _safe_divide(
+    value: np.ndarray, eps: float = float(np.finfo(float).eps)
+) -> np.ndarray:
     """Add small number to avoid dividing by zero."""
     mask = value == 0.0  # noqa: PLR2004
     value[mask] += eps
     return value
 
 
 def normalize(data: np.ndarray, mu: np.ndarray, sigma: np.ndarray) -> np.ndarray:
@@ -105,16 +104,16 @@
     :param sigma: std deviation of the data, array of shape (-1, 1)
     :return: denormalized data, array of shape (-1, m)
     """
     return sigma * data + mu
 
 
 def normalize_partials(
-    partials: np.ndarray, sigma_x: np.ndarray, sigma_y: np.ndarray
-) -> np.ndarray:
+    partials: Union[np.ndarray, None], sigma_x: np.ndarray, sigma_y: np.ndarray
+) -> Union[np.ndarray, None]:
     r"""Normalize partials.
 
     :param partials: training data partials to be normalized
         :math:`J\in\mathbb{R}^{n_y\times n_x \times m}`
     :param sigma_x: std dev of training data factors :math:`\sigma_x`,
         array of shape (-1, 1)
     :param sigma_y: std dev of training data responses :math:`\sigma_y`,
@@ -157,26 +156,47 @@
     :param J: training data Jacobians, array of shape (n_y, n_x, m)
     """
 
     X: np.ndarray
     Y: np.ndarray
     J: Union[np.ndarray, None] = None
 
+    Y_weights: Union[np.ndarray, float] = 1.0
+    J_weights: Union[np.ndarray, float] = 1.0
+
     def __post_init__(self) -> None:  # noqa: D105
         if self.X.shape[1] != self.Y.shape[1]:
             msg = "X and Y must have the same number of examples"
             raise ValueError(msg)
 
         n_y, n_x, m = self.n_y, self.n_x, self.m
 
+        self.Y_weights = self.Y_weights * np.ones((n_y, m))
+        self.J_weights = self.J_weights * np.ones((n_y, n_x, m))
+
         if self.J is not None:
             if self.J.shape != (n_y, n_x, m):
                 msg = f"J must be of shape ({n_y}, {n_x}, {m})"
                 raise ValueError(msg)
 
+    def set_weights(
+        self,
+        beta: Union[np.ndarray, float] = 1.0,
+        gamma: Union[np.ndarray, float] = 1.0,
+    ) -> None:
+        """Prioritize certain points more than others.
+
+        Rational: this can be used to reward the optimizer more in certain regions.
+
+        :param beta: multiplier(s) on Y
+        :param beta: multiplier(s) on J
+        """
+        self.Y_weights = beta * np.ones((self.n_y, self.m))
+        self.J_weights = gamma * np.ones((self.n_y, self.n_x, self.m))
+
     @property
     def m(self) -> int:
         """Return number of training examples."""
         return int(self.X.shape[1])
 
     @property
     def n_x(self) -> int:
@@ -222,18 +242,25 @@
         :param random_state: random seed (useful to make runs
             repeatable)
         :return: list of Dataset representing data broken up in batches
         """
         X = self.X
         Y = self.Y
         J = self.J
+        Y_weights = np.ones(Y.shape) * self.Y_weights
         batches = mini_batches(X, batch_size, shuffle, random_state)
-        if self.J is None:
-            return [Dataset(X[:, b], Y[:, b]) for b in batches]
-        return [Dataset(X[:, b], Y[:, b], J[:, :, b]) for b in batches]  # type: ignore[index]
+        if J is None:
+            return [
+                Dataset(X[:, b], Y[:, b], Y_weights=Y_weights[:, b]) for b in batches
+            ]
+        J_weights = np.ones(J.shape) * self.J_weights
+        return [
+            Dataset(X[:, b], Y[:, b], J[:, :, b], Y_weights[:, b], J_weights[:, :, b])
+            for b in batches
+        ]
 
     def normalize(self) -> "Dataset":
         """Return normalized Dataset."""
         X_norm = normalize(self.X, self.avg_x, self.std_x)
         Y_norm = normalize(self.Y, self.avg_y, self.std_y)
         J_norm = normalize_partials(self.J, self.std_x, self.std_y)
         return Dataset(X_norm, Y_norm, J_norm)
```

### Comparing `jenn-1.0.3/src/jenn/core/optimization.py` & `jenn-1.0.4/src/jenn/core/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,18 +86,18 @@
         self,
         beta_1: float = 0.9,
         beta_2: float = 0.99,
     ):  # noqa D107
         self.beta_1 = beta_1
         self.beta_2 = beta_2
 
-        self._v = None
-        self._s = None
+        self._v: Union[np.ndarray, None] = None
+        self._s: Union[np.ndarray, None] = None
         self._t = 0
-        self._grads = None
+        self._grads: Union[np.ndarray, None] = None
 
     def _update(
         self,
         params: np.ndarray,
         grads: np.ndarray,
         alpha: float,
     ) -> np.ndarray:
@@ -261,39 +261,40 @@
         f: Callable,
         dfdx: Callable,
         alpha: float = 0.01,
         max_iter: int = 100,
         verbose: bool = False,
         epoch: Union[int, None] = None,
         batch: Union[int, None] = None,
+        epsilon_absolute: float = 1e-12,
+        epsilon_relative: float = 1e-12,
     ) -> np.ndarray:
         r"""Minimize single objective function.
 
         :param x: parameters to be updated, array of shape (n,)
         :param f: cost function :math:`y = f(\boldsymbol{x})`
         :param alpha: learning rate :math:`\boldsymbol{x} :=
             \boldsymbol{x} + \alpha \boldsymbol{s}`
         :param max_iter: maximum number of optimizer iterations allowed
         :param verbose: whether or not to send progress output to
             standard out
         :param epoch: the epoch in which this optimization is being run
             (for printing)
         :param batch: the batch in which this optimization is being run
             (for printing)
+        :param epsilon_absolute: absolute error stopping criterion
+        :param epsilon_relative: relative error stopping criterion
         """
         # Stopping criteria (Vanderplaats, "Multidiscipline Design Optimization," ch. 3, p. 121)
         converged = False
         N1 = 0
         N1_max = 100
         N2 = 0
         N2_max = 100
 
-        epsilon_absolute = 1e-6  # absolute error criterion
-        epsilon_relative = 1e-6  # relative error criterion
-
         cost_history: list[np.ndarray] = []
         vars_history: list[np.ndarray] = []
 
         # Iterative update
         for i in range(0, max_iter):
             y = f(x)
 
@@ -328,15 +329,15 @@
                 if N1 > N1_max:
                     converged = True
                     if verbose:
                         print("Absolute stopping criterion satisfied")
 
                 # Relative convergence criterion
                 numerator = abs(cost_history[-1] - cost_history[-2])
-                denominator = max(abs(cost_history[-1]), 1e-6)
+                denominator = max(abs(float(cost_history[-1])), 1e-6)
                 dF2 = numerator / denominator
 
                 if dF2 < epsilon_relative:
                     N2 += 1
                 else:
                     N2 = 0
                 if N2 > N2_max:
@@ -401,15 +402,15 @@
     """
 
     def __init__(
         self,
         beta_1: float = 0.9,
         beta_2: float = 0.99,
         tau: float = 0.5,
-        tol: float = 1e-6,
+        tol: float = 1e-12,
         max_count: int = 1_000,
     ):  # noqa D107
         line_search = Backtracking(
             update=ADAM(beta_1, beta_2),
             tau=tau,
             tol=tol,
             max_count=max_count,
```

### Comparing `jenn-1.0.3/src/jenn/core/parameters.py` & `jenn-1.0.4/src/jenn/core/parameters.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 """Parameters.
 ==============
 
 This module defines a utility class to store and manage neural net parameters and metadata."""
 
+import json
+import os
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Iterable, List, Union
 
+import jsonpointer
+import jsonschema
 import numpy as np
 import orjson
 
+from .activation import ACTIVATIONS
+
+_here = Path(os.path.dirname(os.path.abspath(__file__)))
+SCHEMA = json.loads((_here / "schema.json").read_text())
+
 
 @dataclass
 class Parameters:
     r"""Neural network parameters.
 
     .. warning::
         The attributes of this class are not protected. It's possible
@@ -89,19 +98,17 @@
         return self.layer_sizes[-1]
 
     @property
     def L(self) -> int:
         """Return number of layers."""
         return len(self.layer_sizes)
 
-    def __post_init__(self) -> None:  # noqa D105
-        self.initialize()
-
     def initialize(self, random_state: Union[int, None] = None) -> None:
-        """Use `He initialization <https://arxiv.org/pdf/1502.01852.pdf>`_ to initialize parameters.
+        """Use `He initialization <https://arxiv.org/pdf/1502.01852.pdf>`_ to
+        initialize parameters.
 
         :param random_state: optional random seed (for repeatability)
         """
         rng = np.random.default_rng(random_state)
         self.W = []
         self.b = []
         self.a = []
@@ -134,43 +141,80 @@
             self.dW.append(dW)
             self.db.append(db)
             self.W.append(W)
             self.b.append(b)
             self.a.append(a)
             previous_layer_size = layer_size
 
-    def stack(self, per_layer: bool = False) -> Union[np.ndarray, List[np.ndarray]]:
-        """Stack W, b into a single array for each layer.
-
-        :param per_layer: whether to return answer as list of stacks (one per layer)
-        :return: parameter as either single stacked array or list of stacks (if specified)
+    def stack(self) -> np.ndarray:
+        """Stack W, b into a single array.
 
         .. code-block::
 
-            parameters.stack(per_layer=True)
-            >> [np.array([[W1], [b1]]), [W2], [b2]]), np.array([[W3], [b3]])]
-
             parameters.stack()
             >> np.array([[W1], [b1], [W2], [b2], [W3], [b3]])
 
         .. note::
             This method is used to convert the list format
             used by the neural net into a single array of stacked parameters
             for optimization.
         """
+        stacks = self.stack_per_layer()
+        return np.concatenate(stacks).reshape((-1, 1))
+
+    def stack_per_layer(self) -> List[np.ndarray]:
+        """Stack W, b into a single array for each layer.
+
+        .. code-block::
+
+            parameters.stack_per_layer()
+            >> [np.array([[W1], [b1]]), [W2], [b2]]), np.array([[W3], [b3]])]
+        """
         stacks = []
         for i in range(self.L):
             stack = np.concatenate([self.W[i].ravel(), self.b[i].ravel()]).reshape(
                 (-1, 1)
             )
             stacks.append(stack)
-        if per_layer:
-            return stacks
+        return stacks
+
+    def stack_partials(self) -> np.ndarray:
+        """Stack backprop partials dW, db.
+
+        .. code-block::
+
+            parameters.stack_partials()
+            >> np.array([[dW1], [db1], [dW2], [db2], [dW3], [db3]])
+
+        .. note::
+            This method is used to convert the list format used by the neural
+            net into a single array of stacked parameters for optimization.
+        """
+        stacks = self.stack_partials_per_layer()
         return np.concatenate(stacks).reshape((-1, 1))
 
+    def stack_partials_per_layer(self) -> List[np.ndarray]:
+        """Stack backprop partials dW, db per layer.
+
+        .. code-block::
+
+            parameters.stack_partials_per_layer()
+            >> [np.array([[dW1], [db1]]), np.array([[dW2], [db2]]), np.array([[dW3], [db3]]),]
+        """
+        stacks = []
+        for i in range(self.L):
+            stack = np.concatenate(
+                [
+                    self.dW[i].ravel(),
+                    self.db[i].ravel(),
+                ]
+            ).reshape((-1, 1))
+            stacks.append(stack)
+        return stacks
+
     def _column_to_stacks(self, params: np.ndarray) -> List[np.ndarray]:
         """Convert parameters from single stack to list of stacks.
 
         Neural net parameters are converted from single stack
         representation (for all layers) to a list of stacks (per layer).
 
         Parameters
@@ -224,50 +268,14 @@
         if isinstance(parameters, np.ndarray):  # single column
             parameters = self._column_to_stacks(parameters)
         for i, array in enumerate(parameters):  # stacks to params for each layer
             n, p = self.W[i].shape
             self.W[i][:] = array[: n * p].reshape(n, p)
             self.b[i][:] = array[n * p :].reshape(n, 1)
 
-    def stack_partials(
-        self, per_layer: bool = False
-    ) -> Union[np.ndarray, List[np.ndarray]]:
-        """Stack backprop partials dW, db.
-
-        dW, db are either stacked into a single stack (for all layers)
-        or a list of stacks (one per layer).
-
-        :param per_layer: whether to return answer as list of stacks (one per layer)
-        :return: partials as either single stacked array or list of stacks (if specified)
-
-        .. code-block::
-
-            parameters.stack_partials(per_layer=True)
-            >> [np.array([[dW1], [db1]]), np.array([[dW2], [db2]]), np.array([[dW3], [db3]]),]
-
-            parameters.stack_partials()
-            >> np.array([[dW1], [db1], [dW2], [db2], [dW3], [db3]])
-
-        .. note::
-            This method is used to convert the list format used by the neural
-            net into a single array of stacked parameters for optimization.
-        """
-        stacks = []
-        for i in range(self.L):
-            stack = np.concatenate(
-                [
-                    self.dW[i].ravel(),
-                    self.db[i].ravel(),
-                ]
-            ).reshape((-1, 1))
-            stacks.append(stack)
-        if per_layer:
-            return stacks
-        return np.concatenate(stacks).reshape((-1, 1))
-
     def unstack_partials(self, partials: Union[np.ndarray, List[np.ndarray]]) -> None:
         """Unstack backprop partials dW, db back into list of arrays.
 
         :param partials: neural network partials as either a single
             array where all layers are stacked on top of each other or a list of
             stacked parameters for each layer.
 
@@ -291,37 +299,72 @@
         if isinstance(partials, np.ndarray):  # single column
             partials = self._column_to_stacks(partials)
         for i, array in enumerate(partials):
             n, p = self.dW[i].shape
             self.dW[i][:] = array[: n * p].reshape(n, p)
             self.db[i][:] = array[n * p :].reshape(n, 1)
 
-    def serialize(self) -> bytes:
+    def _serialize(self) -> bytes:
         """Serialize parameters into byte stream for json."""
-        return orjson.dumps(self, option=orjson.OPT_SERIALIZE_NUMPY)
+        keys = jsonpointer.JsonPointer("/properties").get(SCHEMA)
+        data = {key: getattr(self, key) for key in keys}
+        return orjson.dumps(data, option=orjson.OPT_SERIALIZE_NUMPY)
 
-    def deserialize(self, saved_parameters: bytes) -> None:
+    def _deserialize(self, saved_parameters: bytes) -> None:
         """Deserialize and apply saved parameters."""
         params = orjson.loads(saved_parameters)
+        jsonschema.validate(params, SCHEMA)
         self.W = [np.array(value) for value in params["W"]]
         self.b = [np.array(value) for value in params["b"]]
         self.a = params["a"]
-        self.dW = [np.array(value) for value in params["dW"]]
-        self.db = [np.array(value) for value in params["db"]]
         self.mu_x = np.array(params["mu_x"])
         self.mu_y = np.array(params["mu_y"])
         self.sigma_x = np.array(params["sigma_x"])
         self.sigma_y = np.array(params["sigma_y"])
         self.layer_sizes = [W.shape[0] for W in self.W]
         self.output_activation = self.a[-1]
         self.hidden_activation = self.a[-2]
+        self.dW = [np.zeros(array.shape) for array in self.W]
+        self.db = [np.zeros(array.shape) for array in self.b]
+        assert (
+            self.mu_x.size == self.layer_sizes[0]
+        ), "mu_x size is different input layer size"
+        assert (
+            self.mu_y.size == self.layer_sizes[-1]
+        ), "mu_y size is different output layer size"
+        assert (
+            self.sigma_x.size == self.layer_sizes[0]
+        ), "sigma_x size is different input layer size"
+        assert (
+            self.sigma_y.size == self.layer_sizes[-1]
+        ), "sigma_x size is different output layer size"
+        assert (
+            self.mu_x.shape == self.sigma_x.shape
+        ), "mu_x and sigma_x have different shapes"
+        assert (
+            self.mu_y.shape == self.sigma_y.shape
+        ), "mu_y and sigma_y have different shapes"
+        m = self.layer_sizes[0]
+        for i, n in enumerate(self.layer_sizes):
+            assert (
+                self.a[i] in ACTIVATIONS
+            ), f"a[{i}] must be one of {list(ACTIVATIONS.keys())}"
+            assert self.b[i].shape == (
+                n,
+                1,
+            ), f"b[{i}] has the wrong shape (expected {(n, 1)})"
+            assert self.W[i].shape == (
+                n,
+                m,
+            ), f"W[{i}] has the wrong shape (expected {(n, m)})"
+            m = n
 
     def save(self, binary_file: Union[str, Path] = "parameters.json") -> None:
         """Save parameters to specified json file."""
         with open(binary_file, "wb") as file:
-            file.write(self.serialize())
+            file.write(self._serialize())
 
     def load(self, binary_file: Union[str, Path] = "parameters.json") -> None:
         """Load parameters from specified json file."""
         with open(binary_file, "rb") as file:
             byte_stream = file.read()
-        self.deserialize(byte_stream)
+        self._deserialize(byte_stream)
```

### Comparing `jenn-1.0.3/src/jenn/core/propagation.py` & `jenn-1.0.4/src/jenn/core/propagation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 """Propagation.
 ==============
 
 This module contains the critical functionality to propagate information forward and backward through the neural net."""
 
-from typing import List, Tuple, Union
+from typing import Tuple, Union
 
 import numpy as np
 
-from .activation import Linear, Relu, Tanh
+from .activation import ACTIVATIONS
 from .cache import Cache
 from .data import Dataset
 from .parameters import Parameters
 
-ACTIVATIONS = dict(
-    relu=Relu,
-    tanh=Tanh,
-    linear=Linear,
-)
-
 
 def eye(n: int, m: int) -> np.ndarray:
     """Copy identify matrix of shape (n, n) m times."""
     eye = np.eye(n, dtype=float)
     return np.repeat(eye.reshape((n, n, 1)), m, axis=2)
 
 
@@ -48,17 +42,15 @@
     """
     X = X.astype(float, copy=False)
     if cache is not None:
         n_x, m = X.shape
         cache.A_prime[0][:] = eye(n_x, m)
 
 
-def next_layer_partials(
-    layer: int, parameters: Parameters, cache: Cache
-) -> List[np.ndarray]:
+def next_layer_partials(layer: int, parameters: Parameters, cache: Cache) -> np.ndarray:
     """Compute j^th partial in place for one layer (in place).
 
     :param layer: index of current layer.
     :param parameters: object that stores neural net parameters for each
         layer
     :param cache: neural net cache that stores neural net quantities
         computed during forward prop for each layer, so they can be
@@ -152,19 +144,17 @@
     """Propagate backward through last layer (in place).
 
     :param cache: neural net cache that stores neural net quantities
         computed during forward prop for each layer, so they can be
         accessed during backprop to avoid re-computing them
     :param data: object containing training and associated metadata
     """
-    cache.dA[-1][:] = cache.A[-1] - data.Y
+    cache.dA[-1][:] = data.Y_weights * (cache.A[-1] - data.Y)
     if data.J is not None:
-        cache.dA_prime[-1][:] = cache.A_prime[-1] - data.J
-    else:
-        cache.dA_prime[-1][:] = np.zeros((data.n_y, data.n_x, data.m))
+        cache.dA_prime[-1][:] = data.J_weights * (cache.A_prime[-1] - data.J)
 
 
 def next_layer_backward(
     layer: int, parameters: Parameters, cache: Cache, data: Dataset, lambd: float
 ) -> None:
     """Propagate backward through next layer (in place).
 
@@ -187,93 +177,85 @@
     parameters.dW[r] += lambd / data.m * parameters.W[r]
     np.sum(cache.G_prime[r] * cache.dA[r], axis=1, keepdims=True, out=parameters.db[r])
     parameters.db[r] /= data.m
     np.dot(parameters.W[r].T, cache.G_prime[r] * cache.dA[r], out=cache.dA[s])
 
 
 def gradient_enhancement(
-    layer: int, parameters: Parameters, cache: Cache, data: Dataset, gamma: float
+    layer: int,
+    parameters: Parameters,
+    cache: Cache,
+    data: Dataset,
 ) -> None:
     """Add gradient enhancement to backprop (in place).
 
     :param layer: index of current layer.
     :param parameters: object that stores neural net parameters for each
         layer
     :param cache: neural net cache that stores neural net quantities
         computed during forward prop for each layer, so they can be
         accessed during backprop to avoid re-computing them
     :param data: object containing training and associated metadata
-    :param gamma: coefficient that multiplies jacobian-enhancement term
-        in cost function
     """
-    if np.allclose(gamma, 0.0):
+    if data.J is None:
+        return
+    if np.all(data.J_weights == 0.0):
         return
     r = layer
     s = layer - 1
     g = ACTIVATIONS[parameters.a[r]]
     cache.G_prime_prime[r][:] = g.second_derivative(
         cache.Z[r], cache.A[r], cache.G_prime[r]
     )
+    coefficient = 1 / data.m
     for j in range(parameters.n_x):
-        parameters.dW[r] += (
-            gamma
-            / data.m
-            * (
-                np.dot(
-                    cache.dA_prime[r][:, j, :]
-                    * cache.G_prime_prime[r]
-                    * cache.Z_prime[r][:, j, :],
-                    cache.A[s].T,
-                )
-                + np.dot(
-                    cache.dA_prime[r][:, j, :] * cache.G_prime[r],
-                    cache.A_prime[s][:, j, :].T,
-                )
-            )
-        )
-        parameters.db[r] += (
-            gamma
-            / data.m
-            * np.sum(
+        parameters.dW[r] += coefficient * (
+            np.dot(
                 cache.dA_prime[r][:, j, :]
                 * cache.G_prime_prime[r]
                 * cache.Z_prime[r][:, j, :],
-                axis=1,
-                keepdims=True,
+                cache.A[s].T,
+            )
+            + np.dot(
+                cache.dA_prime[r][:, j, :] * cache.G_prime[r],
+                cache.A_prime[s][:, j, :].T,
             )
         )
-        cache.dA[s] += gamma * np.dot(
+        parameters.db[r] += coefficient * np.sum(
+            cache.dA_prime[r][:, j, :]
+            * cache.G_prime_prime[r]
+            * cache.Z_prime[r][:, j, :],
+            axis=1,
+            keepdims=True,
+        )
+        cache.dA[s] += np.dot(
             parameters.W[r].T,
             cache.dA_prime[r][:, j, :]
             * cache.G_prime_prime[r]
             * cache.Z_prime[r][:, j, :],
         )
-        cache.dA_prime[s][:, j, :] = gamma * np.dot(
+        cache.dA_prime[s][:, j, :] = np.dot(
             parameters.W[r].T, cache.dA_prime[r][:, j, :] * cache.G_prime[r]
         )
 
 
 def model_backward(
     data: Dataset,
     parameters: Parameters,
     cache: Cache,
     lambd: float = 0.0,
-    gamma: float = 0.0,
 ) -> None:
     """Propagate backward through all layers (in place).
 
     :param parameters: object that stores neural net parameters for each
         layer
     :param cache: neural net cache that stores neural net quantities
         computed during forward prop for each layer, so they can be
         accessed during backprop to avoid re-computing them
     :param data: object containing training and associated metadata
-    :param lambd: coefficient that multiplies regularization term in
-        cost function
-    :param gamma: coefficient that multiplies jacobian-enhancement term
-        in cost function
+    :param lambd: regularization coefficient to avoid overfitting [defaulted to zero] (optional)
     """
     last_layer_backward(cache, data)
     for layer in reversed(parameters.layers):  # type: ignore[call-overload]
         if layer > 0:
             next_layer_backward(layer, parameters, cache, data, lambd)
-            gradient_enhancement(layer, parameters, cache, data, gamma)
+            gradient_enhancement(layer, parameters, cache, data)
```

### Comparing `jenn-1.0.3/src/jenn/core/training.py` & `jenn-1.0.4/src/jenn/core/training.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Union
 
 import numpy as np
 
 from .cache import Cache
 from .cost import Cost
 from .data import Dataset
-from .optimization import ADAM, Backtracking, Optimizer
+from .optimization import ADAMOptimizer
 from .parameters import Parameters
 from .propagation import model_backward, model_partials_forward
 
 
 def objective_function(
     X: np.ndarray,
     cost: Cost,
@@ -42,15 +42,14 @@
 
 
 def objective_gradient(
     data: Dataset,
     parameters: Parameters,
     cache: Cache,
     lambd: float,
-    gamma: float,
     stacked_params: np.ndarray,
 ) -> np.ndarray:  # noqa: PLR0913
     """Evaluate cost function gradient for backprop.
 
     :param data: object containing training and associated metadata
     :param parameters: object that stores neural net parameters for each
         layer
@@ -62,90 +61,109 @@
     :param gamma: coefficient that multiplies jacobian-enhancement term
         in cost function
     :param stacked_params: neural network parameters returned by the
         optimizer, represented as single array of stacked parameters for
         all layers.
     """
     parameters.unstack(stacked_params)
-    model_backward(data, parameters, cache, lambd, gamma)
+    model_backward(data, parameters, cache, lambd)
     return parameters.stack_partials()
 
 
 def train_model(
     data: Dataset,
     parameters: Parameters,
-    alpha: float = 0.050,
-    lambd: float = 0.000,
-    gamma: float = 0.000,
-    beta1: float = 0.900,
-    beta2: float = 0.999,
+    alpha: float = 0.05,
+    beta: Union[np.ndarray, float] = 1.0,
+    gamma: Union[np.ndarray, float] = 1.0,
+    lambd: float = 0.0,
+    beta1: float = 0.9,
+    beta2: float = 0.99,
+    tau: float = 0.5,
+    tol: float = 1e-12,
+    max_count: int = 1000,
+    epsilon_absolute: float = 1e-12,
+    epsilon_relative: float = 1e-12,
     epochs: int = 1,
     max_iter: int = 200,
     batch_size: Union[int, None] = None,
     shuffle: bool = True,
     random_state: Union[int, None] = None,
     is_backtracking: bool = False,
     is_verbose: bool = False,
 ) -> dict:  # noqa: PLR0913
     r"""Train neural net.
 
     :param data: object containing training and associated metadata
     :param parameters: object that stores neural net parameters for each
         layer
     :param alpha: learning rate :math:`\alpha`
-    :param lambd: regularization term coefficient in cost function
-    :param gamma: jacobian-enhancement term coefficient in cost function
+    :param beta: LSE coefficients [defaulted to one] (optional)
+    :param gamma: jacobian-enhancement regularization coefficient [defaulted to zero] (optional)
+    :param lambd: regularization coefficient to avoid overfitting [defaulted to zero] (optional)
     :param beta_1: exponential decay rate of 1st moment vector
         :math:`\beta_1\in[0, 1)`
     :param beta_2: exponential decay rate of 2nd moment vector
         :math:`\beta_2\in[0, 1)`
+    :param tau: amount by which to reduce :math:`\alpha := \tau \times
+        \alpha` on each iteration
+    :param tol: stop when cost function doesn't improve more than
+        specified tolerance
+    :param max_count: stop when line search iterations exceed maximum
+        count specified
+    :param epsilon_absolute: absolute error stopping criterion
+    :param epsilon_relative: relative error stopping criterion
     :param epochs: number of passes through data
     :param batch_size: mini batch size (if None, single batch with all
         data)
     :param max_iter: maximum number of optimizer iterations allowed
     :param shuffle: swhether to huffle data points or not
     :param random_state: random seed (useful to make runs repeatable)
     :param is_backtracking: whether or not to use backtracking during
         line search
     :param is_verbose: print out progress for each iteration, each
         batch, each epoch
     :return: cost function training history accessed as `cost =
         history[epoch][batch][iter]`
     """
-    history: dict[str, dict[str, Union[list[float], None]]] = defaultdict(dict)
-
-    update = ADAM(beta1, beta2)
-    line_search = Backtracking(update, max_count=is_backtracking * 1_000)
-    optimizer = Optimizer(line_search)
-
+    history: dict[str, dict[str, Union[list[np.ndarray], None]]] = defaultdict(dict)
+    optimizer = ADAMOptimizer(
+        beta_1=beta1,
+        beta_2=beta2,
+        tau=tau,
+        tol=tol,
+        max_count=is_backtracking * max_count,
+    )
+    data.set_weights(beta, gamma)
     for e in range(epochs):
         batches = data.mini_batches(batch_size, shuffle, random_state)
         for b, batch in enumerate(batches):
             cache = Cache(parameters.layer_sizes, batch.m)
-            cost = Cost(batch, parameters, lambd, gamma)
+            cost = Cost(batch, parameters, lambd)
             func = functools.partial(
                 objective_function,
                 batch.X,
                 cost,
                 parameters,
                 cache,
             )
             grad = functools.partial(
                 objective_gradient,
                 batch,
                 parameters,
                 cache,
                 lambd,
-                gamma,
             )
             optimizer.minimize(
                 x=parameters.stack(),
                 f=func,
                 dfdx=grad,
                 alpha=alpha,
                 max_iter=max_iter,
+                epsilon_absolute=epsilon_absolute,
+                epsilon_relative=epsilon_relative,
                 verbose=is_verbose,
                 epoch=e,
                 batch=b,
             )
             history[f"epoch_{e}"][f"batch_{b}"] = optimizer.cost_history
     return history
```

### Comparing `jenn-1.0.3/src/jenn/model.py` & `jenn-1.0.4/src/jenn/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,55 +83,74 @@
 
     def fit(
         self,
         x: np.ndarray,
         y: np.ndarray,
         dydx: Union[np.ndarray, None] = None,
         is_normalize: bool = False,
-        alpha: float = 0.050,
-        lambd: float = 0.000,
-        gamma: float = 1.000,
-        beta1: float = 0.900,
-        beta2: float = 0.999,
+        alpha: float = 0.05,
+        beta: Union[np.ndarray, float] = 1.0,
+        gamma: Union[np.ndarray, float] = 1.0,
+        lambd: float = 0.0,
+        beta1: float = 0.9,
+        beta2: float = 0.99,
+        tau: float = 0.5,
+        tol: float = 1e-12,
+        max_count: int = 1000,
+        epsilon_absolute: float = 1e-12,
+        epsilon_relative: float = 1e-12,
         epochs: int = 1,
         batch_size: Union[int, None] = None,
-        max_iter: int = 200,
+        max_iter: int = 1000,
         shuffle: bool = True,
         random_state: Union[int, None] = None,
         is_backtracking: bool = False,
+        is_warmstart: bool = False,
         is_verbose: bool = False,
     ) -> "NeuralNet":  # noqa: PLR0913
         r"""Train neural network.
 
         :param x: training data inputs, array of shape (n_x, m)
         :param y: training data outputs, array of shape (n_y, m)
         :param dydx: training data Jacobian, array of shape (n_y, n_x, m)
         :param is_normalize: normalize training by mean and variance
         :param alpha: optimizer learning rate for line search
-        :param lambd: regularization coefficient to avoid overfitting
-        :param gamma: jacobian-enhancement regularization coefficient
+        :param beta: LSE coefficients [defaulted to one] (optional)
+        :param gamma: jacobian-enhancement regularization coefficient [defaulted to zero] (optional)
+        :param lambd: regularization coefficient to avoid overfitting [defaulted to zero] (optional)
         :param beta1: `ADAM <https://arxiv.org/abs/1412.6980>`_ optimizer hyperparameter to control momentum
         :param beta2: ADAM optimizer hyperparameter to control momentum
+        :param tau: amount by which to reduce :math:`\alpha := \tau \times
+            \alpha` on each iteration
+        :param tol: stop when cost function doesn't improve more than
+            specified tolerance
+        :param max_count: stop when line search iterations exceed maximum
+            count specified
+        :param epsilon_absolute: absolute error stopping criterion
+        :param epsilon_relative: relative error stopping criterion
         :param epochs: number of passes through data
         :param batch_size: size of each batch for minibatch
         :param max_iter: max number of optimizer iterations
         :param shuffle: shuffle minibatches or not
         :param random_state: control repeatability
         :param is_backtracking: use backtracking line search or not
+        :param is_warmstart: do not initialize parameters
         :param is_verbose: print out progress for each (iteration, batch, epoch)
         :return: NeuralNet instance (self)
 
         .. warning::
                 Normalization usually helps, except when the training
                 data is made up of very small numbers. In that case,
                 normalizing by the variance has the undesirable effect
                 of dividing by a very small number and should not be used.
         """
         data = Dataset(x, y, dydx)
         params = self.parameters
+        if not is_warmstart:
+            params.initialize(random_state)
         params.mu_x[:] = 0.0
         params.mu_y[:] = 0.0
         params.sigma_x[:] = 1.0
         params.sigma_y[:] = 1.0
         if is_normalize:
             params.mu_x[:] = data.avg_x
             params.mu_y[:] = data.avg_y
@@ -139,18 +158,24 @@
             params.sigma_y[:] = data.std_y
             data = data.normalize()
         self.history = train_model(
             data,
             params,
             # hyperparameters
             alpha=alpha,
-            lambd=lambd,
+            beta=beta,
             gamma=gamma,
+            lambd=lambd,
             beta1=beta1,
             beta2=beta2,
+            tau=tau,
+            tol=tol,
+            max_count=max_count,
+            epsilon_absolute=epsilon_absolute,
+            epsilon_relative=epsilon_relative,
             # options
             epochs=epochs,
             max_iter=max_iter,
             batch_size=batch_size,
             shuffle=shuffle,
             random_state=random_state,
             is_backtracking=is_backtracking,
```

### Comparing `jenn-1.0.3/src/jenn/synthetic.py` & `jenn-1.0.4/src/jenn/synthetic.py`

 * *Files 13% similar despite different names*

```diff
@@ -69,41 +69,74 @@
 
         :param x: inputs, array of shape (n_x, m)
         :return: partials, array of shape (n_y, n_x, m)
         """
         raise NotImplementedError
 
     @classmethod
+    def first_derivative_FD(
+        cls,
+        x: np.ndarray,
+        dx: float = 1e-6,
+    ) -> np.ndarray:
+        """Evaluate partial derivative using finite difference.
+
+        :param x: inputs, array of shape (n_x, m)
+        :return: partials, array of shape (n_y, n_x, m)
+        """
+        f = cls.evaluate
+        y = f(x)  # type: ignore
+        n_x, m = x.shape
+        n_y = y.shape[0]
+        dydx = np.zeros((n_y, n_x, m))
+        for i in range(n_x):
+            dx1 = np.zeros((n_x, m))
+            dx2 = np.zeros((n_x, m))
+            dx1[i] += dx
+            dx2[i] += dx
+            x1 = x - dx1
+            x2 = x + dx2
+            y1 = f(x1)  # type: ignore
+            y2 = f(x2)  # type: ignore
+            dydx[:, i] = (y2 - y1) / (2 * dx)
+        return dydx
+
+    @classmethod
     def sample(
         cls,
         m_lhs: int,
         m_levels: int,
         lb: Union[np.ndarray, float],
         ub: Union[np.ndarray, float],
+        dx: float | None = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """Generate synthetic data by sampling the test function.
 
         :param m_lhs: number of latin hypercube samples
         :param m_levels: number of levels per factor for full factorial
         :param lb: lower bound on the factors
         :param ub: upper bound on the factors
+        :param dx: finite difference step size (if None, analytical partials are used)
         :param random_state: random seed (for repeatability)
         """
         rng = np.random.default_rng(seed=random_state)
         lb = np.array([lb]).reshape((-1, 1))  # make sure it's an numpy array
         ub = np.array([ub]).reshape((-1, 1))  # make sure it's an numpy array
         n_x = lb.size
         lh = rng.random(size=(n_x, m_lhs))
         ff = _fullfact(n_x, m_levels)
         doe = np.concatenate([lh, ff], axis=1)
         m = doe.shape[1]
         x = lb + (ub - lb) * doe
         y = cls.evaluate(x).reshape((-1, m))  # type: ignore[call-arg]
-        dydx = cls.first_derivative(x).reshape((-1, n_x, m))  # type: ignore[call-arg]
+        if dx is None:
+            dydx = cls.first_derivative(x).reshape((-1, n_x, m))  # type: ignore[call-arg]
+        else:
+            dydx = cls.first_derivative_FD(x, dx).reshape((-1, n_x, m))
         return x, y, dydx
 
 
 class Linear(TestFunction):
     r"""Linear function.
 
     .. math::
@@ -141,17 +174,18 @@
     @classmethod
     def sample(
         cls,
         m_lhs: int = 100,
         m_levels: int = 0,
         lb: Union[np.ndarray, float] = -1.0,
         ub: Union[np.ndarray, float] = 1.0,
+        dx: float | None = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:  # noqa: D102
-        return super().sample(m_lhs, m_levels, lb, ub, random_state)
+        return super().sample(m_lhs, m_levels, lb, ub, dx, random_state)
 
 
 class Parabola(TestFunction):
     r"""Parabolic function.
 
     .. math::
         f(x) = \frac{1}{n} \sum_{i=1}^p (x_i - {x_0}_i)^2
@@ -180,17 +214,18 @@
     @classmethod
     def sample(
         cls,
         m_lhs: int = 100,
         m_levels: int = 0,
         lb: Union[np.ndarray, float] = -1.0,
         ub: Union[np.ndarray, float] = 1.0,
+        dx: float | None = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:  # noqa: D102
-        return super().sample(m_lhs, m_levels, lb, ub, random_state)
+        return super().sample(m_lhs, m_levels, lb, ub, dx, random_state)
 
 
 class Sinusoid(TestFunction):
     r"""Sinusoidal function.
 
     .. math::
         f(x) = x \sin(x)
@@ -215,17 +250,18 @@
     @classmethod
     def sample(
         cls,
         m_lhs: int = 100,
         m_levels: int = 0,
         lb: Union[np.ndarray, float] = -np.pi,
         ub: Union[np.ndarray, float] = np.pi,
+        dx: float | None = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:  # noqa: D102
-        return super().sample(m_lhs, m_levels, lb, ub, random_state)
+        return super().sample(m_lhs, m_levels, lb, ub, dx, random_state)
 
 
 class Rastrigin(TestFunction):
     r"""Rastrigin function.
 
     .. math::
         f(x) = \sum_{i=1}^p ( x_i^2 - 10 \cos(2\pi x_i) )
@@ -258,17 +294,18 @@
         * np.ones(
             2,
         ),
         ub: Union[np.ndarray, float] = 1.5
         * np.ones(
             2,
         ),
+        dx: float | None = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:  # noqa: D102
-        return super().sample(m_lhs, m_levels, lb, ub, random_state)
+        return super().sample(m_lhs, m_levels, lb, ub, dx, random_state)
 
 
 class Rosenbrock(TestFunction):
     r"""Banana Rosenbrock function.
 
     .. math::
         f(x) = (1 - x_1)^2 + 100 (x_2 - x_1^2)^ 2
@@ -300,10 +337,11 @@
         * np.ones(
             2,
         ),
         ub: Union[np.ndarray, float] = 2.0
         * np.ones(
             2,
         ),
+        dx: float | None = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:  # noqa: D102
-        return super().sample(m_lhs, m_levels, lb, ub, random_state)
+        return super().sample(m_lhs, m_levels, lb, ub, dx, random_state)
```

### Comparing `jenn-1.0.3/src/jenn/utils/metrics.py` & `jenn-1.0.4/src/jenn/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.3/src/jenn/utils/plot.py` & `jenn-1.0.4/src/jenn/utils/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 @requires_matplotlib
 def actual_by_predicted(
     y_pred: np.ndarray,
     y_true: np.ndarray,
     ax: Union[plt.Axes, None] = None,  # noqa: ANN401
     figsize: Tuple[float, float] = (3.25, 3),
-    title: Union[str, None] = None,
+    title: str = "",
     fontsize: int = 9,
     alpha: float = 1.0,
 ) -> plt.Figure:  # noqa: ANN401
     """Create actual by predicted plot for a single response.
 
     :param y_pred: predicted values, array of shape (m,)
     :param y_true: true values, array of shape (m,)
@@ -136,15 +136,15 @@
     predicted = y_pred.ravel()
     ax.scatter(actual, predicted, color="k", alpha=alpha)
     line = [actual.min(), actual.max()]
     ax.plot(line, line, color="r", linestyle=":")
     ax.set_xlabel("Predicted", fontsize=fontsize)
     ax.set_ylabel("Actual", fontsize=fontsize)
     ax.set_title(title, fontsize=fontsize)
-    ax.grid("on")
+    ax.grid(True)
     ax.legend(["predictions", "perfect fit line"], fontsize=fontsize)
     plt.close(fig)
     return fig
 
 
 def contours(
     func: Callable,
@@ -154,25 +154,27 @@
     x_test: Union[np.ndarray, None] = None,
     figsize: Tuple[float, float] = (3.25, 3),
     fontsize: int = 9,
     alpha: float = 0.5,
     title: str = "",
     xlabel: str = "",
     ylabel: str = "",
+    levels: int = 20,
     resolution: int = 100,
     ax: Union[plt.Axes, None] = None,  # noqa: ANN401
-) -> plt.Figure:  # noqa: ANN401
+) -> Union[None, plt.Figure]:  # noqa: ANN401
     """Plot contours of a scalar function of two variables.
 
     :param figsize: figure size
     :param fontsize: text size
     :param alpha: transparency of dots (between 0 and 1)
     :param title: title of figure
     :param xlabel: factor #1 label
     :param ylabel: factor #2 label
+    :param levels: number of contour levels
     :param resolution: line resolution
     :param ax: the matplotlib axes on which to plot the data
     :return: matplotlib figure instance
     """
     # Domain
     m = resolution
     x1 = np.linspace(lb[0], ub[0], m)
@@ -187,15 +189,15 @@
 
     # Plot
     if ax:
         fig = ax.get_figure()
     else:
         fig = plt.figure(figsize=figsize)
         ax = plt.gca()
-    ax.contour(x1, x2, y, 20, cmap="RdGy", alpha=alpha)
+    ax.contour(x1, x2, y, levels, cmap="RdGy", alpha=alpha)
     legend = []
     if x_train is not None:
         ax.scatter(x_train[0], x_train[1], marker=".", c="k", alpha=1)
         legend.append("train")
     if x_test is not None:
         ax.scatter(x_test[0], x_test[1], marker="+", c="r", alpha=1)
         legend.append("test")
@@ -294,15 +296,15 @@
 @requires_matplotlib
 def residuals_by_predicted(
     y_pred: np.ndarray,
     y_true: np.ndarray,
     percent_residuals: bool = False,
     ax: Union[plt.Axes, None] = None,  # noqa: ANN401
     figsize: Tuple[float, float] = (3.25, 3),
-    title: Union[str, None] = None,
+    title: str = "",
     fontsize: int = 9,
     alpha: float = 1.0,
 ) -> plt.Figure:  # noqa: ANN401
     """Create residual by predicted plot for a single response.
 
     :param y_pred: predicted values, array of shape (m,)
     :param y_true: true values, array of shape (m,)
@@ -349,29 +351,29 @@
     ax.axhline(y=0, color="r", linestyle=":")
     ax.set_title(title, fontsize=fontsize)
     if percent_residuals:
         ax.set_ylabel("Residuals (%)", fontsize=fontsize)
     else:
         ax.set_ylabel("Residuals", fontsize=fontsize)
     ax.set_xlabel("Predicted", fontsize=fontsize)
-    ax.grid("on")
+    ax.grid(True)
     ax.legend([f"avg = {avg_error:.3f}", f"std = {std_error:.3f}"], fontsize=fontsize)
     plt.close(fig)
     return fig
 
 
 @requires_matplotlib
 def goodness_of_fit(
     y_true: np.ndarray,
     y_pred: np.ndarray,
     percent_residuals: bool = False,
     figsize: Tuple[float, float] = (6.5, 3),
     fontsize: int = 9,
     alpha: float = 1.0,
-    title: Union[str, None] = None,
+    title: str = "",
 ) -> plt.Figure:  # noqa: ANN401
     """Create 'residual by predicted' and 'actual by predicted' plots.
 
     :param y_true: true values, array of shape (m,)
     :param y_pred: predicted values, array of shape (m,)
     :param percent_residuals: shows residuals as percentages if True
     :param figsize: figure size
@@ -466,15 +468,15 @@
         legend.append("data")
     ax.legend(legend, fontsize=fontsize)
     if show_cursor:
         for n in range(y0.size):
             ax.scatter(x0, y0[n], color="r")
     ax.set_xlabel(xlabel, fontsize=fontsize)
     ax.set_ylabel(ylabel, fontsize=fontsize)
-    ax.grid("on")
+    ax.grid(True)
     plt.close(fig)
     return fig
 
 
 @requires_matplotlib
 def sensitivity_profiles(
     f: Union[Callable, List[Callable]],
```

### Comparing `jenn-1.0.3/src/jenn.egg-info/PKG-INFO` & `jenn-1.0.4/src/jenn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jenn
-Version: 1.0.3
+Version: 1.0.4
 Summary: Jacobian-Enhanced Neural Nets (JENN)
 Author-email: "Steven H. Berguin" <stevenberguin@gmail.com>
 Project-URL: Documentation, https://shb84.github.io/JENN/
 Project-URL: Homepage, https://github.com/shb84/JENN
 Project-URL: Issues, https://github.com/shb84/JENN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jenn-1.0.3/src/jenn.egg-info/SOURCES.txt` & `jenn-1.0.4/src/jenn.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,13 +17,14 @@
 src/jenn/core/optimization.py
 src/jenn/core/parameters.py
 src/jenn/core/propagation.py
 src/jenn/core/training.py
 src/jenn/utils/__init__.py
 src/jenn/utils/metrics.py
 src/jenn/utils/plot.py
+src/jenn/utils/rbf.py
 tests/test_activation.py
 tests/test_cost.py
 tests/test_model.py
 tests/test_optimization.py
 tests/test_parameters.py
 tests/test_propagation.py
```

### Comparing `jenn-1.0.3/tests/test_activation.py` & `jenn-1.0.4/tests/test_activation.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.3/tests/test_cost.py` & `jenn-1.0.4/tests/test_cost.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 
 def test_least_squares():
     """Test that least squares cost function evaluates to known answers."""
     x, y, dydx = jenn.synthetic.Sinusoid.sample(100)
 
     parameters = jenn.core.parameters.Parameters(layer_sizes=[2, 2, 1])
+    parameters.initialize()
+    
     data = jenn.core.data.Dataset(x, y, dydx)
     cost = jenn.core.cost.Cost(data, parameters, lambd=0.0)
 
     # Verify that cost is zero when prediction is perfect
     assert cost.evaluate(y, dydx) == 0
 
     # Verify that cost is non-zero when prediction is imperfect
```

### Comparing `jenn-1.0.3/tests/test_model.py` & `jenn-1.0.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.3/tests/test_optimization.py` & `jenn-1.0.4/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.3/tests/test_parameters.py` & `jenn-1.0.4/tests/test_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 class TestSerialization: 
     """Check that parameters can be saved and reloaded."""
 
     @pytest.fixture
     def params(self) -> jenn.core.parameters.Parameters:
         """Return XOR parameters."""
         parameters = jenn.core.parameters.Parameters(layer_sizes=[2, 2, 1], output_activation='relu')
+        parameters.initialize()
         parameters.b[1][:] = np.array([[0], [-1]])        # layer 1
         parameters.W[1][:] = np.array([[1, 1], [1, 1]])   # layer 1
         parameters.b[2][:] = np.array([[0]])              # layer 2
         parameters.W[2][:] = np.array([[1, -2]])          # layer 2
         return parameters
     
     def test_serialization(self, params: jenn.core.parameters.Parameters) -> None:
```

### Comparing `jenn-1.0.3/tests/test_propagation.py` & `jenn-1.0.4/tests/test_propagation.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         """Return XOR cache."""
         return jenn.core.cache.Cache(layer_sizes=[2, 2, 1], m=Y_test.size)
 
     @pytest.fixture
     def params(self) -> jenn.core.parameters.Parameters:
         """Return XOR parameters."""
         parameters = jenn.core.parameters.Parameters(layer_sizes=[2, 2, 1], output_activation='relu')
+        parameters.initialize()
         parameters.b[1][:] = np.array([[0], [-1]])        # layer 1
         parameters.W[1][:] = np.array([[1, 1], [1, 1]])   # layer 1
         parameters.b[2][:] = np.array([[0]])              # layer 2
         parameters.W[2][:] = np.array([[1, -2]])          # layer 2
         return parameters
 
     def test_model_forward(
@@ -133,16 +134,15 @@
 
         jenn.core.propagation.model_partials_forward(
             data.X, params, cache)  # predict to populate cache
 
         jenn.core.propagation.model_backward(
             data, params, cache)  # partials computed in place
 
-        dydx = params.stack_partials(per_layer=False)
-
+        dydx = params.stack_partials()
         assert np.allclose(dydx, 0.0)  # partials should be 0 at optimum params
 
         ###################
         # Imperfect model #
         ###################
 
         for i in range(params.L): # falsify model so partials are not zero
@@ -158,14 +158,14 @@
         def cost_FD(x):
             parameters = deepcopy(params)  # make copy b/c arrays updated in place
             cost = jenn.core.cost.Cost(data, parameters)
             parameters.unstack(x)
             Y_pred = jenn.core.propagation.model_forward(data.X, parameters, deepcopy(cache))
             return cost.evaluate(Y_pred)
 
-        dydx = params.stack_partials(per_layer=True)
-        dydx_FD = _finite_difference(cost_FD, params.stack(per_layer=True))
+        dydx = params.stack_partials_per_layer()
+        dydx_FD = _finite_difference(cost_FD, params.stack_per_layer())
 
         assert _grad_check(dydx, dydx_FD)
 
 
 # TODO: add test(s) for gradient-enhanced backprop and forward prop of partials
```

