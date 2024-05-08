# Comparing `tmp/hssm-0.2.0.tar.gz` & `tmp/hssm-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hssm-0.2.0.tar", max compression
+gzip compressed data, was "hssm-0.2.0b1.tar", max compression
```

## Comparing `hssm-0.2.0.tar` & `hssm-0.2.0b1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1100 2024-01-19 14:50:07.347828 hssm-0.2.0/LICENSE
--rw-r--r--   0        0        0     5536 2024-01-19 14:50:07.347828 hssm-0.2.0/README.md
--rw-r--r--   0        0        0     4183 2024-01-19 14:50:07.447828 hssm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1121 2024-01-19 14:50:07.447828 hssm-0.2.0/src/hssm/__init__.py
--rw-r--r--   0        0        0     6112 2024-01-19 14:50:07.447828 hssm-0.2.0/src/hssm/config.py
--rw-r--r--   0        0        0   149091 2024-01-19 14:50:07.447828 hssm-0.2.0/src/hssm/datasets/cavanagh_theta_nn.csv
--rw-r--r--   0        0        0   193800 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/datasets/cavanagh_theta_nn_old.csv
--rw-r--r--   0        0        0     2714 2024-01-19 14:50:07.447828 hssm-0.2.0/src/hssm/datasets.py
--rw-r--r--   0        0        0    11897 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/defaults.py
--rw-r--r--   0        0        0      466 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/distribution_utils/__init__.py
--rw-r--r--   0        0        0    25550 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/distribution_utils/dist.py
--rw-r--r--   0        0        0      387 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/distribution_utils/onnx/__init__.py
--rw-r--r--   0        0        0     9942 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/distribution_utils/onnx/onnx.py
--rw-r--r--   0        0        0     1878 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/distribution_utils/onnx/onnx2pt.py
--rw-r--r--   0        0        0     5204 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/distribution_utils/onnx/onnx2xla.py
--rw-r--r--   0        0        0    47766 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/hssm.py
--rw-r--r--   0        0        0      336 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/likelihoods/__init__.py
--rw-r--r--   0        0        0     9595 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/likelihoods/analytical.py
--rw-r--r--   0        0        0     2058 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/likelihoods/blackbox.py
--rw-r--r--   0        0        0     3335 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/link.py
--rw-r--r--   0        0        0    22985 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/param.py
--rw-r--r--   0        0        0      232 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/plotting/__init__.py
--rw-r--r--   0        0        0    16755 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/plotting/posterior_predictive.py
--rw-r--r--   0        0        0    13459 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/plotting/quantile_probability.py
--rw-r--r--   0        0        0    12171 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/plotting/utils.py
--rw-r--r--   0        0        0    11357 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/prior.py
--rw-r--r--   0        0        0     2421 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/simulator.py
--rw-r--r--   0        0        0    13436 2024-01-19 14:50:07.451828 hssm-0.2.0/src/hssm/utils.py
--rw-r--r--   0        0        0     6816 1970-01-01 00:00:00.000000 hssm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-12-29 22:32:56.536443 hssm-0.2.0b1/LICENSE
+-rw-r--r--   0        0        0     5536 2023-12-29 22:32:56.540443 hssm-0.2.0b1/README.md
+-rw-r--r--   0        0        0     4185 2023-12-29 22:32:56.640443 hssm-0.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1121 2023-12-29 22:32:56.640443 hssm-0.2.0b1/src/hssm/__init__.py
+-rw-r--r--   0        0        0     6112 2023-12-29 22:32:56.640443 hssm-0.2.0b1/src/hssm/config.py
+-rw-r--r--   0        0        0   149091 2023-12-29 22:32:56.640443 hssm-0.2.0b1/src/hssm/datasets/cavanagh_theta_nn.csv
+-rw-r--r--   0        0        0   193800 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/datasets/cavanagh_theta_nn_old.csv
+-rw-r--r--   0        0        0     2714 2023-12-29 22:32:56.640443 hssm-0.2.0b1/src/hssm/datasets.py
+-rw-r--r--   0        0        0    11901 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/defaults.py
+-rw-r--r--   0        0        0      466 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/distribution_utils/__init__.py
+-rw-r--r--   0        0        0    24257 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/distribution_utils/dist.py
+-rw-r--r--   0        0        0      387 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/distribution_utils/onnx/__init__.py
+-rw-r--r--   0        0        0     9942 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/distribution_utils/onnx/onnx.py
+-rw-r--r--   0        0        0     1878 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/distribution_utils/onnx/onnx2pt.py
+-rw-r--r--   0        0        0     5204 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/distribution_utils/onnx/onnx2xla.py
+-rw-r--r--   0        0        0    47766 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/hssm.py
+-rw-r--r--   0        0        0      336 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/likelihoods/__init__.py
+-rw-r--r--   0        0        0     9595 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/likelihoods/analytical.py
+-rw-r--r--   0        0        0     2058 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/likelihoods/blackbox.py
+-rw-r--r--   0        0        0     3335 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/link.py
+-rw-r--r--   0        0        0    22985 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/param.py
+-rw-r--r--   0        0        0      232 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/plotting/__init__.py
+-rw-r--r--   0        0        0    16755 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/plotting/posterior_predictive.py
+-rw-r--r--   0        0        0    13459 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/plotting/quantile_probability.py
+-rw-r--r--   0        0        0    12171 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/plotting/utils.py
+-rw-r--r--   0        0        0    11357 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/prior.py
+-rw-r--r--   0        0        0     2421 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/simulator.py
+-rw-r--r--   0        0        0    13436 2023-12-29 22:32:56.644443 hssm-0.2.0b1/src/hssm/utils.py
+-rw-r--r--   0        0        0     6818 1970-01-01 00:00:00.000000 hssm-0.2.0b1/PKG-INFO
```

### Comparing `hssm-0.2.0/LICENSE` & `hssm-0.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/README.md` & `hssm-0.2.0b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,35 +27,35 @@
 - Native ArviZ support for plotting and other convenience functions to aid the Bayesian workflow.
 - Utilizes the ONNX format for translation of differentiable likelihood approximators across backends.
 
 ### [Official documentation](https://lnccbrown.github.io/HSSM/).
 
 ## Installation
 
