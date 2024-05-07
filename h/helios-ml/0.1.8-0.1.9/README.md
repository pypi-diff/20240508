# Comparing `tmp/helios_ml-0.1.8.tar.gz` & `tmp/helios_ml-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios_ml-0.1.8.tar", last modified: Fri May  3 20:20:58 2024, max compression
+gzip compressed data, was "helios_ml-0.1.9.tar", last modified: Tue May  7 21:58:01 2024, max compression
```

## Comparing `helios_ml-0.1.8.tar` & `helios_ml-0.1.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.118081 helios_ml-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.102081 helios_ml-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.102081 helios_ml-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-03 20:20:12.000000 helios_ml-0.1.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-03 20:20:12.000000 helios_ml-0.1.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-03 20:20:12.000000 helios_ml-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-03 20:20:12.000000 helios_ml-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-03 20:20:12.000000 helios_ml-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-03 20:20:58.118081 helios_ml-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-03 20:20:12.000000 helios_ml-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.102081 helios_ml-0.1.8/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/data/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-05-03 20:20:12.000000 helios_ml-0.1.8/data/logo/logo-background.png
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-03 20:20:12.000000 helios_ml-0.1.8/data/logo/logo-transparent.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.102081 helios_ml-0.1.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/examples/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-05-03 20:20:12.000000 helios_ml-0.1.8/examples/cifar10/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-03 20:20:12.000000 helios_ml-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-03 20:20:12.000000 helios_ml-0.1.8/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-03 20:20:12.000000 helios_ml-0.1.8/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-03 20:20:12.000000 helios_ml-0.1.8/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:20:58.118081 helios_ml-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.102081 helios_ml-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/src/helios/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/src/helios/core/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/rng.py
--rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.106081 helios_ml-0.1.8/src/helios/data/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/data/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/losses/weighted_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/metrics/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/model/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/nn/swa_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/nn/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/optim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.110081 helios_ml-0.1.8/src/helios/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/scheduler/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35697 2024-05-03 20:20:12.000000 helios_ml-0.1.8/src/helios/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.114081 helios_ml-0.1.8/src/helios_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-03 20:20:58.000000 helios_ml-0.1.8/src/helios_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-03 20:20:58.000000 helios_ml-0.1.8/src/helios_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:20:58.000000 helios_ml-0.1.8/src/helios_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-03 20:20:58.000000 helios_ml-0.1.8/src/helios_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 20:20:58.000000 helios_ml-0.1.8/src/helios_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.114081 helios_ml-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.114081 helios_ml-0.1.8/test/registry_test/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/foo.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/func_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.114081 helios_ml-0.1.8/test/registry_test/nested/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/nested/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/nested/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/registry_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-05-03 20:20:12.000000 helios_ml-0.1.8/test/test_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:20:58.114081 helios_ml-0.1.8/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-03 20:20:12.000000 helios_ml-0.1.8/tools/generate_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.875946 helios_ml-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.859946 helios_ml-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-07 21:57:03.000000 helios_ml-0.1.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-07 21:57:03.000000 helios_ml-0.1.9/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 21:57:03.000000 helios_ml-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-07 21:57:03.000000 helios_ml-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-07 21:57:03.000000 helios_ml-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-07 21:58:01.875946 helios_ml-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-07 21:57:03.000000 helios_ml-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.859946 helios_ml-0.1.9/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/data/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    20058 2024-05-07 21:57:03.000000 helios_ml-0.1.9/data/logo/logo-background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-07 21:57:03.000000 helios_ml-0.1.9/data/logo/logo-transparent.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.859946 helios_ml-0.1.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/examples/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-05-07 21:57:03.000000 helios_ml-0.1.9/examples/cifar10/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-07 21:57:03.000000 helios_ml-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 21:57:03.000000 helios_ml-0.1.9/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-07 21:57:03.000000 helios_ml-0.1.9/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 21:57:03.000000 helios_ml-0.1.9/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 21:58:01.875946 helios_ml-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.859946 helios_ml-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/src/helios/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/src/helios/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.863946 helios_ml-0.1.9/src/helios/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/data/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/losses/weighted_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/metrics/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13511 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/nn/swa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/optim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.867946 helios_ml-0.1.9/src/helios/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/scheduler/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35899 2024-05-07 21:57:03.000000 helios_ml-0.1.9/src/helios/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.871946 helios_ml-0.1.9/src/helios_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-07 21:58:01.000000 helios_ml-0.1.9/src/helios_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-07 21:58:01.000000 helios_ml-0.1.9/src/helios_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 21:58:01.000000 helios_ml-0.1.9/src/helios_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-07 21:58:01.000000 helios_ml-0.1.9/src/helios_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 21:58:01.000000 helios_ml-0.1.9/src/helios_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.871946 helios_ml-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.871946 helios_ml-0.1.9/test/registry_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/foo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/func_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.871946 helios_ml-0.1.9/test/registry_test/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/nested/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/nested/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/registry_test/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-05-07 21:57:03.000000 helios_ml-0.1.9/test/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:58:01.871946 helios_ml-0.1.9/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-07 21:57:03.000000 helios_ml-0.1.9/tools/generate_requirements.py
```

### Comparing `helios_ml-0.1.8/.github/workflows/publish.yml` & `helios_ml-0.1.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/.github/workflows/tests.yml` & `helios_ml-0.1.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/.pre-commit-config.yaml` & `helios_ml-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/LICENSE` & `helios_ml-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/PKG-INFO` & `helios_ml-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.8
+Version: 0.1.9
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.8/README.rst` & `helios_ml-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/data/logo/logo-background.png` & `helios_ml-0.1.9/data/logo/logo-background.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/data/logo/logo-transparent.png` & `helios_ml-0.1.9/data/logo/logo-transparent.png`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/examples/cifar10/cifar10.py` & `helios_ml-0.1.9/examples/cifar10/cifar10.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/pyproject.toml` & `helios_ml-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/core/__init__.py` & `helios_ml-0.1.9/src/helios/core/__init__.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/core/cuda.py` & `helios_ml-0.1.9/src/helios/core/cuda.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/core/distributed.py` & `helios_ml-0.1.9/src/helios/core/distributed.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/core/logging.py` & `helios_ml-0.1.9/src/helios/core/logging.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/core/rng.py` & `helios_ml-0.1.9/src/helios/core/rng.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/core/utils.py` & `helios_ml-0.1.9/src/helios/core/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/data/__init__.py` & `helios_ml-0.1.9/src/helios/data/__init__.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/data/datamodule.py` & `helios_ml-0.1.9/src/helios/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/data/functional.py` & `helios_ml-0.1.9/src/helios/data/functional.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/data/samplers.py` & `helios_ml-0.1.9/src/helios/data/samplers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/data/transforms.py` & `helios_ml-0.1.9/src/helios/data/transforms.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/losses/utils.py` & `helios_ml-0.1.9/src/helios/losses/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/losses/weighted_loss.py` & `helios_ml-0.1.9/src/helios/losses/weighted_loss.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/metrics/functional.py` & `helios_ml-0.1.9/src/helios/metrics/functional.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/metrics/metrics.py` & `helios_ml-0.1.9/src/helios/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/model/model.py` & `helios_ml-0.1.9/src/helios/model/model.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/model/utils.py` & `helios_ml-0.1.9/src/helios/model/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/nn/swa_utils.py` & `helios_ml-0.1.9/src/helios/nn/swa_utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/nn/utils.py` & `helios_ml-0.1.9/src/helios/nn/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/onnx.py` & `helios_ml-0.1.9/src/helios/onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/optim/utils.py` & `helios_ml-0.1.9/src/helios/optim/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/scheduler/schedulers.py` & `helios_ml-0.1.9/src/helios/scheduler/schedulers.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/scheduler/utils.py` & `helios_ml-0.1.9/src/helios/scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/src/helios/trainer.py` & `helios_ml-0.1.9/src/helios/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,15 @@
         random_seed (int | None): the seed to use for RNGs.
         enable_tensorboard (bool): enable/disable Tensorboard logging.
         enable_file_logging (bool): enable/disable file logging.
         enable_progress_bar (bool): enable/disable the progress bar(s).
         chkpt_root (pathlib.Path): root folder in which checkpoints will be placed.
         log_path (pathlib.Path): root folder in which logs will be saved.
         run_path (pathlib.Path): root folder in which Tensorboard runs will be saved.
+        print_banner (bool): if True, the Helios banner with system info will be printed.
     """
 
     def __init__(
         self,
         run_name: str = "",
         train_unit: TrainingUnit | str = TrainingUnit.EPOCH,
         total_steps: int | float = 0,
@@ -219,14 +220,15 @@
         enable_file_logging: bool = False,
         enable_progress_bar: bool = False,
         chkpt_root: pathlib.Path | None = None,
         log_path: pathlib.Path | None = None,
         run_path: pathlib.Path | None = None,
         src_root: pathlib.Path | None = None,
         import_prefix: str = "",
+        print_banner: bool = True,
     ):
         """Create the trainer."""
         self._model: hlm.Model | None = None
         self._datamodule: data.DataModule | None = None
         self._local_rank: int = 0
         self._rank: int = 0
 
@@ -259,14 +261,15 @@
         self._log_path = log_path
         self._run_path = run_path
 
         self._src_root = src_root
         self._import_prefix = import_prefix
 
         self._run_name = run_name
+        self._print_banner = print_banner
 
         self._validate_flags()
         self._setup_device_flags(use_cpu)
 
     @property
     def model(self) -> hlm.Model:
         """Return the model."""
@@ -541,15 +544,16 @@
 
     def _print_header(
         self, chkpt_path: pathlib.Path | None, for_training: bool = True
     ) -> None:
         """Print the Helios header with system info to the logs."""
         root_logger = logging.get_root_logger()
 
-        dist.global_print(core.get_env_info_str())
+        if self._print_banner:
+            dist.global_print(core.get_env_info_str())
 
         if for_training:
             if chkpt_path is not None:
                 msg = f"Resuming training from checkpoint {str(chkpt_path)}"
                 root_logger.info(msg)
                 dist.global_print(f"{msg}\n")
             else:
```

