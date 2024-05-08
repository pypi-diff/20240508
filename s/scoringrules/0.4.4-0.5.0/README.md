# Comparing `tmp/scoringrules-0.4.4.tar.gz` & `tmp/scoringrules-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoringrules-0.4.4.tar", max compression
+gzip compressed data, was "scoringrules-0.5.0.tar", max compression
```

## Comparing `scoringrules-0.4.4.tar` & `scoringrules-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11348 2023-05-24 14:33:45.077293 scoringrules-0.4.4/LICENSE
--rw-r--r--   0        0        0     2505 2023-12-22 10:04:48.255981 scoringrules-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1158 2023-12-22 10:03:02.914586 scoringrules-0.4.4/scoringrules/__init__.py
--rw-r--r--   0        0        0      952 2023-12-21 16:48:08.583129 scoringrules-0.4.4/scoringrules/_brier.py
--rw-r--r--   0        0        0    13358 2023-12-22 10:03:02.915405 scoringrules-0.4.4/scoringrules/_crps.py
--rw-r--r--   0        0        0     9252 2023-12-22 10:03:02.916646 scoringrules-0.4.4/scoringrules/_energy.py
--rw-r--r--   0        0        0     2052 2023-12-22 10:03:02.917167 scoringrules-0.4.4/scoringrules/_error_spread.py
--rw-r--r--   0        0        0     1120 2023-12-21 16:44:36.814321 scoringrules-0.4.4/scoringrules/_logs.py
--rw-r--r--   0        0        0     9552 2023-12-22 10:03:02.917929 scoringrules-0.4.4/scoringrules/_variogram.py
--rw-r--r--   0        0        0      207 2023-12-21 16:44:36.815394 scoringrules-0.4.4/scoringrules/backend/__init__.py
--rw-r--r--   0        0        0     5274 2023-11-10 08:02:17.495395 scoringrules-0.4.4/scoringrules/backend/base.py
--rw-r--r--   0        0        0     4311 2023-11-10 08:02:17.496121 scoringrules-0.4.4/scoringrules/backend/jax.py
--rw-r--r--   0        0        0     3732 2023-11-10 08:02:17.496560 scoringrules-0.4.4/scoringrules/backend/numpy.py
--rw-r--r--   0        0        0     2409 2023-12-22 10:03:02.918369 scoringrules-0.4.4/scoringrules/backend/registry.py
--rw-r--r--   0        0        0     5500 2023-12-21 16:44:36.815991 scoringrules-0.4.4/scoringrules/backend/tensorflow.py
--rw-r--r--   0        0        0     4775 2023-12-22 10:03:02.918925 scoringrules-0.4.4/scoringrules/backend/torch.py
--rw-r--r--   0        0        0        0 2023-11-10 08:02:17.497880 scoringrules-0.4.4/scoringrules/core/__init__.py
--rw-r--r--   0        0        0      739 2023-12-21 16:44:36.817437 scoringrules-0.4.4/scoringrules/core/brier.py
--rw-r--r--   0        0        0      286 2023-11-10 08:02:17.499474 scoringrules-0.4.4/scoringrules/core/crps/__init__.py
--rw-r--r--   0        0        0     3438 2023-12-21 16:44:36.818142 scoringrules-0.4.4/scoringrules/core/crps/_approx.py
--rw-r--r--   0        0        0     1711 2023-12-21 16:44:36.818479 scoringrules-0.4.4/scoringrules/core/crps/_closed.py
--rw-r--r--   0        0        0     9521 2023-11-10 08:02:17.501847 scoringrules-0.4.4/scoringrules/core/crps/_gufuncs.py
--rw-r--r--   0        0        0      376 2023-11-10 08:02:17.502536 scoringrules-0.4.4/scoringrules/core/energy/__init__.py
--rw-r--r--   0        0        0     2530 2023-11-10 08:02:17.503004 scoringrules-0.4.4/scoringrules/core/energy/_gufuncs.py
--rw-r--r--   0        0        0     2602 2023-12-21 16:44:36.818821 scoringrules-0.4.4/scoringrules/core/energy/_score.py
--rw-r--r--   0        0        0      128 2023-12-22 10:03:02.919393 scoringrules-0.4.4/scoringrules/core/error_spread/__init__.py
--rw-r--r--   0        0        0      839 2023-12-22 10:03:02.919744 scoringrules-0.4.4/scoringrules/core/error_spread/_gufunc.py
--rw-r--r--   0        0        0      621 2023-12-22 10:03:02.920102 scoringrules-0.4.4/scoringrules/core/error_spread/_score.py
--rw-r--r--   0        0        0      677 2023-12-21 16:44:36.819122 scoringrules-0.4.4/scoringrules/core/logarithmic.py
--rw-r--r--   0        0        0      943 2023-12-21 16:44:36.819733 scoringrules-0.4.4/scoringrules/core/stats.py
--rw-r--r--   0        0        0      476 2023-12-21 16:44:36.820351 scoringrules-0.4.4/scoringrules/core/typing.py
--rw-r--r--   0        0        0     1315 2023-11-10 08:02:17.505191 scoringrules-0.4.4/scoringrules/core/utils.py
--rw-r--r--   0        0        0      397 2023-11-10 08:02:17.505745 scoringrules-0.4.4/scoringrules/core/variogram/__init__.py
--rw-r--r--   0        0        0     2922 2023-11-10 08:02:17.506234 scoringrules-0.4.4/scoringrules/core/variogram/_gufuncs.py
--rw-r--r--   0        0        0     3362 2023-12-21 16:44:36.820980 scoringrules-0.4.4/scoringrules/core/variogram/_score.py
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 scoringrules-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-05-10 12:48:41.343565 scoringrules-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2504 2024-05-08 07:29:05.548392 scoringrules-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1158 2024-04-04 18:44:03.729234 scoringrules-0.5.0/scoringrules/__init__.py
+-rw-r--r--   0        0        0      952 2024-05-08 07:26:24.480906 scoringrules-0.5.0/scoringrules/_brier.py
+-rw-r--r--   0        0        0    13391 2024-05-08 07:26:24.481381 scoringrules-0.5.0/scoringrules/_crps.py
+-rw-r--r--   0        0        0     9326 2024-05-08 07:26:24.482229 scoringrules-0.5.0/scoringrules/_energy.py
+-rw-r--r--   0        0        0     1455 2024-05-08 07:26:24.482623 scoringrules-0.5.0/scoringrules/_error_spread.py
+-rw-r--r--   0        0        0     1121 2024-05-08 07:26:24.483091 scoringrules-0.5.0/scoringrules/_logs.py
+-rw-r--r--   0        0        0     9639 2024-05-08 07:26:24.483485 scoringrules-0.5.0/scoringrules/_variogram.py
+-rw-r--r--   0        0        0      207 2023-11-21 10:51:34.399740 scoringrules-0.5.0/scoringrules/backend/__init__.py
+-rw-r--r--   0        0        0     7880 2024-04-30 08:37:43.267646 scoringrules-0.5.0/scoringrules/backend/base.py
+-rw-r--r--   0        0        0     5694 2024-04-30 08:37:43.269594 scoringrules-0.5.0/scoringrules/backend/jax.py
+-rw-r--r--   0        0        0     5253 2024-04-30 08:37:43.272167 scoringrules-0.5.0/scoringrules/backend/numpy.py
+-rw-r--r--   0        0        0     2423 2024-01-12 19:11:22.760540 scoringrules-0.5.0/scoringrules/backend/registry.py
+-rw-r--r--   0        0        0     7083 2024-04-30 08:37:43.275286 scoringrules-0.5.0/scoringrules/backend/tensorflow.py
+-rw-r--r--   0        0        0     6262 2024-04-30 08:37:43.277534 scoringrules-0.5.0/scoringrules/backend/torch.py
+-rw-r--r--   0        0        0        0 2023-11-01 17:12:40.919839 scoringrules-0.5.0/scoringrules/core/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-08 07:26:24.484282 scoringrules-0.5.0/scoringrules/core/brier.py
+-rw-r--r--   0        0        0      286 2024-04-04 18:44:03.730806 scoringrules-0.5.0/scoringrules/core/crps/__init__.py
+-rw-r--r--   0        0        0     3408 2024-05-08 07:26:24.484679 scoringrules-0.5.0/scoringrules/core/crps/_approx.py
+-rw-r--r--   0        0        0     1711 2024-05-08 07:26:24.485021 scoringrules-0.5.0/scoringrules/core/crps/_closed.py
+-rw-r--r--   0        0        0     9081 2024-05-08 07:26:24.485435 scoringrules-0.5.0/scoringrules/core/crps/_gufuncs.py
+-rw-r--r--   0        0        0      376 2023-11-01 17:12:40.931435 scoringrules-0.5.0/scoringrules/core/energy/__init__.py
+-rw-r--r--   0        0        0     2289 2024-05-08 07:26:24.485821 scoringrules-0.5.0/scoringrules/core/energy/_gufuncs.py
+-rw-r--r--   0        0        0     2500 2024-05-08 07:26:24.486413 scoringrules-0.5.0/scoringrules/core/energy/_score.py
+-rw-r--r--   0        0        0      143 2024-04-30 08:37:43.279924 scoringrules-0.5.0/scoringrules/core/error_spread/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-08 07:26:24.486827 scoringrules-0.5.0/scoringrules/core/error_spread/_gufunc.py
+-rw-r--r--   0        0        0      617 2024-05-08 07:26:24.487217 scoringrules-0.5.0/scoringrules/core/error_spread/_score.py
+-rw-r--r--   0        0        0      677 2024-05-08 07:26:24.487554 scoringrules-0.5.0/scoringrules/core/logarithmic.py
+-rw-r--r--   0        0        0     5609 2024-04-30 08:37:43.285897 scoringrules-0.5.0/scoringrules/core/stats.py
+-rw-r--r--   0        0        0      476 2024-04-30 08:37:43.287370 scoringrules-0.5.0/scoringrules/core/typing.py
+-rw-r--r--   0        0        0     1302 2024-05-08 07:26:24.487885 scoringrules-0.5.0/scoringrules/core/utils.py
+-rw-r--r--   0        0        0      397 2023-11-01 17:12:40.944275 scoringrules-0.5.0/scoringrules/core/variogram/__init__.py
+-rw-r--r--   0        0        0     2777 2024-05-08 07:26:24.488244 scoringrules-0.5.0/scoringrules/core/variogram/_gufuncs.py
+-rw-r--r--   0        0        0     3332 2024-05-08 07:26:24.488585 scoringrules-0.5.0/scoringrules/core/variogram/_score.py
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 scoringrules-0.5.0/PKG-INFO
```

### Comparing `scoringrules-0.4.4/LICENSE` & `scoringrules-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scoringrules-0.4.4/pyproject.toml` & `scoringrules-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scoringrules"
-version = "0.4.4"
+version = "0.5.0"
 description = "Scoring rules for probabilistic forecast evaluation."
 authors = [
   "Francesco Zanetta <zanetta.francesco@gmail.com>",
   "Sam Allen <sam.allen@unibe.ch>",
 ]
 homepage = "https://github.com/frazane/scoringrules"
 documentation = "https://frazane.github.io/scoringrules/"
@@ -15,24 +15,24 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 numpy = "^1.23.4"
 numba = "^0.57.0"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "^1.4.3"
-mkdocs-material = "^9.1.11"
-mkdocstrings = { extras = ["python"], version = "^0.21.2" }
+mkdocs = "^1.5.3"
+mkdocs-material = "^9.5.3"
+mkdocstrings = { extras = ["python"], version = "^0.24.0" }
 jupyter = "^1.0.0"
 nbconvert = "7.3.1"
 ipykernel = "6.22.0"
 properscoring = "^0.1"
 matplotlib = "^3.7.1"
-mkdocs-bibtex = "^2.8.16"
-mkdocs-section-index = "^0.3.5"
+mkdocs-bibtex = "^2.11.0"
+mkdocs-section-index = "^0.3.8"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.265"
 black = "^23.3.0"
 pre-commit = "^3.3.1"
 pytest = "^7.3.1"
```

### Comparing `scoringrules-0.4.4/scoringrules/__init__.py` & `scoringrules-0.5.0/scoringrules/__init__.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.4.4/scoringrules/_brier.py` & `scoringrules-0.5.0/scoringrules/_brier.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from scoringrules.core import brier
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, ArrayLike, Backend
 
 
 def brier_score(
-    forecasts: "ArrayLike",
     observations: "ArrayLike",
+    forecasts: "ArrayLike",
     /,
     *,
     backend: "Backend" = None,
 ) -> "Array":
     r"""
     Compute the Brier Score (BS).
 
@@ -20,18 +20,18 @@
 
     $$BS(f, y) = (f - y)^2,$$
 
     where $f \in [0, 1]$ is the predicted probability of an event and $y \in \{0, 1\}$ the actual outcome.
 
     Parameters
     ----------
-    forecasts : NDArray
-        Forecasted probabilities between 0 and 1.
     observations: NDArray
         Observed outcome, either 0 or 1.
+    forecasts : NDArray
+        Forecasted probabilities between 0 and 1.
     backend: str
         The name of the backend used for computations. Defaults to 'numpy'.
 
     Returns
     -------
     brier_score : NDArray
         The computed Brier Score.
```

### Comparing `scoringrules-0.4.4/scoringrules/_crps.py` & `scoringrules-0.5.0/scoringrules/_crps.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 from scoringrules.core import crps
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, ArrayLike, Backend
 
 
 def crps_ensemble(
-    forecasts: "Array",
     observations: "ArrayLike",
+    forecasts: "Array",
     /,
     axis: int = -1,
     *,
     sorted_ensemble: bool = False,
     estimator: str = "pwm",
     backend: "Backend" = None,
 ) -> "Array":
     r"""Estimate the Continuous Ranked Probability Score (CRPS) for a finite ensemble.
 
     Parameters
     ----------
+    observations: ArrayLike
+        The observed values.
     forecasts: ArrayLike
         The predicted forecast ensemble, where the ensemble dimension is by default
         represented by the last axis.