-`hssm` is available through PyPI. You can install it with pip via:
+`hssm` is available through PyPI. You can install it with Pip via:
 
 ```
 pip install hssm
 ```
 
-You can also install the bleeding-edge version of `hssm` directly from this repo:
+You can also install the bleeding edge version of `hssm` directly from this repo:
 
 ```
 pip install git+https://github.com/lnccbrown/HSSM.git
 ```
 
 You will need optional dependencies to use JAX-based samplers and graph the models.
 Please refer to our [installation guide](https://lnccbrown.github.io/HSSM/getting_started/installation/)
 for more detailed instructions.
 
 **Note**: Possible solutions to any issues with installations with hssm can be located
 [here](https://github.com/lnccbrown/HSSM/discussions). We recommend leveraging an
 environment manager with Python 3.10~3.11 to prevent any problems with dependencies
 during the installation process. Please note that hssm is tested for python 3.10,
-3.11. As of HSSM v0.2.0, support for Python 3.9 is dropped. Use other python
+3.11. As of HSSM v0.1.6, support for Python 3.9 is dropped. Use other python
 versions with caution.
 
 ## Example
 
 Here is a simple example of how to use HSSM:
 
 ```python
```

#### html2text {}

```diff
@@ -23,25 +23,25 @@
 novel models with corresponding likelihoods. - Built on PyMC with support from
 the Python Bayesian ecosystem at large. - Incorporates Bambi's intuitive
 `lmer`-like regression parameter specification for within- and between-subject
 effects. - Native ArviZ support for plotting and other convenience functions to
 aid the Bayesian workflow. - Utilizes the ONNX format for translation of
 differentiable likelihood approximators across backends. ### [Official
 documentation](https://lnccbrown.github.io/HSSM/). ## Installation `hssm` is
-available through PyPI. You can install it with pip via: ``` pip install hssm
-``` You can also install the bleeding-edge version of `hssm` directly from this
+available through PyPI. You can install it with Pip via: ``` pip install hssm
+``` You can also install the bleeding edge version of `hssm` directly from this
 repo: ``` pip install git+https://github.com/lnccbrown/HSSM.git ``` You will
 need optional dependencies to use JAX-based samplers and graph the models.
 Please refer to our [installation guide](https://lnccbrown.github.io/HSSM/
 getting_started/installation/) for more detailed instructions. **Note**:
 Possible solutions to any issues with installations with hssm can be located
 [here](https://github.com/lnccbrown/HSSM/discussions). We recommend leveraging
 an environment manager with Python 3.10~3.11 to prevent any problems with
 dependencies during the installation process. Please note that hssm is tested
-for python 3.10, 3.11. As of HSSM v0.2.0, support for Python 3.9 is dropped.
+for python 3.10, 3.11. As of HSSM v0.1.6, support for Python 3.9 is dropped.
 Use other python versions with caution. ## Example Here is a simple example of
 how to use HSSM: ```python import hssm # Set float type to float32 to avoid a
 current bug in PyMC # This will not be necessary in the future hssm.set_floatX
 ("float32") # Load a package-supplied dataset cav_data = hssm.load_data
 ('cavanagh_theta') # Define a basic hierarchical model with trial-level
 covariates model = hssm.HSSM( model="ddm", data=cav_data, include=[ { "name":
 "v", "prior": { "Intercept": {"name": "Normal", "mu": 0.0, "sigma": 0.1},
```

### Comparing `hssm-0.2.0/pyproject.toml` & `hssm-0.2.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "HSSM"
-version = "0.2.0"
+version = "0.2.0b1"
 description = "Bayesian inference for hierarchical sequential sampling models."
 authors = [
     "Alexander Fengler <alexander_fengler@brown.edu>",
     "Paul Xu <yang_xu@brown.edu>",
     "Aisulu Omar <aisulu_omar@brown.edu>",
     "Michael Frank <michael_frank@brown.edu>",
 ]
```

### Comparing `hssm-0.2.0/src/hssm/__init__.py` & `hssm-0.2.0b1/src/hssm/__init__.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/config.py` & `hssm-0.2.0b1/src/hssm/config.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/datasets/cavanagh_theta_nn.csv` & `hssm-0.2.0b1/src/hssm/datasets/cavanagh_theta_nn.csv`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/datasets/cavanagh_theta_nn_old.csv` & `hssm-0.2.0b1/src/hssm/datasets/cavanagh_theta_nn_old.csv`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/datasets.py` & `hssm-0.2.0b1/src/hssm/datasets.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/defaults.py` & `hssm-0.2.0b1/src/hssm/defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,29 +247,29 @@
                     "beta": (0.31, 6.99),
                 },
                 "extra_fields": None,
             },
         },
     },
     "race_no_bias_angle_4": {
-        "list_params": ["v0", "v1", "v2", "v3", "a", "z", "t", "theta"],
+        "list_params": ["v0", "v1", "v2", "v3", "a", "z", "ndt", "theta"],
         "description": None,
         "likelihoods": {
             "approx_differentiable": {
                 "loglik": "race_no_bias_angle_4.onnx",
                 "backend": "jax",
                 "default_priors": {},
                 "bounds": {
                     "v0": (0.0, 2.5),
                     "v1": (0.0, 2.5),
                     "v2": (0.0, 2.5),
                     "v3": (0.0, 2.5),
                     "a": (1.0, 3.0),
                     "z": (0.0, 0.9),
-                    "t": (0.0, 2.0),
+                    "ndt": (0.0, 2.0),
                     "theta": (-0.1, 1.45),
                 },
                 "extra_fields": None,
             },
         },
     },
     "ddm_seq2_no_bias": {
```

### Comparing `hssm-0.2.0/src/hssm/distribution_utils/dist.py` & `hssm-0.2.0b1/src/hssm/distribution_utils/dist.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from .onnx import make_jax_logp_funcs_from_onnx, make_jax_logp_ops, make_pytensor_logp
 
 LogLikeFunc = Callable[..., ArrayLike]
 LogLikeGrad = Callable[..., ArrayLike]
 
 _logger = logging.getLogger("hssm")
 
-LOGP_LB = pm.floatX(-66.1)
+OUT_OF_BOUNDS_VAL = pm.floatX(-66.1)
 
 
 def apply_param_bounds_to_loglik(
     logp: Any,
     list_params: list[str],
     *dist_params: Any,
     bounds: dict[str, tuple[float, float]],
@@ -67,59 +67,19 @@
             continue
 
         lower_bound, upper_bound = bounds[param_name]
 
         param_mask = pt.bitwise_or(pt.lt(param, lower_bound), pt.gt(param, upper_bound))
         out_of_bounds_mask = pt.bitwise_or(out_of_bounds_mask, param_mask)
 
-    logp = pt.where(out_of_bounds_mask, LOGP_LB, logp)
+    logp = pt.where(out_of_bounds_mask, OUT_OF_BOUNDS_VAL, logp)
 
     return logp
 
 
-def ensure_positive_ndt(data, logp, list_params, dist_params):
-    """Ensure that the non-decision time is always positive.
-
-    Replaces the log probability of the model with a lower bound if the non-decision
-    time is not positive.
-
-    Parameters
-    ----------
-    data
-        A two-column numpy array with response time and response.
-    logp
-        The log-likelihoods.
-    list_params
-        A list of parameters that the log-likelihood accepts. The order of the
-        parameters in the list will determine the order in which the parameters
-        are passed to the log-likelihood function.
-    dist_params
-        A list of parameters used in the likelihood computation. The parameters
-        can be both scalars and arrays.
-
-    Returns
-    -------
-    float
-        The log-likelihood of the model.
-    """
-    rt = data[:, 0]
-
-    if "t" not in list_params:
-        return logp
-
-    t = dist_params[list_params.index("t")]
-
-    return pt.where(
-        # consistent with the epsilon in the analytical likelihood
-        rt - t <= 1e-15,
-        LOGP_LB,
-        logp,
-    )
-
-
 def make_ssm_rv(
     model_name: str, list_params: list[str], lapse: bmb.Prior | None = None
 ) -> Type[RandomVariable]:
     """Build a RandomVariable Op according to the list of parameters.
 
     Parameters
     ----------
@@ -440,22 +400,20 @@
                     (1.0 - p_outlier) * pt.exp(logp)
                     + p_outlier * pt.exp(lapse_logp)
                     + 1e-29
                 )
             else:
                 logp = loglik(data, *dist_params, *extra_fields)
 
-            if bounds is not None:
-                logp = apply_param_bounds_to_loglik(
-                    logp, list_params, *dist_params, bounds=bounds
-                )
+            if bounds is None:
+                return logp
 
-            # Ensure that non-decision time is always smaller than rt.
-            # Assuming that the non-decision time parameter is always named "t".
-            return ensure_positive_ndt(data, logp, list_params, dist_params)
+            return apply_param_bounds_to_loglik(
+                logp, list_params, *dist_params, bounds=bounds
+            )
 
     return SSMDistribution
 
 
 def make_distribution_from_onnx(
     rv: str | Type[RandomVariable],
     list_params: list[str],
```

### Comparing `hssm-0.2.0/src/hssm/distribution_utils/onnx/onnx.py` & `hssm-0.2.0b1/src/hssm/distribution_utils/onnx/onnx.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/distribution_utils/onnx/onnx2pt.py` & `hssm-0.2.0b1/src/hssm/distribution_utils/onnx/onnx2pt.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/distribution_utils/onnx/onnx2xla.py` & `hssm-0.2.0b1/src/hssm/distribution_utils/onnx/onnx2xla.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/hssm.py` & `hssm-0.2.0b1/src/hssm/hssm.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/likelihoods/analytical.py` & `hssm-0.2.0b1/src/hssm/likelihoods/analytical.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/likelihoods/blackbox.py` & `hssm-0.2.0b1/src/hssm/likelihoods/blackbox.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/link.py` & `hssm-0.2.0b1/src/hssm/link.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/param.py` & `hssm-0.2.0b1/src/hssm/param.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/plotting/posterior_predictive.py` & `hssm-0.2.0b1/src/hssm/plotting/posterior_predictive.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/plotting/quantile_probability.py` & `hssm-0.2.0b1/src/hssm/plotting/quantile_probability.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/plotting/utils.py` & `hssm-0.2.0b1/src/hssm/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/prior.py` & `hssm-0.2.0b1/src/hssm/prior.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/simulator.py` & `hssm-0.2.0b1/src/hssm/simulator.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/src/hssm/utils.py` & `hssm-0.2.0b1/src/hssm/utils.py`

 * *Files identical despite different names*

### Comparing `hssm-0.2.0/PKG-INFO` & `hssm-0.2.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HSSM
-Version: 0.2.0
+Version: 0.2.0b1
 Summary: Bayesian inference for hierarchical sequential sampling models.
 Home-page: https://github.com/lnccbrown/HSSM
 License: Copyright 2023, Brown University, Providence, RI.
 Keywords: HSSM,sequential sampling models,bayesian,bayes,mcmc
 Author: Alexander Fengler
 Author-email: alexander_fengler@brown.edu
 Requires-Python: >=3.10,<3.12
@@ -59,35 +59,35 @@
 - Native ArviZ support for plotting and other convenience functions to aid the Bayesian workflow.
 - Utilizes the ONNX format for translation of differentiable likelihood approximators across backends.
 
 ### [Official documentation](https://lnccbrown.github.io/HSSM/).
 
 ## Installation
 
-`hssm` is available through PyPI. You can install it with pip via:
+`hssm` is available through PyPI. You can install it with Pip via:
 
 ```
 pip install hssm
 ```
 
-You can also install the bleeding-edge version of `hssm` directly from this repo:
+You can also install the bleeding edge version of `hssm` directly from this repo:
 
 ```
 pip install git+https://github.com/lnccbrown/HSSM.git
 ```
 
 You will need optional dependencies to use JAX-based samplers and graph the models.
 Please refer to our [installation guide](https://lnccbrown.github.io/HSSM/getting_started/installation/)
 for more detailed instructions.
 
 **Note**: Possible solutions to any issues with installations with hssm can be located
 [here](https://github.com/lnccbrown/HSSM/discussions). We recommend leveraging an
 environment manager with Python 3.10~3.11 to prevent any problems with dependencies
 during the installation process. Please note that hssm is tested for python 3.10,
-3.11. As of HSSM v0.2.0, support for Python 3.9 is dropped. Use other python
+3.11. As of HSSM v0.1.6, support for Python 3.9 is dropped. Use other python
 versions with caution.
 
 ## Example
 
 Here is a simple example of how to use HSSM:
 
 ```python
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: HSSM Version: 0.2.0 Summary: Bayesian inference for
-hierarchical sequential sampling models. Home-page: https://github.com/
+Metadata-Version: 2.1 Name: HSSM Version: 0.2.0b1 Summary: Bayesian inference
+for hierarchical sequential sampling models. Home-page: https://github.com/
 lnccbrown/HSSM License: Copyright 2023, Brown University, Providence, RI.
 Keywords: HSSM,sequential sampling models,bayesian,bayes,mcmc Author: Alexander
 Fengler Author-email: alexander_fengler@brown.edu Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: arviz
 (>=0.14.0,<0.15.0) Requires-Dist: bambi (>=0.12.0,<0.13.0) Requires-Dist: hddm-
@@ -41,25 +41,25 @@
 novel models with corresponding likelihoods. - Built on PyMC with support from
 the Python Bayesian ecosystem at large. - Incorporates Bambi's intuitive
 `lmer`-like regression parameter specification for within- and between-subject
 effects. - Native ArviZ support for plotting and other convenience functions to
 aid the Bayesian workflow. - Utilizes the ONNX format for translation of
 differentiable likelihood approximators across backends. ### [Official
 documentation](https://lnccbrown.github.io/HSSM/). ## Installation `hssm` is
-available through PyPI. You can install it with pip via: ``` pip install hssm
-``` You can also install the bleeding-edge version of `hssm` directly from this
+available through PyPI. You can install it with Pip via: ``` pip install hssm
+``` You can also install the bleeding edge version of `hssm` directly from this
 repo: ``` pip install git+https://github.com/lnccbrown/HSSM.git ``` You will
 need optional dependencies to use JAX-based samplers and graph the models.
 Please refer to our [installation guide](https://lnccbrown.github.io/HSSM/
 getting_started/installation/) for more detailed instructions. **Note**:
 Possible solutions to any issues with installations with hssm can be located
 [here](https://github.com/lnccbrown/HSSM/discussions). We recommend leveraging
 an environment manager with Python 3.10~3.11 to prevent any problems with
 dependencies during the installation process. Please note that hssm is tested
-for python 3.10, 3.11. As of HSSM v0.2.0, support for Python 3.9 is dropped.
+for python 3.10, 3.11. As of HSSM v0.1.6, support for Python 3.9 is dropped.
 Use other python versions with caution. ## Example Here is a simple example of
 how to use HSSM: ```python import hssm # Set float type to float32 to avoid a
 current bug in PyMC # This will not be necessary in the future hssm.set_floatX
 ("float32") # Load a package-supplied dataset cav_data = hssm.load_data
 ('cavanagh_theta') # Define a basic hierarchical model with trial-level
 covariates model = hssm.HSSM( model="ddm", data=cav_data, include=[ { "name":
 "v", "prior": { "Intercept": {"name": "Normal", "mu": 0.0, "sigma": 0.1},
```