### Comparing `helios_ml-0.1.8/src/helios_ml.egg-info/PKG-INFO` & `helios_ml-0.1.9/src/helios_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-ml
-Version: 0.1.8
+Version: 0.1.9
 Summary: A light-weight system for training AI networks using PyTorch
 Author-email: "Mauricio A. Rovira Galvez" <maroviragalvez@outlook.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/marovira/helios-ml
 Project-URL: source, https://github.com/marovira/helios-ml
 Project-URL: issues, https://github.com/marovira/helios-ml/issues
 Project-URL: release notes, https://github.com/marovira/helios-ml/releases
```

### Comparing `helios_ml-0.1.8/src/helios_ml.egg-info/SOURCES.txt` & `helios_ml-0.1.9/src/helios_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/test/conftest.py` & `helios_ml-0.1.9/test/conftest.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/test/test_core.py` & `helios_ml-0.1.9/test/test_core.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/test/test_data.py` & `helios_ml-0.1.9/test/test_data.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/test/test_losses.py` & `helios_ml-0.1.9/test/test_losses.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/test/test_metrics.py` & `helios_ml-0.1.9/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/test/test_model.py` & `helios_ml-0.1.9/test/test_model.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/test/test_nn.py` & `helios_ml-0.1.9/test/test_nn.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/test/test_onnx.py` & `helios_ml-0.1.9/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/test/test_trainer.py` & `helios_ml-0.1.9/test/test_trainer.py`

 * *Files identical despite different names*

### Comparing `helios_ml-0.1.8/tools/generate_requirements.py` & `helios_ml-0.1.9/tools/generate_requirements.py`

 * *Files identical despite different names*