-    observations: ArrayLike
-        The observed values.
     axis: int
         The axis corresponding to the ensemble. Default is the last axis.
     sorted_ensemble: bool
         Boolean indicating whether the ensemble members are already in ascending order.
         Default is False.
     estimator: str
         Indicates the CRPS estimator to be used.
@@ -43,37 +43,37 @@
 
     Examples
     --------
     >>> from scoringrules import crps
     >>> crps.ensemble(pred, obs)
     """
     B = backends.active if backend is None else backends[backend]
-    forecasts, observations = map(B.asarray, (forecasts, observations))
+    observations, forecasts = map(B.asarray, (observations, forecasts))
 
     if estimator not in crps.estimator_gufuncs:
         raise ValueError(
             f"{estimator} is not a valid estimator. "
             f"Must be one of {crps.estimator_gufuncs.keys()}"
         )
 
     if axis != -1:
         forecasts = B.moveaxis(forecasts, axis, -1)
 
     if not sorted_ensemble and estimator not in ["nrg", "akr", "akr_circperm", "fair"]:
         forecasts = B.sort(forecasts, axis=-1)
 
     if backend == "numba":
-        return crps.estimator_gufuncs[estimator](forecasts, observations)
+        return crps.estimator_gufuncs[estimator](observations, forecasts)
 
-    return crps.ensemble(forecasts, observations, estimator, backend=backend)
+    return crps.ensemble(observations, forecasts, estimator, backend=backend)
 
 
 def twcrps_ensemble(
-    forecasts: "Array",
     observations: "ArrayLike",
+    forecasts: "Array",
     v_func: tp.Callable[["ArrayLike"], "ArrayLike"],
     /,
     axis: int = -1,
     *,
     estimator: str = "pwm",
     sorted_ensemble: bool = False,
     backend: "Backend" = None,
@@ -87,23 +87,23 @@
 
     where $F_{ens}(x) = \sum_{m=1}^{M} 1 \{ x_{m} \leq x \}/M$ is the empirical
     distribution function associated with an ensemble forecast $x_{1}, \dots, x_{M}$ with
     $M$ members, and $v$ is the chaining function used to target particular outcomes.
 
     Parameters
     ----------
+    observations: ArrayLike
+        The observed values.
     forecasts: ArrayLike
         The predicted forecast ensemble, where the ensemble dimension is by default
         represented by the last axis.
-    observations: ArrayLike
-        The observed values.
     v_func: tp.Callable
         Chaining function used to emphasise particular outcomes. For example, a function that
         only considers values above a certain threshold $t$ by projecting forecasts and observations
-        to $\[t, \inf)$.
+        to $[t, \inf)$.
     axis: int
         The axis corresponding to the ensemble. Default is the last axis.
     backend: str
         The name of the backend used for computations. Defaults to 'numba' if available, else 'numpy'.
 
     Returns
     -------
@@ -111,28 +111,28 @@
         The twCRPS between the forecast ensemble and obs for the chosen chaining function.
 
     Examples
     --------
     >>> from scoringrules import crps
     >>> twcrps.ensemble(pred, obs)
     """
-    forecasts, observations = map(v_func, (forecasts, observations))
+    observations, forecasts = map(v_func, (observations, forecasts))
     return crps_ensemble(
-        forecasts,
         observations,
+        forecasts,
         axis=axis,
         sorted_ensemble=sorted_ensemble,
         estimator=estimator,
         backend=backend,
     )
 
 
 def owcrps_ensemble(
-    forecasts: "Array",
     observations: "ArrayLike",
+    forecasts: "Array",
     w_func: tp.Callable[["ArrayLike"], "ArrayLike"],
     /,
     axis: int = -1,
     *,
     estimator: tp.Literal["nrg"] = "nrg",
     backend: "Backend" = None,
 ) -> "Array":
@@ -145,19 +145,19 @@
 
     where $F_{ens}(x) = \sum_{m=1}^{M} 1\{ x_{m} \leq x \}/M$ is the empirical
     distribution function associated with an ensemble forecast $x_{1}, \dots, x_{M}$ with
     $M$ members, $w$ is the chosen weight function, and $\bar{w} = \sum_{m=1}^{M}w(x_{m})/M$.
 
     Parameters
     ----------
+    observations: ArrayLike
+        The observed values.
     forecasts: ArrayLike
         The predicted forecast ensemble, where the ensemble dimension is by default
         represented by the last axis.
-    observations: ArrayLike
-        The observed values.
     w_func: tp.Callable
         Weight function used to emphasise particular outcomes.
     axis: int
         The axis corresponding to the ensemble. Default is the last axis.
     backend: str
         The name of the backend used for computations. Defaults to 'numba' if available, else 'numpy'.
 
@@ -177,32 +177,32 @@
         raise ValueError(
             "Only the energy form of the estimator is available "
             "for the outcome-weighted CRPS."
         )
     if axis != -1:
         forecasts = B.moveaxis(forecasts, axis, -1)
 
-    fcts_weights, obs_weights = map(w_func, (forecasts, observations))
+    obs_weights, fct_weights = map(w_func, (observations, forecasts))
 
     if backend == "numba":
         return crps.estimator_gufuncs["ow" + estimator](
-            forecasts, observations, fcts_weights, obs_weights
+            observations, forecasts, obs_weights, fct_weights
         )
 
