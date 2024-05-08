# Comparing `tmp/UQPyL-2.0.1.tar.gz` & `tmp/UQPyL-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UQPyL-2.0.1.tar", last modified: Sat Apr 20 03:48:15 2024, max compression
+gzip compressed data, was "UQPyL-2.0.3.tar", last modified: Tue May  7 07:51:21 2024, max compression
```

## Comparing `UQPyL-2.0.1.tar` & `UQPyL-2.0.3.tar`

### file list

```diff
@@ -1,111 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.394303 UQPyL-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-20 03:47:54.000000 UQPyL-2.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-20 03:48:15.394303 UQPyL-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-20 03:47:54.000000 UQPyL-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.366304 UQPyL-2.0.1/UQPyL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.366304 UQPyL-2.0.1/UQPyL/DoE/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/DoE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/DoE/_lhs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/DoE/fast_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/DoE/full_fact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/DoE/lhs.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/DoE/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/DoE/sampler_ABC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/DoE/sobol_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.370303 UQPyL-2.0.1/UQPyL/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/optimization/_binary_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/optimization/_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/optimization/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/optimization/asmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/optimization/boxmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/optimization/ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/optimization/mo_asmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/optimization/nsga_ii.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/optimization/sce_ua.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.370303 UQPyL-2.0.1/UQPyL/problems/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20157 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/problems/multi_DTLZ.py
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/problems/multi_ZDT.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/problems/pratical_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/problems/problem_ABC.py
--rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/problems/single_Benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.370303 UQPyL-2.0.1/UQPyL/problems/utility_functions/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/problems/utility_functions/_NDsort.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/problems/utility_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/problems/utility_functions/_uniformPoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.370303 UQPyL-2.0.1/UQPyL/sensibility/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/sensibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/sensibility/delta_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/sensibility/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/sensibility/mars_sa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/sensibility/morris.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/sensibility/rbd_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/sensibility/rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/sensibility/sa_ABC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/sensibility/sobol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.374304 UQPyL-2.0.1/UQPyL/surrogates/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/BaggingEnsemble.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/BootstrapEnsemble.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/fully_connect_neural_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/gaussian_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.374304 UQPyL-2.0.1/UQPyL/surrogates/gp_kernels/
--rw-r--r--   0 runner    (1001) docker     (127)    13058 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/gp_kernels/Kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/gp_kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/kriging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.374304 UQPyL-2.0.1/UQPyL/surrogates/lasso_/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/lasso_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2178950 2024-04-20 03:48:08.000000 UQPyL-2.0.1/UQPyL/surrogates/lasso_/lasso_fast.c
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    54174 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/mars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.390303 UQPyL-2.0.1/UQPyL/surrogates/mars_/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/mars_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2557498 2024-04-20 03:48:08.000000 UQPyL-2.0.1/UQPyL/surrogates/mars_/_basis.c
--rw-r--r--   0 runner    (1001) docker     (127)  1897710 2024-04-20 03:48:09.000000 UQPyL-2.0.1/UQPyL/surrogates/mars_/_forward.c
--rw-r--r--   0 runner    (1001) docker     (127)  2484731 2024-04-20 03:48:11.000000 UQPyL-2.0.1/UQPyL/surrogates/mars_/_knot_search.c
--rw-r--r--   0 runner    (1001) docker     (127)   883375 2024-04-20 03:48:12.000000 UQPyL-2.0.1/UQPyL/surrogates/mars_/_pruning.c
--rw-r--r--   0 runner    (1001) docker     (127)  1609461 2024-04-20 03:48:13.000000 UQPyL-2.0.1/UQPyL/surrogates/mars_/_qr.c
--rw-r--r--   0 runner    (1001) docker     (127)  1284129 2024-04-20 03:48:14.000000 UQPyL-2.0.1/UQPyL/surrogates/mars_/_record.c
--rw-r--r--   0 runner    (1001) docker     (127)   279598 2024-04-20 03:48:14.000000 UQPyL-2.0.1/UQPyL/surrogates/mars_/_types.c
--rw-r--r--   0 runner    (1001) docker     (127)   570592 2024-04-20 03:48:14.000000 UQPyL-2.0.1/UQPyL/surrogates/mars_/_util.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.394303 UQPyL-2.0.1/UQPyL/surrogates/mars_/pyearth/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/mars_/pyearth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.394303 UQPyL-2.0.1/UQPyL/surrogates/mlp_utility/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/mlp_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/mlp_utility/_activation_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/mlp_utility/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/mo_surrogates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/polynomial_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/radial_basis_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.394303 UQPyL-2.0.1/UQPyL/surrogates/rbf_kernels/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/rbf_kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/rbf_kernels/base_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/rbf_kernels/cubic_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/rbf_kernels/gaussian_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/rbf_kernels/linear_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/rbf_kernels/multiquadric_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/rbf_kernels/thin_plate_spline_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/support_vector_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/surrogate_ABC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.394303 UQPyL-2.0.1/UQPyL/surrogates/svr_/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/svr_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/svr_/libsvm_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    68913 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/surrogates/svr_/svm.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.394303 UQPyL-2.0.1/UQPyL/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/utility/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/utility/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/utility/model_selections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/utility/polynomial_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-20 03:47:54.000000 UQPyL-2.0.1/UQPyL/utility/scalers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:48:15.366304 UQPyL-2.0.1/UQPyL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-20 03:48:15.000000 UQPyL-2.0.1/UQPyL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-20 03:48:15.000000 UQPyL-2.0.1/UQPyL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:48:15.000000 UQPyL-2.0.1/UQPyL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 03:48:15.000000 UQPyL-2.0.1/UQPyL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 03:48:15.000000 UQPyL-2.0.1/UQPyL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-20 03:47:54.000000 UQPyL-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 03:48:15.394303 UQPyL-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-20 03:47:54.000000 UQPyL-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.669001 UQPyL-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 07:50:58.000000 UQPyL-2.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-07 07:51:21.669001 UQPyL-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-07 07:50:58.000000 UQPyL-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.633001 UQPyL-2.0.3/UQPyL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.637001 UQPyL-2.0.3/UQPyL/DoE/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/DoE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/DoE/_lhs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/DoE/fast_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/DoE/full_fact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/DoE/lhs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/DoE/morris_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/DoE/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/DoE/sampler_ABC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/DoE/sobol_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.637001 UQPyL-2.0.3/UQPyL/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/_binary_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/asmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/boxmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/mo_asmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/moea_d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/nsga_ii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/pso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/sce_ua.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.637001 UQPyL-2.0.3/UQPyL/optimization/utility_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/utility_functions/_NDsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/utility_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/optimization/utility_functions/_uniformPoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.641001 UQPyL-2.0.3/UQPyL/problems/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19554 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/problems/multi_DTLZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/problems/multi_ZDT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/problems/pratical_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/problems/problem_ABC.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/problems/single_Benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.641001 UQPyL-2.0.3/UQPyL/problems/utility_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/problems/utility_functions/_NDsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/problems/utility_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/problems/utility_functions/_uniformPoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.641001 UQPyL-2.0.3/UQPyL/sensibility/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/sensibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/sensibility/delta_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/sensibility/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/sensibility/mars_sa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/sensibility/morris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/sensibility/rbd_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/sensibility/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/sensibility/sa_ABC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/sensibility/sobol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.641001 UQPyL-2.0.3/UQPyL/surrogates/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/BaggingEnsemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/BootstrapEnsemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/fully_connect_neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/gaussian_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.645001 UQPyL-2.0.3/UQPyL/surrogates/gp_kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/gp_kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/gp_kernels/base_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/gp_kernels/c_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/gp_kernels/dot_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/gp_kernels/matern_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/gp_kernels/rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/gp_kernels/rq_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.645001 UQPyL-2.0.3/UQPyL/surrogates/krg_kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/krg_kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/krg_kernels/base_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/krg_kernels/cubic_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/krg_kernels/exp_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/krg_kernels/guass_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11412 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/kriging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.645001 UQPyL-2.0.3/UQPyL/surrogates/lasso_/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/lasso_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2178950 2024-05-07 07:51:12.000000 UQPyL-2.0.3/UQPyL/surrogates/lasso_/lasso_fast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54186 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/mars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.665001 UQPyL-2.0.3/UQPyL/surrogates/mars_/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/mars_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2557498 2024-05-07 07:51:14.000000 UQPyL-2.0.3/UQPyL/surrogates/mars_/_basis.c
+-rw-r--r--   0 runner    (1001) docker     (127)  1897710 2024-05-07 07:51:15.000000 UQPyL-2.0.3/UQPyL/surrogates/mars_/_forward.c
+-rw-r--r--   0 runner    (1001) docker     (127)  2484731 2024-05-07 07:51:16.000000 UQPyL-2.0.3/UQPyL/surrogates/mars_/_knot_search.c
+-rw-r--r--   0 runner    (1001) docker     (127)   885800 2024-05-07 07:51:17.000000 UQPyL-2.0.3/UQPyL/surrogates/mars_/_pruning.c
+-rw-r--r--   0 runner    (1001) docker     (127)  1609461 2024-05-07 07:51:19.000000 UQPyL-2.0.3/UQPyL/surrogates/mars_/_qr.c
+-rw-r--r--   0 runner    (1001) docker     (127)  1284129 2024-05-07 07:51:20.000000 UQPyL-2.0.3/UQPyL/surrogates/mars_/_record.c
+-rw-r--r--   0 runner    (1001) docker     (127)   279598 2024-05-07 07:51:20.000000 UQPyL-2.0.3/UQPyL/surrogates/mars_/_types.c
+-rw-r--r--   0 runner    (1001) docker     (127)   570592 2024-05-07 07:51:20.000000 UQPyL-2.0.3/UQPyL/surrogates/mars_/_util.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.665001 UQPyL-2.0.3/UQPyL/surrogates/mars_/pyearth/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/mars_/pyearth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.665001 UQPyL-2.0.3/UQPyL/surrogates/mlp_utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/mlp_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/mlp_utility/_activation_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/mlp_utility/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/polynomial_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/radial_basis_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.665001 UQPyL-2.0.3/UQPyL/surrogates/rbf_kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/rbf_kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/rbf_kernels/base_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/rbf_kernels/cubic_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/rbf_kernels/gaussian_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/rbf_kernels/linear_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/rbf_kernels/multiquadric_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/rbf_kernels/thin_plate_spline_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/support_vector_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/surrogate_ABC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.665001 UQPyL-2.0.3/UQPyL/surrogates/svr_/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/svr_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/svr_/libsvm_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    68913 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/surrogates/svr_/svm.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.669001 UQPyL-2.0.3/UQPyL/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/utility/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/utility/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/utility/model_selections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/utility/polynomial_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-07 07:50:58.000000 UQPyL-2.0.3/UQPyL/utility/scalers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:51:21.633001 UQPyL-2.0.3/UQPyL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-07 07:51:21.000000 UQPyL-2.0.3/UQPyL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-07 07:51:21.000000 UQPyL-2.0.3/UQPyL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:51:21.000000 UQPyL-2.0.3/UQPyL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 07:51:21.000000 UQPyL-2.0.3/UQPyL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 07:51:21.000000 UQPyL-2.0.3/UQPyL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-07 07:50:58.000000 UQPyL-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:51:21.669001 UQPyL-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-07 07:50:58.000000 UQPyL-2.0.3/setup.py
```

### Comparing `UQPyL-2.0.1/LICENSE.md` & `UQPyL-2.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/PKG-INFO` & `UQPyL-2.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UQPyL
-Version: 2.0.1
+Version: 2.0.3
 Summary: A python package for parameter uncertainty quantification and optimization
 Author: wmtSky
 Author-email: wmtSky <wmtsky@hhu.edu.cn>
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,44 +14,76 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Uncertainty Quantification Python Laboratory <br> (UQPyL)
 
-**UQPyL:** The **Uncertainty Quantification Python Laboratory** provide a comprehensive workflow for parameter **uncertainty quantification** and **optimization** in computational numerical simulations. **UQPyL** offers an extensive suite of advanced methodologies(Sobol', Delta Test, EFAST, et al.) and algorithms (NSGA-II, ASMO, MO-ASMO, et al.). In summary, UQPyL consists of four core modules: 
-- Design of Experiments (DoE) 
-- Sensibility Analysis 
-- Optimization
-- Surrogate models
-
-The surrogate models Module can help to solve computational expensive problems caused by intensive numerical simulations.**
-
-Once you have clearly defined the problem you aim to address, you can employ all pre-prepared methods and algorithms to complete following task:
-* Uncertainty Quantification (UQ)
-* Parameter Optimization
-
-Moreover, the versatility of UQPyL allows researchers to craft their own methods or algorithms by incorporating its diverse range of surrogate models. Consequently, users can:
-- Evaluate the effectiveness of their custom-designed algorithms
-- Compare different methods and algorithms under specific problem scenarios
+**UQPyL:** The **Uncertainty Quantification Python Laboratory** provide comprehensive workflows tailored to the **Uncertainty Quantification** and **Optimization** for computational models and their associated applications (e.g. model calibration, resource scheduling, product design). 
 
-  **Website:** http://www.uq-pyl.com/ (**#TODO** it need to update now.) <br>
+The **main characteristics** of UQPyL includes:
+
+1. Implementation of widely used sensitivity analysis methodologies and optimization algorithms.
+
+2. Integration of diverse surrogate models equipped with tunable to solving computational expensive problems.
+
+3. Provision of a comprehensive suite of benchmark problems and practical case studies, enabling users to quick start.
+
+4. A modular and extensible architecture that encourages and facilitates the development of novel methods or algorithms by users, aligning with our commitment to openness and collaboration. (**We appreciate and welcome contributions**)
+
+ **Website:** http://www.uq-pyl.com/ (**#TODO** it need to update now.) <br>
   **Source Code:** https://github.com/smasky/UQPyL/ <br> 
   **Documentation:** **#TODO** <br>
   **Citing in your work:** **#TODO** <br>
 
+# Included Methods and Algorithms
+**Sensibility Analysis:** (all methods support for surrogate models)
+- Sobol'
+- Delta_test (DT)
+- extended Fourier Amplitude Sensitivity Test (eFAST)
+- Random Balance Designs - Fourier Amplitude Sensitivity Test
+- Multivariate Adaptive Regression Splines-Sensibility Analysis (MARS-SA)
+- Morris
+- Regional Sensitivity Analysis (RSA)
+
+**Optimization Algorithms:** (* indicates the use of surrogate models)
+- SCE-UA
+- Genetic Algorithm (GA)
+- Non-dominated Sorting Genetic Algorithm-II (NSGA-II)
+- AMSMO*
+- MO_ASMO*
+- MASTO* #TODO
+- AMSMO* #TODO
+
+**Surrogate Models:**
+- Full connect neural network (FNN)
+- Kriging (KRG)
+- Gaussian Process (GP)
+- Linear Regression (LR)
+- Polynomial Regression (PR)
+- Radial Basis Function (RBF)
+- Support Vector Machine (SVM)
+- Multivariate Adaptive Regression Splines (MARS)
+
 # Installation
 
-` pip install UQPyL ` (Recommend)
+Recommend (PyPi or Conda):
+
+```
+pip install UQPyL
 
-or
+conda install UQPyL
+```
 
-` git clone https://github.com/smasky/UQPyL.git `
+And also:
 
-` cd UQPyL` and ` pip install . `
+```
+git clone https://github.com/smasky/UQPyL.git 
+pip install . 
+```
 
 
 # Call for Contributions
 We appreciate and welcome contributions. Because, we only set up standard workflows here. More advanced quantification methods and optimization algorithms are waited for pulling to this project.
 
 ---
 # Contact:
```

### Comparing `UQPyL-2.0.1/UQPyL/DoE/_lhs.py` & `UQPyL-2.0.3/UQPyL/DoE/_lhs.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/DoE/fast_sampler.py` & `UQPyL-2.0.3/UQPyL/DoE/fast_sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import numpy as np
 
 from .sampler_ABC import Sampler
 
-class FAST_Sampler(Sampler):
+class FAST_Sequence(Sampler):
     '''
     The sample technique for FAST(Fourier Amplitude Sensitivity Test) method
     
     Parameters:
     M: int
         The interference parameter, i.e., the number of harmonics to sum in the
         Fourier series decomposition (defalut 4). 
         But, the number of sample must be greater than 4*M**2!
     
     Methods:
     __call__ or sample: Generate a sample for FAST method
     
     Examples:
-        >>> fast=FAST_Sampler()
-        >>> samples=fast(5, 4) or fast.sample(5,4)
-            
+        >>> fast_seq=FAST_Sequence()
+        >>> samples=fast_seq(5, 4) or fast_seq.sample(5,4)
+    
     '''
     def __init__(self, M: int=4):
         
         super().__init__()
         self.M=M
         
     def _generate(self, nt: int, nx: int) -> np.ndarray:
```

### Comparing `UQPyL-2.0.1/UQPyL/DoE/full_fact.py` & `UQPyL-2.0.3/UQPyL/DoE/full_fact.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             levels = [levels]*nx
         elif isinstance(levels, np.ndarray):
             levels = levels.ravel().tolist()
         
         if len(levels)!=nx:
             raise ValueError('The length of levels should be equal to nx or 1')
         
-        factor_levels = [np.linspace(0, 1, num=level + 1)[:level] for level in levels]
+        factor_levels = [np.linspace(0, 1, num=level)[:level] for level in levels]
                
         factor_combinations = list(product(*factor_levels))
        
         H = np.array(factor_combinations)
         
         return H
```

### Comparing `UQPyL-2.0.1/UQPyL/DoE/lhs.py` & `UQPyL-2.0.3/UQPyL/DoE/lhs.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/DoE/random.py` & `UQPyL-2.0.3/UQPyL/DoE/random.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from .sampler_ABC import Sampler
 
-class RANDOM(Sampler):
+class Random(Sampler):
     '''
     Random Design
     
     Method:
     __call__ or sample: Generate a random design
     
     Examples:
```

### Comparing `UQPyL-2.0.1/UQPyL/DoE/sampler_ABC.py` & `UQPyL-2.0.3/UQPyL/DoE/sampler_ABC.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/optimization/_binary_ga.py` & `UQPyL-2.0.3/UQPyL/optimization/_binary_ga.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import numpy as np
 
 class Binary_GA():
+    '''
+        Binary_GA for Delta Test
+    '''
     def __init__(self, evaluate, n_features, population_size=50, n_generations=100, crossover_rate=0.7, mutation_rate=0.01):
         self.population_size = population_size
         self.n_generations = n_generations
         self.crossover_rate = crossover_rate
         self.mutation_rate = mutation_rate
         self.n_features = n_features
         self.evaluate = evaluate
```

### Comparing `UQPyL-2.0.1/UQPyL/optimization/adam.py` & `UQPyL-2.0.3/UQPyL/optimization/adam.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/optimization/boxmin.py` & `UQPyL-2.0.3/UQPyL/optimization/boxmin.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/problems/__init__.py` & `UQPyL-2.0.3/UQPyL/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/problems/multi_DTLZ.py` & `UQPyL-2.0.3/UQPyL/problems/multi_DTLZ.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,16 @@
     disc_var: list
         Discrete variables of the problem.
     cont_var: list
         Continuous variables of the problem.
     '''
     def __init__(self, n_input:int =30, n_output: int=3, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None) -> None:
         
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
         if n_output!=3:
             raise ValueError("DTLZ1 is a three-objective optimization problem")
     
     def evaluate(self, X, unit=False):
         '''
         Perform the evaluation of the input variables X
         
@@ -115,21 +111,17 @@
         Lower bound of the problem.
     disc_var: list
         Discrete variables of the problem.
     cont_var: list
         Continuous variables of the problem.
     '''
     def __init__(self, n_input:int =30, n_output: int=3, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None) -> None:
+           
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
         
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
-        
-        self.disc_var=disc_var
-        self.cont_var=cont_var
         if n_output!=3:
             raise ValueError("DTLZ2 is a three-objective optimization problem")
     
     def evaluate(self, X, unit=False):
         '''
         Perform the evaluation of the input variables X
         
@@ -195,20 +187,16 @@
     disc_var: list
         Discrete variables of the problem.
     cont_var: list
         Continuous variables of the problem.
     '''
     def __init__(self, n_input:int =30, n_output: int=3, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None) -> None:
         
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
-        
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
+         
         if n_output!=3:
             raise ValueError("DTLZ3 is a three-objective optimization problem")
     
     def evaluate(self, X, unit=False):
         '''
         Perform the evaluation of the input variables X
         
@@ -270,20 +258,16 @@
     disc_var: list
         Discrete variables of the problem.
     cont_var: list
         Continuous variables of the problem.
     '''
     def __init__(self, n_input:int =30, n_output: int=3, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None) -> None:
         
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
         if n_output!=3:
             raise ValueError("DTLZ4 is a three-objective optimization problem")
     
     def evaluate(self, X, unit=False):
         '''
         Perform the evaluation of the input variables X
         
@@ -349,20 +333,16 @@
     disc_var: list
         Discrete variables of the problem.
     cont_var: list
         Continuous variables of the problem.
     '''
     def __init__(self, n_input:int =30, n_output: int=3, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None) -> None:
         
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
-        
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
+         
         if n_output!=3:
             raise ValueError("DTLZ5 is a three-objective optimization problem")
     
     def evaluate(self, X, unit=False):
         '''
         Perform the evaluation of the input variables X
         
@@ -430,20 +410,16 @@
     disc_var: list
         Discrete variables of the problem.
     cont_var: list
         Continuous variables of the problem.
     '''
     def __init__(self, n_input:int =30, n_output: int=3, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None) -> None:
         
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
         if n_output!=3:
             raise ValueError("DTLZ6 is a three-objective optimization problem")
     
     def evaluate(self, X, unit=False):
         '''
         Perform the evaluation of the input variables X
         
@@ -509,20 +485,16 @@
     disc_var: list
         Discrete variables of the problem.
     cont_var: list
         Continuous variables of the problem.
     '''
     def __init__(self, n_input:int =30, n_output: int=3, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None) -> None:
         
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
         if n_output!=3:
             raise ValueError("DTLZ6 is a three-objective optimization problem")
         
     def evaluate(self, X, unit=False):
         '''
         Perform the evaluation of the input variables X
         
@@ -561,17 +533,8 @@
         return R
     
     def get_PF(self):
         '''
         Return the pareto front of the problem.
         '''
         #TODO 
-        pass
-
-
-    
-
-    
-        
-        
-
-        
+        pass
```

### Comparing `UQPyL-2.0.1/UQPyL/problems/multi_ZDT.py` & `UQPyL-2.0.3/UQPyL/problems/multi_ZDT.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,15 @@
 # evolutionary algorithms: Empirical results, Evolutionary computation,
 # 2000, 8(2): 173-195.
 #--------------------------------------##
 class ZDT1(ProblemABC):
     
     def __init__(self, n_input:int =30, n_output: int=2, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None):
         
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
-        
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
         
         if n_output!=2:
             raise ValueError("ZDT1 is a bi-objective optimization problem")
     
     def evaluate(self, X, unit=False):
         
         X=self._check_2d(X)
@@ -49,20 +44,15 @@
         
         return R
 
 class ZDT2(ProblemABC):
     
     def __init__(self, n_input:int =30, n_output: int=2, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None):
         
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
-        
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
         
         if n_output!=2:
             raise ValueError("ZDT2 is a bi-objective optimization problem")
     
     def evaluate(self, X, unit=False):
         
         X=self._check_2d(X)
@@ -91,20 +81,15 @@
         
         return R
     
 class ZDT3(ProblemABC):
     
     def __init__(self, n_input:int =30, n_output: int=2, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None):
         
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
-        
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
         
         if n_output!=2:
             raise ValueError("ZDT4 is a bi-objective optimization problem")
     
     def evaluate(self, X, unit=False):
         
         X=self._check_2d(X)
@@ -138,20 +123,15 @@
         
         return R
 
 class ZDT4(ProblemABC):
     
     def __init__(self, n_input:int =30, n_output: int=2, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None):
        
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
-        
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
         
         if n_output!=2:
             raise ValueError("ZDT4 is a bi-objective optimization problem")
     
     def evaluate(self, X, unit=False):
         
         X=self._check_2d(X)
@@ -180,20 +160,15 @@
         
         return R
 
 class ZDT6(ProblemABC):
     
     def __init__(self, n_input:int =30, n_output: int=2, ub: Union[int,float,np.ndarray] =1, lb: Union[int,float,np.ndarray] =0,disc_var=None,cont_var=None):
         
-        self.n_input=n_input
-        self.n_output=n_output
-        self._set_ub_lb(ub,lb)
-        
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input, n_output, ub, lb, disc_var, cont_var)
         
         if n_output!=2:
             raise ValueError("ZDT6 is a bi-objective optimization problem")
     
     def evaluate(self, X, unit=False):
         
         X=self._check_2d(X)
@@ -209,15 +184,15 @@
         return Y
     
     def get_optimum(self, N):
         
         min=0.280775
         R=np.zeros((N,self.n_output))
         R[:,0]=np.linspace(min,1,N)
-        R[:,1]=1-np.sqrt(R[:,0])
+        R[:,1]=1-R[:,0]**2
         
         return R
     
     def get_PF(self):
         
         R=self.get_optimum(100)
```

### Comparing `UQPyL-2.0.1/UQPyL/problems/pratical_problem.py` & `UQPyL-2.0.3/UQPyL/problems/pratical_problem.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,21 +2,17 @@
 from typing import Callable
 
 from .problem_ABC import ProblemABC
 class Problem(ProblemABC):
     '''
     Class for creating practical problem
     '''
-    def __init__(self, func, dim, n_output, ub, lb):
-        super().__init__()
+    def __init__(self, func, n_input, n_output, ub, lb):
+        super().__init__(n_input, n_output, ub, lb)
         self._func=func
-        self.dim=dim
-        self.n_output=n_output
-        self.ub=ub
-        self.lb=lb
         
     def __check_func__(self,func):
         '''
         check the available of coupling function(algorithm and model)
         '''
         #TODO
         pass
```

### Comparing `UQPyL-2.0.1/UQPyL/problems/single_Benchmarks.py` & `UQPyL-2.0.3/UQPyL/problems/single_Benchmarks.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,22 +18,25 @@
         Dims->30;Ub->np.ones(1,30)*100;LB->np.ones(1,30)*-100
      
     Optimal:
         X*=0 0 0 ... 0
         F*=0
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =100,lb: Union[int,float,np.ndarray] =-100,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
     
     def evaluate(self, X: np.ndarray, unit=False) -> np.ndarray:
+        '''
+            Parameters:
+                X: np.ndarray
+                    the input data
+                unit: bool, default=False
+                    whether to transform X to the bound
+        '''
         X=self._check_2d(X)
         if unit:
             X=self._unit_X_transform_to_bound(np.atleast_2d(X))
         F=np.sum(X**2,axis=1).reshape(-1,1)      
         
         return F
 
@@ -49,20 +52,16 @@
         Dims->30;Ub->np.ones(1,30)*10;LB->np.ones(1,30)*-10
      
     Optimal:
         X*=0 0 0 ... 0
         F*=0
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =10,lb: Union[int,float,np.ndarray] =-10,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
         
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X))
         F=np.sum(np.abs(X),axis=1).reshape(-1,1)+np.prod(np.abs(X),axis=1).reshape(-1,1)
         return F
 
@@ -79,20 +78,16 @@
      
     Optimal:
         X*=0 0 0 ... 0
         F*=0
     '''
     
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =100,lb: Union[int,float,np.ndarray] =-100,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
         
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         F=0
         X=self._unit_X_transform_to_bound(np.atleast_2d(X))
         X=X**2
         for d in range(self.n_input):
@@ -111,20 +106,16 @@
         Dims->30;Ub->np.ones(1,30)*100;LB->np.ones(1,30)*-100
      
     Optimal:
         X*=0 0 0 ... 0
         F*=0
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =100,lb: Union[int,float,np.ndarray] =-100,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
         
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X))
         X=np.abs(X)
         F=np.max(X,axis=1).reshape(-1,1)
         return F
