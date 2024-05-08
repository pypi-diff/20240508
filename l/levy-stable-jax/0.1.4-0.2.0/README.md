# Comparing `tmp/levy_stable_jax-0.1.4.tar.gz` & `tmp/levy_stable_jax-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "levy_stable_jax-0.1.4.tar", max compression
+gzip compressed data, was "levy_stable_jax-0.2.0.tar", max compression
```

## Comparing `levy_stable_jax-0.1.4.tar` & `levy_stable_jax-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-05-06 07:08:26.556737 levy_stable_jax-0.1.4/LICENSE
--rw-r--r--   0        0        0     1259 2024-05-06 07:08:26.556737 levy_stable_jax-0.1.4/README.md
--rw-r--r--   0        0        0     2994 2024-05-06 19:04:42.206410 levy_stable_jax-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      336 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/__init__.py
--rw-r--r--   0        0        0      708 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/_cache.py
--rw-r--r--   0        0        0     4270 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/_generate_data.py
--rw-r--r--   0        0        0      975 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/_interp.py
--rw-r--r--   0        0        0      559 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/_typing.py
--rw-r--r--   0        0        0     7742 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/_utils.py
--rw-r--r--   0        0        0    12470 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/distribution.py
--rw-r--r--   0        0        0     4556 2024-05-06 07:08:26.580737 levy_stable_jax-0.1.4/src/levy_stable_jax/estimation.py
--rw-r--r--   0        0        0  6464128 2024-05-06 07:08:26.628737 levy_stable_jax-0.1.4/src/levy_stable_jax/logpdf.npy
--rw-r--r--   0        0        0     6194 2024-05-06 19:03:37.395619 levy_stable_jax-0.1.4/src/levy_stable_jax/pymc.py
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 levy_stable_jax-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-22 07:47:03.747679 levy_stable_jax-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1259 2024-05-03 14:16:08.822396 levy_stable_jax-0.2.0/README.md
+-rw-r--r--   0        0        0     2994 2024-05-08 15:39:39.030808 levy_stable_jax-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      352 2024-05-08 15:39:31.182742 levy_stable_jax-0.2.0/src/levy_stable_jax/__init__.py
+-rw-r--r--   0        0        0      708 2024-04-24 12:12:58.006634 levy_stable_jax-0.2.0/src/levy_stable_jax/_cache.py
+-rw-r--r--   0        0        0     4270 2024-05-03 11:58:27.607858 levy_stable_jax-0.2.0/src/levy_stable_jax/_generate_data.py
+-rw-r--r--   0        0        0      975 2024-05-03 13:51:24.346392 levy_stable_jax-0.2.0/src/levy_stable_jax/_interp.py
+-rw-r--r--   0        0        0      559 2024-05-03 13:29:34.962247 levy_stable_jax-0.2.0/src/levy_stable_jax/_typing.py
+-rw-r--r--   0        0        0     7703 2024-05-08 15:39:31.182742 levy_stable_jax-0.2.0/src/levy_stable_jax/_utils.py
+-rw-r--r--   0        0        0    16921 2024-05-08 15:39:31.182742 levy_stable_jax-0.2.0/src/levy_stable_jax/distribution.py
+-rw-r--r--   0        0        0     4633 2024-05-08 15:39:31.182742 levy_stable_jax-0.2.0/src/levy_stable_jax/estimation.py
+-rw-r--r--   0        0        0  6464128 2024-05-03 13:29:34.994248 levy_stable_jax-0.2.0/src/levy_stable_jax/logpdf.npy
+-rw-r--r--   0        0        0     6195 2024-05-08 15:39:31.182742 levy_stable_jax-0.2.0/src/levy_stable_jax/pymc.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 levy_stable_jax-0.2.0/PKG-INFO
```

### Comparing `levy_stable_jax-0.1.4/LICENSE` & `levy_stable_jax-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.4/README.md` & `levy_stable_jax-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.4/pyproject.toml` & `levy_stable_jax-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [project]
 name = "levy-stable-jax"
-version = "0.1.4"
+version = "0.2.0"
 authors = [
     {name = "Tim Hunter", email = "tjhunter@cs.stanford.edu"},
 ]
 license = { text = "Apache 2 License" }
 description = "Implementation of the Lévy stable distributions for Jax."
 readme = "README.md"
 requires-python = ">=3.9"