-    forecasts, observations, fcts_weights, obs_weights = map(
-        B.asarray, (forecasts, observations, fcts_weights, obs_weights)
+    observations, forecasts, obs_weights, fct_weights = map(
+        B.asarray, (observations, forecasts, obs_weights, fct_weights)
     )
     return crps.ow_ensemble(
-        forecasts, observations, fcts_weights, obs_weights, backend=backend
+        observations, forecasts, obs_weights, fct_weights, backend=backend
     )
 
 
 def vrcrps_ensemble(
-    forecasts: "Array",
     observations: "ArrayLike",
+    forecasts: "Array",
     w_func: tp.Callable[["ArrayLike"], "ArrayLike"],
     /,
     axis: int = -1,
     *,
     estimator: tp.Literal["nrg"] = "nrg",
     backend: "Backend" = None,
 ) -> "Array":
@@ -220,19 +220,19 @@
 
     where $F_{ens}(x) = \sum_{m=1}^{M} 1 \{ x_{m} \leq x \}/M$ is the empirical
     distribution function associated with an ensemble forecast $x_{1}, \dots, x_{M}$ with
     $M$ members, $w$ is the chosen weight function, and $\bar{w} = \sum_{m=1}^{M}w(x_{m})/M$.
 
     Parameters
     ----------
+    observations: ArrayLike
+        The observed values.
     forecasts: ArrayLike
         The predicted forecast ensemble, where the ensemble dimension is by default
         represented by the last axis.
-    observations: ArrayLike
-        The observed values.
     w_func: tp.Callable
         Weight function used to emphasise particular outcomes.
     axis: int
         The axis corresponding to the ensemble. Default is the last axis.
     backend: str
         The name of the backend used for computations. Defaults to 'numba' if available, else 'numpy'.
 
@@ -252,33 +252,33 @@
         raise ValueError(
             "Only the energy form of the estimator is available "
             "for the outcome-weighted CRPS."
         )
     if axis != -1:
         forecasts = B.moveaxis(forecasts, axis, -1)
 
-    fcts_weights, obs_weights = map(w_func, (forecasts, observations))
+    obs_weights, fct_weights = map(w_func, (observations, forecasts))
 
     if backend == "numba":
         return crps.estimator_gufuncs["vr" + estimator](
-            forecasts, observations, fcts_weights, obs_weights
+            observations, forecasts, obs_weights, fct_weights
         )
 
-    forecasts, observations, fcts_weights, obs_weights = map(
-        B.asarray, (forecasts, observations, fcts_weights, obs_weights)
+    observations, forecasts, obs_weights, fct_weights = map(
+        B.asarray, (observations, forecasts, obs_weights, fct_weights)
     )
     return crps.vr_ensemble(
-        forecasts, observations, fcts_weights, obs_weights, backend=backend
+        observations, forecasts, obs_weights, fct_weights, backend=backend
     )
 
 
 def crps_normal(
+    observation: "ArrayLike",
     mu: "ArrayLike",
     sigma: "ArrayLike",
-    observation: "ArrayLike",
     /,
     *,
     backend: "Backend" = None,
 ) -> "ArrayLike":
     r"""Compute the closed form of the CRPS for the normal distribution.
 
     It is based on the following formulation from
@@ -287,82 +287,81 @@
     $$ \mathrm{CRPS}(\mathcal{N}(\mu, \sigma), y) = \sigma \Bigl\{ \omega [\Phi(ω) - 1] + 2 \phi(\omega) - \frac{1}{\sqrt{\pi}} \Bigl\},$$
 
     where $\Phi(ω)$ and $\phi(ω)$ are respectively the CDF and PDF of the standard normal
     distribution at the normalized prediction error $\omega = \frac{y - \mu}{\sigma}$.
 
     Parameters
     ----------
+    observations: ArrayLike
+        The observed values.
     mu: ArrayLike
         Mean of the forecast normal distribution.
     sigma: ArrayLike
         Standard deviation of the forecast normal distribution.
-    observation: ArrayLike
-        The observed values.
 
     Returns
     -------
     crps: array_like
         The CRPS between Normal(mu, sigma) and obs.
 
     Examples
     --------
     >>> from scoringrules import crps
     >>> crps.normal(0.1, 0.4, 0.0)
     """
-    return crps.normal(mu, sigma, observation, backend=backend)
+    return crps.normal(observation, mu, sigma, backend=backend)
 
 
 def crps_lognormal(
+    observation: "ArrayLike",
     mulog: "ArrayLike",
     sigmalog: "ArrayLike",
-    observation: "ArrayLike",
     backend: "Backend" = None,
 ) -> "ArrayLike":
     r"""Compute the closed form of the CRPS for the lognormal distribution.
 
     It is based on the formulation introduced by
     [Baran and Lerch (2015)](https://rmets.onlinelibrary.wiley.com/doi/full/10.1002/qj.2521)
 
     $$ \mathrm{CRPS}(\mathrm{log}\mathcal{N}(\mu, \sigma), y) =
     y [2 \Phi(y) - 1] - 2 \mathrm{exp}(\mu + \frac{\sigma^2}{2})
     \left[ \Phi(\omega - \sigma) + \Phi(\frac{\sigma}{\sqrt{2}}) \right]$$
 
     where $\Phi$ is the CDF of the standard normal distribution and
     $\omega = \frac{\mathrm{log}y - \mu}{\sigma}$.
 
+    Note that mean and standard deviation are not the values for the distribution itself,
+    but of the underlying normal distribution it is derived from.
 
     Parameters
     ----------
+    observations: ArrayLike
+        The observed values.
     mulog: ArrayLike
         Mean of the normal underlying distribution.
     sigmalog: ArrayLike
         Standard deviation of the underlying normal distribution.
 
     Returns
     -------
     crps: ArrayLike
         The CRPS between Lognormal(mu, sigma) and obs.
 
-    Notes
-    -----
-    The mean and standard deviation are not the values for the distribution itself,
-    but of the underlying normal distribution it is derived from.
-
     Examples
     --------
     >>> from scoringrules import crps
     >>> crps.lognormal(0.1, 0.4, 0.0)
     """
-    return crps.lognormal(mulog, sigmalog, observation, backend=backend)
+    return crps.lognormal(observation, mulog, sigmalog, backend=backend)
 
 
 def crps_logistic(
+    observation: "ArrayLike",
     mu: "ArrayLike",
     sigma: "ArrayLike",
-    observation: "ArrayLike",
     /,
     *,
     backend: "Backend" = None,
 ) -> "ArrayLike":
     r"""Compute the closed form of the CRPS for the logistic distribution.
 
     It is based on the following formulation from
@@ -371,32 +370,32 @@
     $$ \mathrm{CRPS}(\mathcal{L}(\mu, \sigma), y) = \sigma \left\{ \omega - 2 \log F(\omega) - 1 \right\}, $$
 
     where $F(\omega)$ is the CDF of the standard logistic distribution at the
     normalized prediction error $\omega = \frac{y - \mu}{\sigma}$.
 
     Parameters
     ----------
+    observations: ArrayLike
+        Observed values.
     mu: ArrayLike
         Location parameter of the forecast logistic distribution.
     sigma: ArrayLike
         Scale parameter of the forecast logistic distribution.
-    observation: ArrayLike
-        Observed values.
 
     Returns
     -------
     crps: array_like
         The CRPS for the Logistic(mu, sigma) forecasts given the observations.
 
     Examples
     --------
     >>> from scoringrules import crps
     >>> crps.logistic(0.1, 0.4, 0.0)
     """
-    return crps.logistic(mu, sigma, observation, backend=backend)
+    return crps.logistic(observation, mu, sigma, backend=backend)
 
 
 __all__ = [
     "crps_ensemble",
     "twcrps_ensemble",
     "owcrps_ensemble",
     "vrcrps_ensemble",
```

### Comparing `scoringrules-0.4.4/scoringrules/_energy.py` & `scoringrules-0.5.0/scoringrules/_energy.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,67 +5,67 @@
 from scoringrules.core.utils import multivariate_array_check
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, ArrayLike, Backend
 
 
 def energy_score(
-    forecasts: "Array",
     observations: "Array",
+    forecasts: "Array",
     /,
     m_axis: int = -2,
     v_axis: int = -1,
     *,
     backend: "Backend" = None,
 ) -> "Array":
     r"""Compute the Energy Score for a finite multivariate ensemble.
 
     The Energy Score is a multivariate scoring rule expressed as
 
-    $$ES(F, \mathbf{y}) = E_{F} ||\mathbf{X} - \mathbf{y}||
-    - \frac{1}{2}E_{F} ||\mathbf{X} - \mathbf{X'}||,$$
+    $$\text{ES}(F_{ens}, \mathbf{y})= \frac{1}{M} \sum_{m=1}^{M} \| \mathbf{x}_{m} -
+      \mathbf{y} \| - \frac{1}{2 M^{2}} \sum_{m=1}^{M} \sum_{j=1}^{M} \| \mathbf{x}_{m} - \mathbf{x}_{j} \| $$
 
     where $\mathbf{X}$ and $\mathbf{X'}$ are independent samples from $F$
     and $||\cdot||$ is the euclidean norm over the input dimensions (the variables).
 
 
     Parameters
     ----------
+    observations: Array
+        The observed values, where the variables dimension is by default the last axis.
     forecasts: Array
         The predicted forecast ensemble, where the ensemble dimension is by default
         represented by the second last axis and the variables dimension by the last axis.
-    observations: Array
-        The observed values, where the variables dimension is by default the last axis.
     m_axis: int
         The axis corresponding to the ensemble dimension on the forecasts array. Defaults to -2.
     v_axis: int
         The axis corresponding to the variables dimension on the forecasts array (or the observations
         array with an extra dimension on `m_axis`). Defaults to -1.
     backend: str
         The name of the backend used for computations. Defaults to 'numba' if available, else 'numpy'.
 
     Returns
     -------
     energy_score: Array of shape (...)
         The computed Energy Score.
     """
     backend = backend if backend is not None else backends._active
-    forecasts, observations = multivariate_array_check(
-        forecasts, observations, m_axis, v_axis, backend=backend
+    observations, forecasts = multivariate_array_check(
+        observations, forecasts, m_axis, v_axis, backend=backend
     )
 
     if backend == "numba":
-        return energy._energy_score_gufunc(forecasts, observations)
+        return energy._energy_score_gufunc(observations, forecasts)
 
-    return energy.nrg(forecasts, observations, backend=backend)
+    return energy.nrg(observations, forecasts, backend=backend)
 
 
 def twenergy_score(
-    forecasts: "Array",
     observations: "Array",
+    forecasts: "Array",
     v_func: tp.Callable[["ArrayLike"], "ArrayLike"],
     /,
     m_axis: int = -2,
     v_axis: int = -1,
     *,
     backend: "Backend" = None,
 ) -> "Array":
@@ -81,42 +81,42 @@
     where $F_{ens}$ is the ensemble forecast $\mathbf{x}_{1}, \dots, \mathbf{x}_{M}$ with
     $M$ members, $\| \cdotp \|$ is the Euclidean distance, and $v$ is the chaining function
     used to target particular outcomes.
 
 
     Parameters
     ----------
+    observations: ArrayLike of shape (...,D)
+        The observed values, where the variables dimension is by default the last axis.
     forecasts: ArrayLike of shape (..., M, D)
         The predicted forecast ensemble, where the ensemble dimension is by default
         represented by the second last axis and the variables dimension by the last axis.
-    observations: ArrayLike of shape (...,D)
-        The observed values, where the variables dimension is by default the last axis.
     v_func: tp.Callable
         Chaining function used to emphasise particular outcomes.
     m_axis: int
         The axis corresponding to the ensemble dimension. Defaults to -2.
     v_axis: int or tuple(int)
         The axis corresponding to the variables dimension. Defaults to -1.
     backend: str
         The name of the backend used for computations. Defaults to 'numba' if available, else 'numpy'.
 
     Returns
     -------
     twenergy_score: ArrayLike of shape (...)
         The computed Threshold-Weighted Energy Score.
     """
-    forecasts, observations = map(v_func, (forecasts, observations))
+    observations, forecasts = map(v_func, (observations, forecasts))
     return energy_score(
-        forecasts, observations, m_axis=m_axis, v_axis=v_axis, backend=backend
+        observations, forecasts, m_axis=m_axis, v_axis=v_axis, backend=backend
     )
 
 
 def owenergy_score(
-    forecasts: "Array",
     observations: "Array",
+    forecasts: "Array",
     w_func: tp.Callable[["ArrayLike"], "ArrayLike"],
     /,
     m_axis: int = -2,
     v_axis: int = -1,
     *,
     backend: "Backend" = None,
 ) -> "Array":
@@ -132,19 +132,19 @@
     where $F_{ens}$ is the ensemble forecast $\mathbf{x}_{1}, \dots, \mathbf{x}_{M}$ with
     $M$ members, $\| \cdotp \|$ is the Euclidean distance, $w$ is the chosen weight function,
     and $\bar{w} = \sum_{m=1}^{M}w(\mathbf{x}_{m})/M$.
 
 
     Parameters
     ----------
+    observations: ArrayLike of shape (...,D)
+        The observed values, where the variables dimension is by default the last axis.
     forecasts: ArrayLike of shape (..., M, D)
         The predicted forecast ensemble, where the ensemble dimension is by default
         represented by the second last axis and the variables dimension by the last axis.
-    observations: ArrayLike of shape (...,D)
-        The observed values, where the variables dimension is by default the last axis.
     w_func: tp.Callable
         Weight function used to emphasise particular outcomes.
     m_axis: int
         The axis corresponding to the ensemble dimension. Defaults to -2.
     v_axis: int or tuple(int)
         The axis corresponding to the variables dimension. Defaults to -1.
     backend: str
@@ -153,34 +153,34 @@
     Returns
     -------
     owenergy_score: ArrayLike of shape (...)
         The computed Outcome-Weighted Energy Score.
     """
     B = backends.active if backend is None else backends[backend]
 
-    forecasts, observations = multivariate_array_check(
-        forecasts, observations, m_axis, v_axis, backend=backend
+    observations, forecasts = multivariate_array_check(
+        observations, forecasts, m_axis, v_axis, backend=backend
     )
 
-    fcts_weights = B.apply_along_axis(w_func, forecasts, -1)
+    fct_weights = B.apply_along_axis(w_func, forecasts, -1)
     obs_weights = B.apply_along_axis(w_func, observations, -1)
 
-    if backend == "numba":
+    if B.name == "numba":
         return energy._owenergy_score_gufunc(
-            forecasts, observations, fcts_weights, obs_weights
+            observations, forecasts, obs_weights, fct_weights
         )
 
     return energy.ownrg(
-        forecasts, observations, fcts_weights, obs_weights, backend=backend
+        observations, forecasts, obs_weights, fct_weights, backend=backend
     )
 
 
 def vrenergy_score(
-    forecasts: "Array",
     observations: "Array",
+    forecasts: "Array",
     w_func: tp.Callable[["ArrayLike"], "ArrayLike"],
     /,
     *,
     m_axis: int = -2,
     v_axis: int = -1,
     backend: "Backend" = None,
 ) -> "Array":
@@ -198,19 +198,19 @@
 
     where $F_{ens}$ is the ensemble forecast $\mathbf{x}_{1}, \dots, \mathbf{x}_{M}$ with
     $M$ members, and $v$ is the chaining function used to target particular outcomes.
 
 
     Parameters
     ----------
+    observations: ArrayLike of shape (...,D)
+        The observed values, where the variables dimension is by default the last axis.
     forecasts: ArrayLike of shape (..., M, D)
         The predicted forecast ensemble, where the ensemble dimension is by default
         represented by the second last axis and the variables dimension by the last axis.
-    observations: ArrayLike of shape (...,D)
-        The observed values, where the variables dimension is by default the last axis.
     w_func: tp.Callable
         Weight function used to emphasise particular outcomes.
     m_axis: int
         The axis corresponding to the ensemble dimension. Defaults to -2.
     v_axis: int or tuple(int)
         The axis corresponding to the variables dimension. Defaults to -1.
     backend: str
@@ -219,22 +219,22 @@
     Returns
     -------
     vrenergy_score: ArrayLike of shape (...)
         The computed Vertically Re-scaled Energy Score.
     """
     B = backends.active if backend is None else backends[backend]
 
-    forecasts, observations = multivariate_array_check(
-        forecasts, observations, m_axis, v_axis, backend=backend
+    observations, forecasts = multivariate_array_check(
+        observations, forecasts, m_axis, v_axis, backend=backend
     )
 
-    fcts_weights = B.apply_along_axis(w_func, forecasts, -1)
+    fct_weights = B.apply_along_axis(w_func, forecasts, -1)
     obs_weights = B.apply_along_axis(w_func, observations, -1)
 
     if backend == "numba":
         return energy._vrenergy_score_gufunc(
-            forecasts, observations, fcts_weights, obs_weights
+            observations, forecasts, obs_weights, fct_weights
         )
 
     return energy.vrnrg(
-        forecasts, observations, fcts_weights, obs_weights, backend=backend
+        observations, forecasts, obs_weights, fct_weights, backend=backend
     )
```

### Comparing `scoringrules-0.4.4/scoringrules/_logs.py` & `scoringrules-0.5.0/scoringrules/_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 from scoringrules.core import logarithmic
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, ArrayLike, Backend
 
 
 def logs_normal(
+    observation: "ArrayLike",
     mu: "ArrayLike",
     sigma: "ArrayLike",
-    observation: "ArrayLike",
     /,
     *,
     negative: bool = True,
     backend: "Backend" = None,
 ) -> "Array":
     r"""Compute the logarithmic score (LS) for the normal distribution.
 
     This score is equivalent to the negative log likelihood (if `negative = True`)
 
     Parameters
     ----------
+    observations: ArrayLike
+        The observed values.
     mu: ArrayLike
         Mean of the forecast normal distribution.
     sigma: ArrayLike
         Standard deviation of the forecast normal distribution.
-    observation: ArrayLike
-        The observed values.
     backend: str, optional
         The backend used for computations.
 
     Returns
     -------
     ls: array_like
         The LS between Normal(mu, sigma) and obs.
@@ -38,9 +38,9 @@
     Examples
     --------
     >>> import scoringrules as sr
     >>> sr.logs_normal(0.1, 0.4, 0.0)
     >>> 0.033898
     """
     return logarithmic.normal(
-        mu, sigma, observation, negative=negative, backend=backend
+        observation, mu, sigma, negative=negative, backend=backend
     )
```

### Comparing `scoringrules-0.4.4/scoringrules/_variogram.py` & `scoringrules-0.5.0/scoringrules/_variogram.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 from scoringrules.core.utils import multivariate_array_check
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, Backend
 
 
 def variogram_score(
-    forecasts: "Array",
     observations: "Array",
+    forecasts: "Array",
     /,
     m_axis: int = -2,
     v_axis: int = -1,
     *,
     p: float = 1.0,
     backend: "Backend" = None,
 ) -> "Array":
     r"""Compute the Variogram Score for a finite multivariate ensemble.
 
     For a $D$-variate ensemble the Variogram Score
     [(Sheuerer and Hamill, 2015)](https://journals.ametsoc.org/view/journals/mwre/143/4/mwr-d-14-00269.1.xml#bib9)
     of order $p$ is expressed as
 
-    $$VS(F, \mathbf{y}) = \sum_{i,j=1}^{D}(|y_i - y_j|^p - E_F|X_i - X_j|^p)^2 ,$$
+    $$\text{VS}_{p}(F_{ens}, \mathbf{y})= \sum_{i=1}^{d} \sum_{j=1}^{d}
+    \left( \frac{1}{M} \sum_{m=1}^{M} | x_{m,i} - x_{m,j} |^{p} - | y_{i} - y_{j} |^{p} \right)^{2}. $$
 
     where $\mathbf{X}$ and $\mathbf{X'}$ are independently sampled ensembles from from $F$.
 
 
     Parameters
     ----------
     forecasts: Array
@@ -46,27 +47,27 @@
         The name of the backend used for computations. Defaults to 'numba' if available, else 'numpy'.
 
     Returns
     -------
     variogram_score: Array
         The computed Variogram Score.
     """
-    forecasts, observations = multivariate_array_check(
-        forecasts, observations, m_axis, v_axis, backend=backend
+    observations, forecasts = multivariate_array_check(
+        observations, forecasts, m_axis, v_axis, backend=backend
     )
 
     if backend == "numba":
-        return variogram._variogram_score_gufunc(forecasts, observations, p)
+        return variogram._variogram_score_gufunc(observations, forecasts, p)
 
-    return variogram.vs(forecasts, observations, p, backend=backend)
+    return variogram.vs(observations, forecasts, p, backend=backend)
 
 
 def twvariogram_score(
-    forecasts: "Array",
     observations: "Array",
+    forecasts: "Array",
     v_func: tp.Callable,
     /,
     m_axis: int = -2,
     v_axis: int = -1,
     *,
     p: float = 1.0,
     backend: "Backend" = None,
@@ -103,23 +104,23 @@
 
 
     Returns
     -------
     twvariogram_score: ArrayLike of shape (...)
         The computed Threshold-Weighted Variogram Score.
     """
-    forecasts, observations = map(v_func, (forecasts, observations))
+    observations, forecasts = map(v_func, (observations, forecasts))
     return variogram_score(
-        forecasts, observations, m_axis, v_axis, p=p, backend=backend
+        observations, forecasts, m_axis, v_axis, p=p, backend=backend
     )
 
 
 def owvariogram_score(
-    forecasts: "Array",
     observations: "Array",
+    forecasts: "Array",
     w_func: tp.Callable,
     /,
     m_axis: int = -2,
     v_axis: int = -1,
     *,
     p: float = 1.0,
     backend: "Backend" = None,
@@ -160,34 +161,34 @@
     Returns
     -------
     owvariogram_score: ArrayLike of shape (...)
         The computed Outcome-Weighted Variogram Score.
     """
     B = backends.active if backend is None else backends[backend]
 
-    forecasts, observations = multivariate_array_check(
-        forecasts, observations, m_axis, v_axis, backend=backend
+    observations, forecasts = multivariate_array_check(
+        observations, forecasts, m_axis, v_axis, backend=backend
     )
 
-    fcts_weights = B.apply_along_axis(w_func, forecasts, -1)
     obs_weights = B.apply_along_axis(w_func, observations, -1)
+    fct_weights = B.apply_along_axis(w_func, forecasts, -1)
 
     if backend == "numba":
         return variogram._owvariogram_score_gufunc(
-            forecasts, observations, p, fcts_weights, obs_weights
+            observations, forecasts, p, obs_weights, fct_weights
         )
 
     return variogram.owvs(
-        forecasts, observations, fcts_weights, obs_weights, p=p, backend=backend
+        observations, forecasts, obs_weights, fct_weights, p=p, backend=backend
     )
 
 
 def vrvariogram_score(
-    forecasts: "Array",
     observations: "Array",
+    forecasts: "Array",
     w_func: tp.Callable,
     /,
     m_axis: int = -2,
     v_axis: int = -1,
     *,
     p: float = 1.0,
     backend: "Backend" = None,
@@ -206,19 +207,19 @@
     \]
 
     where $F_{ens}$ is the ensemble forecast $\mathbf{x}_{1}, \dots, \mathbf{x}_{M}$ with
     $M$ members, $w$ is the chosen weight function, and $\bar{w} = \sum_{m=1}^{M}w(\mathbf{x}_{m})/M$.
 
     Parameters
     ----------
+    observations: Array
+        The observed values, where the variables dimension is by default the last axis.
     forecasts: Array
         The predicted forecast ensemble, where the ensemble dimension is by default
         represented by the second last axis and the variables dimension by the last axis.
-    observations: Array
-        The observed values, where the variables dimension is by default the last axis.
     p: float
         The order of the Variogram Score. Typical values are 0.5, 1.0 or 2.0. Defaults to 1.0.
     w_func: tp.Callable
         Weight function used to emphasise particular outcomes.
     m_axis: int
         The axis corresponding to the ensemble dimension. Defaults to -2.
     v_axis: int
@@ -229,22 +230,22 @@
     Returns
     -------
     vrvariogram_score: ArrayLike of shape (...)
         The computed Vertically Re-scaled Variogram Score.
     """
     B = backends.active if backend is None else backends[backend]
 
-    forecasts, observations = multivariate_array_check(
-        forecasts, observations, m_axis, v_axis, backend=backend
+    observations, forecasts = multivariate_array_check(
+        observations, forecasts, m_axis, v_axis, backend=backend
     )
 
-    fcts_weights = B.apply_along_axis(w_func, forecasts, -1)
     obs_weights = B.apply_along_axis(w_func, observations, -1)
+    fct_weights = B.apply_along_axis(w_func, forecasts, -1)
 
     if backend == "numba":
         return variogram._vrvariogram_score_gufunc(
-            forecasts, observations, p, fcts_weights, obs_weights
+            observations, forecasts, p, obs_weights, fct_weights
         )
 
     return variogram.vrvs(
-        forecasts, observations, fcts_weights, obs_weights, p=p, backend=backend
+        observations, forecasts, obs_weights, fct_weights, p=p, backend=backend
     )
```

### Comparing `scoringrules-0.4.4/scoringrules/backend/base.py` & `scoringrules-0.5.0/scoringrules/backend/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -170,7 +170,63 @@
         """Return the error function."""
 
     @abc.abstractmethod
     def apply_along_axis(
         self, func1d: tp.Callable[["Array"], "Array"], x: "Array", axis: int
     ) -> "Array":
         """Apply a function along a given axis of the input array."""
+
+    @abc.abstractmethod
+    def floor(self, x: "Array", /) -> "Array":
+        """Calculate the integer component of each element ``x_i`` of the input array ``x``."""
+
+    @abc.abstractmethod
+    def minimum(self, x: "Array", y: "ArrayLike", /) -> "Array":
+        """Calculate the minimum of each element ``x_i`` of the input array ``x`` with the value ``y``."""
+
+    @abc.abstractmethod
+    def maximum(self, x: "Array", y: "ArrayLike", /) -> "Array":
+        """Calculate the maximum of each element ``x_i`` of the input array ``x`` with the value ``y``."""
+
+    @abc.abstractmethod
+    def beta(self, x: "Array", y: "Array", /) -> "Array":
+        """Calculate the beta function at each element ``x_i`` of the input array ``x``."""
+
+    @abc.abstractmethod
+    def betainc(self, x: "Array", y: "Array", z: "Array", /) -> "Array":
+        """Calculate the regularised incomplete beta function at each element ``x_i`` of the input array ``x``."""
+
+    @abc.abstractmethod
+    def mbessel0(self, x: "Array", /) -> "Array":
+        """Calculate the modified Bessel function of the first kind of order 0 at each element ``x_i`` of the input array ``x``."""
+
+    @abc.abstractmethod
+    def mbessel1(self, x: "Array", /) -> "Array":
+        """Calculate the modified Bessel function of the first kind of order 1 at each element ``x_i`` of the input array ``x``."""
+
+    @abc.abstractmethod
+    def gamma(self, x: "Array", /) -> "Array":
+        """Calculate the gamma function at each element ``x_i`` of the input array ``x``."""
+
+    @abc.abstractmethod
+    def gammalinc(self, x: "Array", y: "Array", /) -> "Array":
+        """Calculate the lower incomplete gamma function at each element ``x_i`` of the input array ``x``."""
+
+    @abc.abstractmethod
+    def gammauinc(self, x: "Array", y: "Array", /) -> "Array":
+        """Calculate the upper incomplete gamma function at each element ``x_i`` of the input array ``x``."""
+
+    @abc.abstractmethod
+    def factorial(self, n: "ArrayLike", /) -> "ArrayLike":
+        """Calculate the factorial of the integer ``n``."""
+
+    @abc.abstractmethod
+    def hypergeometric(self, a: "Array", b: "Array", c: "Array", z: "Array") -> "Array":
+        """Calculate the hypergeometric function at each element of the inputs ``a``, ``b``, ``c``, and ``z``."""
+
+    @abc.abstractmethod
+    def comb(self, n: "ArrayLike", k: "ArrayLike", /) -> "ArrayLike":
+        """Calculate ``n`` choose ``k``."""
+
+    @abc.abstractmethod
+    def expi(self, x: "Array", /) -> "Array":
+        """Calculate the exponential integral at each element ``x_i`` of the input array ``x``."""
```

### Comparing `scoringrules-0.4.4/scoringrules/backend/jax.py` & `scoringrules-0.5.0/scoringrules/backend/jax.py`

 * *Files 17% similar despite different names*

```diff
@@ -159,11 +159,53 @@
     ):
         try:
             x_shape = list(x.shape)
             return jax.vmap(func1d)(x.reshape(-1, x_shape.pop(axis))).reshape(x_shape)
         except Exception:
             return jnp.apply_along_axis(func1d, axis, x)
 
+    def floor(self, x: "Array") -> "Array":
+        return jnp.floor(x)
+
+    def minimum(self, x: "Array", y: "ArrayLike") -> "Array":
+        return jnp.minimum(x, y)
+
+    def maximum(self, x: "Array", y: "ArrayLike") -> "Array":
+        return jnp.maximum(x, y)
+
+    def beta(self, x: "Array", y: "Array") -> "Array":
+        return jsp.special.beta(x, y)
+
+    def betainc(self, x: "Array", y: "Array", z: "Array") -> "Array":
+        return jsp.special.betainc(x, y, z)
+
+    def mbessel0(self, x: "Array") -> "Array":
+        return jsp.special.jv(0, x)
+
+    def mbessel1(self, x: "Array") -> "Array":
+        return jsp.special.jv(1, x)
+
+    def gamma(self, x: "Array") -> "Array":
+        return jsp.special.gamma(x)
+
+    def gammalinc(self, x: "Array", y: "Array") -> "Array":
+        return jsp.special.gammainc(x, y) * jsp.special.gamma(x)
+
+    def gammauinc(self, x: "Array", y: "Array") -> "Array":
+        return jsp.special.gammaincc(x, y) * jsp.special.gamma(x)
+
+    def factorial(self, n: "ArrayLike") -> "ArrayLike":
+        return jsp.special.factorial(n)
+
+    def hypergeometric(self, a: "Array", b: "Array", c: "Array", z: "Array"):
+        return jsp.special.hyp2f1(a, b, c, z)
+
+    def comb(self, n: "ArrayLike", k: "ArrayLike") -> "ArrayLike":
+        return jsp.special.comb(n, k)
+
+    def expi(self, x: "Array") -> "Array":
+        return jsp.special.expi(x)
+
 
 if __name__ == "__main__":
     B = JaxBackend()
     out = B.mean(jnp.ones(10))
```

### Comparing `scoringrules-0.4.4/scoringrules/backend/registry.py` & `scoringrules-0.5.0/scoringrules/backend/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import typing as tp
 from importlib.util import find_spec
 
 from .base import ArrayBackend
 from .jax import JaxBackend
-from .numpy import NumpyBackend
+from .numpy import NumbaBackend, NumpyBackend
 from .tensorflow import TensorflowBackend
 from .torch import TorchBackend
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Backend
 
 _ALL_BACKENDS_MAP = {
     "jax": JaxBackend,
     "numpy": NumpyBackend,
     "torch": TorchBackend,
     "tensorflow": TensorflowBackend,
-    "numba": NumpyBackend,
+    "numba": NumbaBackend,
 }
 
 try:
     import numba  # noqa: F401
 
     _NUMBA_IMPORTED = True
 except ImportError:
```

### Comparing `scoringrules-0.4.4/scoringrules/backend/torch.py` & `scoringrules-0.5.0/scoringrules/backend/tensorflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,182 +1,253 @@
+import math
 import typing as tp
 from importlib import import_module
 
 from .base import ArrayBackend
 
 if tp.TYPE_CHECKING:
-    import torch
+    import tensorflow as tf
 
-    Tensor = torch.Tensor
+    Tensor = tf.Tensor
     TensorLike = Tensor | bool | float | int
+    DTYPE = tf.float32
 else:
-    torch = None
+    tf = None
+    DTYPE = None
 Dtype = tp.TypeVar("Dtype")
 
 
-class TorchBackend(ArrayBackend):
-    """Torch backend."""
+class TensorflowBackend(ArrayBackend):
+    """Tensorflow backend."""
 
-    name = "torch"
+    name = "tensorflow"
 
     def __init__(self) -> None:
-        global torch
-        if torch is None and not tp.TYPE_CHECKING:
-            torch = import_module("torch")
-
-        self.pi = torch.asarray(torch.pi)
+        global tf, DTYPE
+        if tf is None and not tp.TYPE_CHECKING:
+            tf = import_module("tensorflow")
+            DTYPE = tf.float32
+        self.pi = tf.constant(math.pi, dtype=DTYPE)
 
     def asarray(
         self,
         obj: "TensorLike",
         /,
         *,
         dtype: Dtype | None = None,
     ) -> "Tensor":
-        return torch.asarray(obj, dtype=dtype)
+        if dtype is None:
+            dtype = DTYPE
+        return tf.convert_to_tensor(obj, dtype=dtype)
 
     def mean(
         self,
         x: "Tensor",
         /,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
     ) -> "Tensor":
-        return torch.mean(x, axis=axis, keepdim=keepdims)
+        return tf.math.reduce_mean(x, axis=axis, keepdims=keepdims)
 
     def moveaxis(
         self,
         x: "Tensor",
         /,
         source: tuple[int, ...] | int,
         destination: tuple[int, ...] | int,
     ) -> "Tensor":
-        return torch.moveaxis(x, source, destination)
+        return tf.experimental.numpy.moveaxis(x, source, destination)
 
     def sum(
         self,
         x: "Tensor",
         /,
         axis: int | tuple[int, ...] | None = None,
         *,
         keepdims: bool = False,
     ) -> "Tensor":
-        return torch.sum(x, axis=axis, keepdim=keepdims)
+        return tf.math.reduce_sum(x, axis=axis, keepdims=keepdims)
 
     def unique_values(self, x: "Tensor", /) -> "Tensor":
-        return torch.unique(x)
+        return tf.unique(x)
 
     def concat(
-        self, arrays: tuple["Tensor", ...] | list["Tensor"], /, *, axis: int | None = 0
+        self,
+        arrays: tuple["Tensor", ...] | list["Tensor"],
+        /,
+        *,
+        axis: int | None = 0,
     ) -> "Tensor":
-        return torch.concat(arrays, axis=axis)
+        return tf.concat(arrays, axis=axis)
 
+    # tf.expand_dims() doesn't support tuples in v2.15
     def expand_dims(self, x: "Tensor", /, axis: int | tuple[int] = 0) -> "Tensor":
         if isinstance(axis, int):
-            return torch.unsqueeze(x, dim=axis)
+            return tf.expand_dims(x, axis=axis)
         elif isinstance(axis, tuple | list):
             out_ndim = len(axis) + x.ndim
             axis = [a + out_ndim if a < 0 else a for a in axis]
             shape_it = iter(x.shape)
             shape = [1 if ax in axis else next(shape_it) for ax in range(out_ndim)]
-            return x.reshape(shape)
+            return tf.reshape(x, shape=shape)
 
     def squeeze(
         self, x: "Tensor", /, *, axis: int | tuple[int, ...] | None = None
     ) -> "Tensor":
-        return torch.squeeze(x, dim=() if axis is None else axis)
+        return tf.squeeze(x, axis=axis)
 
     def stack(
         self, arrays: tuple["Tensor", ...] | list["Tensor"], /, *, axis: int = 0
     ) -> "Tensor":
-        return torch.stack(arrays, dim=axis)
+        return tf.stack(arrays, axis=axis)
 
     def arange(
         self,
         start: int | float,
         /,
         stop: int | float | None = None,
         step: int | float = 1,
         *,
         dtype: Dtype | None = None,
     ) -> "Tensor":
-        return torch.arange(start)  # TODO: fix this
+        if dtype is None:
+            dtype = DTYPE
+        return tf.range(start, stop, step, dtype=dtype)
 
     def zeros(
         self,
         shape: int | tuple[int, ...],
         *,
         dtype: Dtype | None = None,
     ) -> "Tensor":
-        return torch.zeros(shape, dtype=dtype)
+        if dtype is None:
+            dtype = DTYPE
+        return tf.zeros(shape, dtype=dtype)
 
     def abs(self, x: "Tensor") -> "Tensor":
-        return torch.abs(x)
+        return tf.math.abs(x)
 
     def exp(self, x: "Tensor") -> "Tensor":
-        return torch.exp(x)
+        return tf.math.exp(x)
 
-    def isnan(self, x: "Tensor") -> "Tensor":
-        return torch.isnan(x)
+    def isnan(
+        self,
+        x: "Tensor",
+        *,
+        dtype: Dtype | None = None,
+    ) -> "Tensor":
+        if dtype is None:
+            dtype = DTYPE
+        return tf.cast(tf.math.is_nan(x), dtype=dtype)
 
     def log(self, x: "Tensor") -> "Tensor":
-        return torch.log(x)
+        return tf.math.log(x)
 
     def sqrt(self, x: "Tensor") -> "Tensor":
-        return torch.sqrt(torch.asarray(x))
+        return tf.math.sqrt(x)
 
     def any(
         self,
         x: "Tensor",
         /,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
+        dtype: Dtype | None = None,
     ) -> "Tensor":
-        return torch.any(x, dim=axis, keepdim=keepdims)
+        if dtype is None:
+            dtype = DTYPE
+        return tf.cast(tf.math.reduce_any(x, axis=axis, keepdims=keepdims), dtype=dtype)
 
     def all(
         self,
         x: "Tensor",
         /,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
+        dtype: Dtype | None = None,
     ) -> "Tensor":
-        if axis is None:
-            return torch.all(x)
-        else:
-            return torch.all(x, dim=axis, keepdim=keepdims)
+        if dtype is None:
+            dtype = DTYPE
+        return tf.cast(tf.math.reduce_all(x, axis=axis, keepdims=keepdims), dtype=dtype)
 
     def sort(
         self,
         x: "Tensor",
         /,
         *,
         axis: int = -1,
         descending: bool = False,
-        stable: bool = True,
     ) -> "Tensor":
-        return torch.sort(x, stable=stable, dim=axis, descending=descending)[0]
+        direction = "DESCENDING" if descending else "ASCENDING"
+        return tf.sort(x, axis=axis, direction=direction)
 
     def norm(self, x: "Tensor", axis: int | tuple[int, ...] | None = None) -> "Tensor":
-        return torch.norm(x, dim=axis)
+        return tf.norm(x, axis=axis)
 
     def erf(self, x: "Tensor") -> "Tensor":
-        return torch.special.erf(x)
+        return tf.math.erf(x)
 
     def apply_along_axis(
         self, func1d: tp.Callable[["Tensor"], "Tensor"], x: "Tensor", axis: int
     ):
         try:
-            x_shape = list(x.shape)
-            return torch.vmap(func1d)(x.reshape(-1, x_shape.pop(axis))).reshape(x_shape)
+            x_shape = x.shape.as_list()
+            flat = tf.map_fn(func1d, tf.reshape(x, [-1, x_shape.pop(axis)]))
+            return tf.reshape(flat, x_shape)
         except Exception:
-            return torch.stack(
-                [func1d(x_i) for x_i in torch.unbind(x, dim=axis)], dim=axis
+            return tf.stack(
+                [func1d(x_i) for x_i in tf.unstack(x, axis=axis)], axis=axis
             )
 
+    def floor(self, x: "Tensor") -> "Tensor":
+        return tf.math.floor(x)
+
+    def minimum(self, x: "Tensor", y: "TensorLike") -> "Tensor":
+        return tf.math.minimum(x, y)
+
+    def maximum(self, x: "Tensor", y: "TensorLike") -> "Tensor":
+        return tf.math.maximum(x, y)
+
+    def beta(self, x: "Tensor", y: "Tensor") -> "Tensor":
+        return tf.math.exp(
+            tf.math.lgamma(x) + tf.math.lgamma(y) - tf.math.lgamma(x + y)
+        )
+
+    def betainc(self, x: "Tensor", y: "Tensor", z: "Tensor") -> "Tensor":
+        return tf.math.betainc(x, y, z)
+
+    def mbessel0(self, x: "Tensor") -> "Tensor":
+        return tf.math.bessel_i0e(x)
+
+    def mbessel1(self, x: "Tensor") -> "Tensor":
+        return tf.math.bessel_i1e(x)
+
+    def gamma(self, x: "Tensor") -> "Tensor":
+        return tf.math.exp(tf.math.lgamma(x))
+
+    def gammalinc(self, x: "Tensor", y: "Tensor") -> "Tensor":
+        return tf.math.igamma(x, y) * tf.math.exp(tf.math.lgamma(x))
+
+    def gammauinc(self, x: "Tensor", y: "Tensor") -> "Tensor":
+        return tf.math.igammac(x, y) * tf.math.exp(tf.math.lgamma(x))
+
+    def factorial(self, n: "TensorLike") -> "TensorLike":
+        return tf.math.exp(tf.math.lgamma(n + 1))
+
+    def hypergeometric(
+        self, a: "Tensor", b: "Tensor", c: "Tensor", z: "Tensor"
+    ) -> "Tensor":
+        raise NotImplementedError
+
+    def comb(self, n: "Tensor", k: "Tensor") -> "Tensor":
+        return self.factorial(n) / (self.factorial(k) * self.factorial(n - k))
+
+    def expi(self, x: "Tensor") -> "Tensor":
+        return tf.math.special.expint(x)
+
 
 if __name__ == "__main__":
-    B = TorchBackend()
-    out = B.mean(torch.ones(10))
+    B = TensorflowBackend()
+    out = B.mean(tf.ones(10))
```

### Comparing `scoringrules-0.4.4/scoringrules/core/brier.py` & `scoringrules-0.5.0/scoringrules/core/brier.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, ArrayLike, Backend
 
 EPSILON = 1e-5
 
 
 def brier_score(
-    fcts: "ArrayLike", obs: "ArrayLike", backend: "Backend" = None
+    obs: "ArrayLike", fct: "ArrayLike", backend: "Backend" = None
 ) -> "Array":
     """Compute the Brier Score for predicted probabilities of events."""
     B = backends.active if backend is None else backends[backend]
-    fcts, obs = map(B.asarray, (fcts, obs))
+    obs, fct = map(B.asarray, (obs, fct))
 
-    if B.any(fcts < 0.0) or B.any(fcts > 1.0 + EPSILON):
+    if B.any(fct < 0.0) or B.any(fct > 1.0 + EPSILON):
         raise ValueError("Forecasted probabilities must be within 0 and 1.")
 
     if not set(B.unique_values(obs)) <= {0, 1}:
         raise ValueError("Observations must be 0, 1, or NaN.")
 
-    return B.asarray((fcts - obs) ** 2)
+    return B.asarray((fct - obs) ** 2)
```

### Comparing `scoringrules-0.4.4/scoringrules/core/crps/_approx.py` & `scoringrules-0.5.0/scoringrules/core/crps/_approx.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,104 +3,104 @@
 from scoringrules.backend import backends
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, ArrayLike, Backend
 
 
 def ensemble(
-    fcts: "Array",
     obs: "ArrayLike",
+    fct: "Array",
     estimator: str = "pwm",
     backend: "Backend" = None,
 ) -> "Array":
     """Compute the CRPS for a finite ensemble."""
     if estimator == "nrg":
-        out = _crps_ensemble_nrg(fcts, obs, backend=backend)
+        out = _crps_ensemble_nrg(obs, fct, backend=backend)
     elif estimator == "pwm":
-        out = _crps_ensemble_pwm(fcts, obs, backend=backend)
+        out = _crps_ensemble_pwm(obs, fct, backend=backend)
     elif estimator == "fair":
-        out = _crps_ensemble_fair(fcts, obs, backend=backend)
+        out = _crps_ensemble_fair(obs, fct, backend=backend)
     else:
         raise ValueError(
             f"{estimator} can only be used with `numpy` "
             "backend and needs `numba` to be installed"
         )
 
     return out
 
 
 def _crps_ensemble_fair(
-    fcts: "Array", obs: "Array", backend: "Backend" = None
+    obs: "Array", fct: "Array", backend: "Backend" = None
 ) -> "Array":
     """Fair version of the CRPS estimator based on the energy form."""
     B = backends.active if backend is None else backends[backend]
-    M: int = fcts.shape[-1]
-    e_1 = B.sum(B.abs(obs[..., None] - fcts), axis=-1) / M
+    M: int = fct.shape[-1]
+    e_1 = B.sum(B.abs(obs[..., None] - fct), axis=-1) / M
     e_2 = B.sum(
-        B.abs(fcts[..., None] - fcts[..., None, :]),
+        B.abs(fct[..., None] - fct[..., None, :]),
         axis=(-1, -2),
     ) / (M * (M - 1))
     return e_1 - 0.5 * e_2
 
 
 def _crps_ensemble_nrg(
-    fcts: "Array", obs: "Array", backend: "Backend" = None
+    obs: "Array", fct: "Array", backend: "Backend" = None
 ) -> "Array":
     """CRPS estimator based on the energy form."""
     B = backends.active if backend is None else backends[backend]
-    M: int = fcts.shape[-1]
-    e_1 = B.sum(B.abs(obs[..., None] - fcts), axis=-1) / M
-    e_2 = B.sum(B.abs(fcts[..., None] - fcts[..., None, :]), (-1, -2)) / (M**2)
+    M: int = fct.shape[-1]
+    e_1 = B.sum(B.abs(obs[..., None] - fct), axis=-1) / M
+    e_2 = B.sum(B.abs(fct[..., None] - fct[..., None, :]), (-1, -2)) / (M**2)
     return e_1 - 0.5 * e_2
 
 
 def _crps_ensemble_pwm(
-    fcts: "Array", obs: "Array", backend: "Backend" = None
+    obs: "Array", fct: "Array", backend: "Backend" = None
 ) -> "Array":
     """CRPS estimator based on the probability weighted moment (PWM) form."""
     B = backends.active if backend is None else backends[backend]
-    M: int = fcts.shape[-1]
-    expected_diff = B.sum(B.abs(obs[..., None] - fcts), axis=-1) / M
-    β_0 = B.sum(fcts, axis=-1) / M
-    β_1 = B.sum(fcts * B.arange(M), axis=-1) / (M * (M - 1.0))
+    M: int = fct.shape[-1]
+    expected_diff = B.sum(B.abs(obs[..., None] - fct), axis=-1) / M
+    β_0 = B.sum(fct, axis=-1) / M
+    β_1 = B.sum(fct * B.arange(M), axis=-1) / (M * (M - 1.0))
     return expected_diff + β_0 - 2.0 * β_1
 
 
 def ow_ensemble(
-    fcts: "Array",
     obs: "Array",
-    fw: "Array",
+    fct: "Array",
     ow: "Array",
+    fw: "Array",
     backend: "Backend" = None,
 ) -> "Array":
     """Outcome-Weighted CRPS estimator based on the energy form."""
     B = backends.active if backend is None else backends[backend]
-    M: int = fcts.shape[-1]
+    M: int = fct.shape[-1]
     wbar = B.mean(fw, axis=-1)
-    e_1 = B.sum(B.abs(obs[..., None] - fcts) * fw, axis=-1) * ow / (M * wbar)
+    e_1 = B.sum(B.abs(obs[..., None] - fct) * fw, axis=-1) * ow / (M * wbar)
     e_2 = B.sum(
-        B.abs(fcts[..., None] - fcts[..., None, :]) * fw[..., None] * fw[..., None, :],
+        B.abs(fct[..., None] - fct[..., None, :]) * fw[..., None] * fw[..., None, :],
         axis=(-1, -2),
     )
     e_2 *= ow / (M**2 * wbar**2)
     return e_1 - 0.5 * e_2
 
 
 def vr_ensemble(
-    fcts: "Array",
     obs: "Array",
-    fw: "Array",
+    fct: "Array",
     ow: "Array",
+    fw: "Array",
     backend: "Backend" = None,
 ) -> "Array":
     """Vertically Re-scaled CRPS estimator based on the energy form."""
     B = backends.active if backend is None else backends[backend]
-    M: int = fcts.shape[-1]
-    e_1 = B.sum(B.abs(obs[..., None] - fcts) * fw, axis=-1) * ow / M
+    M: int = fct.shape[-1]
+    e_1 = B.sum(B.abs(obs[..., None] - fct) * fw, axis=-1) * ow / M
     e_2 = B.sum(
-        B.abs(B.expand_dims(fcts, axis=-1) - B.expand_dims(fcts, axis=-2))
+        B.abs(B.expand_dims(fct, axis=-1) - B.expand_dims(fct, axis=-2))
         * (B.expand_dims(fw, axis=-1) * B.expand_dims(fw, axis=-2)),
         axis=(-1, -2),
     ) / (M**2)
-    e_3 = B.mean(B.abs(fcts) * fw, axis=-1) - B.abs(obs) * ow
+    e_3 = B.mean(B.abs(fct) * fw, axis=-1) - B.abs(obs) * ow
     e_3 *= B.mean(fw, axis=1) - ow
     return e_1 - 0.5 * e_2 + e_3
```

### Comparing `scoringrules-0.4.4/scoringrules/core/crps/_closed.py` & `scoringrules-0.5.0/scoringrules/core/crps/_closed.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 from scoringrules.core.stats import _logis_cdf, _norm_cdf, _norm_pdf
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, ArrayLike, Backend
 
 
 def normal(
-    mu: "ArrayLike", sigma: "ArrayLike", obs: "ArrayLike", backend: "Backend" = None
+    obs: "ArrayLike", mu: "ArrayLike", sigma: "ArrayLike", backend: "Backend" = None
 ) -> "Array":
     """Compute the CRPS for the normal distribution."""
     B = backends.active if backend is None else backends[backend]
     mu, sigma, obs = map(B.asarray, (mu, sigma, obs))
     ω = (obs - mu) / sigma
     return sigma * (
         ω * (2.0 * _norm_cdf(ω, backend=backend) - 1.0)
         + 2.0 * _norm_pdf(ω, backend=backend)
         - 1.0 / B.sqrt(B.pi)
     )
 
 
 def lognormal(
+    obs: "ArrayLike",
     mulog: "ArrayLike",
     sigmalog: "ArrayLike",
-    obs: "ArrayLike",
     backend: "Backend" = None,
 ) -> "Array":
     """Compute the CRPS for the lognormal distribution."""
     B = backends.active if backend is None else backends[backend]
     mulog, sigmalog, obs = map(B.asarray, (mulog, sigmalog, obs))
     ω = (B.log(obs) - mulog) / sigmalog
     ex = 2 * B.exp(mulog + sigmalog**2 / 2)
@@ -36,14 +36,14 @@
         _norm_cdf(ω - sigmalog, backend=backend)
         + _norm_cdf(sigmalog / B.sqrt(B.asarray(2.0)), backend=backend)
         - 1
     )
 
 
 def logistic(
-    mu: "ArrayLike", sigma: "ArrayLike", obs: "ArrayLike", backend: "Backend" = None
+    obs: "ArrayLike", mu: "ArrayLike", sigma: "ArrayLike", backend: "Backend" = None
 ) -> "Array":
     """Compute the CRPS for the normal distribution."""
     B = backends.active if backend is None else backends[backend]
     mu, sigma, obs = map(B.asarray, (mu, sigma, obs))
     ω = (obs - mu) / sigma
     return sigma * (ω - 2 * B.log(_logis_cdf(ω, backend=backend)) - 1)
```

### Comparing `scoringrules-0.4.4/scoringrules/core/crps/_gufuncs.py` & `scoringrules-0.5.0/scoringrules/core/crps/_gufuncs.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,33 +8,31 @@
 
 
 @guvectorize(
     [
         "void(float32[:], float32[:], float32[:])",
         "void(float64[:], float64[:], float64[:])",
     ],
-    "(n),()->()",
+    "(),(n)->()",
 )
-def _crps_ensemble_int_gufunc(
-    forecasts: np.ndarray, observation: np.ndarray, out: np.ndarray
-):
+def _crps_ensemble_int_gufunc(obs: np.ndarray, fct: np.ndarray, out: np.ndarray):
     """CRPS estimator based on the integral form."""
-    obs = observation[0]
-    M = forecasts.shape[0]
+    obs = obs[0]
+    M = fct.shape[0]
 
     if np.isnan(obs):
         out[0] = np.nan
         return
 
     obs_cdf = 0
     forecast_cdf = 0.0
     prev_forecast = 0.0
     integral = 0.0
 
-    for n, forecast in enumerate(forecasts):
+    for n, forecast in enumerate(fct):
         if np.isnan(forecast):
             if n == 0:
                 integral = np.nan
             forecast = prev_forecast  # noqa: PLW2901
             break
 
         if obs_cdf == 0 and obs < forecast:
@@ -55,241 +53,231 @@
 
 
 @guvectorize(
     [
         "void(float32[:], float32[:], float32[:])",
         "void(float64[:], float64[:], float64[:])",
     ],
-    "(n),()->()",
+    "(),(n)->()",
 )
-def _crps_ensemble_qd_gufunc(
-    forecasts: np.ndarray, observation: np.ndarray, out: np.ndarray
-):
+def _crps_ensemble_qd_gufunc(obs: np.ndarray, fct: np.ndarray, out: np.ndarray):
     """CRPS estimator based on the quantile decomposition form."""
-    obs = observation[0]
-    M = forecasts.shape[-1]
+    obs = obs[0]
+    M = fct.shape[-1]
 
     if np.isnan(obs):
         out[0] = np.nan
         return
 
     obs_cdf = 0.0
     integral = 0.0
 
-    for i, forecast in enumerate(forecasts):
+    for i, forecast in enumerate(fct):
         if obs < forecast:
             obs_cdf = 1.0
 
         integral += (forecast - obs) * (M * obs_cdf - (i + 1) + 0.5)
 
     out[0] = (2 / M**2) * integral
 
 
 @guvectorize(
     [
         "void(float32[:], float32[:], float32[:])",
         "void(float64[:], float64[:], float64[:])",
     ],
-    "(n),()->()",
+    "(),(n)->()",
 )
-def _crps_ensemble_nrg_gufunc(
-    forecasts: np.ndarray, observation: np.ndarray, out: np.ndarray
-):
+def _crps_ensemble_nrg_gufunc(obs: np.ndarray, fct: np.ndarray, out: np.ndarray):
     """CRPS estimator based on the energy form."""
-    obs = observation[0]
-    M = forecasts.shape[-1]
+    obs = obs[0]
+    M = fct.shape[-1]
 
     if np.isnan(obs):
         out[0] = np.nan
         return
 
     e_1 = 0
     e_2 = 0
 
-    for x_i in forecasts:
+    for x_i in fct:
         e_1 += abs(x_i - obs)
-        for x_j in forecasts:
+        for x_j in fct:
             e_2 += abs(x_i - x_j)
 
     out[0] = e_1 / M - 0.5 * e_2 / (M**2)
 
 
 @guvectorize(
     [
         "void(float32[:], float32[:], float32[:])",
         "void(float64[:], float64[:], float64[:])",
     ],
-    "(n),()->()",
+    "(),(n)->()",
 )
-def _crps_ensemble_fair_gufunc(
-    forecasts: np.ndarray, observation: np.ndarray, out: np.ndarray
-):
+def _crps_ensemble_fair_gufunc(obs: np.ndarray, fct: np.ndarray, out: np.ndarray):
     """Fair version of the CRPS estimator based on the energy form."""
-    obs = observation[0]
-    M = forecasts.shape[-1]
+    obs = obs[0]
+    M = fct.shape[-1]
 
     if np.isnan(obs):
         out[0] = np.nan
         return
 
     e_1 = 0
     e_2 = 0
 
-    for x_i in forecasts:
+    for x_i in fct:
         e_1 += abs(x_i - obs)
-        for x_j in forecasts:
+        for x_j in fct:
             e_2 += abs(x_i - x_j)
 
     out[0] = e_1 / M - 0.5 * e_2 / (M * (M - 1))
 
 
 @guvectorize(
     [
         "void(float32[:], float32[:], float32[:])",
         "void(float64[:], float64[:], float64[:])",
     ],
-    "(n),()->()",
+    "(),(n)->()",
 )
-def _crps_ensemble_pwm_gufunc(
-    forecasts: np.ndarray, observation: np.ndarray, out: np.ndarray
-):
+def _crps_ensemble_pwm_gufunc(obs: np.ndarray, fct: np.ndarray, out: np.ndarray):
     """CRPS estimator based on the probability weighted moment (PWM) form."""
-    obs = observation[0]
-    M = forecasts.shape[-1]
+    obs = obs[0]
+    M = fct.shape[-1]
 
     if np.isnan(obs):
         out[0] = np.nan
         return
 
     expected_diff = 0.0
     β_0 = 0.0
     β_1 = 0.0
 
-    for i, forecast in enumerate(forecasts):
+    for i, forecast in enumerate(fct):
         expected_diff += np.abs(forecast - obs)
         β_0 += forecast
         β_1 += forecast * i
 
     out[0] = expected_diff / M + β_0 / M - 2 * β_1 / (M * (M - 1))
 
 
 @guvectorize(
     [
         "void(float32[:], float32[:], float32[:])",
         "void(float64[:], float64[:], float64[:])",
     ],
-    "(n),()->()",
+    "(),(n)->()",
 )
-def _crps_ensemble_akr_gufunc(
-    forecasts: np.ndarray, observation: np.ndarray, out: np.ndarray
-):
+def _crps_ensemble_akr_gufunc(obs: np.ndarray, fct: np.ndarray, out: np.ndarray):
     """CRPS estimaton based on the approximate kernel representation."""
-    M = forecasts.shape[-1]
-    obs = observation[0]
+    M = fct.shape[-1]
+    obs = obs[0]
     e_1 = 0
     e_2 = 0
-    for i, forecast in enumerate(forecasts):
+    for i, forecast in enumerate(fct):
         if i == 0:
             i = M - 1
         e_1 += abs(forecast - obs)
-        e_2 += abs(forecast - forecasts[i - 1])
+        e_2 += abs(forecast - fct[i - 1])
     out[0] = e_1 / M - 0.5 * 1 / M * e_2
 
 
 @guvectorize(
     [
         "void(float32[:], float32[:], float32[:])",
         "void(float64[:], float64[:], float64[:])",
     ],
-    "(n),()->()",
+    "(),(n)->()",
 )
 def _crps_ensemble_akr_circperm_gufunc(
-    forecasts: np.ndarray, observation: np.ndarray, out: np.ndarray
+    obs: np.ndarray, fct: np.ndarray, out: np.ndarray
 ):
     """CRPS estimaton based on the AKR with cyclic permutation."""
-    M = forecasts.shape[-1]
-    obs = observation[0]
+    M = fct.shape[-1]
+    obs = obs[0]
     e_1 = 0.0
     e_2 = 0.0
-    for i, forecast in enumerate(forecasts):
+    for i, forecast in enumerate(fct):
         sigma_i = int((i + 1 + ((M - 1) / 2)) % M)
         e_1 += abs(forecast - obs)
-        e_2 += abs(forecast - forecasts[sigma_i])
+        e_2 += abs(forecast - fct[sigma_i])
     out[0] = e_1 / M - 0.5 * 1 / M * e_2
 
 
 @guvectorize(
     [
         "void(float32[:], float32[:], float32[:], float32[:], float32[:])",
         "void(float64[:], float64[:], float64[:], float64[:], float64[:])",
     ],
-    "(n),(),(n),()->()",
+    "(),(n),(),(n)->()",
 )
 def _owcrps_ensemble_nrg_gufunc(
-    forecasts: np.ndarray,
-    observation: np.ndarray,
-    fw: np.ndarray,
+    obs: np.ndarray,
+    fct: np.ndarray,
     ow: np.ndarray,
+    fw: np.ndarray,
     out: np.ndarray,
 ):
     """Outcome-weighted CRPS estimator based on the energy form."""
-    obs = observation[0]
+    obs = obs[0]
     ow = ow[0]
-    M = forecasts.shape[-1]
+    M = fct.shape[-1]
 
     if np.isnan(obs):
         out[0] = np.nan
         return
 
     e_1 = 0.0
     e_2 = 0.0
 
-    for i, x_i in enumerate(forecasts):
+    for i, x_i in enumerate(fct):
         e_1 += abs(x_i - obs) * fw[i] * ow
-        for j, x_j in enumerate(forecasts):
+        for j, x_j in enumerate(fct):
             e_2 += abs(x_i - x_j) * fw[i] * fw[j] * ow
 
     wbar = np.mean(fw)
 
     out[0] = e_1 / (M * wbar) - 0.5 * e_2 / ((M * wbar) ** 2)
 
 
 @guvectorize(
     [
         "void(float32[:], float32[:], float32[:], float32[:], float32[:])",
         "void(float64[:], float64[:], float64[:], float64[:], float64[:])",
     ],
-    "(n),(),(n),()->()",
+    "(),(n),(),(n)->()",
 )
 def _vrcrps_ensemble_nrg_gufunc(
-    forecasts: np.ndarray,
-    observation: np.ndarray,
-    fw: np.ndarray,
+    obs: np.ndarray,
+    fct: np.ndarray,
     ow: np.ndarray,
+    fw: np.ndarray,
     out: np.ndarray,
 ):
     """Vertically re-scaled CRPS estimator based on the energy form."""
-    obs = observation[0]
+    obs = obs[0]
     ow = ow[0]
-    M = forecasts.shape[-1]
+    M = fct.shape[-1]
 
     if np.isnan(obs):
         out[0] = np.nan
         return
 
     e_1 = 0.0
     e_2 = 0.0
 
-    for i, x_i in enumerate(forecasts):
+    for i, x_i in enumerate(fct):
         e_1 += abs(x_i - obs) * fw[i] * ow
-        for j, x_j in enumerate(forecasts):
+        for j, x_j in enumerate(fct):
             e_2 += abs(x_i - x_j) * fw[i] * fw[j]
 
     wbar = np.mean(fw)
-    wabs_x = np.mean(np.abs(forecasts) * fw)
+    wabs_x = np.mean(np.abs(fct) * fw)
     wabs_y = abs(obs) * ow
 
     out[0] = e_1 / M - 0.5 * e_2 / (M**2) + (wabs_x - wabs_y) * (wbar - ow)
 
 
 @njit(["float32(float32)", "float64(float64)"])
 def _norm_cdf(x: float) -> float:
@@ -309,33 +297,33 @@
 def _logis_cdf(x: float) -> float:
     """Cumulative distribution function for the standard logistic distribution."""
     out: float = 1.0 / (1.0 + math.exp(-x))
     return out
 
 
 @vectorize(["float32(float32, float32, float32)", "float64(float64, float64, float64)"])
-def _crps_normal_ufunc(mu: float, sigma: float, observation: float) -> float:
-    ω = (observation - mu) / sigma
+def _crps_normal_ufunc(obs: float, mu: float, sigma: float) -> float:
+    ω = (obs - mu) / sigma
     out: float = sigma * (ω * (2 * _norm_cdf(ω) - 1) + 2 * _norm_pdf(ω) - INV_SQRT_PI)
     return out
 
 
 @vectorize(["float32(float32, float32, float32)", "float64(float64, float64, float64)"])
-def _crps_lognormal_ufunc(mulog: float, sigmalog: float, observation: float) -> float:
-    ω = (np.log(observation) - mulog) / sigmalog
+def _crps_lognormal_ufunc(obs: float, mulog: float, sigmalog: float) -> float:
+    ω = (np.log(obs) - mulog) / sigmalog
     ex = 2 * np.exp(mulog + sigmalog**2 / 2)
-    out: float = observation * (2 * _norm_cdf(ω) - 1) - ex * (
+    out: float = obs * (2 * _norm_cdf(ω) - 1) - ex * (
         _norm_cdf(ω - sigmalog) + _norm_cdf(sigmalog / np.sqrt(2)) - 1
     )
     return out
 
 
 @vectorize(["float32(float32, float32, float32)", "float64(float64, float64, float64)"])
-def _crps_logistic_ufunc(mu: float, sigma: float, observation: float) -> float:
-    ω = (observation - mu) / sigma
+def _crps_logistic_ufunc(obs: float, mu: float, sigma: float) -> float:
+    ω = (obs - mu) / sigma
     out: float = sigma * (ω - 2 * np.log(_logis_cdf(ω)) - 1)
     return out
 
 
 estimator_gufuncs = {
     "akr_circperm": _crps_ensemble_akr_circperm_gufunc,
     "akr": _crps_ensemble_akr_gufunc,
```

### Comparing `scoringrules-0.4.4/scoringrules/core/energy/_gufuncs.py` & `scoringrules-0.5.0/scoringrules/core/energy/_gufuncs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,96 +1,91 @@
 import numpy as np
 from numba import guvectorize
-from numpy.typing import NDArray
-
-_NDArray = NDArray[np.float32 | np.float64]
 
 
 @guvectorize(
     [
-        "void(float32[:,:], float32[:], float32[:])",
-        "void(float64[:,:], float64[:], float64[:])",
+        "void(float32[:], float32[:,:], float32[:])",
+        "void(float64[:], float64[:,:], float64[:])",
     ],
-    "(m,d),(d)->()",
+    "(d),(m,d)->()",
 )
 def _energy_score_gufunc(
-    forecasts: _NDArray,
-    observations: _NDArray,
-    out: _NDArray,
+    obs: np.ndarray,
+    fct: np.ndarray,
+    out: np.ndarray,
 ):
     """Compute the Energy Score for a finite ensemble."""
-    M = forecasts.shape[0]
+    M = fct.shape[0]
 
     e_1 = 0.0
     e_2 = 0.0
     for i in range(M):
-        e_1 += float(np.linalg.norm(forecasts[i] - observations))
+        e_1 += float(np.linalg.norm(fct[i] - obs))
         for j in range(M):
-            e_2 += float(np.linalg.norm(forecasts[i] - forecasts[j]))
+            e_2 += float(np.linalg.norm(fct[i] - fct[j]))
 
     out[0] = e_1 / M - 0.5 / (M**2) * e_2
 
 
 @guvectorize(
     [
-        "void(float32[:,:], float32[:], float32[:], float32[:], float32[:])",
-        "void(float64[:,:], float64[:], float64[:], float64[:], float64[:])",
+        "void(float32[:], float32[:,:], float32[:], float32[:], float32[:])",
+        "void(float64[:], float64[:,:], float64[:], float64[:], float64[:])",
     ],
-    "(m,d),(d),(m),()->()",
+    "(d),(m,d),(),(m)->()",
 )
 def _owenergy_score_gufunc(
-    forecasts: _NDArray,
-    observations: _NDArray,
-    fw: _NDArray,
-    ow: _NDArray,
-    out: _NDArray,
+    obs: np.ndarray,
+    fct: np.ndarray,
+    ow: np.ndarray,
+    fw: np.ndarray,
+    out: np.ndarray,
 ):
     """Compute the Outcome-Weighted Energy Score for a finite ensemble."""
-    M = forecasts.shape[0]
+    M = fct.shape[0]
     ow = ow[0]
 
     e_1 = 0.0
     e_2 = 0.0
     for i in range(M):
-        e_1 += float(np.linalg.norm(forecasts[i] - observations) * fw[i] * ow)
+        e_1 += float(np.linalg.norm(fct[i] - obs) * fw[i] * ow)
         for j in range(M):
-            e_2 += float(
-                np.linalg.norm(forecasts[i] - forecasts[j]) * fw[i] * fw[j] * ow
-            )
+            e_2 += float(np.linalg.norm(fct[i] - fct[j]) * fw[i] * fw[j] * ow)
 
     wbar = np.mean(fw)
 
     out[0] = e_1 / (M * wbar) - 0.5 * e_2 / (M**2 * wbar**2)
 
 
 @guvectorize(
     [
-        "void(float32[:,:], float32[:], float32[:], float32[:], float32[:])",
-        "void(float64[:,:], float64[:], float64[:], float64[:], float64[:])",
+        "void(float32[:], float32[:,:], float32[:], float32[:], float32[:])",
+        "void(float64[:], float64[:,:], float64[:], float64[:], float64[:])",
     ],
-    "(m,d),(d),(m),()->()",
+    "(d),(m,d),(),(m)->()",
 )
 def _vrenergy_score_gufunc(
-    forecasts: _NDArray,
-    observations: _NDArray,
-    fw: _NDArray,
-    ow: _NDArray,
-    out: _NDArray,
+    obs: np.ndarray,
+    fct: np.ndarray,
+    ow: np.ndarray,
+    fw: np.ndarray,
+    out: np.ndarray,
 ):
     """Compute the Vertically Re-scaled Energy Score for a finite ensemble."""
-    M = forecasts.shape[0]
+    M = fct.shape[0]
     ow = ow[0]
 
     e_1 = 0.0
     e_2 = 0.0
     wabs_x = 0.0
     for i in range(M):
-        e_1 += float(np.linalg.norm(forecasts[i] - observations) * fw[i] * ow)
-        wabs_x += np.linalg.norm(forecasts[i]) * fw[i]
+        e_1 += float(np.linalg.norm(fct[i] - obs) * fw[i] * ow)
+        wabs_x += np.linalg.norm(fct[i]) * fw[i]
         for j in range(M):
-            e_2 += float(np.linalg.norm(forecasts[i] - forecasts[j]) * fw[i] * fw[j])
+            e_2 += float(np.linalg.norm(fct[i] - fct[j]) * fw[i] * fw[j])
 
     wabs_x = wabs_x / M
     wbar = np.mean(fw)
-    wabs_y = np.linalg.norm(observations) * ow
+    wabs_y = np.linalg.norm(obs) * ow
 
     out[0] = e_1 / M - 0.5 * e_2 / (M**2) + (wabs_x - wabs_y) * (wbar - ow)
```

### Comparing `scoringrules-0.4.4/scoringrules/core/energy/_score.py` & `scoringrules-0.5.0/scoringrules/core/energy/_score.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,78 +2,74 @@
 
 from scoringrules.backend import backends
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, Backend
 
 
-def energy_score(
-    fcts: "Array", obs: "Array", backend=None  # (... M D)  # (... D)
-) -> "Array":
+def energy_score(obs: "Array", fct: "Array", backend=None) -> "Array":
     """
     Compute the energy score based on a finite ensemble.
 
     The ensemble and variables axes are on the second last and last dimensions respectively.
     """
     B = backends.active if backend is None else backends[backend]
-    M: int = fcts.shape[-2]
+    M: int = fct.shape[-2]
 
-    err_norm = B.norm(fcts - B.expand_dims(obs, -2), -1)  # (... M)
-    E_1 = B.sum(err_norm, -1) / M  # (...)
+    err_norm = B.norm(fct - B.expand_dims(obs, -2), -1)
+    E_1 = B.sum(err_norm, -1) / M
 
-    spread_norm = B.norm(
-        B.expand_dims(fcts, -3) - B.expand_dims(fcts, -2), -1
-    )  # (... M M)
-    E_2 = B.sum(spread_norm, (-2, -1)) / (M**2)  # (...)
+    spread_norm = B.norm(B.expand_dims(fct, -3) - B.expand_dims(fct, -2), -1)
+    E_2 = B.sum(spread_norm, (-2, -1)) / (M**2)
     return E_1 - 0.5 * E_2
 
 
 def owenergy_score(
-    fcts: "Array",  # (... M D)
     obs: "Array",  # (... D)
-    fw: "Array",  # (... M)
+    fct: "Array",  # (... M D)
     ow: "Array",  # (...)
+    fw: "Array",  # (... M)
     backend: "Backend" = None,
 ) -> "Array":
     """Compute the outcome-weighted energy score based on a finite ensemble."""
     B = backends.active if backend is None else backends[backend]
-    M = fcts.shape[-2]
+    M = fct.shape[-2]
     wbar = B.sum(fw, -1) / M
 
-    err_norm = B.norm(fcts - B.expand_dims(obs, -2), -1)  # (... M)
+    err_norm = B.norm(fct - B.expand_dims(obs, -2), -1)  # (... M)
     E_1 = B.sum(err_norm * fw * B.expand_dims(ow, -1), -1) / (M * wbar)  # (...)
 
     spread_norm = B.norm(
-        B.expand_dims(fcts, -2) - B.expand_dims(fcts, -3), -1
+        B.expand_dims(fct, -2) - B.expand_dims(fct, -3), -1
     )  # (... M M)
     fw_prod = B.expand_dims(fw, -1) * B.expand_dims(fw, -2)  # (... M M)
     spread_norm *= fw_prod * B.expand_dims(ow, (-2, -1))  # (... M M)
     E_2 = B.sum(spread_norm, (-2, -1)) / (M**2 * wbar**2)  # (...)
 
     return E_1 - 0.5 * E_2
 
 
 def vrenergy_score(
-    fcts: "Array",
     obs: "Array",
-    fw: "Array",
+    fct: "Array",
     ow: "Array",
+    fw: "Array",
     backend: "Backend" = None,
 ) -> "Array":
     """Compute the vertically re-scaled energy score based on a finite ensemble."""
     B = backends.active if backend is None else backends[backend]
-    M, D = fcts.shape[-2:]
+    M, D = fct.shape[-2:]
     wbar = B.sum(fw, -1) / M
 
-    err_norm = B.norm(fcts - B.expand_dims(obs, -2), -1)  # (... M)
+    err_norm = B.norm(fct - B.expand_dims(obs, -2), -1)  # (... M)
     err_norm *= fw * B.expand_dims(ow, -1)  # (... M)
     E_1 = B.sum(err_norm, -1) / M  # (...)
 
     spread_norm = B.norm(
-        B.expand_dims(fcts, -2) - B.expand_dims(fcts, -3), -1
+        B.expand_dims(fct, -2) - B.expand_dims(fct, -3), -1
     )  # (... M M)
     fw_prod = B.expand_dims(fw, -2) * B.expand_dims(fw, -1)  # (... M M)
     E_2 = B.sum(spread_norm * fw_prod, (-2, -1)) / (M**2)  # (...)
 
-    rhobar = B.sum(B.norm(fcts, -1) * fw, -1) / M  # (...)
+    rhobar = B.sum(B.norm(fct, -1) * fw, -1) / M  # (...)
     E_3 = (rhobar - B.norm(obs, -1) * ow) * (wbar - ow)  # (...)
     return E_1 - 0.5 * E_2 + E_3
```

### Comparing `scoringrules-0.4.4/scoringrules/core/error_spread/_gufunc.py` & `scoringrules-0.5.0/scoringrules/core/error_spread/_gufunc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-import math
-
 import numpy as np
 from numba import guvectorize
 
 INV_SQRT_PI = 1 / np.sqrt(np.pi)
 EPSILON = 1e-6
 
 
 @guvectorize(
     [
         "void(float32[:], float32[:], float32[:])",
         "void(float64[:], float64[:], float64[:])",
     ],
-    "(n),()->()",
+    "(),(n)->()",
 )
-def _error_spread_score_gufunc(
-    forecasts: np.ndarray, observation: np.ndarray, out: np.ndarray
-):
+def _error_spread_score_gufunc(obs: np.ndarray, fct: np.ndarray, out: np.ndarray):
     """Error spread score."""
-    M = forecasts.shape[0]
+    M = fct.shape[0]
     m = 0.0
     s = 0.0
     g = 0.0
     e = 0.0
 
     for i in range(M):
-        m += forecasts[i]
+        m += fct[i]
     m /= M
 
     for i in range(M):
-        s += (forecasts[i] - m) ** 2
-    s /= (M - 1)
+        s += (fct[i] - m) ** 2
+    s /= M - 1
     s = np.sqrt(s)
 
     for i in range(M):
-        g += ((forecasts[i] - m) / s) ** 3
-    g /= ((M - 1) * (M - 2))
+        g += ((fct[i] - m) / s) ** 3
+    g /= (M - 1) * (M - 2)
 
     for i in range(M):
-        e += forecasts[i] - observation[i]
+        e += fct[i] - obs[i]
 
     out[0] = (s**2 - e**2 - e * s * g) ** 2
-
```

### Comparing `scoringrules-0.4.4/scoringrules/core/error_spread/_score.py` & `scoringrules-0.5.0/scoringrules/core/error_spread/_score.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 from scoringrules.backend import backends
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, Backend
 
 
 def error_spread_score(
-    fcts: "Array", obs: "Array", backend: "Backend" = None
+    obs: "Array", fct: "Array", backend: "Backend" = None
 ) -> "Array":
     """Error spread score."""
     B = backends.active if backend is None else backends[backend]
-    M: int = fcts.shape[-1]
-    m = B.mean(fcts, axis=-1)
-    s = B.sqrt(B.sum((fcts - m[...,None]) ** 2, axis=-1) / (M - 1))
-    g = B.sum(((fcts - m[...,None]) / s[...,None]) ** 3, axis=-1) / ((M - 1) * (M - 2))
+    M: int = fct.shape[-1]
+    m = B.mean(fct, axis=-1)
+    s = B.sqrt(B.sum((fct - m[..., None]) ** 2, axis=-1) / (M - 1))
+    g = B.sum(((fct - m[..., None]) / s[..., None]) ** 3, axis=-1) / ((M - 1) * (M - 2))
     e = m - obs
     return B.squeeze((s**2 - e**2 - e * s * g) ** 2)
-
-
```

### Comparing `scoringrules-0.4.4/scoringrules/core/logarithmic.py` & `scoringrules-0.5.0/scoringrules/core/logarithmic.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from scoringrules.core.stats import _norm_pdf
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, ArrayLike, Backend
 
 
 def normal(
+    obs: "ArrayLike",
     mu: "ArrayLike",
     sigma: "ArrayLike",
-    obs: "ArrayLike",
     negative: bool = True,
     backend: "Backend" = None,
 ) -> "Array":
     """Compute the logarithmic score for the normal distribution."""
     B = backends.active if backend is None else backends[backend]
     mu, sigma, obs = map(B.asarray, (mu, sigma, obs))
```

### Comparing `scoringrules-0.4.4/scoringrules/core/utils.py` & `scoringrules-0.5.0/scoringrules/core/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from scoringrules.backend import backends
 
 _V_AXIS = -1
 _M_AXIS = -2
 
 
-def _multivariate_shape_compatibility(fcts, obs, m_axis) -> None:
-    f_shape = fcts.shape
+def _multivariate_shape_compatibility(obs, fct, m_axis) -> None:
+    f_shape = fct.shape
     o_shape = obs.shape
     o_shape_broadcast = o_shape[:m_axis] + (f_shape[m_axis],) + o_shape[m_axis:]
     if o_shape_broadcast != f_shape:
         raise ValueError(
             f"Forecasts shape {f_shape} and observations shape {o_shape} are not compatible for broadcasting!"
         )
 
 
-def _multivariate_shape_permute(fcts, obs, m_axis, v_axis, backend=None):
+def _multivariate_shape_permute(obs, fct, m_axis, v_axis, backend=None):
     B = backends.active if backend is None else backends[backend]
     v_axis_obs = v_axis - 1 if m_axis < v_axis else v_axis
-    fcts = B.moveaxis(fcts, (m_axis, v_axis), (_M_AXIS, _V_AXIS))
+    fct = B.moveaxis(fct, (m_axis, v_axis), (_M_AXIS, _V_AXIS))
     obs = B.moveaxis(obs, v_axis_obs, _V_AXIS)
-    return fcts, obs
+    return obs, fct
 
 
-def multivariate_array_check(fcts, obs, m_axis, v_axis, backend=None):
+def multivariate_array_check(obs, fct, m_axis, v_axis, backend=None):
     """Check and adapt the shapes of multivariate forecasts and observations arrays."""
     B = backends.active if backend is None else backends[backend]
-    fcts, obs = map(B.asarray, (fcts, obs))
-    m_axis = m_axis if m_axis >= 0 else fcts.ndim + m_axis
-    v_axis = v_axis if v_axis >= 0 else fcts.ndim + v_axis
-    _multivariate_shape_compatibility(fcts, obs, m_axis)
-    return _multivariate_shape_permute(fcts, obs, m_axis, v_axis, backend=backend)
+    obs, fct = map(B.asarray, (obs, fct))
+    m_axis = m_axis if m_axis >= 0 else fct.ndim + m_axis
+    v_axis = v_axis if v_axis >= 0 else fct.ndim + v_axis
+    _multivariate_shape_compatibility(obs, fct, m_axis)
+    return _multivariate_shape_permute(obs, fct, m_axis, v_axis, backend=backend)
```

### Comparing `scoringrules-0.4.4/scoringrules/core/variogram/_gufuncs.py` & `scoringrules-0.5.0/scoringrules/core/variogram/_gufuncs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,89 @@
 import numpy as np
 from numba import guvectorize
-from numpy.typing import NDArray
-
-Array = NDArray[np.float32 | np.float64]
 
 
 @guvectorize(
     [
-        "void(float32[:,:], float32[:], float32, float32[:])",
-        "void(float64[:,:], float64[:], float64, float64[:])",
+        "void(float32[:], float32[:,:], float32, float32[:])",
+        "void(float64[:], float64[:,:], float64, float64[:])",
     ],
-    "(m,d),(d),()->()",
+    "(d),(m,d),()->()",
 )
-def _variogram_score_gufunc(fcst: Array, obs: Array, p, out):
-    M = fcst.shape[-2]
-    D = fcst.shape[-1]
+def _variogram_score_gufunc(obs, fct, p, out):
+    M = fct.shape[-2]
+    D = fct.shape[-1]
     out[0] = 0.0
     for i in range(D):
         for j in range(D):
-            vfcts = 0.0
+            vfct = 0.0
             for m in range(M):
-                vfcts += abs(fcst[m, i] - fcst[m, j]) ** p
-            vfcts = vfcts / M
+                vfct += abs(fct[m, i] - fct[m, j]) ** p
+            vfct = vfct / M
             vobs = abs(obs[i] - obs[j]) ** p
-            out[0] += (vobs - vfcts) ** 2
+            out[0] += (vobs - vfct) ** 2
 
 
 @guvectorize(
     [
-        "void(float32[:,:], float32[:], float32, float32[:], float32, float32[:])",
-        "void(float64[:,:], float64[:], float64, float64[:], float64, float64[:])",
+        "void(float32[:], float32[:,:], float32, float32, float32[:], float32[:])",
+        "void(float64[:], float64[:,:], float64, float64, float64[:], float64[:])",
     ],
-    "(m,d),(d),(),(m),()->()",
+    "(d),(m,d),(),(),(m)->()",
 )
-def _owvariogram_score_gufunc(fcst: Array, obs: Array, p, fw, ow, out):
-    M = fcst.shape[-2]
-    D = fcst.shape[-1]
+def _owvariogram_score_gufunc(obs, fct, p, ow, fw, out):
+    M = fct.shape[-2]
+    D = fct.shape[-1]
 
     e_1 = 0.0
     e_2 = 0.0
     for k in range(M):
         for i in range(D):
             for j in range(D):
-                rho1 = abs(fcst[k, i] - fcst[k, j]) ** p
+                rho1 = abs(fct[k, i] - fct[k, j]) ** p
                 rho2 = abs(obs[i] - obs[j]) ** p
                 e_1 += (rho1 - rho2) ** 2 * fw[k] * ow
         for m in range(M):
             for i in range(D):
                 for j in range(D):
-                    rho1 = abs(fcst[k, i] - fcst[k, j]) ** p
-                    rho2 = abs(fcst[m, i] - fcst[m, j]) ** p
+                    rho1 = abs(fct[k, i] - fct[k, j]) ** p
+                    rho2 = abs(fct[m, i] - fct[m, j]) ** p
                     e_2 += (rho1 - rho2) ** 2 * fw[k] * fw[m] * ow
 
     wbar = np.mean(fw)
 
     out[0] = e_1 / (M * wbar) - 0.5 * e_2 / (M**2 * wbar**2)
 
 
 @guvectorize(
     [
-        "void(float32[:,:], float32[:], float32, float32[:], float32, float32[:])",
-        "void(float64[:,:], float64[:], float64, float64[:], float64, float64[:])",
+        "void(float32[:], float32[:,:], float32, float32, float32[:], float32[:])",
+        "void(float64[:], float64[:,:], float64, float64, float64[:], float64[:])",
     ],
-    "(m,d),(d),(),(m),()->()",
+    "(d),(m,d),(),(),(m)->()",
 )
-def _vrvariogram_score_gufunc(fcst: Array, obs: Array, p, fw, ow, out):
-    M = fcst.shape[-2]
-    D = fcst.shape[-1]
+def _vrvariogram_score_gufunc(obs, fct, p, ow, fw, out):
+    M = fct.shape[-2]
+    D = fct.shape[-1]
 
     e_1 = 0.0
     e_2 = 0.0
     e_3_x = 0.0
     for k in range(M):
         for i in range(D):
             for j in range(D):
-                rho1 = abs(fcst[k, i] - fcst[k, j]) ** p
+                rho1 = abs(fct[k, i] - fct[k, j]) ** p
                 rho2 = abs(obs[i] - obs[j]) ** p
                 e_1 += (rho1 - rho2) ** 2 * fw[k] * ow
                 e_3_x += (rho1) ** 2 * fw[k]
         for m in range(M):
             for i in range(D):
                 for j in range(D):
-                    rho1 = abs(fcst[k, i] - fcst[k, j]) ** p
-                    rho2 = abs(fcst[m, i] - fcst[m, j]) ** p
+                    rho1 = abs(fct[k, i] - fct[k, j]) ** p
+                    rho2 = abs(fct[m, i] - fct[m, j]) ** p
                     e_2 += (rho1 - rho2) ** 2 * fw[k] * fw[m]
 
     e_3_x *= 1 / M
     wbar = np.mean(fw)
     e_3_y = 0.0
     for i in range(D):
         for j in range(D):
```

### Comparing `scoringrules-0.4.4/scoringrules/core/variogram/_score.py` & `scoringrules-0.5.0/scoringrules/core/variogram/_score.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,93 +3,93 @@
 from scoringrules.backend import backends
 
 if tp.TYPE_CHECKING:
     from scoringrules.core.typing import Array, Backend
 
 
 def variogram_score(
-    fcst: "Array",  # (... M D)
     obs: "Array",  # (... D)
+    fct: "Array",  # (... M D)
     p: float = 1,
     backend: "Backend" = None,
 ) -> "Array":
     """Compute the Variogram Score for a multivariate finite ensemble."""
     B = backends.active if backend is None else backends[backend]
-    M: int = fcst.shape[-2]
-    fcst_diff = B.expand_dims(fcst, -2) - B.expand_dims(fcst, -1)  # (... M D D)
-    vfcts = B.sum(B.abs(fcst_diff) ** p, axis=-3) / M  # (... D D)
+    M: int = fct.shape[-2]
+    fct_diff = B.expand_dims(fct, -2) - B.expand_dims(fct, -1)  # (... M D D)
+    vfct = B.sum(B.abs(fct_diff) ** p, axis=-3) / M  # (... D D)
     obs_diff = B.expand_dims(obs, -2) - B.expand_dims(obs, -1)  # (... D D)
     vobs = B.abs(obs_diff) ** p  # (... D D)
-    return B.sum((vobs - vfcts) ** 2, axis=(-2, -1))  # (...)
+    return B.sum((vobs - vfct) ** 2, axis=(-2, -1))  # (...)
 
 
 def owvariogram_score(
-    fcst: "Array",
     obs: "Array",
-    fw: "Array",
+    fct: "Array",
     ow: "Array",
+    fw: "Array",
     p: float = 1,
     backend: "Backend" = None,
 ) -> "Array":
     """Compute the Outcome-Weighted Variogram Score for a multivariate finite ensemble."""
     B = backends.active if backend is None else backends[backend]
-    M: int = fcst.shape[-2]
+    M: int = fct.shape[-2]
     wbar = B.mean(fw, axis=-1)
 
-    fcst_diff = B.expand_dims(fcst, -2) - B.expand_dims(fcst, -1)  # (... M D D)
-    fcst_diff = B.abs(fcst_diff) ** p  # (... M D D)
+    fct_diff = B.expand_dims(fct, -2) - B.expand_dims(fct, -1)  # (... M D D)
+    fct_diff = B.abs(fct_diff) ** p  # (... M D D)
 
     obs_diff = B.expand_dims(obs, -2) - B.expand_dims(obs, -1)  # (... D D)
     obs_diff = B.abs(obs_diff) ** p  # (... D D)
-    del fcst, obs
+    del obs, fct
 
-    E_1 = (fcst_diff - B.expand_dims(obs_diff, -3)) ** 2  # (... M D D)
+    E_1 = (fct_diff - B.expand_dims(obs_diff, -3)) ** 2  # (... M D D)
     E_1 = B.sum(E_1, axis=(-2, -1))  # (... M)
     E_1 = B.sum(E_1 * fw * B.expand_dims(ow, -1), axis=-1) / (M * wbar)  # (...)
 
-    fcst_diff_spread = B.expand_dims(fcst_diff, -3) - B.expand_dims(
-        fcst_diff, -4
+    fct_diff_spread = B.expand_dims(fct_diff, -3) - B.expand_dims(
+        fct_diff, -4
     )  # (... M M D D)
     fw_prod = B.expand_dims(fw, -2) * B.expand_dims(fw, -1)  # (... M M)
-    E_2 = B.sum(fcst_diff_spread**2, axis=(-2, -1))  # (... M M)
+    E_2 = B.sum(fct_diff_spread**2, axis=(-2, -1))  # (... M M)
     E_2 *= fw_prod * B.expand_dims(ow, (-2, -1))  # (... M M)
     E_2 = B.sum(E_2, axis=(-2, -1)) / (M**2 * wbar**2)  # (...)
 
     return E_1 - 0.5 * E_2
 
 
 def vrvariogram_score(
-    fcst: "Array",
     obs: "Array",
-    fw: "Array",
+    fct: "Array",
     ow: "Array",
+    fw: "Array",
     p: float = 1,
     backend: "Backend" = None,
 ) -> "Array":
     """Compute the Vertically Re-scaled Variogram Score for a multivariate finite ensemble."""
     B = backends.active if backend is None else backends[backend]
-    M: int = fcst.shape[-2]
+    M: int = fct.shape[-2]
     wbar = B.mean(fw, axis=-1)
 
-    fcst_diff = (
-        B.abs(B.expand_dims(fcst, -2) - B.expand_dims(fcst, -1)) ** p
+    fct_diff = (
+        B.abs(B.expand_dims(fct, -2) - B.expand_dims(fct, -1)) ** p
     )  # (... M D D)
     obs_diff = B.abs(B.expand_dims(obs, -2) - B.expand_dims(obs, -1)) ** p  # (... D D)
 
-    E_1 = (fcst_diff - B.expand_dims(obs_diff, axis=-3)) ** 2  # (... M D D)
+    E_1 = (fct_diff - B.expand_dims(obs_diff, axis=-3)) ** 2  # (... M D D)
     E_1 = B.sum(E_1, axis=(-2, -1))  # (... M)
     E_1 = B.sum(E_1 * fw * B.expand_dims(ow, axis=-1), axis=-1) / M  # (...)
 
     E_2 = (
-        B.expand_dims(fcst_diff, -3) - B.expand_dims(fcst_diff, -4)
+        B.expand_dims(fct_diff, -3) - B.expand_dims(fct_diff, -4)
     ) ** 2  # (... M M D D)
     E_2 = B.sum(E_2, axis=(-2, -1))  # (... M M)
 
     fw_prod = B.expand_dims(fw, axis=-2) * B.expand_dims(fw, axis=-1)  # (... M M)
     E_2 = B.sum(E_2 * fw_prod, axis=(-2, -1)) / (M**2)  # (...)
 
-    E_3 = B.sum(fcst_diff**2, axis=(-2, -1))  # (... M)
+    E_3 = B.sum(fct_diff**2, axis=(-2, -1))  # (... M)
     E_3 = B.sum(E_3 * fw, axis=-1) / M  # (...)
     E_3 -= B.sum(obs_diff**2, axis=(-2, -1)) * ow  # (...)
     E_3 *= wbar - ow  # (...)
 
     return E_1 - 0.5 * E_2 + E_3
```

### Comparing `scoringrules-0.4.4/PKG-INFO` & `scoringrules-0.5.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoringrules
-Version: 0.4.4
+Version: 0.5.0
 Summary: Scoring rules for probabilistic forecast evaluation.
 Home-page: https://github.com/frazane/scoringrules
 Keywords: probabilistic,forecasting,verification
 Author: Francesco Zanetta
 Author-email: zanetta.francesco@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
```