@@ -141,20 +132,16 @@
         Dims->30;Ub->np.ones(1,30)*30;LB->np.ones(1,30)*-30
      
     Optimal:
         X*=1 1 1 ... 1
         F*=0
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =30,lb: Union[int,float,np.ndarray] =-30,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
         
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X))    
         Temp1=100*np.square(X[:,1:]-np.square(X[:,:-1]))
         Temp2=np.square(X[:,:-1]-1)
         F=np.sum(Temp1+Temp2,axis=1).reshape(-1,1)
@@ -172,20 +159,16 @@
         Dims->30;Ub->np.ones(1,30)*100;LB->np.ones(1,30)*-100
      
     Optimal:
         X*=1 1 1 ... 1
         F*=0
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =100,lb: Union[int,float,np.ndarray] =-100,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
         
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X))     
         F=np.sum(np.square(np.floor(X)+0.5),axis=1).reshape(-1,1)
         
         return F
@@ -202,20 +185,16 @@
         Dims->30;Ub->np.ones(1,30)*1.28;LB->np.ones(1,30)*-1.28
      
     Optimal:
         X*=1 1 1 ... 1
         F*=0
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =1.28,lb: Union[int,float,np.ndarray] =-1.28,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
         
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X))  
         Temp=np.linspace(1,self.n_input,self.n_input)*np.power(X,4)
         F=np.sum(Temp,axis=1).reshape(-1,1)+np.random.random((Temp.shape[0],1))          
         return F
@@ -232,20 +211,16 @@
         Dims->30;Ub->np.ones(1,30)*500;LB->np.ones(1,30)*-500
      
     Optimal:
         X*=420.9687 420.9687 ... 420.9687
         F*=-12569.5
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =500,lb: Union[int,float,np.ndarray] =-500,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
         
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X)) 
         Temp=np.sin(np.sqrt(np.abs(X)))*X
         F=np.sum(Temp,axis=1).reshape(-1,1)*-1         
         return F
@@ -262,20 +237,16 @@
         Dims->30;Ub->np.ones(1,30)*5.12;LB->np.ones(1,30)*-5.12
      
     Optimal:
         X*=0 0 0 ... 0
         F*=0
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =5.12,lb: Union[int,float,np.ndarray] =-5.12,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
         
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X)) 
         F=np.sum(np.square(X)-10*np.cos(2*np.pi*X)+10,axis=1).reshape(-1,1)
         return F
 
@@ -292,20 +263,16 @@
         Dims->30;Ub->np.ones(1,30)*32;LB->np.ones(1,30)*-32
      
     Optimal:
         X*=0 0 0 ... 0
         F*=0
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =32,lb: Union[int,float,np.ndarray] =-32,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
     
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X)) 
         Temp1=np.exp(np.sqrt(np.sum(np.square(X),axis=1)/self.n_input)*-0.2)*-20
         Temp2=np.exp(np.sum(np.cos(2*np.pi*X),axis=1)/self.n_input)*-1+20+np.e  
         F=(Temp1+Temp2).reshape(-1,1)
@@ -323,20 +290,16 @@
         Dims->30;Ub->np.ones(1,30)*600;LB->np.ones(1,30)*-600
      
     Optimal:
         X*=0 0 0 ... 0
         F*=0
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =600,lb: Union[int,float,np.ndarray] =-600,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
     
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X)) 
         I=np.sqrt(np.atleast_2d(np.linspace(1,self.n_input,self.n_input)))
         F=np.sum(np.square(X), axis=1).reshape(-1,1)/4000-np.prod(np.cos(X/I),axis=1).reshape(-1,1)+1     
         return F
@@ -357,20 +320,16 @@
         Dims->30;Ub->np.ones(1,30)*(30^2);LB->np.ones(1,30)*-(30^2)
      
     Optimal:
         X_i^*=i(D+1-i),i=1,2,...,D
         F^*=-D(D+4)(D-1)/6
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =900,lb: Union[int,float,np.ndarray] =-900,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
     
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X))
         F=np.sum(np.square(X-1),axis=1).reshape(-1,1)-np.sum(X[:,1:]*X[:,:-1],axis=1).reshape(-1,1)
         return F
 
@@ -386,20 +345,16 @@
         Dims->30;Ub->np.ones(1,30)*10;LB->np.ones(1,30)*-10
      
     Optimal:
         X^*=0 0 0 ...0
         F^*=0
     '''
     def __init__(self, n_input: int =30, ub: Union[int,float,np.ndarray] =10, lb: Union[int,float,np.ndarray] =-10, disc_var=None, cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
     
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X))
         F=((X[:,0]**2)+np.sum(np.square(X[:,1:]),axis=1)*(10**6)).reshape(-1,1)
         return F
     
@@ -415,20 +370,16 @@
         Dims->30;Ub->np.ones(1,30)*10;LB->np.ones(1,30)*-10
      
     Optimal:
         X^*=0 0 0 ...0
         F^*=0
     '''
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =10,lb: Union[int,float,np.ndarray] =-10,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
     
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X))
         F=(X[:,0]**2*(10**6)+np.sum(np.square(X[:,1:]),axis=1)).reshape(-1,1)
         return F
     