@@ -42,15 +42,15 @@
 Homepage = "https://github.com/tjhunter/levy-stable-jax"
 Documentation = "https://github.com/tjhunter/levy-stable-jax"
 Repository = "https://github.com/tjhunter/levy-stable-jax"
 
 [tool.poetry]
 packages = [{include = "levy_stable_jax", from="src"}]
 name = "levy-stable-jax"
-version = "0.1.4"
+version = "0.2.0"
 authors = ["Tim Hunter <tjhunter@cs.stanford.edu>"]
 description = "Implementation of the Lévy alpha-stable distributions for Jax."
 readme = "README.md"
 license = "Apache 2.0"
 homepage = "https://github.com/tjhunter/levy-stable-jax"
 documentation = "https://levy-stable-jax.readthedocs.io/en/latest/"
 repository = "https://github.com/tjhunter/levy-stable-jax"
```

### Comparing `levy_stable_jax-0.1.4/src/levy_stable_jax/_cache.py` & `levy_stable_jax-0.2.0/src/levy_stable_jax/_cache.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.4/src/levy_stable_jax/_generate_data.py` & `levy_stable_jax-0.2.0/src/levy_stable_jax/_generate_data.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.4/src/levy_stable_jax/_interp.py` & `levy_stable_jax-0.2.0/src/levy_stable_jax/_interp.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.4/src/levy_stable_jax/_typing.py` & `levy_stable_jax-0.2.0/src/levy_stable_jax/_typing.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.4/src/levy_stable_jax/_utils.py` & `levy_stable_jax-0.2.0/src/levy_stable_jax/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         beta: The skewness parameter of the stable distribution.
         loc: The location parameter of the stable distribution.
         scale: The scale parameter of the stable distribution.
         param_from: The initial parametrization of the stable distribution.
         param_to: The requested parametrization
 
     Returns:
-        The parameters of the stable distribution in the parametrization used by scipy.
+        (loc, scale) in the requested parametrization.
     """
 
     # For now, we only need to shift the location. The conversion of the scale
     # will only be needed for N2/N3 parametrization.
     def _phi():
         return jnp.tan(jnp.pi * alpha / 2)
 
@@ -158,28 +158,29 @@
     Computes the sum of independent stable random distributions.
 
     Args:
         alpha: The stability parameter of the stable distribution (0-2.0]. It is fixed
             for all distributions.
         beta: The skewness parameter of the stable distribution.
         loc: The location parameter of the stable distribution (exact definition
-        depending on the choice of pametrization)
+            depending on the choice of pametrization)
         scale: The scale parameter of the stable distribution.
         param: The parametrization of the stable distribution.
 
     Returns: A tuple of (beta_sum, loc_sum, scale_sum)
 
     Example: the sum of two centered Gaussian distributions is a centered Gaussian distribution with
     a standard deviation of sqrt(2).
     ```python
     import jax.numpy as jnp
     >>> sum(2.0, 0.0, 0.0, jnp.asarray([1.0, 1.0]), Params.N1) # doctest: +ELLIPSIS
-    (Array(0., dtype=float64), Array(0., dtype=float64), Array(1.4142135..., dtype=float64))
+    (Array(0., dtype=float64), Array(0., dtype=float64), Array(1.4142135...,...))
 
     ```
+
     Example: dot product.
     Say that x1 ~ S(2, 0, 1, 1) and x2 ~ S(2, 0, 1.1, 1) are independent.
     We want to compute the distribution z = A . x + b where
     x = [x1, x2], A is a 3 x 2 matrix, b is a 3-vector, and . is the matrix-vector product.
 
     This can be written by a summing a scale operation:
```

### Comparing `levy_stable_jax-0.1.4/src/levy_stable_jax/distribution.py` & `levy_stable_jax-0.2.0/src/levy_stable_jax/distribution.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 Univariate stable distribution by John Nolan, 2020.
 
 """
 
 from __future__ import annotations  # for the | syntax.
 
 from math import pi as PI
-from typing import Tuple, List
+from typing import Tuple, List, Sequence
 
