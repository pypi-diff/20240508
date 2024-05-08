# Comparing `tmp/posteriors-0.0.2.tar.gz` & `tmp/posteriors-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posteriors-0.0.2.tar", last modified: Tue Apr 16 18:00:00 2024, max compression
+gzip compressed data, was "posteriors-0.0.3.tar", last modified: Wed May  8 17:06:12 2024, max compression
```

## Comparing `posteriors-0.0.2.tar` & `posteriors-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 17:59:55.000000 posteriors-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-16 18:00:00.548081 posteriors-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-16 17:59:55.000000 posteriors-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.544081 posteriors-0.0.2/posteriors/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/posteriors/ekf/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/ekf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/ekf/diag_fisher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/posteriors/laplace/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/laplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/laplace/dense_fisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/laplace/diag_fisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/optim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/posteriors/sgmcmc/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/sgmcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/sgmcmc/sghmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/sgmcmc/sgld.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/torchopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    22478 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/posteriors/vi/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/vi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-16 17:59:55.000000 posteriors-0.0.2/posteriors/vi/diag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/posteriors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-16 18:00:00.000000 posteriors-0.0.2/posteriors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-16 18:00:00.000000 posteriors-0.0.2/posteriors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:00:00.000000 posteriors-0.0.2/posteriors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-16 18:00:00.000000 posteriors-0.0.2/posteriors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 18:00:00.000000 posteriors-0.0.2/posteriors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-16 17:59:55.000000 posteriors-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:00:00.548081 posteriors-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:00:00.548081 posteriors-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-16 17:59:55.000000 posteriors-0.0.2/tests/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-16 17:59:55.000000 posteriors-0.0.2/tests/test_torchopt.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-16 17:59:55.000000 posteriors-0.0.2/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16698 2024-04-16 17:59:55.000000 posteriors-0.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:06:12.555000 posteriors-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 17:06:07.000000 posteriors-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-08 17:06:12.555000 posteriors-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-08 17:06:07.000000 posteriors-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:06:12.551000 posteriors-0.0.3/posteriors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:06:12.555000 posteriors-0.0.3/posteriors/ekf/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/ekf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/ekf/diag_fisher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:06:12.555000 posteriors-0.0.3/posteriors/laplace/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/laplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/laplace/dense_fisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/laplace/dense_ggn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/laplace/diag_fisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/laplace/diag_ggn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/optim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:06:12.555000 posteriors-0.0.3/posteriors/sgmcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/sgmcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/sgmcmc/sghmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/sgmcmc/sgld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/torchopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31456 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:06:12.555000 posteriors-0.0.3/posteriors/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/vi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-05-08 17:06:07.000000 posteriors-0.0.3/posteriors/vi/diag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:06:12.555000 posteriors-0.0.3/posteriors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-08 17:06:12.000000 posteriors-0.0.3/posteriors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-08 17:06:12.000000 posteriors-0.0.3/posteriors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:06:12.000000 posteriors-0.0.3/posteriors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-08 17:06:12.000000 posteriors-0.0.3/posteriors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 17:06:12.000000 posteriors-0.0.3/posteriors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-08 17:06:07.000000 posteriors-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:06:12.559000 posteriors-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:06:12.555000 posteriors-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-08 17:06:07.000000 posteriors-0.0.3/tests/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-08 17:06:07.000000 posteriors-0.0.3/tests/test_torchopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-08 17:06:07.000000 posteriors-0.0.3/tests/test_tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-08 17:06:07.000000 posteriors-0.0.3/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26630 2024-05-08 17:06:07.000000 posteriors-0.0.3/tests/test_utils.py
```

### Comparing `posteriors-0.0.2/LICENSE` & `posteriors-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.2/PKG-INFO` & `posteriors-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posteriors
-Version: 0.0.2
+Version: 0.0.3
 Summary: Uncertainty quantification with PyTorch
 Author-email: Sam Duffield <sam@normalcomputing.ai>
 License: Apache-2.0
 Keywords: pytorch,uncertainty
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `posteriors-0.0.2/README.md` & `posteriors-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.2/posteriors/__init__.py` & `posteriors-0.0.3/posteriors/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,30 +6,35 @@
 
 from posteriors.utils import CatchAuxError
 from posteriors.utils import model_to_function
 from posteriors.utils import linearized_forward_diag
 from posteriors.utils import hvp
 from posteriors.utils import fvp
 from posteriors.utils import empirical_fisher
+from posteriors.utils import ggnvp
+from posteriors.utils import ggn
+from posteriors.utils import diag_ggn
+from posteriors.utils import cg
 from posteriors.utils import diag_normal_log_prob
 from posteriors.utils import diag_normal_sample
-from posteriors.utils import tree_size
-from posteriors.utils import tree_extract
-from posteriors.utils import tree_insert
-from posteriors.utils import tree_insert_
-from posteriors.utils import extract_requires_grad
-from posteriors.utils import insert_requires_grad
-from posteriors.utils import insert_requires_grad_
-from posteriors.utils import extract_requires_grad_and_func
-from posteriors.utils import inplacify
-from posteriors.utils import tree_map_inplacify_
-from posteriors.utils import flexi_tree_map
 from posteriors.utils import per_samplify
 from posteriors.utils import is_scalar
 
+from posteriors.tree_utils import tree_size
+from posteriors.tree_utils import tree_extract
+from posteriors.tree_utils import tree_insert
+from posteriors.tree_utils import tree_insert_
+from posteriors.tree_utils import extract_requires_grad
+from posteriors.tree_utils import insert_requires_grad
+from posteriors.tree_utils import insert_requires_grad_
+from posteriors.tree_utils import extract_requires_grad_and_func
+from posteriors.tree_utils import inplacify
+from posteriors.tree_utils import tree_map_inplacify_
+from posteriors.tree_utils import flexi_tree_map
+
 import logging
 
 logger = logging.getLogger("torch.distributed.elastic.multiprocessing.redirects")
 logger.setLevel(logging.ERROR)
 
 from posteriors import vi
 from posteriors import torchopt
```