@@ -448,20 +399,16 @@
         X^*=0 0 0 ...0
         F^*=0
     '''
     kMax=20
     a=0.5
     b=3
     def __init__(self, n_input:int =30, ub: Union[int,float,np.ndarray] =0.5,lb: Union[int,float,np.ndarray] =-0.5,disc_var=None,cont_var=None):
-        self.n_input=n_input
-        self._set_ub_lb(ub,lb)
-        self.n_output=1
         
-        self.disc_var=disc_var
-        self.cont_var=cont_var
+        super().__init__(n_input,1,ub,lb,disc_var,cont_var)
         
     def evaluate(self, X: np.ndarray) -> np.ndarray:
         
         X=self._unit_X_transform_to_bound(np.atleast_2d(X))
         K=np.atleast_2d(np.linspace(1,self.kMax,self.kMax))
         aK=np.power(self.a,K)
         bK=np.power(self.b,K)
```

### Comparing `UQPyL-2.0.1/UQPyL/problems/utility_functions/_NDsort.py` & `UQPyL-2.0.3/UQPyL/optimization/utility_functions/_NDsort.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/problems/utility_functions/_uniformPoint.py` & `UQPyL-2.0.3/UQPyL/problems/utility_functions/_uniformPoint.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/__init__.py` & `UQPyL-2.0.3/UQPyL/surrogates/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from . import rbf_kernels
 from . import gp_kernels
-from .surrogate_ABC import Surrogate
+from .surrogate_ABC import Surrogate, Mo_Surrogates
 from .linear_regression import LinearRegression
 from .gaussian_process import GPR
 from .radial_basis_function import RBF
 from .polynomial_regression import PolynomialRegression
 from .support_vector_machine import SVR
 from .fully_connect_neural_network import FNN
-from .kriging import Kriging as KRG
-from .mo_surrogates import MO_Surrogates
+from .kriging import KRG
 from .mars import MARS
 
 kernels=["rbf_kernels", "gp_kernels"]
 surrogates=["LinearRegression", "PolynomialRegression", "RBF", "Kriging", "MLP",
             "SVR", "GPR", "FNN", "KRG", "MARS"]
-utility=["MO_Surrogates", "Surrogate"]
+utility=["Mo_Surrogates", "Surrogate"]
 
 __all__=[
     kernels,
     surrogates,
     utility
 ]
```

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/fully_connect_neural_network.py` & `UQPyL-2.0.3/UQPyL/surrogates/fully_connect_neural_network.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/gaussian_process.py` & `UQPyL-2.0.3/UQPyL/surrogates/gaussian_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import numpy as np
 from scipy.linalg import cholesky, cho_solve, solve_triangular
-from typing import Callable, Tuple, Optional, Literal
+from typing import Tuple, Optional, Literal
 
-from .surrogate_ABC import Surrogate, Scale_T
-from .gp_kernels.Kernel import RBF, Matern, Kernel
+from .surrogate_ABC import Surrogate
+from .gp_kernels import RBF, Matern, Gp_Kernel
 from ..optimization import GA, Boxmin, MP_List, EA_List
 from ..utility.model_selections import RandSelect
 from ..utility.metrics import r2_score
 from ..utility.scalers import Scaler
 from ..utility.polynomial_features import PolynomialFeatures
 
 class GPR(Surrogate):
     
-    def __init__(self, scalers: Tuple[Optional[Scaler], Optional[Scaler]]=(None, None),
+    def __init__(self, kernel: Gp_Kernel, scalers: Tuple[Optional[Scaler], Optional[Scaler]]=(None, None),
                  poly_feature: PolynomialFeatures=None,
-                optimizer: Literal['Boxmin', 'GA']='Boxmin', n_restarts_optimizer: int=1,
-                fitMode: Literal['likelihood', 'predictError']='likelihood',
-                kernel: Optional[Kernel]=None, alpha: float=1e-10):
+                 optimizer: Literal['Boxmin', 'GA']='Boxmin', n_restarts_optimizer: int=1,
+                 fitMode: Literal['likelihood', 'predictError']='likelihood',
+                 alpha: float=1e-10):
+        
+        if not isinstance(kernel, Gp_Kernel):
+            raise TypeError("Variable kernel must be an instance of Gp_Kernel!")
         
         self.optimizer=optimizer
         self.fitMode=fitMode
         self.kernel=kernel
         self.alpha=alpha
         self.std=False
         self.n_restarts_optimizer=n_restarts_optimizer
```

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/gp_kernels/Kernel.py` & `UQPyL-2.0.3/UQPyL/surrogates/rbf_kernels/base_kernel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,459 +1,447 @@
 import numpy as np
+from scipy.spatial.distance import pdist,squareform
 import abc
-from typing import Any, Optional, Union
-from scipy.spatial.distance import pdist, squareform, cdist
-class Kernel():
+
+class Kernel(metaclass=abc.ABCMeta):
+    n_samples=None
+    n_features=None
     def __init__(self):
+        
         self._theta={}
         self._theta_ub={}
         self._theta_lb={}
     
-    def __check_array__(self, value: Union[float,np.ndarray]):
-        
+    def __check_array__(self, value):
+            
         if isinstance(value, float):
             value=np.array([value])
         elif isinstance(value, np.ndarray):
             if value.ndim>1:
                 value=value.ravel()
         else:
-            raise ValueError("Please make sure the type of value")
+            raise ValueError("Please make sure the used type (float or np.ndarray) of value")
         
         return value
+    
+    
+    def evaluate(self,pdist):
+        pass
+    
+    def get_A_Matrix(self,train_X):
+        dist=squareform(pdist(train_X,'euclidean'))
+        Phi=self.evaluate(dist)
+        
+        self.n_samples, self.n_features=train_X.shape
+        
+        S,Tail=self.get_Tail_Matrix(train_X)
+        if(S):
+            temp1=np.hstack((Phi,Tail))
+            t1=Tail.transpose()
+            t2=np.zeros((self.get_degree(self.n_features),self.get_degree(self.n_features)))
+            
+            temp2=np.hstack((Tail.transpose(),np.zeros((self.get_degree(self.n_features),self.get_degree(self.n_features)))))
+            A_Matrix=np.vstack((temp1,temp2))
+        else:
+            A_Matrix=Phi
+        return A_Matrix
+            
+    def get_Tail_Matrix(self,train_X): 
+        return (False,None)
+    
+    def get_degree(self,n_samples):
+        return None
+
+class Cubic(Kernel):
+    """
+        Cubic Kernel
+
+    """
+    name="Cubic"
+    def __init__(self):
+        
+        super().__init__()
+    
+    def evaluate(self, dist: np.ndarray):
         
-class RBF(Kernel):
+        return np.power(dist,3)
+    
+    def get_Tail_Matrix(self, train_X: np.ndarray):
+        Tail=np.ones((self.n_samples,self.n_features+1))
+        Tail[:self.n_samples,:self.n_features]=train_X.copy()
+        return (True,Tail)
+    
+    def get_degree(self, n_samples: int):
+        return n_samples+1
+    ##############################Attribute##########################
+    @property
+    def theta(self):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
+    
+    @theta.setter
+    def theta(self, value):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
+    
+    @property
+    def theta_ub(self):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
+    
+    @theta_ub.setter
+    def theta_ub(self, value):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
+    
+    @property
+    def theta_lb(self):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
+    
+    @theta_lb.setter
+    def theta_lb(self, value):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
+    
+class Gaussian(Kernel):
     """
-        RBF kernel
+        Gaussian Kernel
+        
+        theta: gamma
     """
-    def __init__(self, length_scale: Union[float, np.ndarray]=1.0,
-                 l_ub: Union[float, np.ndarray]=1e5,l_lb: Union[float, np.ndarray]=1e-5):
+    
+    name="Gaussian"
+    
+    def __init__(self, gamma: float=1.0, gamma_ub: float=1e5, gamma_lb: float=1e-5):
         
         super().__init__()
         
-        if not isinstance(l_ub, type(l_lb)) and not isinstance(length_scale, type(l_ub)):
-            raise ValueError("the type of length_scale, ub and lb is not consistent")
+        self.gamma=gamma
+        self.gamma_ub=gamma_ub
+        self.gamma_lb=gamma_lb
         
-        if isinstance(length_scale, float):
-            length_scale=np.array([length_scale])
-            l_lb=np.array([l_lb])
-            l_ub=np.array([l_ub])
-        
-        self.length_scale=length_scale
-        self.l_lb=l_lb
-        self.l_ub=l_ub
-
-    def __call__(self, trainX1: np.ndarray, trainX2: Optional[np.ndarray]=None):
+    def evaluate(self,dist):
         
-        if trainX2 is None:
-            dists=pdist(trainX1/self.length_scale, metric="sqeuclidean")
-            K=squareform(np.exp(-0.5*dists))
-            np.fill_diagonal(K,1.0)
-        else:
-            dists=cdist(trainX1/self.length_scale, trainX2/self.length_scale, metric="sqeuclidean")
-            K = np.exp(-0.5 * dists)
-        return K
+        return np.exp(-1*self.gamma*np.power(dist,2))
     
-    ##################################Attribute############################################
-    #--------------------------------length_scale----------------------------------------#
+    ###########################Attribute###################################
+    #----------------------------gamma------------------------------------#
     @property
-    def length_scale(self):
-        return self._length_scale
+    def gamma(self):
+        
+        return self._gamma
     
-    @length_scale.setter
-    def length_scale(self, value):
+    @gamma.setter
+    def gamma(self, value):
+        
         value=self.__check_array__(value)
-        self._length_scale=value
-        self._theta['length_scale']=value
+        self._gamma=value
+        self._theta['gamma']=value
     
     @property
-    def l_lb(self):
-        return self._l_lb
+    def gamma_ub(self):
+        
+        return self._gamma_ub
     
-    @l_lb.setter
-    def l_lb(self, value):
+    @gamma_ub.setter
+    def gamma_ub(self, value):
+        
         value=self.__check_array__(value)
-        self._l_lb=value
-        self._theta_lb['length_scale']=value
-    
+        self._gamma_ub=value
+        self._theta_ub['gamma']=value
+        
     @property
-    def l_ub(self):
-        return self._l_ub
+    def gamma_lb(self):
+        
+        return self._gamma_lb
     
-    @l_ub.setter
-    def l_ub(self, value):
+    @gamma_lb.setter
+    def gamma_lb(self, value):
+        
         value=self.__check_array__(value)
-        self._l_ub=value
-        self._theta_ub['length_scale']=value
-    #--------------------------------------theta-------------------------------------------#
+        self._gamma_lb=value
+        self._theta_lb['gamma']=value
+    #------------------------------theta--------------------------#
     @property
     def theta(self):
         return np.concatenate(list(self._theta.values()))
     
     @theta.setter
     def theta(self, value):
-        self.length_scale=value
+        self.gamma=value
     
     @property
     def theta_ub(self):
         return np.concatenate(list(self._theta_ub.values()))
     
     @theta_ub.setter
     def theta_ub(self, value):
-        self.l_ub=value
+        self.gamma_ub=value
     
     @property
     def theta_lb(self):
         return np.concatenate(list(self._theta_lb.values())) 
     
     @theta_lb.setter
     def theta_lb(self, value):
-        self.l_lb=value
+        self.gamma_lb=value
+    
+
+class Gaussian(Kernel):
+    
+    name="Gaussian"
+    
+    def __init__(self, gamma: float=1.0, gamma_ub: float=1e5, gamma_lb: float=1e-5):
         
-class Matern(Kernel):
-    """
-       Matern Kernel
-       
-       Parameters:
-       
-       nu: this parameter determine the smooth of the prediction
-       
-       length_scale:  a scaler or vector to determine the correlation of the input data
-       
-       ub, lb: the upper or lower bound of the length_scale
-       
-       Attribute:
-       
-       theta: the set of unknown parameters 
- 
-    """
-    def __init__(self, length_scale: Union[float, np.ndarray]=1.0,
-                 l_ub: Union[float, np.ndarray]=1e5, l_lb: Union[float, np.ndarray]=1e-5,
-                 nu: float=1.5):
-                
         super().__init__()
         
-        if not isinstance(l_ub, type(l_lb)) and not isinstance(length_scale, type(l_ub)):
-            raise ValueError("the type of length_scale, ub and lb is not consistent")
+        self.gamma=gamma
+        self.gamma_ub=gamma_ub
+        self.gamma_lb=gamma_lb
         
-        self.length_scale=length_scale
-        self.l_ub=l_ub
-        self.l_lb=l_lb
-        self.nu=nu
-    
-    def __call__(self, trainX1: np.ndarray, trainX2: Optional[np.ndarray]=None):
+    def evaluate(self,dist):
         
-        if trainX2 is None:
-            dists=pdist(trainX1/self.length_scale, metric="euclidean")
-        else:
-            dists = cdist(trainX1/self.length_scale, trainX2/self.length_scale, metric="euclidean")
-        if self.nu==0.5:
-            K=np.exp(-dists)
-        elif self.nu==1.5:
-            K=dists*np.sqrt(3)
-        elif self.nu==2.5:
-            K=dists*np.sqrt(5)
-            K=(1.0+K+K**2/3.0) * np.exp(-K)
-        elif self.nu==np.inf:
-            K=np.exp(-(dists**2)/2.0)
-        else:
-            ##TODO 
-            #gamma kv
-            raise ValueError("Current do not support other value of nu,\
-                             Please use 0.5, 1.5, 2.5, or np.inf.")
-        if trainX2 is None:
-            K=squareform(K)
-            np.fill_diagonal(K,1.0)
-        
-        return K
+        return np.exp(-1*self.gamma*np.power(dist,2))
     
-    ##################################Attribute########################################
-    #--------------------------------length_scale------------------------------------#
+    ###########################Attribute###################################
+    #----------------------------gamma------------------------------------#
     @property
-    def length_scale(self):
-        return self._length_scale
+    def gamma(self):
+        
+        return self._gamma
     
-    @length_scale.setter
-    def length_scale(self, value):
+    @gamma.setter
+    def gamma(self, value):
+        
         value=self.__check_array__(value)
-        self._length_scale=value
-        self._theta['length_scale']=value
+        self._gamma=value
+        self._theta['gamma']=value
     
     @property
-    def l_lb(self):
-        return self._l_lb
+    def gamma_ub(self):
+        
+        return self._gamma_ub
     
-    @l_lb.setter
-    def l_lb(self, value):
+    @gamma_ub.setter
+    def gamma_ub(self, value):
+        
         value=self.__check_array__(value)
-        self._l_lb=value
-        self._theta_lb['length_scale']=value
+        self._gamma_ub=value
+        self._theta_ub['gamma']=value
         
     @property
-    def l_ub(self):
-        return self._l_ub
+    def gamma_lb(self):
+        
+        return self._gamma_lb
     
-    @l_ub.setter
-    def l_ub(self, value):
+    @gamma_lb.setter
+    def gamma_lb(self, value):
+        
         value=self.__check_array__(value)
-        self._l_ub=value
-        self._theta_ub['length_scale']=value
-    #------------------------------------theta--------------------------------------#
+        self._gamma_lb=value
+        self._theta_lb['gamma']=value
+    #------------------------------theta--------------------------#
     @property
     def theta(self):
         return np.concatenate(list(self._theta.values()))
     
     @theta.setter
     def theta(self, value):
-        self.length_scale=value
+        self.gamma=value
     
     @property
     def theta_ub(self):
         return np.concatenate(list(self._theta_ub.values()))
     
     @theta_ub.setter
     def theta_ub(self, value):
-        self.l_ub=value
+        self.gamma_ub=value
     
     @property
     def theta_lb(self):
         return np.concatenate(list(self._theta_lb.values())) 
     
     @theta_lb.setter
     def theta_lb(self, value):
-        self.l_lb=value
-        
-class RationalQuadratic(Kernel):
+        self.gamma_lb=value
+
+class Linear(Kernel):
     """
-    Constant Kernel
+    Linear Kernel
+    """
+    name="Linear"
+    def evaluate(self,dist):
+        
+        return -dist
+    #TODO check the formula
+    def get_degree(self,n_samples):
+        
+        return 1
+    
+    def get_Tail_Matrix(self,train_X):
+        
+        return (True,np.ones((train_X.shape[0],1)))
+    
+    ###########################Attribute###################################
+    @property
+    def theta(self):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
+    
+    @theta.setter
+    def theta(self, value):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
+    
+    @property
+    def theta_ub(self):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
     
-    Attribute:
+    @theta_ub.setter
+    def theta_ub(self, value):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
     
-    theta: the set of unknown parameters. np.vstack(length_scale, alpha)
+    @property
+    def theta_lb(self):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
+    
+    @theta_lb.setter
+    def theta_lb(self, value):
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
 
+class Multiquadric(Kernel):
+    """
+    Multiquaric kernel
+    
     """
-    def __init__(self, length_scale: float=1.0, l_ub: float=10.0, l_lb:float=0.0, 
-                 alpha: float=1.0, alpha_ub: float=1e5, alpha_lb: float=1e-5):
+    name="Multiquadric"
+    def __init__(self, gamma: float=1.0, gamma_ub: float=1e5, gamma_lb: float=1e-5):
         
         super().__init__()
-        if not isinstance(l_ub, type(l_lb)) and not isinstance(length_scale, type(l_ub)):
-            raise ValueError("the type of length_scale, ub and lb is not consistent")
         
-        # if not isinstance(l_ub, float):
-        #     raise ValueError("the RationalQuadratic Kernel only support scale length_scale")
+        self.gamma=gamma
+        self.gamma_ub=gamma_ub
+        self.gamma_lb=gamma_lb
         
-        self.length_scale=length_scale
-        self.l_ub=l_ub; self.l_lb=l_lb
-        self.alpha=alpha
-        self.alpha_ub=alpha_ub;self.alpha_lb=alpha_lb
-   
-    def __call__(self, trainX: np.ndarray, trainY: Optional[np.ndarray]=None):
-        
-        if trainY is None:
-            dists=squareform(pdist(trainX, metric="sqeuclidean"))
-            tmp= dists / (2*self.alpha* self.length_scale**2)
-            base=1 + tmp
-            K=base**-self.alpha
-            np.fill_diagonal(K,1)
-        else:
-            dists=cdist(trainX, trainY, metric="sqeuclidean")
-            K= (1+dists / (2* self.alpha * self.length_scale**2)) ** -self.alpha
+    def evaluate(self,dist):
         
-        return K
-    #################################Attributes##########3########################
-    #------------------------------length_scale-----------------------------------#
-    @property
-    def length_scale(self):
-        return self._length_scale
-    
-    @length_scale.setter
-    def length_scale(self, value):
-        value=self.__check_array__(value)
-        self._length_scale=value.copy()
-        self._theta['length_scale']=value.copy()
+        return np.sqrt(np.power(dist,2)+self.gamma*self.gamma)
+
+    def get_degree(self,n_samples):
         
-    @property
-    def l_ub(self):
-        return self._l_ub
+        return 1
     
-    @l_ub.setter
-    def l_ub(self, value):
-        value=self.__check_array__(value)
-        self._l_ub=value
-        self._theta_ub['length_scale']=value
+    def get_Tail_Matrix(self,train_X):
         
+        return (True,np.ones((train_X.shape[0],1)))
+    ###########################Attribute###################################
+    #----------------------------gamma------------------------------------#
     @property
-    def l_lb(self):
-        return self._l_lb
+    def gamma(self):
+        
+        return self._gamma
     
-    @l_lb.setter
-    def l_lb(self, value):
+    @gamma.setter
+    def gamma(self, value):
+        
         value=self.__check_array__(value)
-        self._l_lb=value
-        self._theta_lb['length_scale']=value
-    #---------------------------------alpha-----------------------------------#
-    @property
-    def alpha(self):
-        return self._alpha
+        self._gamma=value
+        self._theta['gamma']=value
     
-    @alpha.setter
-    def alpha(self, value):
-        value=self.__check_array__(value)
-        self._alpha=value
-        self._theta['alpha']=value
-
     @property
-    def alpha_ub(self):
-        return self._alpha_ub
+    def gamma_ub(self):
+        
+        return self._gamma_ub
     
-    @alpha_ub.setter
-    def alpha_ub(self, value):
+    @gamma_ub.setter
+    def gamma_ub(self, value):
+        
         value=self.__check_array__(value)
-        self._alpha_ub=value
-        self._theta_ub['alpha']=value
-    
+        self._gamma_ub=value
+        self._theta_ub['gamma']=value
+        
     @property
-    def alpha_lb(self):
-        return self._alpha_lb
+    def gamma_lb(self):
+        
+        return self._gamma_lb
     
-    @alpha_lb.setter
-    def alpha_lb(self, value):
+    @gamma_lb.setter
+    def gamma_lb(self, value):
+        
         value=self.__check_array__(value)
-        self._theta_lb['alpha']=value
-        self._alpha_lb=value
-    #--------------------------------theta----------------------------------#
+        self._gamma_lb=value
+        self._theta_lb['gamma']=value
+    #----------------------------------theta----------------------------#
     @property
     def theta(self):
         return np.concatenate(list(self._theta.values()))
     
     @theta.setter
     def theta(self, value):
-        self.alpha=value[-1]
-        self.length_scale=value[:-1]
+        self.gamma=value
     
     @property
     def theta_ub(self):
         return np.concatenate(list(self._theta_ub.values()))
     
     @theta_ub.setter
     def theta_ub(self, value):
-        self.alpha_ub=value[-1]
-        self.l_ub=value[:-1]
+        self.gamma_ub=value
     
     @property
     def theta_lb(self):
-        return np.concatenate(list(self._theta_lb.values()))
+        return np.concatenate(list(self._theta_lb.values())) 
     
     @theta_lb.setter
     def theta_lb(self, value):
-        self.alpha_lb=value[-1]
-        self.l_lb=value[:-1]
-        
-class Constant(Kernel):
-    """
-    Constant
-    """
-    def __init__(self, c: float=1.0):
-        self.c=c
-    
-    def setHyperPara(self, theta: np.ndarray):
-        self.c=theta[0]
-    
-    def __call__(self, trainX: np.ndarray, trainY: Optional[np.ndarray]=None):
-    
-        if trainY is None:
-            K=np.ones((trainX.shape[0],trainY.shape[0]))*self.c
-        else:
-            K=np.ones((trainX.shape[0], trainX.shape[0]))*self.c
-        
-        return K
+        self.gamma_lb=value
 
-class DotProduct(Kernel):
+class Thin_plate_spline(Kernel):
     """
-    Dot-Product Kernel
     
-    """
+    Thin_plate_spline
     
-    def __init__(self, sigma: float=1.0, sigma_ub: float=1e5, sigma_lb=1e-5):
-        
+    """
+    name="Thin_plate_spline"
+    def __init__(self):
         super().__init__()
-        
-        self.sigma=sigma
-        self.sigma_ub=sigma_ub
-        self.sigma_lb=sigma_lb
     
-    def __call__(self, trainX, trainY: Optional[np.ndarray]=None):
-        
-        if trainY is None:
-            K=np.inner(trainX, trainX) + self.sigma**2
-        else:
-            K=np.inner(trainX, trainY) + self.sigma**2
+    def evaluate(self,dist):
         
-        return K
-    #################################Attributes##################################
-    #--------------------------------sigma--------------------------------------#
-    @property
-    def sigma(self):
-        return self._sigma
+        dist[dist < np.finfo(float).eps] = np.finfo(float).eps
+        return np.power(dist,2)*np.log(dist)
     
-    @sigma.setter
-    def sigma(self, value):
-        value=self.__check_array__(value)
-        self._sigma=value
-        self._theta['sigma']=value
-    
-    @property
-    def sigma_ub(self):
-        return self._sigma_ub
-    
-    @sigma_ub.setter
-    def sigma_ub(self, value):
-        value=self.__check_array__(value)
-        self._sigma_ub=value
-        self._theta_ub['sigma']=value
+    def get_Tail_Matrix(self,train_X):
+        
+        Tail=np.ones((self.n_samples,self.n_features+1))
+        Tail[:self.n_samples,:self.n_features]=train_X.copy()
+        return (True,Tail)
     
-    @property
-    def sigma_lb(self):
-        return self._sigma_lb
+    def get_degree(self,n_samples):
+        
+        return n_samples+1
     
-    @sigma_lb.setter
-    def sigma_lb(self, value):
-        value=self.__check_array__(value)
-        self._sigma_lb=value
-        self._theta_lb['sigma']=value
-    #--------------------------------theta--------------------------------------#
+    ###########################Attribute###################################
     @property
     def theta(self):
-        return np.concatenate(list(self._theta.values()))
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
     
     @theta.setter
     def theta(self, value):
-        self.sigma=value
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
     
     @property
     def theta_ub(self):
-        return np.concatenate(list(self._theta_ub.values()))
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
     
     @theta_ub.setter
     def theta_ub(self, value):
-        self.sigma_ub=value
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
     
     @property
     def theta_lb(self):
-        return np.concatenate(list(self._theta_lb.values()))
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
     
     @theta_lb.setter
     def theta_lb(self, value):
-        self.sigma_lb=value
+        raise ValueError("There is no hyper-parameters in Cubic kernel")
     
     
     
     
-     
     
-
-
-         
             
-        
-        
-        
-    
+    
+
```

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/kriging.py` & `UQPyL-2.0.3/UQPyL/surrogates/kriging.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from scipy.linalg import LinAlgError, cholesky, qr, lstsq
 from scipy.spatial.distance import pdist
 from typing import Literal, Tuple, Optional, Union
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 from .surrogate_ABC import Surrogate, Scale_T
+from .krg_kernels import Krg_Kernel
 from ..utility.metrics import r2_score
 from ..optimization import Boxmin, GA, MP_List, EA_List
 from ..utility.model_selections import RandSelect
 from ..utility.scalers import Scaler
 from ..utility.polynomial_features import PolynomialFeatures
 from ..problems import Problem
 
@@ -34,35 +35,36 @@
     for k in np.arange(1, n_feature + 1):
         F[:, j + np.arange(q)] = np.tile(S[:, (k - 1):k],
                                             (1, q)) * S[:, np.arange(k - 1, n_feature)]
         j += q;q -= 1
     return F
 
 ###-------------------------kernerls---------------------------###
-def guass(theta, d):
+# def guass(theta, d):
         
-    td = d * -theta
-    r = np.exp(np.sum(d * td, axis=1))
+#     td = d * -theta
+#     r = np.exp(np.sum(d * td, axis=1))
     
-    return r
+#     return r
 
-def exp(theta, d):
-    td= -theta
-    r= np.exp(np.sum(d*td, axis=1))
-    
-    return r
-def cubic(theta, d):
-    td=np.sum(d*theta, axis=1)
-    ones=np.ones(td.shape)
-    td=np.minimum(ones, td)
-    r=1-3*td**2+2*td**3
-    return r
+# def exp(theta, d):
+#     td= -theta
+#     r= np.exp(np.sum(d*td, axis=1))
+    
+#     return r
+# def cubic(theta, d):
+#     td=np.sum(d*theta, axis=1)
+#     ones=np.ones(td.shape)
+#     td=np.minimum(ones, td)
+#     r=1-3*td**2+2*td**3
+#     return r
+
+# K={"GAUSSIAN": guass, "EXP": exp, "CUBIC": cubic}
 
-K={"GAUSSIAN": guass, "EXP": exp, "CUBIC": cubic}
-class Kriging(Surrogate):
+class KRG(Surrogate):
     """
     A Kriging implementation based on python env includes the new training method(prediction error), 
     from the DACE toolbox(MATLAB).
     
     parameters:
     
     theta0: initial theta
@@ -87,34 +89,34 @@
                 *'predictError' new way
     
     normalized: the sign to normalize input data(x, y) or not
     
     Scale_type: the normalized method, containing:
             *'StandardScaler'
             *'MaxminScaler'
-    
+            
     """
-    def __init__(self, theta0: np.ndarray, ub: np.ndarray, lb: np.ndarray,
+    def __init__(self, kernel: Krg_Kernel,
                  regression: Literal['poly0','poly1','poly2']='poly0',
                  optimizer: Literal['Boxmin', 'GA'] = 'Boxmin', 
                  fitMode: Literal['likelihood', 'predictError']='likelihood',
                  scalers: Tuple[Optional[Scaler], Optional[Scaler]]=(None, None),
                  poly_feature: PolynomialFeatures=None,
-                 kernel: Literal['gaussian', 'exp', 'cubic']='gaussian',
                  n_restart_optimize: int=1):
         
         self.regression=regression
         self.optimizer=optimizer
         self.fitMode=fitMode
-        self.theta0=theta0
-        self.ub=ub
-        self.lb=lb
         self.n_restart_optimize=n_restart_optimize
         self.OPFunc=None
-        self.kernelFunc=K[kernel.upper()]
+        
+        if not isinstance(kernel, Krg_Kernel):
+            raise ValueError("The kernel must be the instance of Krg_Kernel")
+        
+        self.kernel=kernel
         
         if(regression=='poly0'):
             self.regrFunc=regrpoly0
         elif(regression=='poly1'):
             self.regrFunc=regrpoly1
         elif(regression=='poly2'):
             self.regrFunc=regrpoly2
@@ -125,23 +127,28 @@
 
     def predict(self,predictX: np.ndarray, only_value=True) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
         
         predictX=self.__X_transform__(predictX)
         n_sample, n_feature=self.trainX.shape
         n_pre,_=predictX.shape
         
+        
+        
+        #TODO
         dx = np.zeros((n_pre * n_sample, n_feature))
         kk = np.arange(n_sample)
 
         for k in np.arange(n_pre):
             dx[kk, :] = predictX[k, :] - self.trainX
             kk = kk + n_sample
+        ####################
         
         F=self.regrFunc(predictX)
-        r = np.reshape(self.kernelFunc(self.theta, dx),(n_sample, n_pre), order='F')
+        # self.kernel.theta=self.fitPar['theta'] #TODO
+        r = np.reshape(self.kernel(dx),(n_sample, n_pre), order='F')
         sy = F @ self.fitPar['beta'] + (self.fitPar['gamma'] @ r).T
         
         predictY=self.__Y_inverse_transform__(sy)
 
         #mse
         rt=lstsq(self.fitPar['C'], r)[0]
         u = lstsq(self.fitPar['G'],
@@ -152,14 +159,19 @@
             return predictY
         else:
             return predictY, mse
     
     def fit(self, trainX: np.ndarray, trainY: np.ndarray):
         
         self.trainX, self.trainY=self.__check_and_scale__(trainX, trainY)
+        
+        _, n_feature=self.trainX.shape
+        self.kernel.n_input=n_feature
+        self.theta0=self.kernel.theta
+        
         if(self.fitMode=='likelihood'):
             self._fit_likelihood()
         elif(self.fitMode=='predictError'):
             self._fit_predict_error()
             
 ###-------------------private functions----------------------###
 
@@ -173,99 +185,101 @@
         
         testX=TotalX[test,:];testY=TotalY[test,:]
         trainX=TotalX[train,:];trainY=TotalY[train,:]
         self.F, self.D=self._initialize(trainX)
         
         if self.optimizer in MP_List: 
             ###Using Mathematical Programming
-            self.OPModel=eval(self.optimizer)(self.theta0, self.ub, self.lb)
+            self.OPModel=eval(self.optimizer)(self.theta0, self.kernel.theta_ub, self.kernel.theta_lb)
 
             #Wrap _objFunc
             if not self.OPFunc:
                 def objFunc(theta):
                     self.trainY=trainY
                     self.trainX=trainX
                     self._objFunc(theta,record=True)
-                    self.theta=theta
-                    predictY,_=self.predict(self.X_scaler.inverse_transform(testX))
-                    obj=-1*r2_score(self.Y_scaler.inverse_transform(testY),predictY)
+                    self.kernel.theta=theta
+                    predictY=self.predict(self.__X_inverse_transform__(testX))
+                    obj=-1*r2_score(self.__Y_inverse_transform__(testY),predictY)
                     return obj
                 
                 self.OPFunc=objFunc
             bestTheta, obj=self.OPModel.run(self.OPFunc)
-            self.theta=bestTheta
+            self.kernel.theta=bestTheta
+            
         elif self.optimizer in EA_List:
             ###Using Evolutionary Algorithm
             if not self.OPFunc:
                 def objFunc(thetas):
                     self.trainY=trainY
                     self.trainX=trainX
                     objs=np.zeros(thetas.shape[0])
                     for i,theta in enumerate(thetas):
                         self._objFunc(np.power(np.e,theta),record=True)
-                        self.theta=np.power(np.e,theta).ravel()
-                        predictY=self.predict(self.X_scaler.inverse_transform(testX))
-                        objs[i]=-1*r2_score(self.Y_scaler.inverse_transform(testY),predictY)
+                        self.kernel.theta=np.power(np.e,theta).ravel()
+                        #TODO
+                        predictY=self.predict(self.__X_inverse_transform__(testX))
+                        objs[i]=-1*r2_score(self.__Y_inverse_transform__(testY),predictY)
                     return objs.reshape(-1,1)
                 self.OPFunc=objFunc
                 
-            problem=Problem(self.OPFunc, self.theta0.size, 1, np.log(self.ub), np.log(self.lb))
+            problem=Problem(self.OPFunc, self.theta0.size, 1, np.log(self.kernel.theta_ub), np.log(self.kernel.theta_lb))
             
             self.OPModel=eval(self.optimizer)(problem, 50)
 
             bestObj=np.inf
             bestTheta=None
             for _ in range(self.n_restart_optimize):
                 theta, obj=self.OPModel.run()
                 if obj<bestObj:
                     bestTheta=theta
                     bestObj=obj
-            self.theta=np.power(np.e,bestTheta).ravel()
+            self.kernel.theta=np.power(np.e,bestTheta).ravel()
         #reset
         self.OPFunc=None
         self.trainY=TotalY
         self.trainX=TotalX
         self.F, self.D=self._initialize(self.trainX)
-        self._objFunc(self.theta,record=True)
-               
+        self._objFunc(self.kernel.theta,record=True)
+        
     def _fit_likelihood(self):
         
         trainX=self.trainX
         trainY=self.trainY
         self.F, self.D=self._initialize(trainX)
         
         if self.optimizer in MP_List:
             ###Using Mathematical Programming
-            self.OPModel=eval(self.optimizer)(self.theta0, self.ub, self.lb)
+            self.OPModel=eval(self.optimizer)(self.theta0, self.kernel.theta_ub, self.kernel.theta_lb)
             bestTheta, _ =self.OPModel.run(self._objFunc)
-            self.theta=bestTheta
+            self.kernel.theta=bestTheta
             
         elif self.optimizer in EA_List:
             ###Using Evolutionary Algorithm
             def objFunc(thetas):
                 self.trainY=trainY
                 self.trainX=trainX
                 objs=np.zeros(thetas.shape[0])
                 for i,theta in enumerate(thetas):
                     objs[i]=self._objFunc(np.power(np.e,theta), record=False)
                 return objs.reshape(-1,1)
-            problem=Problem(objFunc, self.theta0.size, 1, np.log(self.ub), np.log(self.lb), )
+            problem=Problem(objFunc, self.theta0.size, 1, np.log(self.kernel.theta_ub), np.log(self.kernel.theta_lb), )
             self.OPModel=eval(self.optimizer)(problem, 50)
             
             for _ in range(self.n_restart_optimize):
                 bestObj=np.inf
                 bestTheta=None
                 theta, obj=self.OPModel.run()
                 if obj<bestObj:
                     bestTheta=theta
                     bestObj=obj
                     
-            self.theta=np.power(np.e,bestTheta)
+            self.kernel.theta=np.power(np.e,bestTheta)
         # Record coef
-        self._objFunc(self.theta,record=True)
+        self._objFunc(self.kernel.theta,record=True)
         
     def _initialize(self, trainX: np.ndarray):
         
         n_sample, n_feature=trainX.shape
         
         D = np.zeros((int((n_sample*(n_sample-1)/2)), n_feature))
         for k in range(n_feature):
@@ -278,15 +292,18 @@
         return F, D
     
     def _objFunc(self,theta,record=False):
         
         obj=np.inf
         
         m=self.F.shape[0]
-        r=self.kernelFunc(theta, self.D)
+        #set theta to kernel
+        self.kernel.theta=theta
+        
+        r=self.kernel(self.D)
         
         mu = (10 + m) * np.spacing(1)
         R = np.triu(np.ones((m, m)), 1)
         R[R == 1.0] = r
         np.fill_diagonal(R, 1.0 + mu)
         try:
             C = cholesky(R).T
```

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/lasso_/lasso_fast.c` & `UQPyL-2.0.3/UQPyL/surrogates/lasso_/lasso_fast.c`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/linear_regression.py` & `UQPyL-2.0.3/UQPyL/surrogates/linear_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,39 +13,39 @@
     Support three type:
     'Origin'-------'Least Square Method'
     'Ridge'--------'Ridge'
     'Lasso'--------'Lasso'
     '''
     def __init__(self, scalers: Tuple[Optional[Scaler], Optional[Scaler]]=(None, None),
                  poly_feature: PolynomialFeatures=None,
-                 Type: Literal['Origin', 'Ridge', 'Lasso']='Origin',
+                 loss_type: Literal['Origin', 'Ridge', 'Lasso']='Origin',
                  fit_intercept: bool= True, alpha: float=0.1,
                  epoch: int=100, lr: float=1e-5, tl: float=1e-5):
         
         