+import jax
 import jax.numpy as jnp
 from jax import Array as JArray
 import jax.scipy.special as jax_special
 from jax import lax
 import numpy as np
 import numpy.typing as npt
 
 from ._interp import interp_linear
 from ._typing import Param, Params
 from ._cache import jax_read_from_cache
 
+Shape = Sequence[int]  # TODO: unsure how to obtain from jax.
 
 NUM_X_POINTS = 200  # 200
 NUM_ALPHA_POINTS = 80  # 76
 NUM_BETA_POINTS = 101  # 101
 
 # Some bounds and parameters
 ALPHA_MIN: float = 1.1
@@ -79,15 +81,38 @@
     loc: INPUT_TYPE = 0.0,
     scale: INPUT_TYPE = 1.0,
     param: Param = Params.N0,
 ) -> JArray | float:
     """
     The probability density function for the Levy-Stable distribution.
 
-    TODO: documentation
+    Parameters:
+
+    - x: the values at which to evaluate the PDF
+    - alpha: the alpha parameter of the distribution
+    - beta: the beta parameter of the distribution
+    - loc: the location parameter of the distribution
+        (default 0.0, meaning depends on the parametrization)
+    - scale: the scale parameter of the distribution
+        (default 1.0, meaning depends on the parametrization)
+    - param: the parametrization of the distribution
+
+    Returns:
+    - the value of the PDF at the given point(s)
+
+    Examples:
+
+    Evaluation of the unit Levy-stable distribution at 0.0, with alpha=1.5, beta=0.0.
+    ```py
+    >>> pdf(0.0, 1.5, 0.0) # doctest: +ELLIPSIS
+    0.28568...
+    >>> pdf(0.0, 1.5, 0.0,param=Params.N0) # doctest: +ELLIPSIS
+    0.28568...
+
+    ```
     """
     # TODO: implement the other parametrizations
     (alpha_, beta_, x_, loc_, scale_), is_scalar = _canonicalize_input(
         [alpha, beta, x, loc, scale]
     )
 
     assert param == Params.N0, param