### Comparing `posteriors-0.0.2/posteriors/ekf/diag_fisher.py` & `posteriors-0.0.3/posteriors/ekf/diag_fisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from functools import partial
 import torch
 from torch.func import jacrev
 from optree import tree_map
 from dataclasses import dataclass
 
 from posteriors.types import TensorTree, Transform, LogProbFn, TransformState
+from posteriors.tree_utils import flexi_tree_map
 from posteriors.utils import (
     diag_normal_sample,
-    flexi_tree_map,
     per_samplify,
     is_scalar,
     CatchAuxError,
 )
 
 
 def build(
```

### Comparing `posteriors-0.0.2/posteriors/laplace/dense_fisher.py` & `posteriors-0.0.3/posteriors/laplace/dense_fisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any
 from dataclasses import dataclass
 from functools import partial
 import torch
 from optree import tree_map
 from optree.integration.torch import tree_ravel
 
-from posteriors.types import TensorTree, Transform, LogProbFn, Tensor, TransformState
+from posteriors.types import TensorTree, Transform, LogProbFn, TransformState
+from posteriors.tree_utils import tree_size
 from posteriors.utils import (
     per_samplify,
-    tree_size,
     empirical_fisher,
     is_scalar,
     CatchAuxError,
 )
 
 
 def build(
     log_posterior: LogProbFn,
     per_sample: bool = False,
-    init_prec: Tensor | float = 0.0,
+    init_prec: torch.Tensor | float = 0.0,
 ) -> Transform:
     """Builds a transform for dense empirical Fisher information
     Laplace approximation.
 
     The empirical Fisher is defined here as:
     $$
     F(θ) = \\sum_i ∇_θ \\log p(y_i, θ | x_i) ∇_θ \\log p(y_i, θ | x_i)^T
@@ -63,21 +63,21 @@
     Args:
         params: Mean of the Normal distribution.
         prec: Precision matrix of the Normal distribution.
         aux: Auxiliary information from the log_posterior call.
     """
 
     params: TensorTree
-    prec: Tensor
+    prec: torch.Tensor
     aux: Any = None
 
 
 def init(
     params: TensorTree,
-    init_prec: Tensor | float = 0.0,
+    init_prec: torch.Tensor | float = 0.0,
 ) -> DenseLaplaceState:
     """Initialise Normal distribution over parameters
     with a dense precision matrix.
 
     Args:
         params: Mean of the Normal distribution.
         init_prec: Initial precision matrix.
```

### Comparing `posteriors-0.0.2/posteriors/laplace/diag_fisher.py` & `posteriors-0.0.3/posteriors/laplace/diag_fisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from typing import Any
 import torch
 from torch.func import jacrev
 from optree import tree_map
 from dataclasses import dataclass
 
 from posteriors.types import TensorTree, Transform, LogProbFn, TransformState
+from posteriors.tree_utils import flexi_tree_map
 from posteriors.utils import (
     diag_normal_sample,
-    flexi_tree_map,
     per_samplify,
     is_scalar,
     CatchAuxError,
 )
 
 
 def build(
```

### Comparing `posteriors-0.0.2/posteriors/optim.py` & `posteriors-0.0.3/posteriors/optim.py`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.2/posteriors/sgmcmc/sghmc.py` & `posteriors-0.0.3/posteriors/sgmcmc/sghmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from functools import partial
 import torch
 from torch.func import grad_and_value
 from optree import tree_map
 from dataclasses import dataclass
 
 from posteriors.types import TensorTree, Transform, LogProbFn, TransformState
-from posteriors.utils import flexi_tree_map, is_scalar, CatchAuxError
+from posteriors.tree_utils import flexi_tree_map
+from posteriors.utils import is_scalar, CatchAuxError
 
 
 def build(
     log_posterior: LogProbFn,
     lr: float,
     alpha: float = 0.01,
     beta: float = 0.0,
@@ -20,25 +21,25 @@
     """Builds SGHMC transform.
 
     Algorithm from [Chen et al, 2014](https://arxiv.org/abs/1402.4102):
 
     \\begin{align}
     θ_{t+1} &= θ_t + ε m_t \\\\
     m_{t+1} &= m_t + ε \\nabla \\log p(θ_t, \\text{batch}) - ε α m_t
-    + N(0, ε T (2 α - ε β) T \\mathbb{I})\\
+    + N(0, ε T (2 α - ε β T) \\mathbb{I})\\
     \\end{align}
     
     for learning rate $\\epsilon$ and temperature $T$
 
     Targets $p_T(θ, m) \\propto \\exp( (\\log p(θ) - \\frac12 m^Tm) / T)$
     with temperature $T$.
 
     The log posterior and temperature are recommended to be [constructed in tandem](../../log_posteriors.md)
-    to ensure robust scaling for a large amount of data.
-
+    to ensure robust scaling for a large amount of data and variable batch size.
+    
     Args:
         log_posterior: Function that takes parameters and input batch and
             returns the log posterior value (which can be unnormalised)
             as well as auxiliary information, e.g. from the model call.
         lr: Learning rate.
         alpha: Friction coefficient.
         beta: Gradient noise coefficient (estimated variance).
@@ -116,15 +117,15 @@
     """Updates parameters and momenta for SGHMC.
     
     Update rule from [Chen et al, 2014](https://arxiv.org/abs/1402.4102):
 
     \\begin{align}
     θ_{t+1} &= θ_t + ε m_t \\\\
     m_{t+1} &= m_t + ε \\nabla \\log p(θ_t, \\text{batch}) - ε α m_t
-    + N(0, ε T (2 α - ε β) T \\mathbb{I})\\
+    + N(0, ε T (2 α - ε β T) \\mathbb{I})\\
     \\end{align}
     
     for learning rate $\\epsilon$ and temperature $T$
 
     Args:
         state: SGHMCState containing params and momenta.
         batch: Data batch to be send to log_posterior.
```

### Comparing `posteriors-0.0.2/posteriors/sgmcmc/sgld.py` & `posteriors-0.0.3/posteriors/sgmcmc/sgld.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Any
 from functools import partial
 import torch
 from torch.func import grad_and_value
 from dataclasses import dataclass
 
 from posteriors.types import TensorTree, Transform, LogProbFn, TransformState
-from posteriors.utils import flexi_tree_map, CatchAuxError
+from posteriors.tree_utils import flexi_tree_map
+from posteriors.utils import CatchAuxError
 
 
 def build(
     log_posterior: LogProbFn,
     lr: float,
     beta: float = 0.0,
     temperature: float = 1.0,
@@ -21,15 +22,15 @@
     θ_{t+1} = θ_t + ε \\nabla \\log p(θ_t, \\text{batch}) + N(0, ε  (2 - ε β) T \\mathbb{I})
     $$
     for learning rate $\\epsilon$ and temperature $T$.
 
     Targets $p_T(θ) \\propto \\exp( \\log p(θ) / T)$ with temperature $T$.
 
     The log posterior and temperature are recommended to be [constructed in tandem](../../log_posteriors.md)
-    to ensure robust scaling for a large amount of data.
+    to ensure robust scaling for a large amount of data and variable batch size.
 
     Args:
         log_posterior: Function that takes parameters and input batch and
             returns the log posterior value (which can be unnormalised)
             as well as auxiliary information, e.g. from the model call.
         lr: Learning rate.
         beta: Gradient noise coefficient (estimated variance).
```

### Comparing `posteriors-0.0.2/posteriors/torchopt.py` & `posteriors-0.0.3/posteriors/torchopt.py`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.2/posteriors/types.py` & `posteriors-0.0.3/posteriors/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from optree import registry
 from torch import Tensor
 
 TensorTree: TypeAlias = PyTreeTypeVar("TensorTree", Tensor)  # type: ignore
 
 LogProbFn = Callable[[TensorTree, TensorTree], Tuple[float, TensorTree]]
 ForwardFn = Callable[[TensorTree, TensorTree], Tuple[Tensor, TensorTree]]
+OuterLogProbFn = Callable[[TensorTree, TensorTree], float]
 
 namespace = registry.__GLOBAL_NAMESPACE
 
 
 @register_pytree_node_class(namespace=namespace)
 class TransformState:
     """A `posteriors` transform state is a `dataclass` containing the required
```

### Comparing `posteriors-0.0.2/posteriors/vi/diag.py` & `posteriors-0.0.3/posteriors/vi/diag.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,24 +184,30 @@
     temperature: float = 1.0,
     n_samples: int = 1,
     stl: bool = True,
 ) -> Tuple[float, Any]:
     """Returns the negative evidence lower bound (NELBO) for a diagonal Normal
     variational distribution over the parameters of a model.
 
-    Averages NELBO over the batch. Monte Carlo estimate with n_samples from q.
+    Monte Carlo estimate with `n_samples` from q.
+    $$
+    \\text{NELBO} = - 𝔼_{q(θ)}[\\log p(y|x, θ) + \\log p(θ) - \\log q(θ) * T])
+    $$
+    for temperature $T$.
 
-    NELBO = - (E_q[log p(y|x, θ) + log p(θ) - log q(θ) * temperature])
-
-    log_posterior expects to take parameters and input batch and return a scalar:
+    `log_posterior` expects to take parameters and input batch and return a scalar
+    as well as a TensorTree of any auxiliary information:
 
     ```
-    log_posterior_eval = log_posterior(params, batch)
+    log_posterior_eval, aux = log_posterior(params, batch)
     ```
 
+    The log posterior and temperature are recommended to be [constructed in tandem](../../log_posteriors.md)
+    to ensure robust scaling for a large amount of data and variable batch size.
+
     Args:
         mean: Mean of the variational distribution.
         sd_diag: Square-root diagonal of the covariance matrix of the
             variational distribution.
         batch: Input data to log_posterior.
         log_posterior: Function that takes parameters and input batch and
             returns the log posterior (which can be unnormalised).
```

### Comparing `posteriors-0.0.2/posteriors.egg-info/PKG-INFO` & `posteriors-0.0.3/posteriors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posteriors
-Version: 0.0.2
+Version: 0.0.3
 Summary: Uncertainty quantification with PyTorch
 Author-email: Sam Duffield <sam@normalcomputing.ai>
 License: Apache-2.0
 Keywords: pytorch,uncertainty
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `posteriors-0.0.2/posteriors.egg-info/SOURCES.txt` & `posteriors-0.0.3/posteriors.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 LICENSE
 README.md
 pyproject.toml
 posteriors/__init__.py
 posteriors/optim.py
 posteriors/torchopt.py
+posteriors/tree_utils.py
 posteriors/types.py
 posteriors/utils.py
 posteriors.egg-info/PKG-INFO
 posteriors.egg-info/SOURCES.txt
 posteriors.egg-info/dependency_links.txt
 posteriors.egg-info/requires.txt
 posteriors.egg-info/top_level.txt
 posteriors/ekf/__init__.py
 posteriors/ekf/diag_fisher.py
 posteriors/laplace/__init__.py
 posteriors/laplace/dense_fisher.py
+posteriors/laplace/dense_ggn.py
 posteriors/laplace/diag_fisher.py
+posteriors/laplace/diag_ggn.py
 posteriors/sgmcmc/__init__.py
 posteriors/sgmcmc/sghmc.py
 posteriors/sgmcmc/sgld.py
 posteriors/vi/__init__.py
 posteriors/vi/diag.py
 tests/test_optim.py
 tests/test_torchopt.py
+tests/test_tree_utils.py
 tests/test_types.py
 tests/test_utils.py
```

### Comparing `posteriors-0.0.2/pyproject.toml` & `posteriors-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "posteriors"
-version = "0.0.2"
+version = "0.0.3"
 description = "Uncertainty quantification with PyTorch"
 readme = "README.md"
 requires-python =">=3.9"
 license = {text = "Apache-2.0"}
 authors = [
     {name = "Sam Duffield", email = "sam@normalcomputing.ai"},
 ]
```

### Comparing `posteriors-0.0.2/tests/test_optim.py` & `posteriors-0.0.3/tests/test_optim.py`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.2/tests/test_torchopt.py` & `posteriors-0.0.3/tests/test_torchopt.py`

 * *Files identical despite different names*

### Comparing `posteriors-0.0.2/tests/test_types.py` & `posteriors-0.0.3/tests/test_types.py`

 * *Files identical despite different names*