-        self.type=Type
+        self.loss_type=loss_type
         self.fit_intercept=fit_intercept
         self.alpha=alpha
         self.epoch=epoch
         self.lr=lr
         self.tl=tl
         
         super().__init__(scalers, poly_feature)
         
 ###---------------------------------public function---------------------------------------###
 
     def fit(self, trainX: np.ndarray, trainY: np.ndarray):
         
         trainX, trainY=self.__check_and_scale__(trainX, trainY)
         
-        if self.type=='Origin':
+        if self.loss_type=='Origin':
             self._fit_Origin(trainX, trainY)
-        elif self.type=='Ridge':
+        elif self.loss_type=='Ridge':
             self._fit_Ridge(trainX, trainY)
-        elif self.type=='Lasso':
+        elif self.loss_type=='Lasso':
             self._fit_Lasso(trainX, trainY)
         else:
             raise ValueError('Using wrong model type!')
         
     # def predict(self, predict_X: np.ndarray) -> np.ndarray:
         
     #     predict_X=self.__X_transform__(predict_X)
@@ -58,15 +58,15 @@
         
         predict_X=self.__X_transform__(predict_X)
         
         if(self.fit_intercept):
             predict_Y=predict_X@self.coef_+self.intercept_
         else:
             predict_Y=predict_X@self.coef_
-        
+        predict_Y=predict_Y.reshape(-1,1)
         return self.__Y_inverse_transform__(predict_Y)
     
 ###--------------------------private functions----------------------------###
 
     def _fit_Origin(self, trainX: np.ndarray, trainY: np.ndarray):
         
         trainX_=trainX.copy()
```

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/mars.py` & `UQPyL-2.0.3/UQPyL/surrogates/mars.py`

 * *Files 0% similar despite different names*

```diff
@@ -911,15 +911,15 @@
             weighted_y = y.copy()
             weighted_y *= np.sqrt(w[:, np.newaxis])
 
             # Compute the mse0
             mse0 += np.sum((weighted_y[:, i] -
                             np.average(weighted_y[:, i])) ** 2)
 
-            coef, resid = np.linalg.lstsq(B, weighted_y[:, i])[0:2]
+            coef, resid = np.linalg.lstsq(B, weighted_y[:, i], rcond=None)[0:2]
             self.coef_.append(coef)
             if not resid:
                 resid = np.array(
                     [np.sum((np.dot(B, coef) - weighted_y[:, i]) ** 2)])
             resid_.append(resid)
         resid_ = np.array(resid_)
         self.coef_ = np.array(self.coef_)
```

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/mars_/_basis.c` & `UQPyL-2.0.3/UQPyL/surrogates/mars_/_basis.c`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/mars_/_forward.c` & `UQPyL-2.0.3/UQPyL/surrogates/mars_/_forward.c`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/mars_/_knot_search.c` & `UQPyL-2.0.3/UQPyL/surrogates/mars_/_knot_search.c`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/mars_/_pruning.c` & `UQPyL-2.0.3/UQPyL/surrogates/mars_/_pruning.c`

 * *Files 1% similar despite different names*