@@ -104,20 +129,29 @@
     loc: INPUT_TYPE = 0.0,
     scale: INPUT_TYPE = 1.0,
     param: Param = Params.N0,
 ) -> JArray | float:
     """
     The probability density function for the Levy-Stable distribution.
 
-    TODO: documentation
+    Parameters:
+
+    - x: the values at which to evaluate the PDF
+    - alpha: the alpha parameter of the distribution
+    - beta: the beta parameter of the distribution
+    - loc: the location parameter of the distribution
+        (default 0.0, meaning depends on the parametrization)
+    - scale: the scale parameter of the distribution
+        (default 1.0, meaning depends on the parametrization)
+    - param: the parametrization of the distribution (see Params)
 
     Examples:
 
     ```py
-    >>> logpdf(0.0, 1.5, 0.0, 1.0)
+    >>> logpdf(0.0, 1.5, 0.0, 1.0) # doctest: +ELLIPSIS
     -1.603550...
 
     ```
 
     """
     (alpha_, beta_, x_, loc_, scale_), is_scalar = _canonicalize_input(
         [alpha, beta, x, loc, scale]
@@ -127,14 +161,83 @@
     assert param == Params.N0, param
     res = _logpdf_n0(x_, alpha_, beta_, loc_, scale_)
     if is_scalar:
         res = res.item()
     return res
 
 
+def rvs(
+    alpha: INPUT_TYPE,
+    beta: INPUT_TYPE,
+    prng: jax.random.PRNGKey,
+    loc: INPUT_TYPE = 0.0,
+    scale: INPUT_TYPE = 1.0,
+    shape: Shape = (),
+    param: Param = Params.N0,
+) -> JArray:
+    """
+    Generate random samples from the Levy-Stable distribution.
+
+    Args:
+        alpha: the alpha parameter of the distribution
+        beta: the beta parameter of the distribution
+        prng: the pseudo-random number generator key
+        loc: the location parameter of the distribution
+        scale: the scale parameter of the distribution
+        shape: the shape of the output array
+        param: the parametrization of the distribution
+
+    Returns:
+    - the generated samples
+
+    Examples:
+
+    ```py
+    >>> import jax
+    >>> prng = jax.random.PRNGKey(1)
+    >>> rvs(alpha=1.5, beta=0.0, loc=0.0, scale=1.0, param=Params.N1,
+    ...  shape=(10,), prng=prng) # doctest: +ELLIPSIS
+    Array([-0.750..., -0.495..., ...], ...)
+
+    ```
+    """
+    # The sampling algorithm is for N1 parametrization.
+    unit_n1 = _sample_unit_n1(alpha, beta, prng, shape)
+    return _values_n1_to_param(alpha, beta, unit_n1, loc, scale, param)
+
+
+def _values_n1_to_param(
+    alpha: INPUT_TYPE,
+    beta: INPUT_TYPE,
+    values: INPUT_TYPE,
+    loc: INPUT_TYPE,
+    scale: INPUT_TYPE,
+    to_param: Param,
+) -> Tuple[JArray, JArray]:
+    """
+    Takes values in the unit N1 parametrization and shifts them to the requested parametrization.
+
+    Valid for all alpha.
+    """
+    # TODO: merge with utils.scale?
+    if to_param == Params.N0:
+        return jnp.where(
+            jnp.abs(alpha - 1) < 1e-10,
+            loc + scale * values,
+            loc + scale * (values - beta * jnp.tan(PI * alpha / 2)),
+        )
+    elif to_param == Params.N1:
+        # TODO: have a separate function to define x log(x) around x == 1 with Taylor expansion
+        return jnp.where(
+            jnp.abs(alpha - 1) < 1e-10,
+            loc + scale * (values + beta * 2 / PI * scale * jnp.log(scale)),
+            loc + scale * values,
+        )
+
+
 def _pdf_n0(
     x: JArray, alpha: JArray, beta: JArray, loc: JArray, scale: JArray
 ) -> JArray:
     """
     The PDF of the stable-Levy distribution, as parametrized in Nolan's 0 notation.
     """
     return jnp.exp(_logpdf_n0(x, alpha, beta, loc, scale))
@@ -380,7 +483,42 @@
         if arr.size == max_len:
             return arr
         if arr.size == 1:
             return jnp.tile(arr, max_len)
         raise AssertionError(f"Size mismatch: {arr.shape} vs {max_len}")
 
     return [_check_size(arr) for arr in arrs], False
+
+
+def _sample_unit_n1(
+    alpha: JArray, beta: JArray, prng: jax.random.PRNGKey, shape: Shape
+) -> JArray:
+    """
+    Sample from the unit Levy-stable distribution in the N1 parametrization.
+
+    This implementation only support alpha != 1, it will diverge or return NaNs for alpha == 1.
+
+    Algorithm based on Nolan (2020), Theorem 1.3
+
+    Based on the scipy code:
+    https://github.com/scipy/scipy/blob/v1.13.0/scipy/stats/_levy_stable/__init__.py#L422
+    """
+    k1, k2 = jax.random.split(prng, 2)
+    TH = (jax.random.uniform(k1, shape=shape) - 0.5) * PI
+    W = jax.random.exponential(k2, shape=shape)
+    aTH = alpha * TH
+    cosTH = jnp.cos(TH)
+    tanTH = jnp.tan(TH)
+
+    # Not implementing the special cases for alpha = 1 or beta=0
+    val0 = beta * np.tan(np.pi * alpha / 2)
+    th0 = jnp.arctan(val0) / alpha
+    val3 = W / (cosTH / jnp.tan(alpha * (th0 + TH)) + jnp.sin(TH))
+    res3 = val3 * (
+        (
+            jnp.cos(aTH)
+            + jnp.sin(aTH) * tanTH
+            - val0 * (jnp.sin(aTH) - jnp.cos(aTH) * tanTH)
+        )
+        / W
+    ) ** (1.0 / alpha)
+    return res3
```

### Comparing `levy_stable_jax-0.1.4/src/levy_stable_jax/estimation.py` & `levy_stable_jax-0.2.0/src/levy_stable_jax/estimation.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import jax.numpy as jnp
 from jax import Array as JArray
 import jaxopt  # type: ignore
 import scipy.stats._levy_stable  # type: ignore
 
 from .distribution import logpdf, Params, Param
+from ._utils import param_convert
 
 
 def fit_quantiles(samples: JArray, param: Param) -> JArray:
     """
     A rough approximation of the distribution parameters based on quantiles.
 
     For now, it is just wrapping the scipy code.
@@ -53,39 +54,33 @@
     weights: Optional[JArray] = None,
     alpha: Optional[float] = None,
     beta: Optional[float] = None,
 ):
     """
     Maximum likelihood evaluation for univariate Lévy-Stable distributions.
 
-    d: a distribution object
-    param: the parametrization of the returned distribution
-    samples: a 1-d array with the observed samples.
-    weights: optional, the weights on each of the samples.
-
-    Return a len-4 array with the parameters of the distribution: (alpha, beta, loc, scale)
-
-    TODO: add the possibility to pass tuples to constraint the search space.
-
-    TODO: N1 parametrization is not implemented yet.
-
+    Args:
+        param: the parametrization of the returned distribution
+        samples: a 1-d array with the observed samples.
+        weights: optional, the weights on each of the samples.
+        alpha: optional, the value of alpha to be used in the optimization.
+        beta: optional, the value of beta to be used in the optimization.
 
     Examples:
 
     ```py
     >>> samples = jnp.array([1.0, 2.0, 3.0, 4.0, 5.0])
     >>> fit_quantiles(samples, Params.N0) # doctest: +ELLIPSIS
     Array([2.        , 0.        , 3.        , 1.048...], dtype=float64)
 
     ```
 
     The first value is alpha, then beta, then the location parameter and then
      the scale parameter.
     """
-    assert param == Params.N0, param
     assert samples.ndim == 1, samples
     assert samples.size > 4, samples.size
 
     def _unpack(theta):
         idx = 0
         if alpha is None:
             alpha_ = theta[idx]
@@ -148,10 +143,12 @@
         upper.append(1e4)
         # Scale
         lower.append(1e-3)
         upper.append(1e2)
         return (jnp.array(lower), jnp.array(upper))
 
     theta_bounds = _bounds()
-    res = solver.run(theta_start, bounds=theta_bounds)
-    # TODO: convert back to the requested parametrization
-    return res.params
+    sres = solver.run(theta_start, bounds=theta_bounds)
+    (alpha0, beta0, loc0, scale0) = _unpack(sres.params)
+    # Convert to the requested parametrization
+    (loc_x, scale_x) = param_convert(alpha0, beta0, loc0, scale0, Params.N0, param)
+    return jnp.array([alpha0, beta0, loc_x, scale_x])
```

### Comparing `levy_stable_jax-0.1.4/src/levy_stable_jax/logpdf.npy` & `levy_stable_jax-0.2.0/src/levy_stable_jax/logpdf.npy`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.4/src/levy_stable_jax/pymc.py` & `levy_stable_jax-0.2.0/src/levy_stable_jax/pymc.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,19 @@
 
 
 def LevyStableN0(name, alpha, beta, loc, scale, observed=None):
     """
     A Lévy-stable distribution. The parametrization follows the "0" notation
     from Nolan (2022). It is also known as the "S0" parametrization in scipy.
 
-    Parameters:
-
-    - alpha: the stability parameter. Must be in (1.1, 2].
-    - beta: the skewness parameter. Must be in [-1, 1].
-    - loc: the location parameter (delta in Nolan's notation).
-    - scale: the scale parameter (gamma in Nolan's notation).
+    Args:
+        alpha: the stability parameter. Must be in (1.1, 2].
+        beta: the skewness parameter. Must be in [-1, 1].
+        loc: the location parameter (delta in Nolan's notation).
+        scale: the scale parameter (gamma in Nolan's notation).
 
     This distribution is explicitly implemented and parametrized for the N0
     parametrization, because the N1 parametrization is not continuous
     for alpha close to 1, and is not recommended in general for numerical work.
     Use the `shift_scale` function if you wish to convert to other parametrizations.
 
     **Practical tips**
```

### Comparing `levy_stable_jax-0.1.4/PKG-INFO` & `levy_stable_jax-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: levy-stable-jax
-Version: 0.1.4
+Version: 0.2.0
 Summary: Implementation of the Lévy alpha-stable distributions for Jax.
 Home-page: https://github.com/tjhunter/levy-stable-jax
 License: Apache 2.0
 Keywords: levy,stable,jax,probability,statistics
 Author: Tim Hunter
 Author-email: tjhunter@cs.stanford.edu
 Requires-Python: >=3.10,<3.13
```