```diff
@@ -3781,14 +3781,15 @@
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_lstsq[] = "lstsq";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_prune[] = "prune";
 static const char __pyx_k_range[] = "range";
+static const char __pyx_k_rcond[] = "rcond";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_state[] = "state";
 static const char __pyx_k_trace[] = "trace";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_dict_2[] = "_dict";
 static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_import[] = "__import__";
@@ -4099,14 +4100,15 @@
   PyObject *__pyx_n_s_pyx_checksum;
   PyObject *__pyx_n_s_pyx_result;
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_pyx_type;
   PyObject *__pyx_n_s_pyx_unpickle_PruningPasser;
   PyObject *__pyx_n_s_pyx_vtable;
   PyObject *__pyx_n_s_range;
+  PyObject *__pyx_n_s_rcond;
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_rss;
   PyObject *__pyx_n_s_run;
   PyObject *__pyx_n_s_sample_weight;
   PyObject *__pyx_n_s_self;
@@ -4305,14 +4307,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_PruningPasser);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_vtable);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
+  Py_CLEAR(clear_module_state->__pyx_n_s_rcond);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_rss);
   Py_CLEAR(clear_module_state->__pyx_n_s_run);
   Py_CLEAR(clear_module_state->__pyx_n_s_sample_weight);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
@@ -4489,14 +4492,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_PruningPasser);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_vtable);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
+  Py_VISIT(traverse_module_state->__pyx_n_s_rcond);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_rss);
   Py_VISIT(traverse_module_state->__pyx_n_s_run);
   Py_VISIT(traverse_module_state->__pyx_n_s_sample_weight);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
@@ -4781,14 +4785,15 @@
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
 #define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
 #define __pyx_n_s_pyx_unpickle_PruningPasser __pyx_mstate_global->__pyx_n_s_pyx_unpickle_PruningPasser
 #define __pyx_n_s_pyx_vtable __pyx_mstate_global->__pyx_n_s_pyx_vtable
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
+#define __pyx_n_s_rcond __pyx_mstate_global->__pyx_n_s_rcond
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_rss __pyx_mstate_global->__pyx_n_s_rss
 #define __pyx_n_s_run __pyx_mstate_global->__pyx_n_s_run
 #define __pyx_n_s_sample_weight __pyx_mstate_global->__pyx_n_s_sample_weight
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
@@ -8086,15 +8091,15 @@
       goto __pyx_L7;
     }
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":98
  *                 self.basis.weighted_transform(X, missing, B, sample_weight[:, 0])
  *             else:
  *                 self.basis.weighted_transform(X, missing, B, sample_weight[:, p])             # <<<<<<<<<<<<<<
- *             beta, mse_ = np.linalg.lstsq(B[:, 0:(basis_size)], weighted_y)[0:2]
+ *             beta, mse_ = np.linalg.lstsq(B[:, 0:(basis_size)], weighted_y, rcond=None)[0:2]
  *             if mse_:
  */
     /*else*/ {
       __pyx_t_19 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_p); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 98, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
       __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
@@ -8114,122 +8119,115 @@
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __pyx_L7:;
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":99
  *             else:
  *                 self.basis.weighted_transform(X, missing, B, sample_weight[:, p])
- *             beta, mse_ = np.linalg.lstsq(B[:, 0:(basis_size)], weighted_y)[0:2]             # <<<<<<<<<<<<<<
+ *             beta, mse_ = np.linalg.lstsq(B[:, 0:(basis_size)], weighted_y, rcond=None)[0:2]             # <<<<<<<<<<<<<<
  *             if mse_:
  *                 pass
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_19, __pyx_n_s_np); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_linalg); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 99, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_19);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_19, __pyx_n_s_linalg); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_19, __pyx_n_s_lstsq); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-    __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_lstsq); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __pyx_t_19 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_basis_size); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 99, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_19);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_basis_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PySlice_New(__pyx_int_0, __pyx_t_3, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __pyx_t_3 = PySlice_New(__pyx_int_0, __pyx_t_19, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+    __pyx_t_19 = PyTuple_New(2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_19);
     __Pyx_INCREF(__pyx_slice__3);
     __Pyx_GIVEREF(__pyx_slice__3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_slice__3)) __PYX_ERR(0, 99, __pyx_L1_error);
-    __Pyx_GIVEREF(__pyx_t_2);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error);
-    __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_B), __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = NULL;
-    __pyx_t_5 = 0;
-    #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_19))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_19);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_19);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_19, function);
-        __pyx_t_5 = 1;
-      }
-    }
-    #endif
-    {
-      PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_t_2, ((PyObject *)__pyx_v_weighted_y)};
-      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_19, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-    }
-    __pyx_t_19 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 2, NULL, NULL, &__pyx_slice__6, 1, 1, 0); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 99, __pyx_L1_error)
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_slice__3)) __PYX_ERR(0, 99, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error);
+    __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_B), __pyx_t_19); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+    __pyx_t_19 = PyTuple_New(2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 99, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_19);
+    __Pyx_GIVEREF(__pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error);
+    __Pyx_INCREF((PyObject *)__pyx_v_weighted_y);
+    __Pyx_GIVEREF((PyObject *)__pyx_v_weighted_y);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_19, 1, ((PyObject *)__pyx_v_weighted_y))) __PYX_ERR(0, 99, __pyx_L1_error);
+    __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_rcond, Py_None) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_19, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if ((likely(PyTuple_CheckExact(__pyx_t_19))) || (PyList_CheckExact(__pyx_t_19))) {
-      PyObject* sequence = __pyx_t_19;
+    __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_2, 0, 2, NULL, NULL, &__pyx_slice__6, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
+      PyObject* sequence = __pyx_t_3;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
         __PYX_ERR(0, 99, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
-        __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
-        __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
+        __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
+        __pyx_t_19 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
-        __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
-        __pyx_t_2 = PyList_GET_ITEM(sequence, 1); 
+        __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
+        __pyx_t_19 = PyList_GET_ITEM(sequence, 1); 
       }
-      __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_19);
       #else
-      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
+      __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_19 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 99, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
       #endif
-      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_3 = PyObject_GetIter(__pyx_t_19); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-      __pyx_t_24 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3);
-      index = 0; __pyx_t_1 = __pyx_t_24(__pyx_t_3); if (unlikely(!__pyx_t_1)) goto __pyx_L8_unpacking_failed;
+      __pyx_t_1 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      index = 1; __pyx_t_2 = __pyx_t_24(__pyx_t_3); if (unlikely(!__pyx_t_2)) goto __pyx_L8_unpacking_failed;
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_24 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1);
+      index = 0; __pyx_t_2 = __pyx_t_24(__pyx_t_1); if (unlikely(!__pyx_t_2)) goto __pyx_L8_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_2);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_24(__pyx_t_3), 2) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+      index = 1; __pyx_t_19 = __pyx_t_24(__pyx_t_1); if (unlikely(!__pyx_t_19)) goto __pyx_L8_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_19);
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_24(__pyx_t_1), 2) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
       __pyx_t_24 = NULL;
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L9_unpacking_done;
       __pyx_L8_unpacking_failed:;
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_24 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
       __PYX_ERR(0, 99, __pyx_L1_error)
       __pyx_L9_unpacking_done:;
     }
-    __Pyx_XDECREF_SET(__pyx_v_beta, __pyx_t_1);
-    __pyx_t_1 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_mse_, __pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_beta, __pyx_t_2);
     __pyx_t_2 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_mse_, __pyx_t_19);
+    __pyx_t_19 = 0;
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":100
  *                 self.basis.weighted_transform(X, missing, B, sample_weight[:, p])
- *             beta, mse_ = np.linalg.lstsq(B[:, 0:(basis_size)], weighted_y)[0:2]
+ *             beta, mse_ = np.linalg.lstsq(B[:, 0:(basis_size)], weighted_y, rcond=None)[0:2]
  *             if mse_:             # <<<<<<<<<<<<<<
  *                 pass
  *             else:
  */
     __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_mse_); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 100, __pyx_L1_error)
     if (__pyx_t_8) {
       goto __pyx_L10;
@@ -8239,177 +8237,177 @@
  *                 pass
  *             else:
  *                 mse_ = np.sum(             # <<<<<<<<<<<<<<
  *                     (np.dot(B[:, 0:basis_size], beta) - weighted_y) ** 2)
  *             mse += mse_
  */
     /*else*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_19, __pyx_n_s_np); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 103, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_19, __pyx_n_s_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":104
  *             else:
  *                 mse_ = np.sum(
  *                     (np.dot(B[:, 0:basis_size], beta) - weighted_y) ** 2)             # <<<<<<<<<<<<<<
  *             mse += mse_
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_dot); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dot); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_basis_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PySlice_New(__pyx_int_0, __pyx_t_3, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_basis_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_4 = PySlice_New(__pyx_int_0, __pyx_t_1, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_slice__3);
       __Pyx_GIVEREF(__pyx_slice__3);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_slice__3)) __PYX_ERR(0, 104, __pyx_L1_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_slice__3)) __PYX_ERR(0, 104, __pyx_L1_error);
       __Pyx_GIVEREF(__pyx_t_4);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error);
       __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_B), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_B), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = NULL;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_20))) {
-        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_20);
-        if (likely(__pyx_t_3)) {
+        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_20);
+        if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_20);
-          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_20, function);
           __pyx_t_5 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_t_4, __pyx_v_beta};
-        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_20, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
-        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        PyObject *__pyx_callargs[3] = {__pyx_t_1, __pyx_t_4, __pyx_v_beta};
+        __pyx_t_19 = __Pyx_PyObject_FastCall(__pyx_t_20, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
+        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
+        if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 104, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_19);
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
       }
-      __pyx_t_20 = PyNumber_Subtract(__pyx_t_2, ((PyObject *)__pyx_v_weighted_y)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __pyx_t_20 = PyNumber_Subtract(__pyx_t_19, ((PyObject *)__pyx_v_weighted_y)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 104, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = PyNumber_Power(__pyx_t_20, __pyx_int_2, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+      __pyx_t_19 = PyNumber_Power(__pyx_t_20, __pyx_int_2, Py_None); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 104, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
       __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
       __pyx_t_20 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (unlikely(PyMethod_Check(__pyx_t_1))) {
-        __pyx_t_20 = PyMethod_GET_SELF(__pyx_t_1);
+      if (unlikely(PyMethod_Check(__pyx_t_2))) {
+        __pyx_t_20 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_20)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_20);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_1, function);
+          __Pyx_DECREF_SET(__pyx_t_2, function);
           __pyx_t_5 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_20, __pyx_t_2};
-        __pyx_t_19 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+        PyObject *__pyx_callargs[2] = {__pyx_t_20, __pyx_t_19};
+        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
         __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
+        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 103, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_19);
-        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __Pyx_DECREF_SET(__pyx_v_mse_, __pyx_t_19);
-      __pyx_t_19 = 0;
+      __Pyx_DECREF_SET(__pyx_v_mse_, __pyx_t_3);
+      __pyx_t_3 = 0;
     }
     __pyx_L10:;
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":105
  *                 mse_ = np.sum(
  *                     (np.dot(B[:, 0:basis_size], beta) - weighted_y) ** 2)
  *             mse += mse_             # <<<<<<<<<<<<<<
  * 
  *         # Create the record object
  */
-    __pyx_t_19 = PyFloat_FromDouble(__pyx_v_mse); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 105, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_19);
-    __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_t_19, __pyx_v_mse_); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-    __pyx_t_18 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_18 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_mse); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_t_3, __pyx_v_mse_); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_18 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_18 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_mse = __pyx_t_18;
   }
 
   /* "UQPyL/surrogates/mars_/_pruning.pyx":109
  *         # Create the record object
  *         self.record = PruningPassRecord(
  *             self.m, self.n, self.penalty, mse0 / total_weight, pruned_basis_size, mse / total_weight)             # <<<<<<<<<<<<<<
  *         gcv_ = self.record.gcv(0)
  *         best_gcv = gcv_
  */
-  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->m); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_19 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->n); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_19);
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_self->penalty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->m); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_self->n); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_19 = PyFloat_FromDouble(__pyx_v_self->penalty); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_19);
   __pyx_t_20 = PyFloat_FromDouble((__pyx_v_mse0 / __pyx_v_total_weight)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_20);
   __pyx_t_4 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_pruned_basis_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyFloat_FromDouble((__pyx_v_mse / __pyx_v_total_weight)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_mse / __pyx_v_total_weight)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
 
   /* "UQPyL/surrogates/mars_/_pruning.pyx":108
  * 
  *         # Create the record object
  *         self.record = PruningPassRecord(             # <<<<<<<<<<<<<<
  *             self.m, self.n, self.penalty, mse0 / total_weight, pruned_basis_size, mse / total_weight)
  *         gcv_ = self.record.gcv(0)
  */
   __pyx_t_22 = PyTuple_New(6); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_22);
-  __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 0, __pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_19);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 1, __pyx_t_19)) __PYX_ERR(0, 108, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 2, __pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 0, __pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 1, __pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_19);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 2, __pyx_t_19)) __PYX_ERR(0, 108, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_20);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 3, __pyx_t_20)) __PYX_ERR(0, 108, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 4, __pyx_t_4)) __PYX_ERR(0, 108, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 5, __pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error);
-  __pyx_t_1 = 0;
-  __pyx_t_19 = 0;
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 5, __pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error);
   __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+  __pyx_t_19 = 0;
   __pyx_t_20 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5UQPyL_10surrogates_5mars__7_record_PruningPassRecord), __pyx_t_22, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5UQPyL_10surrogates_5mars__7_record_PruningPassRecord), __pyx_t_22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-  __Pyx_GIVEREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF((PyObject *)__pyx_v_self->record);
   __Pyx_DECREF((PyObject *)__pyx_v_self->record);
-  __pyx_v_self->record = ((struct __pyx_obj_5UQPyL_10surrogates_5mars__7_record_PruningPassRecord *)__pyx_t_3);
-  __pyx_t_3 = 0;
+  __pyx_v_self->record = ((struct __pyx_obj_5UQPyL_10surrogates_5mars__7_record_PruningPassRecord *)__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "UQPyL/surrogates/mars_/_pruning.pyx":110
  *         self.record = PruningPassRecord(
  *             self.m, self.n, self.penalty, mse0 / total_weight, pruned_basis_size, mse / total_weight)
  *         gcv_ = self.record.gcv(0)             # <<<<<<<<<<<<<<
  *         best_gcv = gcv_
  *         best_iteration = 0
@@ -8448,22 +8446,22 @@
     /* "UQPyL/surrogates/mars_/_pruning.pyx":115
  * 
  *         if self.verbose >= 1:
  *             print(self.record.partial_str(slice(-1, None, None), print_footer=False))             # <<<<<<<<<<<<<<
  * 
  *         # init feature importance
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->record), __pyx_n_s_partial_str); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->record), __pyx_n_s_partial_str); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_22 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_22);
     if (PyDict_SetItem(__pyx_t_22, __pyx_n_s_print_footer, Py_False) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__8, __pyx_t_22); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__8, __pyx_t_22); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
     __pyx_t_22 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_4); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 115, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_22);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":114
@@ -8554,32 +8552,32 @@
  *                 bf = self.basis[j]
  *                 if bf.is_pruned():             # <<<<<<<<<<<<<<
  *                     continue
  *                 if not bf.is_prunable():
  */
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_bf, __pyx_n_s_is_pruned); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = NULL;
+      __pyx_t_1 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_4))) {
-        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-        if (likely(__pyx_t_3)) {
+        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_5 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+        PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
         __pyx_t_22 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
-        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 129, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
       __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_22); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 129, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
       if (__pyx_t_8) {
@@ -8607,32 +8605,32 @@
  *                     continue
  *                 if not bf.is_prunable():             # <<<<<<<<<<<<<<
  *                     continue
  *                 bf.prune()
  */
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_bf, __pyx_n_s_is_prunable); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = NULL;
+      __pyx_t_1 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_4))) {
-        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-        if (likely(__pyx_t_3)) {
+        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_5 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+        PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
         __pyx_t_22 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
-        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 131, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
       __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_22); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 131, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
       __pyx_t_30 = (!__pyx_t_8);
@@ -8661,32 +8659,32 @@
  *                     continue
  *                 bf.prune()             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_bf, __pyx_n_s_prune); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = NULL;
+      __pyx_t_1 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_4))) {
-        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-        if (likely(__pyx_t_3)) {
+        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_5 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+        PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
         __pyx_t_22 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
-        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 133, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_22);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":136
@@ -8738,40 +8736,40 @@
           if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_slice__3)) __PYX_ERR(0, 139, __pyx_L1_error);
           __Pyx_GIVEREF(__pyx_t_22);
           if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_22)) __PYX_ERR(0, 139, __pyx_L1_error);
           __pyx_t_22 = 0;
           __pyx_t_22 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_y), __pyx_t_4); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sqrt); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 139, __pyx_L1_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sqrt); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_20);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_sample_weight), __pyx_tuple__4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_2 = NULL;
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_sample_weight), __pyx_tuple__4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __pyx_t_19 = NULL;
           __pyx_t_5 = 0;
           #if CYTHON_UNPACK_METHODS
           if (unlikely(PyMethod_Check(__pyx_t_20))) {
-            __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_20);
-            if (likely(__pyx_t_2)) {
+            __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_20);
+            if (likely(__pyx_t_19)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_20);
-              __Pyx_INCREF(__pyx_t_2);
+              __Pyx_INCREF(__pyx_t_19);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_20, function);
               __pyx_t_5 = 1;
             }
           }
           #endif
           {
-            PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_3};
+            PyObject *__pyx_callargs[2] = {__pyx_t_19, __pyx_t_1};
             __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_20, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
-            __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_4);
             __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
           }
           __pyx_t_20 = PyNumber_Multiply(__pyx_t_22, __pyx_t_4); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_20);
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
@@ -8843,59 +8841,59 @@
           if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error);
           __pyx_t_4 = 0;
           __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_y), __pyx_t_20); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
           __Pyx_GetModuleGlobalName(__pyx_t_22, __pyx_n_s_np); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 142, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_sqrt); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_sqrt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
           __pyx_t_22 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_p); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 142, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_19 = PyTuple_New(2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 142, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_19);
           __Pyx_INCREF(__pyx_slice__3);
           __Pyx_GIVEREF(__pyx_slice__3);
-          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_slice__3)) __PYX_ERR(0, 142, __pyx_L1_error);
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_slice__3)) __PYX_ERR(0, 142, __pyx_L1_error);
           __Pyx_GIVEREF(__pyx_t_22);
-          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_22)) __PYX_ERR(0, 142, __pyx_L1_error);
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_22)) __PYX_ERR(0, 142, __pyx_L1_error);
           __pyx_t_22 = 0;
-          __pyx_t_22 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_sample_weight), __pyx_t_2); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 142, __pyx_L1_error)
+          __pyx_t_22 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_sample_weight), __pyx_t_19); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 142, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __pyx_t_2 = NULL;
+          __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+          __pyx_t_19 = NULL;
           __pyx_t_5 = 0;
           #if CYTHON_UNPACK_METHODS
-          if (unlikely(PyMethod_Check(__pyx_t_3))) {
-            __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-            if (likely(__pyx_t_2)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-              __Pyx_INCREF(__pyx_t_2);
+          if (unlikely(PyMethod_Check(__pyx_t_1))) {
+            __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_1);
+            if (likely(__pyx_t_19)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+              __Pyx_INCREF(__pyx_t_19);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_3, function);
+              __Pyx_DECREF_SET(__pyx_t_1, function);
               __pyx_t_5 = 1;
             }
           }
           #endif
           {
-            PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_22};
-            __pyx_t_20 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
-            __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+            PyObject *__pyx_callargs[2] = {__pyx_t_19, __pyx_t_22};
+            __pyx_t_20 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+            __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
             __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
             if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 142, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_20);
-            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           }
-          __pyx_t_3 = PyNumber_Multiply(__pyx_t_4, __pyx_t_20); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
+          __pyx_t_1 = PyNumber_Multiply(__pyx_t_4, __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-          if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 142, __pyx_L1_error)
-          __pyx_t_14 = ((PyArrayObject *)__pyx_t_3);
+          if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 142, __pyx_L1_error)
+          __pyx_t_14 = ((PyArrayObject *)__pyx_t_1);
           {
             __Pyx_BufFmt_StackElem __pyx_stack[1];
             __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_weighted_y.rcbuffer->pybuffer);
             __pyx_t_5 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_weighted_y.rcbuffer->pybuffer, (PyObject*)__pyx_t_14, &__Pyx_TypeInfo_nn___pyx_t_5UQPyL_10surrogates_5mars__6_types_FLOAT_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
             if (unlikely(__pyx_t_5 < 0)) {
               PyErr_Fetch(&__pyx_t_17, &__pyx_t_16, &__pyx_t_15);
               if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_weighted_y.rcbuffer->pybuffer, (PyObject*)__pyx_v_weighted_y, &__Pyx_TypeInfo_nn___pyx_t_5UQPyL_10surrogates_5mars__6_types_FLOAT_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
@@ -8906,172 +8904,197 @@
               }
               __pyx_t_17 = __pyx_t_16 = __pyx_t_15 = 0;
             }
             __pyx_pybuffernd_weighted_y.diminfo[0].strides = __pyx_pybuffernd_weighted_y.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_weighted_y.diminfo[0].shape = __pyx_pybuffernd_weighted_y.rcbuffer->pybuffer.shape[0];
             if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 142, __pyx_L1_error)
           }
           __pyx_t_14 = 0;
-          __Pyx_XDECREF_SET(__pyx_v_weighted_y, ((PyArrayObject *)__pyx_t_3));
-          __pyx_t_3 = 0;
+          __Pyx_XDECREF_SET(__pyx_v_weighted_y, ((PyArrayObject *)__pyx_t_1));
+          __pyx_t_1 = 0;
 
           /* "UQPyL/surrogates/mars_/_pruning.pyx":143
  *                     else:
  *                         weighted_y = y[:,p] * np.sqrt(sample_weight[:,p])
  *                         self.basis.weighted_transform(X, missing, B, sample_weight[:, p])             # <<<<<<<<<<<<<<
  *                     beta, mse_ = np.linalg.lstsq(
- *                         B[:, 0:pruned_basis_size], weighted_y)[0:2]
+ *                         B[:, 0:pruned_basis_size], weighted_y , rcond=None)[0:2]
  */
-          __pyx_t_3 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_p); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
+          __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_p); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_20 = PyTuple_New(2); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 143, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_20);
           __Pyx_INCREF(__pyx_slice__3);
           __Pyx_GIVEREF(__pyx_slice__3);
           if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 0, __pyx_slice__3)) __PYX_ERR(0, 143, __pyx_L1_error);
-          __Pyx_GIVEREF(__pyx_t_3);
-          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error);
-          __pyx_t_3 = 0;
-          __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_sample_weight), __pyx_t_20); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_GIVEREF(__pyx_t_1);
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error);
+          __pyx_t_1 = 0;
+          __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_sample_weight), __pyx_t_20); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-          if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 143, __pyx_L1_error)
-          __pyx_t_20 = ((struct __pyx_vtabstruct_5UQPyL_10surrogates_5mars__6_basis_Basis *)__pyx_v_self->basis->__pyx_vtab)->weighted_transform(__pyx_v_self->basis, ((PyArrayObject *)__pyx_v_X), ((PyArrayObject *)__pyx_v_missing), ((PyArrayObject *)__pyx_v_B), ((PyArrayObject *)__pyx_t_3), 0); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 143, __pyx_L1_error)
+          if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 143, __pyx_L1_error)
+          __pyx_t_20 = ((struct __pyx_vtabstruct_5UQPyL_10surrogates_5mars__6_basis_Basis *)__pyx_v_self->basis->__pyx_vtab)->weighted_transform(__pyx_v_self->basis, ((PyArrayObject *)__pyx_v_X), ((PyArrayObject *)__pyx_v_missing), ((PyArrayObject *)__pyx_v_B), ((PyArrayObject *)__pyx_t_1), 0); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 143, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_20);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
         }
         __pyx_L20:;
 
         /* "UQPyL/surrogates/mars_/_pruning.pyx":144
  *                         weighted_y = y[:,p] * np.sqrt(sample_weight[:,p])
  *                         self.basis.weighted_transform(X, missing, B, sample_weight[:, p])
  *                     beta, mse_ = np.linalg.lstsq(             # <<<<<<<<<<<<<<
- *                         B[:, 0:pruned_basis_size], weighted_y)[0:2]
+ *                         B[:, 0:pruned_basis_size], weighted_y , rcond=None)[0:2]
  *                     if mse_:
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_linalg); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 144, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_lstsq); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_GetModuleGlobalName(__pyx_t_20, __pyx_n_s_np); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_20);
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_20, __pyx_n_s_linalg); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+        __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_lstsq); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_20);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         /* "UQPyL/surrogates/mars_/_pruning.pyx":145
  *                         self.basis.weighted_transform(X, missing, B, sample_weight[:, p])
  *                     beta, mse_ = np.linalg.lstsq(
- *                         B[:, 0:pruned_basis_size], weighted_y)[0:2]             # <<<<<<<<<<<<<<
+ *                         B[:, 0:pruned_basis_size], weighted_y , rcond=None)[0:2]             # <<<<<<<<<<<<<<
  *                     if mse_:
  *                         pass
  */
-        __pyx_t_4 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_pruned_basis_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_22 = PySlice_New(__pyx_int_0, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 145, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_22);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_pruned_basis_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_4 = PySlice_New(__pyx_int_0, __pyx_t_1, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
         __Pyx_INCREF(__pyx_slice__3);
         __Pyx_GIVEREF(__pyx_slice__3);
-        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_slice__3)) __PYX_ERR(0, 145, __pyx_L1_error);
-        __Pyx_GIVEREF(__pyx_t_22);
-        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_22)) __PYX_ERR(0, 145, __pyx_L1_error);
-        __pyx_t_22 = 0;
-        __pyx_t_22 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_B), __pyx_t_4); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 145, __pyx_L1_error)
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_slice__3)) __PYX_ERR(0, 145, __pyx_L1_error);
+        __Pyx_GIVEREF(__pyx_t_4);
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error);
+        __pyx_t_4 = 0;
+        __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_B), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+        /* "UQPyL/surrogates/mars_/_pruning.pyx":144
+ *                         weighted_y = y[:,p] * np.sqrt(sample_weight[:,p])
+ *                         self.basis.weighted_transform(X, missing, B, sample_weight[:, p])
+ *                     beta, mse_ = np.linalg.lstsq(             # <<<<<<<<<<<<<<
+ *                         B[:, 0:pruned_basis_size], weighted_y , rcond=None)[0:2]
+ *                     if mse_:
+ */
+        __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_GIVEREF(__pyx_t_4);
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4)) __PYX_ERR(0, 144, __pyx_L1_error);
+        __Pyx_INCREF((PyObject *)__pyx_v_weighted_y);
+        __Pyx_GIVEREF((PyObject *)__pyx_v_weighted_y);
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)__pyx_v_weighted_y))) __PYX_ERR(0, 144, __pyx_L1_error);
+        __pyx_t_4 = 0;
+
+        /* "UQPyL/surrogates/mars_/_pruning.pyx":145
+ *                         self.basis.weighted_transform(X, missing, B, sample_weight[:, p])
+ *                     beta, mse_ = np.linalg.lstsq(
+ *                         B[:, 0:pruned_basis_size], weighted_y , rcond=None)[0:2]             # <<<<<<<<<<<<<<
+ *                     if mse_:
+ *                         pass
+ */
+        __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_rcond, Py_None) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+
+        /* "UQPyL/surrogates/mars_/_pruning.pyx":144
+ *                         weighted_y = y[:,p] * np.sqrt(sample_weight[:,p])
+ *                         self.basis.weighted_transform(X, missing, B, sample_weight[:, p])
+ *                     beta, mse_ = np.linalg.lstsq(             # <<<<<<<<<<<<<<
+ *                         B[:, 0:pruned_basis_size], weighted_y , rcond=None)[0:2]
+ *                     if mse_:
+ */
+        __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_20, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 144, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_22);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_4 = NULL;
-        __pyx_t_5 = 0;
-        #if CYTHON_UNPACK_METHODS
-        if (likely(PyMethod_Check(__pyx_t_3))) {
-          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-          if (likely(__pyx_t_4)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-            __Pyx_INCREF(__pyx_t_4);
-            __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_3, function);
-            __pyx_t_5 = 1;
-          }
-        }
-        #endif
-        {
-          PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_22, ((PyObject *)__pyx_v_weighted_y)};
-          __pyx_t_20 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
-          __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 144, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_20);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        }
-        __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_20, 0, 2, NULL, NULL, &__pyx_slice__6, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-        if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
-          PyObject* sequence = __pyx_t_3;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+        /* "UQPyL/surrogates/mars_/_pruning.pyx":145
+ *                         self.basis.weighted_transform(X, missing, B, sample_weight[:, p])
+ *                     beta, mse_ = np.linalg.lstsq(
+ *                         B[:, 0:pruned_basis_size], weighted_y , rcond=None)[0:2]             # <<<<<<<<<<<<<<
+ *                     if mse_:
+ *                         pass
+ */
+        __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_t_22, 0, 2, NULL, NULL, &__pyx_slice__6, 1, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+        if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
+          PyObject* sequence = __pyx_t_4;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
             __PYX_ERR(0, 144, __pyx_L1_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
-            __pyx_t_20 = PyTuple_GET_ITEM(sequence, 0); 
-            __pyx_t_22 = PyTuple_GET_ITEM(sequence, 1); 
+            __pyx_t_22 = PyTuple_GET_ITEM(sequence, 0); 
+            __pyx_t_1 = PyTuple_GET_ITEM(sequence, 1); 
           } else {
-            __pyx_t_20 = PyList_GET_ITEM(sequence, 0); 
-            __pyx_t_22 = PyList_GET_ITEM(sequence, 1); 
+            __pyx_t_22 = PyList_GET_ITEM(sequence, 0); 
+            __pyx_t_1 = PyList_GET_ITEM(sequence, 1); 
           }
-          __Pyx_INCREF(__pyx_t_20);
           __Pyx_INCREF(__pyx_t_22);
+          __Pyx_INCREF(__pyx_t_1);
           #else
-          __pyx_t_20 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 144, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_20);
-          __pyx_t_22 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 144, __pyx_L1_error)
+          __pyx_t_22 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 144, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
+          __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
           #endif
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_4 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 144, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __pyx_t_24 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4);
-          index = 0; __pyx_t_20 = __pyx_t_24(__pyx_t_4); if (unlikely(!__pyx_t_20)) goto __pyx_L21_unpacking_failed;
+          __pyx_t_20 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 144, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_20);
-          index = 1; __pyx_t_22 = __pyx_t_24(__pyx_t_4); if (unlikely(!__pyx_t_22)) goto __pyx_L21_unpacking_failed;
+          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+          __pyx_t_24 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_20);
+          index = 0; __pyx_t_22 = __pyx_t_24(__pyx_t_20); if (unlikely(!__pyx_t_22)) goto __pyx_L21_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_22);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_24(__pyx_t_4), 2) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+          index = 1; __pyx_t_1 = __pyx_t_24(__pyx_t_20); if (unlikely(!__pyx_t_1)) goto __pyx_L21_unpacking_failed;
+          __Pyx_GOTREF(__pyx_t_1);
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_24(__pyx_t_20), 2) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
           __pyx_t_24 = NULL;
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+          __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
           goto __pyx_L22_unpacking_done;
           __pyx_L21_unpacking_failed:;
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+          __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
           __pyx_t_24 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
           __PYX_ERR(0, 144, __pyx_L1_error)
           __pyx_L22_unpacking_done:;
         }
 
         /* "UQPyL/surrogates/mars_/_pruning.pyx":144
  *                         weighted_y = y[:,p] * np.sqrt(sample_weight[:,p])
  *                         self.basis.weighted_transform(X, missing, B, sample_weight[:, p])
  *                     beta, mse_ = np.linalg.lstsq(             # <<<<<<<<<<<<<<
- *                         B[:, 0:pruned_basis_size], weighted_y)[0:2]
+ *                         B[:, 0:pruned_basis_size], weighted_y , rcond=None)[0:2]
  *                     if mse_:
  */
-        __Pyx_XDECREF_SET(__pyx_v_beta, __pyx_t_20);
-        __pyx_t_20 = 0;
-        __Pyx_XDECREF_SET(__pyx_v_mse_, __pyx_t_22);
+        __Pyx_XDECREF_SET(__pyx_v_beta, __pyx_t_22);
         __pyx_t_22 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_mse_, __pyx_t_1);
+        __pyx_t_1 = 0;
 
         /* "UQPyL/surrogates/mars_/_pruning.pyx":146
  *                     beta, mse_ = np.linalg.lstsq(
- *                         B[:, 0:pruned_basis_size], weighted_y)[0:2]
+ *                         B[:, 0:pruned_basis_size], weighted_y , rcond=None)[0:2]
  *                     if mse_:             # <<<<<<<<<<<<<<
  *                         pass
  * #                         mse_ /= np.sum(self.sample_weight)
  */
         __pyx_t_30 = __Pyx_PyObject_IsTrue(__pyx_v_mse_); if (unlikely((__pyx_t_30 < 0))) __PYX_ERR(0, 146, __pyx_L1_error)
         if (__pyx_t_30) {
           goto __pyx_L23;
@@ -9081,164 +9104,164 @@
  * #                         mse_ /= np.sum(self.sample_weight)
  *                     else:
  *                         mse_ = np.sum((np.dot(B[:, 0:pruned_basis_size], beta) -             # <<<<<<<<<<<<<<
  *                                     weighted_y) ** 2) #/ np.sum(sample_weight)
  *                     mse += mse_# * output_weight[p]
  */
         /*else*/ {
-          __Pyx_GetModuleGlobalName(__pyx_t_22, __pyx_n_s_np); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 150, __pyx_L1_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sum); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 150, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_sum); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 150, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __Pyx_GetModuleGlobalName(__pyx_t_20, __pyx_n_s_np); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 150, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_20);
-          __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_dot); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __pyx_t_4 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_pruned_basis_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_19 = PySlice_New(__pyx_int_0, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 150, __pyx_L1_error)
+          __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_t_20, __pyx_n_s_dot); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 150, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_19);
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_4);
+          __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+          __pyx_t_20 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_pruned_basis_size); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 150, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_20);
+          __pyx_t_3 = PySlice_New(__pyx_int_0, __pyx_t_20, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+          __pyx_t_20 = PyTuple_New(2); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 150, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_20);
           __Pyx_INCREF(__pyx_slice__3);
           __Pyx_GIVEREF(__pyx_slice__3);
-          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_slice__3)) __PYX_ERR(0, 150, __pyx_L1_error);
-          __Pyx_GIVEREF(__pyx_t_19);
-          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_19)) __PYX_ERR(0, 150, __pyx_L1_error);
-          __pyx_t_19 = 0;
-          __pyx_t_19 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_B), __pyx_t_4); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 150, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_19);
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __pyx_t_4 = NULL;
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 0, __pyx_slice__3)) __PYX_ERR(0, 150, __pyx_L1_error);
+          __Pyx_GIVEREF(__pyx_t_3);
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error);
+          __pyx_t_3 = 0;
+          __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_B), __pyx_t_20); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+          __pyx_t_20 = NULL;
           __pyx_t_5 = 0;
           #if CYTHON_UNPACK_METHODS
-          if (unlikely(PyMethod_Check(__pyx_t_2))) {
-            __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-            if (likely(__pyx_t_4)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-              __Pyx_INCREF(__pyx_t_4);
+          if (unlikely(PyMethod_Check(__pyx_t_19))) {
+            __pyx_t_20 = PyMethod_GET_SELF(__pyx_t_19);
+            if (likely(__pyx_t_20)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_19);
+              __Pyx_INCREF(__pyx_t_20);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_2, function);
+              __Pyx_DECREF_SET(__pyx_t_19, function);
               __pyx_t_5 = 1;
             }
           }
           #endif
           {
-            PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_19, __pyx_v_beta};
-            __pyx_t_22 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
-            __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+            PyObject *__pyx_callargs[3] = {__pyx_t_20, __pyx_t_3, __pyx_v_beta};
+            __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_19, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
+            __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
+            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-            if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 150, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_22);
-            __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           }
 
           /* "UQPyL/surrogates/mars_/_pruning.pyx":151
  *                     else:
  *                         mse_ = np.sum((np.dot(B[:, 0:pruned_basis_size], beta) -
  *                                     weighted_y) ** 2) #/ np.sum(sample_weight)             # <<<<<<<<<<<<<<
  *                     mse += mse_# * output_weight[p]
  *                 gcv_ = gcv(mse / np.sum(sample_weight), pruned_basis_size, self.m, self.penalty)
  */
-          __pyx_t_2 = PyNumber_Subtract(__pyx_t_22, ((PyObject *)__pyx_v_weighted_y)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          __pyx_t_22 = PyNumber_Power(__pyx_t_2, __pyx_int_2, Py_None); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 151, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_22);
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __pyx_t_2 = NULL;
+          __pyx_t_19 = PyNumber_Subtract(__pyx_t_1, ((PyObject *)__pyx_v_weighted_y)); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 150, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_19);
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __pyx_t_1 = PyNumber_Power(__pyx_t_19, __pyx_int_2, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+          __pyx_t_19 = NULL;
           __pyx_t_5 = 0;
           #if CYTHON_UNPACK_METHODS
-          if (unlikely(PyMethod_Check(__pyx_t_20))) {
-            __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_20);
-            if (likely(__pyx_t_2)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_20);
-              __Pyx_INCREF(__pyx_t_2);
+          if (unlikely(PyMethod_Check(__pyx_t_22))) {
+            __pyx_t_19 = PyMethod_GET_SELF(__pyx_t_22);
+            if (likely(__pyx_t_19)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_22);
+              __Pyx_INCREF(__pyx_t_19);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_20, function);
+              __Pyx_DECREF_SET(__pyx_t_22, function);
               __pyx_t_5 = 1;
             }
           }
           #endif
           {
-            PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_22};
-            __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_20, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
-            __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+            PyObject *__pyx_callargs[2] = {__pyx_t_19, __pyx_t_1};
+            __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_22, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+            __Pyx_XDECREF(__pyx_t_19); __pyx_t_19 = 0;
+            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+            if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_4);
             __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-            if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_3);
-            __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
           }
-          __Pyx_DECREF_SET(__pyx_v_mse_, __pyx_t_3);
-          __pyx_t_3 = 0;
+          __Pyx_DECREF_SET(__pyx_v_mse_, __pyx_t_4);
+          __pyx_t_4 = 0;
         }
         __pyx_L23:;
 
         /* "UQPyL/surrogates/mars_/_pruning.pyx":152
  *                         mse_ = np.sum((np.dot(B[:, 0:pruned_basis_size], beta) -
  *                                     weighted_y) ** 2) #/ np.sum(sample_weight)
  *                     mse += mse_# * output_weight[p]             # <<<<<<<<<<<<<<
  *                 gcv_ = gcv(mse / np.sum(sample_weight), pruned_basis_size, self.m, self.penalty)
  * 
  */
-        __pyx_t_3 = PyFloat_FromDouble(__pyx_v_mse); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 152, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_20 = PyNumber_InPlaceAdd(__pyx_t_3, __pyx_v_mse_); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 152, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_20);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_18 = __pyx_PyFloat_AsDouble(__pyx_t_20); if (unlikely((__pyx_t_18 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 152, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+        __pyx_t_4 = PyFloat_FromDouble(__pyx_v_mse); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __pyx_t_22 = PyNumber_InPlaceAdd(__pyx_t_4, __pyx_v_mse_); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 152, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_22);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __pyx_t_18 = __pyx_PyFloat_AsDouble(__pyx_t_22); if (unlikely((__pyx_t_18 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 152, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
         __pyx_v_mse = __pyx_t_18;
       }
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":153
  *                                     weighted_y) ** 2) #/ np.sum(sample_weight)
  *                     mse += mse_# * output_weight[p]
  *                 gcv_ = gcv(mse / np.sum(sample_weight), pruned_basis_size, self.m, self.penalty)             # <<<<<<<<<<<<<<
  * 
  *                 if gcv_ <= best_iteration_gcv or first:
  */
-      __pyx_t_20 = PyFloat_FromDouble(__pyx_v_mse); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 153, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_20);
-      __Pyx_GetModuleGlobalName(__pyx_t_22, __pyx_n_s_np); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __pyx_t_22 = PyFloat_FromDouble(__pyx_v_mse); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 153, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-      __pyx_t_22 = NULL;
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sum); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (unlikely(PyMethod_Check(__pyx_t_2))) {
-        __pyx_t_22 = PyMethod_GET_SELF(__pyx_t_2);
-        if (likely(__pyx_t_22)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-          __Pyx_INCREF(__pyx_t_22);
+      if (unlikely(PyMethod_Check(__pyx_t_19))) {
+        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_19);
+        if (likely(__pyx_t_1)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_19);
+          __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_2, function);
+          __Pyx_DECREF_SET(__pyx_t_19, function);
           __pyx_t_5 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_22, ((PyObject *)__pyx_v_sample_weight)};
-        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
-        __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        PyObject *__pyx_callargs[2] = {__pyx_t_1, ((PyObject *)__pyx_v_sample_weight)};
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_19, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
       }
-      __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_t_20, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_18 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_18 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 153, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_19 = __Pyx_PyNumber_Divide(__pyx_t_22, __pyx_t_4); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_18 = __pyx_PyFloat_AsDouble(__pyx_t_19); if (unlikely((__pyx_t_18 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 153, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
       __pyx_t_31 = __pyx_f_5UQPyL_10surrogates_5mars__5_util_gcv(__pyx_t_18, __pyx_v_pruned_basis_size, __pyx_v_self->m, __pyx_v_self->penalty, 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 153, __pyx_L1_error)
       __pyx_v_gcv_ = __pyx_t_31;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":155
  *                 gcv_ = gcv(mse / np.sum(sample_weight), pruned_basis_size, self.m, self.penalty)
  * 
  *                 if gcv_ <= best_iteration_gcv or first:             # <<<<<<<<<<<<<<
@@ -9303,39 +9326,39 @@
       /* "UQPyL/surrogates/mars_/_pruning.pyx":160
  *                     best_bf_to_prune = j
  *                     first = False
  *                 bf.unprune()             # <<<<<<<<<<<<<<
  * 
  *             # Feature importance
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_bf, __pyx_n_s_unprune); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 160, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_20 = NULL;
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_bf, __pyx_n_s_unprune); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_22 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_3))) {
-        __pyx_t_20 = PyMethod_GET_SELF(__pyx_t_3);
-        if (likely(__pyx_t_20)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-          __Pyx_INCREF(__pyx_t_20);
+      if (likely(PyMethod_Check(__pyx_t_4))) {
+        __pyx_t_22 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_22)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_22);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_5 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_20, NULL};
-        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
-        __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        PyObject *__pyx_callargs[2] = {__pyx_t_22, NULL};
+        __pyx_t_19 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
+        __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
+        if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 160, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_19);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
       __pyx_L14_continue:;
     }
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":163
  * 
  *             # Feature importance
  *             if i > 1:             # <<<<<<<<<<<<<<
@@ -9348,235 +9371,235 @@
       /* "UQPyL/surrogates/mars_/_pruning.pyx":167
  *                 # that basis decreased the mse and gcv relative to the previous mse and gcv
  *                 # respectively.
  *                 mse_decrease = (best_iteration_mse - prev_best_iteration_mse)             # <<<<<<<<<<<<<<
  *                 gcv_decrease = (best_iteration_gcv - prev_best_iteration_gcv)
  *                 variables = set()
  */
-      __pyx_t_2 = PyFloat_FromDouble(__pyx_v_best_iteration_mse); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = PyNumber_Subtract(__pyx_t_2, __pyx_v_prev_best_iteration_mse); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_mse_decrease, __pyx_t_3);
-      __pyx_t_3 = 0;
+      __pyx_t_19 = PyFloat_FromDouble(__pyx_v_best_iteration_mse); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __pyx_t_4 = PyNumber_Subtract(__pyx_t_19, __pyx_v_prev_best_iteration_mse); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_mse_decrease, __pyx_t_4);
+      __pyx_t_4 = 0;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":168
  *                 # respectively.
  *                 mse_decrease = (best_iteration_mse - prev_best_iteration_mse)
  *                 gcv_decrease = (best_iteration_gcv - prev_best_iteration_gcv)             # <<<<<<<<<<<<<<
  *                 variables = set()
  *                 bf = self.basis[best_bf_to_prune]
  */
-      __pyx_t_3 = PyFloat_FromDouble(__pyx_v_best_iteration_gcv); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_2 = PyNumber_Subtract(__pyx_t_3, __pyx_v_prev_best_iteration_gcv); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_gcv_decrease, __pyx_t_2);
-      __pyx_t_2 = 0;
+      __pyx_t_4 = PyFloat_FromDouble(__pyx_v_best_iteration_gcv); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 168, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_19 = PyNumber_Subtract(__pyx_t_4, __pyx_v_prev_best_iteration_gcv); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 168, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_gcv_decrease, __pyx_t_19);
+      __pyx_t_19 = 0;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":169
  *                 mse_decrease = (best_iteration_mse - prev_best_iteration_mse)
  *                 gcv_decrease = (best_iteration_gcv - prev_best_iteration_gcv)
  *                 variables = set()             # <<<<<<<<<<<<<<
  *                 bf = self.basis[best_bf_to_prune]
  *                 for v in bf.variables():
  */
-      __pyx_t_2 = PySet_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_XDECREF_SET(__pyx_v_variables, ((PyObject*)__pyx_t_2));
-      __pyx_t_2 = 0;
+      __pyx_t_19 = PySet_New(0); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 169, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __Pyx_XDECREF_SET(__pyx_v_variables, ((PyObject*)__pyx_t_19));
+      __pyx_t_19 = 0;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":170
  *                 gcv_decrease = (best_iteration_gcv - prev_best_iteration_gcv)
  *                 variables = set()
  *                 bf = self.basis[best_bf_to_prune]             # <<<<<<<<<<<<<<
  *                 for v in bf.variables():
  *                     variables.add(v)
  */
-      __pyx_t_2 = __Pyx_GetItemInt(((PyObject *)__pyx_v_self->basis), __pyx_v_best_bf_to_prune, __pyx_t_5UQPyL_10surrogates_5mars__6_types_INDEX_t, 1, __Pyx_PyInt_From_Py_intptr_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_XDECREF_SET(__pyx_v_bf, __pyx_t_2);
-      __pyx_t_2 = 0;
+      __pyx_t_19 = __Pyx_GetItemInt(((PyObject *)__pyx_v_self->basis), __pyx_v_best_bf_to_prune, __pyx_t_5UQPyL_10surrogates_5mars__6_types_INDEX_t, 1, __Pyx_PyInt_From_Py_intptr_t, 0, 0, 0); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 170, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __Pyx_XDECREF_SET(__pyx_v_bf, __pyx_t_19);
+      __pyx_t_19 = 0;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":171
  *                 variables = set()
  *                 bf = self.basis[best_bf_to_prune]
  *                 for v in bf.variables():             # <<<<<<<<<<<<<<
  *                     variables.add(v)
  *                 for v in variables:
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_bf, __pyx_n_s_variables); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 171, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_20 = NULL;
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_bf, __pyx_n_s_variables); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_22 = NULL;
       __pyx_t_5 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_3))) {
-        __pyx_t_20 = PyMethod_GET_SELF(__pyx_t_3);
-        if (likely(__pyx_t_20)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-          __Pyx_INCREF(__pyx_t_20);
+      if (likely(PyMethod_Check(__pyx_t_4))) {
+        __pyx_t_22 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_22)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_22);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_5 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_20, NULL};
-        __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
-        __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        PyObject *__pyx_callargs[2] = {__pyx_t_22, NULL};
+        __pyx_t_19 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
+        __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
+        if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 171, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_19);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
-      if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
-        __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3);
+      if (likely(PyList_CheckExact(__pyx_t_19)) || PyTuple_CheckExact(__pyx_t_19)) {
+        __pyx_t_4 = __pyx_t_19; __Pyx_INCREF(__pyx_t_4);
         __pyx_t_6 = 0;
         __pyx_t_32 = NULL;
       } else {
-        __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 171, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_32 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_32)) __PYX_ERR(0, 171, __pyx_L1_error)
+        __pyx_t_6 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_19); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __pyx_t_32 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_32)) __PYX_ERR(0, 171, __pyx_L1_error)
       }
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
       for (;;) {
         if (likely(!__pyx_t_32)) {
-          if (likely(PyList_CheckExact(__pyx_t_3))) {
+          if (likely(PyList_CheckExact(__pyx_t_4))) {
             {
-              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_3);
+              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_4);
               #if !CYTHON_ASSUME_SAFE_MACROS
               if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 171, __pyx_L1_error)
               #endif
               if (__pyx_t_6 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 171, __pyx_L1_error)
+            __pyx_t_19 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_6); __Pyx_INCREF(__pyx_t_19); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 171, __pyx_L1_error)
             #else
-            __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_2);
+            __pyx_t_19 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 171, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_19);
             #endif
           } else {
             {
-              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_3);
+              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
               #if !CYTHON_ASSUME_SAFE_MACROS
               if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 171, __pyx_L1_error)
               #endif
               if (__pyx_t_6 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 171, __pyx_L1_error)
+            __pyx_t_19 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_6); __Pyx_INCREF(__pyx_t_19); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 171, __pyx_L1_error)
             #else
-            __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_2);
+            __pyx_t_19 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 171, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_19);
             #endif
           }
         } else {
-          __pyx_t_2 = __pyx_t_32(__pyx_t_3);
-          if (unlikely(!__pyx_t_2)) {
+          __pyx_t_19 = __pyx_t_32(__pyx_t_4);
+          if (unlikely(!__pyx_t_19)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
               else __PYX_ERR(0, 171, __pyx_L1_error)
             }
             break;
           }
-          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_GOTREF(__pyx_t_19);
         }
-        __pyx_t_33 = __Pyx_PyInt_As_long(__pyx_t_2); if (unlikely((__pyx_t_33 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 171, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __pyx_t_33 = __Pyx_PyInt_As_long(__pyx_t_19); if (unlikely((__pyx_t_33 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 171, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
         __pyx_v_v = __pyx_t_33;
 
         /* "UQPyL/surrogates/mars_/_pruning.pyx":172
  *                 bf = self.basis[best_bf_to_prune]
  *                 for v in bf.variables():
  *                     variables.add(v)             # <<<<<<<<<<<<<<
  *                 for v in variables:
  *                     if RSS in self.feature_importance:
  */
-        __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_v); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_34 = PySet_Add(__pyx_v_variables, __pyx_t_2); if (unlikely(__pyx_t_34 == ((int)-1))) __PYX_ERR(0, 172, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __pyx_t_19 = __Pyx_PyInt_From_long(__pyx_v_v); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 172, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_19);
+        __pyx_t_34 = PySet_Add(__pyx_v_variables, __pyx_t_19); if (unlikely(__pyx_t_34 == ((int)-1))) __PYX_ERR(0, 172, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
 
         /* "UQPyL/surrogates/mars_/_pruning.pyx":171
  *                 variables = set()
  *                 bf = self.basis[best_bf_to_prune]
  *                 for v in bf.variables():             # <<<<<<<<<<<<<<
  *                     variables.add(v)
  *                 for v in variables:
  */
       }
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":173
  *                 for v in bf.variables():
  *                     variables.add(v)
  *                 for v in variables:             # <<<<<<<<<<<<<<
  *                     if RSS in self.feature_importance:
  *                         self.feature_importance[RSS][v] += mse_decrease
  */
       __pyx_t_6 = 0;
-      __pyx_t_2 = __Pyx_set_iterator(__pyx_v_variables, 1, (&__pyx_t_35), (&__pyx_t_5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_XDECREF(__pyx_t_3);
-      __pyx_t_3 = __pyx_t_2;
-      __pyx_t_2 = 0;
+      __pyx_t_19 = __Pyx_set_iterator(__pyx_v_variables, 1, (&__pyx_t_35), (&__pyx_t_5)); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 173, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __Pyx_XDECREF(__pyx_t_4);
+      __pyx_t_4 = __pyx_t_19;
+      __pyx_t_19 = 0;
       while (1) {
-        __pyx_t_36 = __Pyx_set_iter_next(__pyx_t_3, __pyx_t_35, &__pyx_t_6, &__pyx_t_2, __pyx_t_5);
+        __pyx_t_36 = __Pyx_set_iter_next(__pyx_t_4, __pyx_t_35, &__pyx_t_6, &__pyx_t_19, __pyx_t_5);
         if (unlikely(__pyx_t_36 == 0)) break;
         if (unlikely(__pyx_t_36 == -1)) __PYX_ERR(0, 173, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_33 = __Pyx_PyInt_As_long(__pyx_t_2); if (unlikely((__pyx_t_33 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_GOTREF(__pyx_t_19);
+        __pyx_t_33 = __Pyx_PyInt_As_long(__pyx_t_19); if (unlikely((__pyx_t_33 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
         __pyx_v_v = __pyx_t_33;
 
         /* "UQPyL/surrogates/mars_/_pruning.pyx":174
  *                     variables.add(v)
  *                 for v in variables:
  *                     if RSS in self.feature_importance:             # <<<<<<<<<<<<<<
  *                         self.feature_importance[RSS][v] += mse_decrease
  *                     if GCV in self.feature_importance:
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_RSS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_GetModuleGlobalName(__pyx_t_19, __pyx_n_s_RSS); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 174, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_19);
         if (unlikely(__pyx_v_self->feature_importance == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
           __PYX_ERR(0, 174, __pyx_L1_error)
         }
-        __pyx_t_30 = (__Pyx_PyDict_ContainsTF(__pyx_t_2, __pyx_v_self->feature_importance, Py_EQ)); if (unlikely((__pyx_t_30 < 0))) __PYX_ERR(0, 174, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __pyx_t_30 = (__Pyx_PyDict_ContainsTF(__pyx_t_19, __pyx_v_self->feature_importance, Py_EQ)); if (unlikely((__pyx_t_30 < 0))) __PYX_ERR(0, 174, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
         if (__pyx_t_30) {
 
           /* "UQPyL/surrogates/mars_/_pruning.pyx":175
  *                 for v in variables:
  *                     if RSS in self.feature_importance:
  *                         self.feature_importance[RSS][v] += mse_decrease             # <<<<<<<<<<<<<<
  *                     if GCV in self.feature_importance:
  *                         self.feature_importance[GCV][v] += gcv_decrease
  */
           if (unlikely(__pyx_v_self->feature_importance == Py_None)) {
             PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
             __PYX_ERR(0, 175, __pyx_L1_error)
           }
-          __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_RSS); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_20 = __Pyx_PyDict_GetItem(__pyx_v_self->feature_importance, __pyx_t_2); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 175, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_20);
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __pyx_t_33 = __pyx_v_v;
-          __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_20, __pyx_t_33, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_22 = PyNumber_InPlaceAdd(__pyx_t_2, __pyx_v_mse_decrease); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 175, __pyx_L1_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_19, __pyx_n_s_RSS); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 175, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_19);
+          __pyx_t_22 = __Pyx_PyDict_GetItem(__pyx_v_self->feature_importance, __pyx_t_19); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 175, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely((__Pyx_SetItemInt(__pyx_t_20, __pyx_t_33, __pyx_t_22, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0))) __PYX_ERR(0, 175, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+          __pyx_t_33 = __pyx_v_v;
+          __pyx_t_19 = __Pyx_GetItemInt(__pyx_t_22, __pyx_t_33, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 175, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_19);
+          __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_t_19, __pyx_v_mse_decrease); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+          if (unlikely((__Pyx_SetItemInt(__pyx_t_22, __pyx_t_33, __pyx_t_1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0))) __PYX_ERR(0, 175, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
           /* "UQPyL/surrogates/mars_/_pruning.pyx":174
  *                     variables.add(v)
  *                 for v in variables:
  *                     if RSS in self.feature_importance:             # <<<<<<<<<<<<<<
  *                         self.feature_importance[RSS][v] += mse_decrease
  *                     if GCV in self.feature_importance:
@@ -9586,49 +9609,49 @@
         /* "UQPyL/surrogates/mars_/_pruning.pyx":176
  *                     if RSS in self.feature_importance:
  *                         self.feature_importance[RSS][v] += mse_decrease
  *                     if GCV in self.feature_importance:             # <<<<<<<<<<<<<<
  *                         self.feature_importance[GCV][v] += gcv_decrease
  *                     if NB_SUBSETS in self.feature_importance:
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_20, __pyx_n_s_GCV); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 176, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_20);
+        __Pyx_GetModuleGlobalName(__pyx_t_22, __pyx_n_s_GCV); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 176, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_22);
         if (unlikely(__pyx_v_self->feature_importance == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
           __PYX_ERR(0, 176, __pyx_L1_error)
         }
-        __pyx_t_30 = (__Pyx_PyDict_ContainsTF(__pyx_t_20, __pyx_v_self->feature_importance, Py_EQ)); if (unlikely((__pyx_t_30 < 0))) __PYX_ERR(0, 176, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+        __pyx_t_30 = (__Pyx_PyDict_ContainsTF(__pyx_t_22, __pyx_v_self->feature_importance, Py_EQ)); if (unlikely((__pyx_t_30 < 0))) __PYX_ERR(0, 176, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
         if (__pyx_t_30) {
 
           /* "UQPyL/surrogates/mars_/_pruning.pyx":177
  *                         self.feature_importance[RSS][v] += mse_decrease
  *                     if GCV in self.feature_importance:
  *                         self.feature_importance[GCV][v] += gcv_decrease             # <<<<<<<<<<<<<<
  *                     if NB_SUBSETS in self.feature_importance:
  *                         self.feature_importance[NB_SUBSETS][v] += 1
  */
           if (unlikely(__pyx_v_self->feature_importance == Py_None)) {
             PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
             __PYX_ERR(0, 177, __pyx_L1_error)
           }
-          __Pyx_GetModuleGlobalName(__pyx_t_20, __pyx_n_s_GCV); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 177, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_20);
-          __pyx_t_22 = __Pyx_PyDict_GetItem(__pyx_v_self->feature_importance, __pyx_t_20); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 177, __pyx_L1_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_22, __pyx_n_s_GCV); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 177, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+          __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_self->feature_importance, __pyx_t_22); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
           __pyx_t_33 = __pyx_v_v;
-          __pyx_t_20 = __Pyx_GetItemInt(__pyx_t_22, __pyx_t_33, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 177, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_20);
-          __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_t_20, __pyx_v_gcv_decrease); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-          if (unlikely((__Pyx_SetItemInt(__pyx_t_22, __pyx_t_33, __pyx_t_2, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0))) __PYX_ERR(0, 177, __pyx_L1_error)
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          __pyx_t_22 = __Pyx_GetItemInt(__pyx_t_1, __pyx_t_33, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 177, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_22);
+          __pyx_t_19 = PyNumber_InPlaceAdd(__pyx_t_22, __pyx_v_gcv_decrease); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 177, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_19);
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+          if (unlikely((__Pyx_SetItemInt(__pyx_t_1, __pyx_t_33, __pyx_t_19, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0))) __PYX_ERR(0, 177, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
           /* "UQPyL/surrogates/mars_/_pruning.pyx":176
  *                     if RSS in self.feature_importance:
  *                         self.feature_importance[RSS][v] += mse_decrease
  *                     if GCV in self.feature_importance:             # <<<<<<<<<<<<<<
  *                         self.feature_importance[GCV][v] += gcv_decrease
  *                     if NB_SUBSETS in self.feature_importance:
@@ -9638,60 +9661,60 @@
         /* "UQPyL/surrogates/mars_/_pruning.pyx":178
  *                     if GCV in self.feature_importance:
  *                         self.feature_importance[GCV][v] += gcv_decrease
  *                     if NB_SUBSETS in self.feature_importance:             # <<<<<<<<<<<<<<
  *                         self.feature_importance[NB_SUBSETS][v] += 1
  *             # The inner loop found the best basis function to remove for this
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_22, __pyx_n_s_NB_SUBSETS); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 178, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_22);
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_NB_SUBSETS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
         if (unlikely(__pyx_v_self->feature_importance == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
           __PYX_ERR(0, 178, __pyx_L1_error)
         }
-        __pyx_t_30 = (__Pyx_PyDict_ContainsTF(__pyx_t_22, __pyx_v_self->feature_importance, Py_EQ)); if (unlikely((__pyx_t_30 < 0))) __PYX_ERR(0, 178, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+        __pyx_t_30 = (__Pyx_PyDict_ContainsTF(__pyx_t_1, __pyx_v_self->feature_importance, Py_EQ)); if (unlikely((__pyx_t_30 < 0))) __PYX_ERR(0, 178, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         if (__pyx_t_30) {
 
           /* "UQPyL/surrogates/mars_/_pruning.pyx":179
  *                         self.feature_importance[GCV][v] += gcv_decrease
  *                     if NB_SUBSETS in self.feature_importance:
  *                         self.feature_importance[NB_SUBSETS][v] += 1             # <<<<<<<<<<<<<<
  *             # The inner loop found the best basis function to remove for this
  *             # iteration. Now check whether this iteration is better than all
  */
           if (unlikely(__pyx_v_self->feature_importance == Py_None)) {
             PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
             __PYX_ERR(0, 179, __pyx_L1_error)
           }
-          __Pyx_GetModuleGlobalName(__pyx_t_22, __pyx_n_s_NB_SUBSETS); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 179, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_self->feature_importance, __pyx_t_22); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_NB_SUBSETS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __pyx_t_19 = __Pyx_PyDict_GetItem(__pyx_v_self->feature_importance, __pyx_t_1); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 179, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_19);
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_t_33 = __pyx_v_v;
-          __pyx_t_22 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_33, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 179, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_19, __pyx_t_33, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __pyx_t_22 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 179, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_22);
-          __pyx_t_20 = __Pyx_PyInt_AddObjC(__pyx_t_22, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 179, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_20);
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          if (unlikely((__Pyx_SetItemInt(__pyx_t_19, __pyx_t_33, __pyx_t_22, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0))) __PYX_ERR(0, 179, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-          if (unlikely((__Pyx_SetItemInt(__pyx_t_2, __pyx_t_33, __pyx_t_20, long, 1, __Pyx_PyInt_From_long, 0, 0, 0) < 0))) __PYX_ERR(0, 179, __pyx_L1_error)
-          __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+          __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
 
           /* "UQPyL/surrogates/mars_/_pruning.pyx":178
  *                     if GCV in self.feature_importance:
  *                         self.feature_importance[GCV][v] += gcv_decrease
  *                     if NB_SUBSETS in self.feature_importance:             # <<<<<<<<<<<<<<
  *                         self.feature_importance[NB_SUBSETS][v] += 1
  *             # The inner loop found the best basis function to remove for this
  */
         }
       }
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":163
  * 
  *             # Feature importance
  *             if i > 1:             # <<<<<<<<<<<<<<
  *                 # having selected the best basis to prune, we compute how much
  *                 # that basis decreased the mse and gcv relative to the previous mse and gcv
@@ -9738,106 +9761,106 @@
     /* "UQPyL/surrogates/mars_/_pruning.pyx":187
  *                 best_iteration = i
  * 
  *             prev_best_iteration_gcv = best_iteration_gcv             # <<<<<<<<<<<<<<
  *             prev_best_iteration_mse = best_iteration_mse
  *             # Update the record and prune the selected basis function
  */
-    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_best_iteration_gcv); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF_SET(__pyx_v_prev_best_iteration_gcv, __pyx_t_3);
-    __pyx_t_3 = 0;
+    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_best_iteration_gcv); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF_SET(__pyx_v_prev_best_iteration_gcv, __pyx_t_4);
+    __pyx_t_4 = 0;
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":188
  * 
  *             prev_best_iteration_gcv = best_iteration_gcv
  *             prev_best_iteration_mse = best_iteration_mse             # <<<<<<<<<<<<<<
  *             # Update the record and prune the selected basis function
  *             self.record.append(PruningPassIteration(
  */
-    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_best_iteration_mse); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF_SET(__pyx_v_prev_best_iteration_mse, __pyx_t_3);
-    __pyx_t_3 = 0;
+    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_best_iteration_mse); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF_SET(__pyx_v_prev_best_iteration_mse, __pyx_t_4);
+    __pyx_t_4 = 0;
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":191
  *             # Update the record and prune the selected basis function
  *             self.record.append(PruningPassIteration(
  *                 best_bf_to_prune, pruned_basis_size, best_iteration_mse / total_weight))             # <<<<<<<<<<<<<<
  *             self.basis[best_bf_to_prune].prune()
  * 
  */
-    __pyx_t_3 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_best_bf_to_prune); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_pruned_basis_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_20 = PyFloat_FromDouble((__pyx_v_best_iteration_mse / __pyx_v_total_weight)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 191, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_20);
+    __pyx_t_4 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_best_bf_to_prune); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_19 = __Pyx_PyInt_From_Py_intptr_t(__pyx_v_pruned_basis_size); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_19);
+    __pyx_t_22 = PyFloat_FromDouble((__pyx_v_best_iteration_mse / __pyx_v_total_weight)); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_22);
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":190
  *             prev_best_iteration_mse = best_iteration_mse
  *             # Update the record and prune the selected basis function
  *             self.record.append(PruningPassIteration(             # <<<<<<<<<<<<<<
  *                 best_bf_to_prune, pruned_basis_size, best_iteration_mse / total_weight))
  *             self.basis[best_bf_to_prune].prune()
  */
-    __pyx_t_22 = PyTuple_New(3); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 190, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_22);
-    __Pyx_GIVEREF(__pyx_t_3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 0, __pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error);
-    __Pyx_GIVEREF(__pyx_t_2);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 1, __pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error);
-    __Pyx_GIVEREF(__pyx_t_20);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_22, 2, __pyx_t_20)) __PYX_ERR(0, 190, __pyx_L1_error);
-    __pyx_t_3 = 0;
-    __pyx_t_2 = 0;
-    __pyx_t_20 = 0;
-    __pyx_t_20 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5UQPyL_10surrogates_5mars__7_record_PruningPassIteration), __pyx_t_22, NULL); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 190, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_20);
-    __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-    __pyx_t_22 = ((struct __pyx_vtabstruct_5UQPyL_10surrogates_5mars__7_record_PruningPassRecord *)__pyx_v_self->record->__pyx_base.__pyx_vtab)->__pyx_base.append(((struct __pyx_obj_5UQPyL_10surrogates_5mars__7_record_Record *)__pyx_v_self->record), ((struct __pyx_obj_5UQPyL_10surrogates_5mars__7_record_Iteration *)__pyx_t_20), 0); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_4);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4)) __PYX_ERR(0, 190, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_19);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_19)) __PYX_ERR(0, 190, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_22);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_22)) __PYX_ERR(0, 190, __pyx_L1_error);
+    __pyx_t_4 = 0;
+    __pyx_t_19 = 0;
+    __pyx_t_22 = 0;
+    __pyx_t_22 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5UQPyL_10surrogates_5mars__7_record_PruningPassIteration), __pyx_t_1, NULL); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_22);
-    __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = ((struct __pyx_vtabstruct_5UQPyL_10surrogates_5mars__7_record_PruningPassRecord *)__pyx_v_self->record->__pyx_base.__pyx_vtab)->__pyx_base.append(((struct __pyx_obj_5UQPyL_10surrogates_5mars__7_record_Record *)__pyx_v_self->record), ((struct __pyx_obj_5UQPyL_10surrogates_5mars__7_record_Iteration *)__pyx_t_22), 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":192
  *             self.record.append(PruningPassIteration(
  *                 best_bf_to_prune, pruned_basis_size, best_iteration_mse / total_weight))
  *             self.basis[best_bf_to_prune].prune()             # <<<<<<<<<<<<<<
  * 
  *             if self.verbose >= 1:
  */
-    __pyx_t_20 = __Pyx_GetItemInt(((PyObject *)__pyx_v_self->basis), __pyx_v_best_bf_to_prune, __pyx_t_5UQPyL_10surrogates_5mars__6_types_INDEX_t, 1, __Pyx_PyInt_From_Py_intptr_t, 0, 0, 0); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 192, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_20);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_20, __pyx_n_s_prune); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-    __pyx_t_20 = NULL;
+    __pyx_t_22 = __Pyx_GetItemInt(((PyObject *)__pyx_v_self->basis), __pyx_v_best_bf_to_prune, __pyx_t_5UQPyL_10surrogates_5mars__6_types_INDEX_t, 1, __Pyx_PyInt_From_Py_intptr_t, 0, 0, 0); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_22);
+    __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_t_22, __pyx_n_s_prune); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_19);
+    __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+    __pyx_t_22 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_20 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_20)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_20);
+    if (likely(PyMethod_Check(__pyx_t_19))) {
+      __pyx_t_22 = PyMethod_GET_SELF(__pyx_t_19);
+      if (likely(__pyx_t_22)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_19);
+        __Pyx_INCREF(__pyx_t_22);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_19, function);
         __pyx_t_5 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_20, NULL};
-      __pyx_t_22 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
-      __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
-      if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 192, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_22);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_22, NULL};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_19, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
+      __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
     }
-    __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":194
  *             self.basis[best_bf_to_prune].prune()
  * 
  *             if self.verbose >= 1:             # <<<<<<<<<<<<<<
  *                 print(self.record.partial_str(slice(-1, None, None), print_header=False, print_footer=(pruned_basis_size == 1)))
  * 
@@ -9848,31 +9871,31 @@
       /* "UQPyL/surrogates/mars_/_pruning.pyx":195
  * 
  *             if self.verbose >= 1:
  *                 print(self.record.partial_str(slice(-1, None, None), print_header=False, print_footer=(pruned_basis_size == 1)))             # <<<<<<<<<<<<<<
  * 
  *         # Unprune the basis functions pruned after the best iteration
  */
-      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->record), __pyx_n_s_partial_str); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->record), __pyx_n_s_partial_str); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_19 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      if (PyDict_SetItem(__pyx_t_19, __pyx_n_s_print_header, Py_False) < 0) __PYX_ERR(0, 195, __pyx_L1_error)
+      __pyx_t_22 = __Pyx_PyBool_FromLong((__pyx_v_pruned_basis_size == 1)); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 195, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_22);
-      __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_print_header, Py_False) < 0) __PYX_ERR(0, 195, __pyx_L1_error)
-      __pyx_t_20 = __Pyx_PyBool_FromLong((__pyx_v_pruned_basis_size == 1)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_20);
-      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_print_footer, __pyx_t_20) < 0) __PYX_ERR(0, 195, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-      __pyx_t_20 = __Pyx_PyObject_Call(__pyx_t_22, __pyx_tuple__8, __pyx_t_2); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_20);
+      if (PyDict_SetItem(__pyx_t_19, __pyx_n_s_print_footer, __pyx_t_22) < 0) __PYX_ERR(0, 195, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_22 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__8, __pyx_t_19); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_22);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+      __pyx_t_19 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_22); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 195, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":194
  *             self.basis[best_bf_to_prune].prune()
  * 
  *             if self.verbose >= 1:             # <<<<<<<<<<<<<<
  *                 print(self.record.partial_str(slice(-1, None, None), print_header=False, print_footer=(pruned_basis_size == 1)))
  * 
@@ -9883,31 +9906,31 @@
   /* "UQPyL/surrogates/mars_/_pruning.pyx":198
  * 
  *         # Unprune the basis functions pruned after the best iteration
  *         self.record.set_selected(best_iteration)             # <<<<<<<<<<<<<<
  *         self.record.roll_back(self.basis)
  *         if self.verbose >= 1:
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_5UQPyL_10surrogates_5mars__7_record_PruningPassRecord *)__pyx_v_self->record->__pyx_base.__pyx_vtab)->set_selected(__pyx_v_self->record, __pyx_v_best_iteration, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_19 = ((struct __pyx_vtabstruct_5UQPyL_10surrogates_5mars__7_record_PruningPassRecord *)__pyx_v_self->record->__pyx_base.__pyx_vtab)->set_selected(__pyx_v_self->record, __pyx_v_best_iteration, 0); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_19);
+  __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
 
   /* "UQPyL/surrogates/mars_/_pruning.pyx":199
  *         # Unprune the basis functions pruned after the best iteration
  *         self.record.set_selected(best_iteration)
  *         self.record.roll_back(self.basis)             # <<<<<<<<<<<<<<
  *         if self.verbose >= 1:
  *             print(self.record.final_str())
  */
-  __pyx_t_2 = ((PyObject *)__pyx_v_self->basis);
-  __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_20 = ((struct __pyx_vtabstruct_5UQPyL_10surrogates_5mars__7_record_PruningPassRecord *)__pyx_v_self->record->__pyx_base.__pyx_vtab)->roll_back(__pyx_v_self->record, ((struct __pyx_obj_5UQPyL_10surrogates_5mars__6_basis_Basis *)__pyx_t_2), 0); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 199, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_20);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+  __pyx_t_19 = ((PyObject *)__pyx_v_self->basis);
+  __Pyx_INCREF(__pyx_t_19);
+  __pyx_t_22 = ((struct __pyx_vtabstruct_5UQPyL_10surrogates_5mars__7_record_PruningPassRecord *)__pyx_v_self->record->__pyx_base.__pyx_vtab)->roll_back(__pyx_v_self->record, ((struct __pyx_obj_5UQPyL_10surrogates_5mars__6_basis_Basis *)__pyx_t_19), 0); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_22);
+  __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+  __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
 
   /* "UQPyL/surrogates/mars_/_pruning.pyx":200
  *         self.record.set_selected(best_iteration)
  *         self.record.roll_back(self.basis)
  *         if self.verbose >= 1:             # <<<<<<<<<<<<<<
  *             print(self.record.final_str())
  * 
@@ -9918,42 +9941,42 @@
     /* "UQPyL/surrogates/mars_/_pruning.pyx":201
  *         self.record.roll_back(self.basis)
  *         if self.verbose >= 1:
  *             print(self.record.final_str())             # <<<<<<<<<<<<<<
  * 
  *         # normalize feature importance values
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->record), __pyx_n_s_final_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_22 = NULL;
+    __pyx_t_19 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self->record), __pyx_n_s_final_str); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_19);
+    __pyx_t_1 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_22 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_22)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_22);
+    if (likely(PyMethod_Check(__pyx_t_19))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_19);
+      if (likely(__pyx_t_1)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_19);
+        __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_19, function);
         __pyx_t_5 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_22, NULL};
-      __pyx_t_20 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
-      __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
-      if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 201, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_20);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
+      __pyx_t_22 = __Pyx_PyObject_FastCall(__pyx_t_19, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
+      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 201, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_22);
+      __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
     }
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_19 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_22); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_19);
+    __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+    __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":200
  *         self.record.set_selected(best_iteration)
  *         self.record.roll_back(self.basis)
  *         if self.verbose >= 1:             # <<<<<<<<<<<<<<
  *             print(self.record.final_str())
  * 
@@ -9968,29 +9991,29 @@
  *                 val[val < 0] = 0 # gcv can have negative feature importance correponding to an increase of gcv, set them to zero
  */
   __pyx_t_35 = 0;
   if (unlikely(__pyx_v_self->feature_importance == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
     __PYX_ERR(0, 204, __pyx_L1_error)
   }
-  __pyx_t_20 = __Pyx_dict_iterator(__pyx_v_self->feature_importance, 1, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_5)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 204, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_20);
-  __Pyx_XDECREF(__pyx_t_2);
-  __pyx_t_2 = __pyx_t_20;
-  __pyx_t_20 = 0;
+  __pyx_t_22 = __Pyx_dict_iterator(__pyx_v_self->feature_importance, 1, __pyx_n_s_items, (&__pyx_t_6), (&__pyx_t_5)); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_22);
+  __Pyx_XDECREF(__pyx_t_19);
+  __pyx_t_19 = __pyx_t_22;
+  __pyx_t_22 = 0;
   while (1) {
-    __pyx_t_36 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_6, &__pyx_t_35, &__pyx_t_20, &__pyx_t_22, NULL, __pyx_t_5);
+    __pyx_t_36 = __Pyx_dict_iter_next(__pyx_t_19, __pyx_t_6, &__pyx_t_35, &__pyx_t_22, &__pyx_t_1, NULL, __pyx_t_5);
     if (unlikely(__pyx_t_36 == 0)) break;
     if (unlikely(__pyx_t_36 == -1)) __PYX_ERR(0, 204, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_20);
     __Pyx_GOTREF(__pyx_t_22);
-    __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_20);
-    __pyx_t_20 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_val, __pyx_t_22);
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_22);
     __pyx_t_22 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_val, __pyx_t_1);
+    __pyx_t_1 = 0;
 
     /* "UQPyL/surrogates/mars_/_pruning.pyx":205
  *         # normalize feature importance values
  *         for name, val in self.feature_importance.items():
  *             if name == 'gcv':             # <<<<<<<<<<<<<<
  *                 val[val < 0] = 0 # gcv can have negative feature importance correponding to an increase of gcv, set them to zero
  *             if val.sum() > 0:
@@ -10001,17 +10024,17 @@
       /* "UQPyL/surrogates/mars_/_pruning.pyx":206
  *         for name, val in self.feature_importance.items():
  *             if name == 'gcv':
  *                 val[val < 0] = 0 # gcv can have negative feature importance correponding to an increase of gcv, set them to zero             # <<<<<<<<<<<<<<
  *             if val.sum() > 0:
  *                 val /= val.sum()
  */
-      __pyx_t_22 = PyObject_RichCompare(__pyx_v_val, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_22); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 206, __pyx_L1_error)
-      if (unlikely((PyObject_SetItem(__pyx_v_val, __pyx_t_22, __pyx_int_0) < 0))) __PYX_ERR(0, 206, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+      __pyx_t_1 = PyObject_RichCompare(__pyx_v_val, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
+      if (unlikely((PyObject_SetItem(__pyx_v_val, __pyx_t_1, __pyx_int_0) < 0))) __PYX_ERR(0, 206, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":205
  *         # normalize feature importance values
  *         for name, val in self.feature_importance.items():
  *             if name == 'gcv':             # <<<<<<<<<<<<<<
  *                 val[val < 0] = 0 # gcv can have negative feature importance correponding to an increase of gcv, set them to zero
  *             if val.sum() > 0:
@@ -10021,80 +10044,80 @@
     /* "UQPyL/surrogates/mars_/_pruning.pyx":207
  *             if name == 'gcv':
  *                 val[val < 0] = 0 # gcv can have negative feature importance correponding to an increase of gcv, set them to zero
  *             if val.sum() > 0:             # <<<<<<<<<<<<<<
  *                 val /= val.sum()
  *             self.feature_importance[name] = val
  */
-    __pyx_t_20 = __Pyx_PyObject_GetAttrStr(__pyx_v_val, __pyx_n_s_sum); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_20);
-    __pyx_t_3 = NULL;
+    __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_v_val, __pyx_n_s_sum); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_22);
+    __pyx_t_4 = NULL;
     __pyx_t_36 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_20))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_20);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_20);
-        __Pyx_INCREF(__pyx_t_3);
+    if (likely(PyMethod_Check(__pyx_t_22))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_22);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_22);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_20, function);
+        __Pyx_DECREF_SET(__pyx_t_22, function);
         __pyx_t_36 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
-      __pyx_t_22 = __Pyx_PyObject_FastCall(__pyx_t_20, __pyx_callargs+1-__pyx_t_36, 0+__pyx_t_36);
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 207, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_22);
-      __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_22, __pyx_callargs+1-__pyx_t_36, 0+__pyx_t_36);
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
     }
-    __pyx_t_20 = PyObject_RichCompare(__pyx_t_22, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_20); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __pyx_t_22 = PyObject_RichCompare(__pyx_t_1, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_22); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_30 = __Pyx_PyObject_IsTrue(__pyx_t_22); if (unlikely((__pyx_t_30 < 0))) __PYX_ERR(0, 207, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
-    __pyx_t_30 = __Pyx_PyObject_IsTrue(__pyx_t_20); if (unlikely((__pyx_t_30 < 0))) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     if (__pyx_t_30) {
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":208
  *                 val[val < 0] = 0 # gcv can have negative feature importance correponding to an increase of gcv, set them to zero
  *             if val.sum() > 0:
  *                 val /= val.sum()             # <<<<<<<<<<<<<<
  *             self.feature_importance[name] = val
  * 
  */
-      __pyx_t_22 = __Pyx_PyObject_GetAttrStr(__pyx_v_val, __pyx_n_s_sum); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 208, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_22);
-      __pyx_t_3 = NULL;
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_val, __pyx_n_s_sum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_4 = NULL;
       __pyx_t_36 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (likely(PyMethod_Check(__pyx_t_22))) {
-        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_22);
-        if (likely(__pyx_t_3)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_22);
-          __Pyx_INCREF(__pyx_t_3);
+      if (likely(PyMethod_Check(__pyx_t_1))) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_4)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+          __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_22, function);
+          __Pyx_DECREF_SET(__pyx_t_1, function);
           __pyx_t_36 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
-        __pyx_t_20 = __Pyx_PyObject_FastCall(__pyx_t_22, __pyx_callargs+1-__pyx_t_36, 0+__pyx_t_36);
-        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 208, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_20);
-        __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+        PyObject *__pyx_callargs[2] = {__pyx_t_4, NULL};
+        __pyx_t_22 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_36, 0+__pyx_t_36);
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 208, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_22);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __pyx_t_22 = __Pyx_PyNumber_InPlaceDivide(__pyx_v_val, __pyx_t_20); if (unlikely(!__pyx_t_22)) __PYX_ERR(0, 208, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_22);
-      __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-      __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_22);
-      __pyx_t_22 = 0;
+      __pyx_t_1 = __Pyx_PyNumber_InPlaceDivide(__pyx_v_val, __pyx_t_22); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_22); __pyx_t_22 = 0;
+      __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_1);
+      __pyx_t_1 = 0;
 
       /* "UQPyL/surrogates/mars_/_pruning.pyx":207
  *             if name == 'gcv':
  *                 val[val < 0] = 0 # gcv can have negative feature importance correponding to an increase of gcv, set them to zero
  *             if val.sum() > 0:             # <<<<<<<<<<<<<<
  *                 val /= val.sum()
  *             self.feature_importance[name] = val
@@ -10110,15 +10133,15 @@
  */
     if (unlikely(__pyx_v_self->feature_importance == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(0, 209, __pyx_L1_error)
     }
     if (unlikely((PyDict_SetItem(__pyx_v_self->feature_importance, __pyx_v_name, __pyx_v_val) < 0))) __PYX_ERR(0, 209, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
 
   /* "UQPyL/surrogates/mars_/_pruning.pyx":47
  *             self.feature_importance[criterion] = np.zeros((self.n,))
  * 
  *     cpdef run(PruningPasser self):             # <<<<<<<<<<<<<<
  *         # This is a totally naive implementation and could potentially be made
  *         # faster through the use of updating algorithms.  It is not clear that
@@ -11954,14 +11977,15 @@
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_PruningPasser, __pyx_k_pyx_unpickle_PruningPasser, sizeof(__pyx_k_pyx_unpickle_PruningPasser), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
+    {&__pyx_n_s_rcond, __pyx_k_rcond, sizeof(__pyx_k_rcond), 0, 0, 1, 1},
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
     {&__pyx_n_s_rss, __pyx_k_rss, sizeof(__pyx_k_rss), 0, 0, 1, 1},
     {&__pyx_n_s_run, __pyx_k_run, sizeof(__pyx_k_run), 0, 0, 1, 1},
     {&__pyx_n_s_sample_weight, __pyx_k_sample_weight, sizeof(__pyx_k_sample_weight), 0, 0, 1, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
@@ -12048,15 +12072,15 @@
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_Beginning_pruning_pass); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "UQPyL/surrogates/mars_/_pruning.pyx":99
  *             else:
  *                 self.basis.weighted_transform(X, missing, B, sample_weight[:, p])
- *             beta, mse_ = np.linalg.lstsq(B[:, 0:(basis_size)], weighted_y)[0:2]             # <<<<<<<<<<<<<<
+ *             beta, mse_ = np.linalg.lstsq(B[:, 0:(basis_size)], weighted_y, rcond=None)[0:2]             # <<<<<<<<<<<<<<
  *             if mse_:
  *                 pass
  */
   __pyx_slice__6 = PySlice_New(__pyx_int_0, __pyx_int_2, Py_None); if (unlikely(!__pyx_slice__6)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__6);
   __Pyx_GIVEREF(__pyx_slice__6);
```

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/mars_/_qr.c` & `UQPyL-2.0.3/UQPyL/surrogates/mars_/_qr.c`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/mars_/_record.c` & `UQPyL-2.0.3/UQPyL/surrogates/mars_/_record.c`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/mars_/_types.c` & `UQPyL-2.0.3/UQPyL/surrogates/mars_/_types.c`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/mars_/_util.c` & `UQPyL-2.0.3/UQPyL/surrogates/mars_/_util.c`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/mlp_utility/_activation_funcs.py` & `UQPyL-2.0.3/UQPyL/surrogates/mlp_utility/_activation_funcs.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/mlp_utility/base.py` & `UQPyL-2.0.3/UQPyL/surrogates/mlp_utility/base.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/polynomial_regression.py` & `UQPyL-2.0.3/UQPyL/surrogates/polynomial_regression.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,54 +10,54 @@
 class PolynomialRegression(LinearRegression):
     """
     PolynomialRegression
     """
     
     def __init__(self, scalers: Tuple[Optional[Scaler], Optional[Scaler]]=(None, None),
                  poly_feature: PolynomialFeatures=None,
-                 Type: Literal['Origin', 'Ridge', 'Lasso']='Origin',
+                 loss_type: Literal['Origin', 'Ridge', 'Lasso']='Origin',
                  interaction_only: bool=False,
                  degree: int=2, fit_intercept: bool=True,
                  alpha: float=0.6, epoch: int=100, lr: float=1e-6, tl: float=1e-4):
         
         super().__init__(scalers=scalers, poly_feature=poly_feature,
-                         Type=Type, fit_intercept=fit_intercept, alpha=alpha,
+                         loss_type=loss_type, fit_intercept=fit_intercept, alpha=alpha,
                          epoch=epoch, lr=lr, tl=tl)
         
         self.degree=degree
         self.interaction_only=interaction_only
         
         if self.poly_feature and self.poly_feature.include_bias and self.fit_intercept:
             raise ValueError("The setting ( include_bias of PolyFeature and fit_intercept ) can not be turned on together.")
         
 ###------------------------public functions-----------------------------###
     def fit(self, trainX: np.ndarray, trainY: np.ndarray):
         
         trainX, trainY=self.__check_and_scale__(trainX, trainY)
         
-        # self.outTrainX_=self.polynomial_features(trainX)
+        trainX_=self.polynomial_features(trainX)
         
-        if self.type=='Origin':
-            self._fit_Origin(trainX, trainY)
-        elif self.type=='Ridge':
-            self._fit_Ridge(trainX, trainY)
-        elif self.type=='Lasso':
-            self._fit_Lasso(trainX, trainY)
+        if self.loss_type=='Origin':
+            self._fit_Origin(trainX_, trainY)
+        elif self.loss_type=='Ridge':
+            self._fit_Ridge(trainX_, trainY)
+        elif self.loss_type=='Lasso':
+            self._fit_Lasso(trainX_, trainY)
         else:
             raise ValueError('Using wrong model type!')
         
     def predict(self, predict_X: np.ndarray) -> np.ndarray:
         
         predict_X=self.__X_transform__(predict_X)
-       
+        predict_X_=self.polynomial_features(predict_X)
         if self.fit_intercept:
-            predict_Y=predict_X@self.coef_+self.intercept_
+            predict_Y=predict_X_@self.coef_+self.intercept_
         else:
-            predict_Y=predict_X@self.coef_
-        
+            predict_Y=predict_X_@self.coef_
+        predict_Y=predict_Y.reshape(-1,1)
         return self.__Y_inverse_transform__(predict_Y)
     
 ###------------------------private functions-----------------------------###
     def polynomial_features(self, trainX: np.ndarray):
         
         n_samples, n_features=trainX.shape
         n_output_features=0
```

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/radial_basis_function.py` & `UQPyL-2.0.3/UQPyL/surrogates/radial_basis_function.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/rbf_kernels/thin_plate_spline_kernel.py` & `UQPyL-2.0.3/UQPyL/surrogates/rbf_kernels/thin_plate_spline_kernel.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/support_vector_machine.py` & `UQPyL-2.0.3/UQPyL/surrogates/support_vector_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from .svr_ import svm_fit, svm_predict, Parameter 
-from typing import Tuple, Literal, Optional
-from .surrogate_ABC import Scale_T, Surrogate
+from typing import Literal, Optional
+from .surrogate_ABC import Surrogate
 from ..utility.polynomial_features import PolynomialFeatures
 LINEAR = 0
 POLYNOMIAL = 1
 RBF = 2
 SIGMOID = 3
 
 class SVR(Surrogate):
```

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/svr_/libsvm_interface.cpp` & `UQPyL-2.0.3/UQPyL/surrogates/svr_/libsvm_interface.cpp`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/surrogates/svr_/svm.cpp` & `UQPyL-2.0.3/UQPyL/surrogates/svr_/svm.cpp`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/utility/grid_search.py` & `UQPyL-2.0.3/UQPyL/utility/grid_search.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/utility/metrics.py` & `UQPyL-2.0.3/UQPyL/utility/metrics.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/utility/model_selections.py` & `UQPyL-2.0.3/UQPyL/utility/model_selections.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/utility/polynomial_features.py` & `UQPyL-2.0.3/UQPyL/utility/polynomial_features.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL/utility/scalers.py` & `UQPyL-2.0.3/UQPyL/utility/scalers.py`

 * *Files identical despite different names*

### Comparing `UQPyL-2.0.1/UQPyL.egg-info/PKG-INFO` & `UQPyL-2.0.3/UQPyL.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UQPyL
-Version: 2.0.1
+Version: 2.0.3
 Summary: A python package for parameter uncertainty quantification and optimization
 Author: wmtSky
 Author-email: wmtSky <wmtsky@hhu.edu.cn>
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,44 +14,76 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Uncertainty Quantification Python Laboratory <br> (UQPyL)
 
-**UQPyL:** The **Uncertainty Quantification Python Laboratory** provide a comprehensive workflow for parameter **uncertainty quantification** and **optimization** in computational numerical simulations. **UQPyL** offers an extensive suite of advanced methodologies(Sobol', Delta Test, EFAST, et al.) and algorithms (NSGA-II, ASMO, MO-ASMO, et al.). In summary, UQPyL consists of four core modules: 
-- Design of Experiments (DoE) 
-- Sensibility Analysis 
-- Optimization
-- Surrogate models
-
-The surrogate models Module can help to solve computational expensive problems caused by intensive numerical simulations.**
-
-Once you have clearly defined the problem you aim to address, you can employ all pre-prepared methods and algorithms to complete following task:
-* Uncertainty Quantification (UQ)
-* Parameter Optimization
-
-Moreover, the versatility of UQPyL allows researchers to craft their own methods or algorithms by incorporating its diverse range of surrogate models. Consequently, users can:
-- Evaluate the effectiveness of their custom-designed algorithms
-- Compare different methods and algorithms under specific problem scenarios
+**UQPyL:** The **Uncertainty Quantification Python Laboratory** provide comprehensive workflows tailored to the **Uncertainty Quantification** and **Optimization** for computational models and their associated applications (e.g. model calibration, resource scheduling, product design). 
 
-  **Website:** http://www.uq-pyl.com/ (**#TODO** it need to update now.) <br>
+The **main characteristics** of UQPyL includes:
+
+1. Implementation of widely used sensitivity analysis methodologies and optimization algorithms.
+
+2. Integration of diverse surrogate models equipped with tunable to solving computational expensive problems.
+
+3. Provision of a comprehensive suite of benchmark problems and practical case studies, enabling users to quick start.
+
+4. A modular and extensible architecture that encourages and facilitates the development of novel methods or algorithms by users, aligning with our commitment to openness and collaboration. (**We appreciate and welcome contributions**)
+
+ **Website:** http://www.uq-pyl.com/ (**#TODO** it need to update now.) <br>
   **Source Code:** https://github.com/smasky/UQPyL/ <br> 
   **Documentation:** **#TODO** <br>
   **Citing in your work:** **#TODO** <br>
 
+# Included Methods and Algorithms
+**Sensibility Analysis:** (all methods support for surrogate models)
+- Sobol'
+- Delta_test (DT)
+- extended Fourier Amplitude Sensitivity Test (eFAST)
+- Random Balance Designs - Fourier Amplitude Sensitivity Test
+- Multivariate Adaptive Regression Splines-Sensibility Analysis (MARS-SA)
+- Morris
+- Regional Sensitivity Analysis (RSA)
+
+**Optimization Algorithms:** (* indicates the use of surrogate models)
+- SCE-UA
+- Genetic Algorithm (GA)
+- Non-dominated Sorting Genetic Algorithm-II (NSGA-II)
+- AMSMO*
+- MO_ASMO*
+- MASTO* #TODO
+- AMSMO* #TODO
+
+**Surrogate Models:**
+- Full connect neural network (FNN)
+- Kriging (KRG)
+- Gaussian Process (GP)
+- Linear Regression (LR)
+- Polynomial Regression (PR)
+- Radial Basis Function (RBF)
+- Support Vector Machine (SVM)
+- Multivariate Adaptive Regression Splines (MARS)
+
 # Installation
 
-` pip install UQPyL ` (Recommend)
+Recommend (PyPi or Conda):
+
+```
+pip install UQPyL
 
-or
+conda install UQPyL
+```
 
-` git clone https://github.com/smasky/UQPyL.git `
+And also:
 
-` cd UQPyL` and ` pip install . `
+```
+git clone https://github.com/smasky/UQPyL.git 
+pip install . 
+```
 
 
 # Call for Contributions
 We appreciate and welcome contributions. Because, we only set up standard workflows here. More advanced quantification methods and optimization algorithms are waited for pulling to this project.
 
 ---
 # Contact:
```

### Comparing `UQPyL-2.0.1/UQPyL.egg-info/SOURCES.txt` & `UQPyL-2.0.3/UQPyL.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,30 +6,35 @@
 UQPyL.egg-info/PKG-INFO
 UQPyL.egg-info/SOURCES.txt
 UQPyL.egg-info/dependency_links.txt
 UQPyL.egg-info/requires.txt
 UQPyL.egg-info/top_level.txt
 UQPyL/DoE/__init__.py
 UQPyL/DoE/_lhs.py
-UQPyL/DoE/fast_sampler.py
+UQPyL/DoE/fast_sequence.py
 UQPyL/DoE/full_fact.py
 UQPyL/DoE/lhs.py
+UQPyL/DoE/morris_sequence.py
 UQPyL/DoE/random.py
 UQPyL/DoE/sampler_ABC.py
 UQPyL/DoE/sobol_sequence.py
 UQPyL/optimization/__init__.py
 UQPyL/optimization/_binary_ga.py
-UQPyL/optimization/_ga.py
 UQPyL/optimization/adam.py
 UQPyL/optimization/asmo.py
 UQPyL/optimization/boxmin.py
 UQPyL/optimization/ga.py
 UQPyL/optimization/mo_asmo.py
+UQPyL/optimization/moea_d.py
 UQPyL/optimization/nsga_ii.py
+UQPyL/optimization/pso.py
 UQPyL/optimization/sce_ua.py
+UQPyL/optimization/utility_functions/_NDsort.py
+UQPyL/optimization/utility_functions/__init__.py
+UQPyL/optimization/utility_functions/_uniformPoint.py
 UQPyL/problems/__init__.py
 UQPyL/problems/multi_DTLZ.py
 UQPyL/problems/multi_ZDT.py
 UQPyL/problems/pratical_problem.py
 UQPyL/problems/problem_ABC.py
 UQPyL/problems/single_Benchmarks.py
 UQPyL/problems/utility_functions/_NDsort.py
@@ -48,21 +53,30 @@
 UQPyL/surrogates/BootstrapEnsemble.py
 UQPyL/surrogates/__init__.py
 UQPyL/surrogates/fully_connect_neural_network.py
 UQPyL/surrogates/gaussian_process.py
 UQPyL/surrogates/kriging.py
 UQPyL/surrogates/linear_regression.py
 UQPyL/surrogates/mars.py
-UQPyL/surrogates/mo_surrogates.py
 UQPyL/surrogates/polynomial_regression.py
 UQPyL/surrogates/radial_basis_function.py
 UQPyL/surrogates/support_vector_machine.py
 UQPyL/surrogates/surrogate_ABC.py
-UQPyL/surrogates/gp_kernels/Kernel.py
 UQPyL/surrogates/gp_kernels/__init__.py
+UQPyL/surrogates/gp_kernels/base_kernel.py
+UQPyL/surrogates/gp_kernels/c_kernel.py
+UQPyL/surrogates/gp_kernels/dot_kernel.py
+UQPyL/surrogates/gp_kernels/matern_kernel.py
+UQPyL/surrogates/gp_kernels/rbf_kernel.py
+UQPyL/surrogates/gp_kernels/rq_kernel.py
+UQPyL/surrogates/krg_kernels/__init__.py
+UQPyL/surrogates/krg_kernels/base_kernel.py
+UQPyL/surrogates/krg_kernels/cubic_kernel.py
+UQPyL/surrogates/krg_kernels/exp_kernel.py
+UQPyL/surrogates/krg_kernels/guass_kernel.py
 UQPyL/surrogates/lasso_/__init__.py
 UQPyL/surrogates/lasso_/lasso_fast.c
 UQPyL/surrogates/mars_/__init__.py
 UQPyL/surrogates/mars_/_basis.c
 UQPyL/surrogates/mars_/_forward.c
 UQPyL/surrogates/mars_/_knot_search.c
 UQPyL/surrogates/mars_/_pruning.c
```

### Comparing `UQPyL-2.0.1/pyproject.toml` & `UQPyL-2.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "numpy",
     
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "UQPyL"
-version = "2.0.1"
+version = "2.0.3"
 authors = [
     {name = "wmtSky", email = "wmtsky@hhu.edu.cn"}
 ]
 description = "A python package for parameter uncertainty quantification and optimization"
 readme = "README.md"
 dependencies = [
   "numpy",
```

### Comparing `UQPyL-2.0.1/setup.py` & `UQPyL-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 #     author="wmtSky",
 #     url='https://https://github.com/smasky/UQPyL',
 #     ext_modules=extensions,
 # )
 setup(
     name="UQPyL",
     author="wmtSky",
-    version="2.0.1",
+    version="2.0.3",
     author_email="wmtsky@hhu.edu.cn",
     # ... 其他常规setup参数 ...
     ext_modules=extensions,  # 如果有自定义的编译行为
     packages=find_packages(),
     description="A python package for parameter uncertainty quantification and optimization",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",  # 如果是Markdown格式
```

