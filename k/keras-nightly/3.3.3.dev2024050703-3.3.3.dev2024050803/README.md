# Comparing `tmp/keras_nightly-3.3.3.dev2024050703.tar.gz` & `tmp/keras_nightly-3.3.3.dev2024050803.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.3.3.dev2024050703.tar", last modified: Tue May  7 03:21:51 2024, max compression
+gzip compressed data, was "keras_nightly-3.3.3.dev2024050803.tar", last modified: Wed May  8 03:23:28 2024, max compression
```

## Comparing `keras_nightly-3.3.3.dev2024050703.tar` & `keras_nightly-3.3.3.dev2024050803.tar`

### file list

```diff
@@ -1,698 +1,698 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.479807 keras_nightly-3.3.3.dev2024050703/
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-07 03:21:51.479807 keras_nightly-3.3.3.dev2024050703/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.411807 keras_nightly-3.3.3.dev2024050703/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.411807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.415807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.415807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    28948 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    30999 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.419807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    28249 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.423807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    28490 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    78825 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.423807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    48116 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.427807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.427807 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.427807 keras_nightly-3.3.3.dev2024050703/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.431807 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.431807 keras_nightly-3.3.3.dev2024050703/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.431807 keras_nightly-3.3.3.dev2024050703/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.431807 keras_nightly-3.3.3.dev2024050703/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33588 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.431807 keras_nightly-3.3.3.dev2024050703/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.435807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.435807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.435807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.439807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.439807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25225 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    42009 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    17438 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    64128 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.443807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.443807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.443807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.451807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.451807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.451807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.455807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    28138 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.455807 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.455807 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.459807 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.459807 keras_nightly-3.3.3.dev2024050703/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    69039 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.459807 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.463807 keras_nightly-3.3.3.dev2024050703/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    30043 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22763 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.463807 keras_nightly-3.3.3.dev2024050703/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    37275 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    67512 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   196510 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.467807 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.467807 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.467807 keras_nightly-3.3.3.dev2024050703/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.467807 keras_nightly-3.3.3.dev2024050703/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.467807 keras_nightly-3.3.3.dev2024050703/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.471807 keras_nightly-3.3.3.dev2024050703/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/keras_saveable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.471807 keras_nightly-3.3.3.dev2024050703/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.471807 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25904 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.471807 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.475807 keras_nightly-3.3.3.dev2024050703/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/tree/tree_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.479807 keras_nightly-3.3.3.dev2024050703/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16629 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 03:21:49.000000 keras_nightly-3.3.3.dev2024050703/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.479807 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-07 03:21:51.000000 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-05-07 03:21:51.000000 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:21:51.000000 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 03:21:51.000000 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 03:21:51.000000 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:21:51.479807 keras_nightly-3.3.3.dev2024050703/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-07 03:21:49.000000 keras_nightly-3.3.3.dev2024050703/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.572954 keras_nightly-3.3.3.dev2024050803/
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-08 03:23:28.572954 keras_nightly-3.3.3.dev2024050803/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.472955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.476955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-08 03:23:22.000000 keras_nightly-3.3.3.dev2024050803/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.480955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.484955 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.488955 keras_nightly-3.3.3.dev2024050803/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.492955 keras_nightly-3.3.3.dev2024050803/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.496955 keras_nightly-3.3.3.dev2024050803/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.496955 keras_nightly-3.3.3.dev2024050803/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.500954 keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.500954 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31232 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.504954 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28249 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.504954 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28490 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78825 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.508954 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48117 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.512954 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.512954 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.512954 keras_nightly-3.3.3.dev2024050803/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.516954 keras_nightly-3.3.3.dev2024050803/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.516954 keras_nightly-3.3.3.dev2024050803/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.516954 keras_nightly-3.3.3.dev2024050803/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.516954 keras_nightly-3.3.3.dev2024050803/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33588 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.516954 keras_nightly-3.3.3.dev2024050803/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.520954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.520954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.520954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.524954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.524954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42225 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17438 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64221 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.528954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.528954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.532954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.536954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.536954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.540954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.544954 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28138 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.544954 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.544954 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.548954 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.548954 keras_nightly-3.3.3.dev2024050803/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69039 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.548954 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.552954 keras_nightly-3.3.3.dev2024050803/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30043 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22763 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.552954 keras_nightly-3.3.3.dev2024050803/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37642 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67512 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196510 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.556954 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.556954 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.556954 keras_nightly-3.3.3.dev2024050803/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.560954 keras_nightly-3.3.3.dev2024050803/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.560954 keras_nightly-3.3.3.dev2024050803/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.560954 keras_nightly-3.3.3.dev2024050803/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/saving/keras_saveable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.560954 keras_nightly-3.3.3.dev2024050803/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.560954 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25904 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.564954 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.564954 keras_nightly-3.3.3.dev2024050803/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/tree/tree_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.568954 keras_nightly-3.3.3.dev2024050803/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16629 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-08 03:21:42.000000 keras_nightly-3.3.3.dev2024050803/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-08 03:23:26.000000 keras_nightly-3.3.3.dev2024050803/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:23:28.572954 keras_nightly-3.3.3.dev2024050803/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-08 03:23:28.000000 keras_nightly-3.3.3.dev2024050803/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-05-08 03:23:28.000000 keras_nightly-3.3.3.dev2024050803/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 03:23:28.000000 keras_nightly-3.3.3.dev2024050803/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 03:23:28.000000 keras_nightly-3.3.3.dev2024050803/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 03:23:28.000000 keras_nightly-3.3.3.dev2024050803/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 03:23:28.572954 keras_nightly-3.3.3.dev2024050803/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-08 03:23:26.000000 keras_nightly-3.3.3.dev2024050803/setup.py
```

### Comparing `keras_nightly-3.3.3.dev2024050703/PKG-INFO` & `keras_nightly-3.3.3.dev2024050803/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.3.dev2024050703
+Version: 3.3.3.dev2024050803
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.3.dev2024050703/README.md` & `keras_nightly-3.3.3.dev2024050803/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/activations/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/applications/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/backend/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/config/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/layers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/losses/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/ops/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/random/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/saving/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/tree/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/api/utils/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/activations/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/activations/activations.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/api_export.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/convnext.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/densenet.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/efficientnet.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/inception_v3.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/nasnet.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/resnet.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/resnet_v2.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/vgg16.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/vgg19.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/applications/xception.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/dtypes.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/global_state.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/name_scope.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/variables.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/config.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/exports.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/core.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/image.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/linalg.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/math.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/nn.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,17 +269,19 @@
     if channels % kernel_in_channels > 0:
         raise ValueError(
             "The number of input channels must be evenly divisible by "
             f"kernel's in_channels. Received input channels {channels} and "
             f"kernel in_channels {kernel_in_channels}. "
         )
     feature_group_count = channels // kernel_in_channels
+    kernel = convert_to_tensor(kernel)
+    inputs = convert_to_tensor(inputs, dtype=kernel.dtype)
     return jax.lax.conv_general_dilated(
-        convert_to_tensor(inputs),
-        convert_to_tensor(kernel),
+        inputs,
+        kernel,
         strides,
         padding,
         rhs_dilation=dilation_rate,
         dimension_numbers=dimension_numbers,
         feature_group_count=feature_group_count,
     )
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/numpy.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -989,15 +989,19 @@
 def tile(x, repeats):
     return jnp.tile(x, repeats)
 
 
 def trace(x, offset=0, axis1=0, axis2=1):
     x = convert_to_tensor(x)
     dtype = None
-    if standardize_dtype(x.dtype) == "bool":
+    # TODO: Remove the condition of uint8 and uint16 once we have jax>=0.4.27
+    # for both CPU & GPU environments.
+    # uint8 and uint16 will be casted to uint32 when jax>=0.4.27 but to int32
+    # otherwise.
+    if standardize_dtype(x.dtype) in ("bool", "uint8", "uint16"):
         dtype = "int32"
     return jnp.trace(x, offset=offset, axis1=axis1, axis2=axis2, dtype=dtype)
 
 
 def tri(N, M=None, k=0, dtype=None):
     dtype = dtype or config.floatx()
     return jnp.tri(N, M=M, k=k, dtype=dtype)
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/random.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/rnn.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/sparse.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/trainer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/core.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/image.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/math.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/nn.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/random.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/core.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/image.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/layer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/linalg.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/math.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/nn.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/numpy.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1247,16 +1247,16 @@
         chunk_sizes = dim // indices_or_sections
     out = torch.split(
         tensor=x,
         split_size_or_sections=chunk_sizes,
         dim=axis,
     )
     if dim == 0 and isinstance(indices_or_sections, int):
-        out = tuple(out[0].clone() for _ in range(indices_or_sections))
-    return out
+        out = [out[0].clone() for _ in range(indices_or_sections)]
+    return list(out)
 
 
 def stack(x, axis=0):
     x = [convert_to_tensor(elem) for elem in x]
     return torch.stack(x, dim=axis)
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/random.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/rnn.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/trainer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/callback.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/callback_list.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/history.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/constraints/constraints.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/boston_housing.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/california_housing.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar10.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar100.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/imdb.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/mnist.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/reuters.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/export/export_lib.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/initializers/initializer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/initializers/random_initializers.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/activation.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/elu.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/prelu.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/relu.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/softmax.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/attention.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,20 +59,22 @@
             function must take as input the unprojected variable and must return
             the projected variable (which must have the same shape). Constraints
             are not safe to use when doing asynchronous distributed training.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         A 3D tensor with shape: `(batch_shape, steps, channels)`
     - If `data_format="channels_first"`:
         A 3D tensor with shape: `(batch_shape, channels, steps)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         A 3D tensor with shape: `(batch_shape, new_steps, filters)`
     - If `data_format="channels_first"`:
         A 3D tensor with shape: `(batch_shape, filters, new_steps)`
 
     Returns:
         A 3D tensor representing `activation(conv1d(inputs, kernel) + bias)`.
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,20 +53,22 @@
             function must take as input the unprojected variable and must return
             the projected variable (which must have the same shape). Constraints
             are not safe to use when doing asynchronous distributed training.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         A 3D tensor with shape: `(batch_shape, steps, channels)`
     - If `data_format="channels_first"`:
         A 3D tensor with shape: `(batch_shape, channels, steps)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         A 3D tensor with shape: `(batch_shape, new_steps, filters)`
     - If `data_format="channels_first"`:
         A 3D tensor with shape: `(batch_shape, filters, new_steps)`
 
     Returns:
         A 3D tensor representing
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,20 +55,22 @@
             function must take as input the unprojected variable and must return
             the projected variable (which must have the same shape). Constraints
             are not safe to use when doing asynchronous distributed training.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         A 4D tensor with shape: `(batch_size, height, width, channels)`
     - If `data_format="channels_first"`:
         A 4D tensor with shape: `(batch_size, channels, height, width)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         A 4D tensor with shape: `(batch_size, new_height, new_width, filters)`
     - If `data_format="channels_first"`:
         A 4D tensor with shape: `(batch_size, filters, new_height, new_width)`
 
     Returns:
         A 4D tensor representing `activation(conv2d(inputs, kernel) + bias)`.
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,20 +55,22 @@
             function must take as input the unprojected variable and must return
             the projected variable (which must have the same shape). Constraints
             are not safe to use when doing asynchronous distributed training.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         A 4D tensor with shape: `(batch_size, height, width, channels)`
     - If `data_format="channels_first"`:
         A 4D tensor with shape: `(batch_size, channels, height, width)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         A 4D tensor with shape: `(batch_size, new_height, new_width, filters)`
     - If `data_format="channels_first"`:
         A 4D tensor with shape: `(batch_size, filters, new_height, new_width)`
 
     Returns:
         A 4D tensor representing
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,22 +55,24 @@
             function must take as input the unprojected variable and must return
             the projected variable (which must have the same shape). Constraints
             are not safe to use when doing asynchronous distributed training.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         5D tensor with shape:
         `(batch_size, spatial_dim1, spatial_dim2, spatial_dim3, channels)`
     - If `data_format="channels_first"`:
         5D tensor with shape:
         `(batch_size, channels, spatial_dim1, spatial_dim2, spatial_dim3)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         5D tensor with shape:
         `(batch_size, new_spatial_dim1, new_spatial_dim2, new_spatial_dim3,
         filters)`
     - If `data_format="channels_first"`:
         5D tensor with shape:
         `(batch_size, filters, new_spatial_dim1, new_spatial_dim2,
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,22 +55,24 @@
             function must take as input the unprojected variable and must return
             the projected variable (which must have the same shape). Constraints
             are not safe to use when doing asynchronous distributed training.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         5D tensor with shape:
         `(batch_size, spatial_dim1, spatial_dim2, spatial_dim3, channels)`
     - If `data_format="channels_first"`:
         5D tensor with shape:
         `(batch_size, channels, spatial_dim1, spatial_dim2, spatial_dim3)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         5D tensor with shape:
         `(batch_size, new_spatial_dim1, new_spatial_dim2, new_spatial_dim3,
         filters)`
     - If `data_format="channels_first"`:
         5D tensor with shape:
         `(batch_size, filters, new_spatial_dim1, new_spatial_dim2,
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,20 +63,22 @@
             function must take as input the unprojected variable and must return
             the projected variable (which must have the same shape). Constraints
             are not safe to use when doing asynchronous distributed training.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         A 3D tensor with shape: `(batch_shape, steps, channels)`
     - If `data_format="channels_first"`:
         A 3D tensor with shape: `(batch_shape, channels, steps)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         A 3D tensor with shape:
         `(batch_shape, new_steps, channels * depth_multiplier)`
     - If `data_format="channels_first"`:
         A 3D tensor with shape:
         `(batch_shape, channels * depth_multiplier, new_steps)`
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,20 +64,22 @@
             function must take as input the unprojected variable and must return
             the projected variable (which must have the same shape). Constraints
             are not safe to use when doing asynchronous distributed training.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         A 4D tensor with shape: `(batch_size, height, width, channels)`
     - If `data_format="channels_first"`:
         A 4D tensor with shape: `(batch_size, channels, height, width)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         A 4D tensor with shape:
         `(batch_size, new_height, new_width, channels * depth_multiplier)`
     - If `data_format="channels_first"`:
         A 4D tensor with shape:
         `(batch_size, channels * depth_multiplier, new_height, new_width)`
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,20 +66,22 @@
             the projected variable (which must have the same shape).
         pointwise_constraint: Optional projection function to be applied to the
             pointwise kernel after being updated by an `Optimizer`.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         A 3D tensor with shape: `(batch_shape, steps, channels)`
     - If `data_format="channels_first"`:
         A 3D tensor with shape: `(batch_shape, channels, steps)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         A 3D tensor with shape: `(batch_shape, new_steps, filters)`
     - If `data_format="channels_first"`:
         A 3D tensor with shape: `(batch_shape, filters, new_steps)`
 
     Returns:
         A 3D tensor representing
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,20 +67,22 @@
             the projected variable (which must have the same shape).
         pointwise_constraint: Optional projection function to be applied to the
             pointwise kernel after being updated by an `Optimizer`.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         A 4D tensor with shape: `(batch_size, height, width, channels)`
     - If `data_format="channels_first"`:
         A 4D tensor with shape: `(batch_size, channels, height, width)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         A 4D tensor with shape: `(batch_size, new_height, new_width, filters)`
     - If `data_format="channels_first"`:
         A 4D tensor with shape: `(batch_size, filters, new_height, new_width)`
 
     Returns:
         A 4D tensor representing
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/dense.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/dense.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             )
         if self.lora_enabled:
             return self._kernel + ops.matmul(
                 self.lora_kernel_a, self.lora_kernel_b
             )
         return self._kernel
 
-    def call(self, inputs):
+    def call(self, inputs, training=None):
         x = ops.matmul(inputs, self.kernel)
         if self.bias is not None:
             x = ops.add(x, self.bias)
         if self.activation is not None:
             x = self.activation(x)
         return x
 
@@ -306,15 +306,15 @@
             raise ValueError(
                 f"Layer '{self.name}' expected {len(all_vars)} variables, "
                 "but received "
                 f"{len(store.keys())} variables during loading. "
                 f"Expected: {[v.name for v in all_vars]}"
             )
 
-    """Quantization-related (int8 and float8) methods"""
+    # Quantization-related (int8 and float8) methods
 
     QUANTIZATION_MODE_ERROR_TEMPLATE = (
         f"Invalid quantization mode. Expected one of "
         f"{dtype_policies.QUANTIZATION_MODES}. "
         "Received: quantization_mode={mode}"
     )
 
@@ -398,19 +398,19 @@
         self.inputs_amax_history.overwrite_with_gradient = True
         self.kernel_scale.overwrite_with_gradient = True
         self.kernel_amax_history.overwrite_with_gradient = True
         self.outputs_grad_scale.overwrite_with_gradient = True
         self.outputs_grad_amax_history.overwrite_with_gradient = True
         self._is_quantized = True
 
-    def quantized_call(self, inputs):
+    def quantized_call(self, inputs, training=None):
         if self.dtype_policy.quantization_mode == "int8":
             return self._int8_call(inputs)
         elif self.dtype_policy.quantization_mode == "float8":
-            return self._float8_call(inputs)
+            return self._float8_call(inputs, training=training)
         else:
             mode = self.dtype_policy.quantization_mode
             raise NotImplementedError(
                 self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
             )
 
     def _int8_call(self, inputs):
@@ -444,35 +444,39 @@
             x = ops.add(x, lora_x)
         if self.bias is not None:
             x = ops.add(x, self.bias)
         if self.activation is not None:
             x = self.activation(x)
         return x
 
-    def _float8_call(self, inputs):
+    def _float8_call(self, inputs, training=None):
         if self.lora_enabled:
             raise NotImplementedError(
                 "Currently, `_float8_call` doesn't support LoRA"
             )
 
         @ops.custom_gradient
         def quantized_dequantize_inputs(inputs, scale, amax_history):
-            new_scale = quantizers.compute_float8_scale(
-                ops.max(amax_history, axis=0),
-                scale,
-                ops.cast(
-                    float(ml_dtypes.finfo("float8_e4m3fn").max), "float32"
-                ),
-            )
+            if training:
+                new_scale = quantizers.compute_float8_scale(
+                    ops.max(amax_history, axis=0),
+                    scale,
+                    ops.cast(
+                        float(ml_dtypes.finfo("float8_e4m3fn").max), "float32"
+                    ),
+                )
+                new_amax_history = quantizers.compute_float8_amax_history(
+                    inputs, amax_history
+                )
+            else:
+                new_scale = None
+                new_amax_history = None
             qdq_inputs = quantizers.quantize_and_dequantize(
                 inputs, scale, "float8_e4m3fn", self.compute_dtype
             )
-            new_amax_history = quantizers.compute_float8_amax_history(
-                inputs, amax_history
-            )
 
             def grad(*args, upstream=None, variables=None):
                 if upstream is None:
                     (upstream,) = args
                 return upstream, new_scale, new_amax_history
 
             return qdq_inputs, grad
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/einsum_dense.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
                 self.lora_kernel_a, self.lora_kernel_b
             )
         return self._kernel
 
     def compute_output_shape(self, _):
         return self.full_output_shape
 
-    def call(self, inputs):
+    def call(self, inputs, training=None):
         x = ops.einsum(self.equation, inputs, self.kernel)
         if self.bias is not None:
             x += self.bias
         if self.activation is not None:
             x = self.activation(x)
         return x
 
@@ -365,15 +365,15 @@
             raise ValueError(
                 f"Layer '{self.name}' expected {len(all_vars)} variables, "
                 "but received "
                 f"{len(store.keys())} variables during loading. "
                 f"Expected: {[v.name for v in all_vars]}"
             )
 
-    """Quantization-related (int8 and float8) methods"""
+    # Quantization-related (int8 and float8) methods
 
     QUANTIZATION_MODE_ERROR_TEMPLATE = (
         f"Invalid quantization mode. Expected one of "
         f"{dtype_policies.QUANTIZATION_MODES}. "
         "Received: quantization_mode={mode}"
     )
 
@@ -484,19 +484,19 @@
         self.inputs_amax_history.overwrite_with_gradient = True
         self.kernel_scale.overwrite_with_gradient = True
         self.kernel_amax_history.overwrite_with_gradient = True
         self.outputs_grad_scale.overwrite_with_gradient = True
         self.outputs_grad_amax_history.overwrite_with_gradient = True
         self._is_quantized = True
 
-    def quantized_call(self, inputs):
+    def quantized_call(self, inputs, training=None):
         if self.dtype_policy.quantization_mode == "int8":
             return self._int8_call(inputs)
         elif self.dtype_policy.quantization_mode == "float8":
-            return self._float8_call(inputs)
+            return self._float8_call(inputs, training=training)
         else:
             mode = self.dtype_policy.quantization_mode
             raise NotImplementedError(
                 self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
             )
 
     def _int8_call(self, inputs):
@@ -558,35 +558,39 @@
             x = ops.add(x, lora_x)
         if self.bias is not None:
             x += self.bias
         if self.activation is not None:
             x = self.activation(x)
         return x
 
-    def _float8_call(self, inputs):
+    def _float8_call(self, inputs, training=None):
         if self.lora_enabled:
             raise NotImplementedError(
                 "Currently, `_float8_call` doesn't support LoRA"
             )
 
         @ops.custom_gradient
         def quantized_dequantize_inputs(inputs, scale, amax_history):
-            new_scale = quantizers.compute_float8_scale(
-                ops.max(amax_history, axis=0),
-                scale,
-                ops.cast(
-                    float(ml_dtypes.finfo("float8_e4m3fn").max), "float32"
-                ),
-            )
+            if training:
+                new_scale = quantizers.compute_float8_scale(
+                    ops.max(amax_history, axis=0),
+                    scale,
+                    ops.cast(
+                        float(ml_dtypes.finfo("float8_e4m3fn").max), "float32"
+                    ),
+                )
+                new_amax_history = quantizers.compute_float8_amax_history(
+                    inputs, amax_history
+                )
+            else:
+                new_scale = None
+                new_amax_history = None
             qdq_inputs = quantizers.quantize_and_dequantize(
                 inputs, scale, "float8_e4m3fn", self.compute_dtype
             )
-            new_amax_history = quantizers.compute_float8_amax_history(
-                inputs, amax_history
-            )
 
             def grad(*args, upstream=None, variables=None):
                 if upstream is None:
                     (upstream,) = args
                 return upstream, new_scale, new_amax_history
 
             return qdq_inputs, grad
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/embedding.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/identity.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/input_layer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/masking.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/wrapper.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/input_spec.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/layer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -866,20 +866,22 @@
                     for output in tree.flatten(outputs):
                         if backend.is_tensor(output):
                             self.add_loss(self.activity_regularizer(output))
 
             # Set masks on outputs,
             # provided only the first positional input arg and its mask.
             # TODO: consider extending this to all args and kwargs.
-            previous_mask = getattr(call_spec.first_arg, "_keras_mask", None)
+            previous_mask = tree.map_structure(
+                lambda x: getattr(x, "_keras_mask", None), call_spec.first_arg
+            )
             if self.supports_masking:
                 self._set_mask_metadata(
                     call_spec.first_arg, outputs, previous_mask
                 )
-            elif previous_mask is not None:
+            elif any(m is not None for m in tree.flatten(previous_mask)):
                 warnings.warn(
                     f"Layer '{self.name}' (of type {self.__class__.__name__}) "
                     "was passed an input with a mask attached to it. "
                     "However, this layer does not support masking and will "
                     "therefore destroy the mask information. Downstream "
                     "layers will not see the mask."
                 )
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/add.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/average.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/base_merge.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,51 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.supports_masking = True
 
     def _merge_function(self, inputs):
         raise NotImplementedError
 
+    def _apply_merge_op_and_or_mask(self, op_fn, inputs):
+        """Merge a set of inputs by applying `op_fn` and ORing the masks.
+
+        We use this for `Minimum` and `Maximum` as it handles the fact that
+        there is no identity element. If applicable, the mask obtained by ORing
+        all masks is set on the output.
+
+        Args:
+            op_fn: binary operation to apply to tensor pair.
+            inputs: array of tensors to apply operation on.
+        """
+        output = None
+        output_mask = None
+
+        for x in inputs:
+            mask = getattr(x, "_keras_mask", None)
+            if mask is not None:
+                mask = ops.broadcast_to(ops.expand_dims(mask, -1), ops.shape(x))
+            if output is None:
+                output = x
+                output_mask = mask
+                continue
+            if mask is not None:
+                x = ops.where(mask, x, output)
+            if output_mask is not None:
+                output = ops.where(output_mask, output, x)
+            if mask is not None and output_mask is not None:
+                output_mask = ops.logical_or(output_mask, mask)
+            else:
+                output_mask = None
+            output = op_fn(output, x)
+
+        if output_mask is not None:
+            output_mask = ops.any(output_mask, axis=-1, keepdims=False)
+            output._keras_mask = output_mask
+        return output
+
     def _compute_elemwise_op_output_shape(self, shape1, shape2):
         """Computes the shape of the resultant of an elementwise operation.
 
         Args:
             shape1: Tuple or None. Shape of the first tensor
             shape2: Tuple or None. Shape of the second tensor
 
@@ -227,14 +264,18 @@
             )
         if len(mask) != len(inputs):
             raise ValueError(
                 "The lists `inputs` and `mask` should have the same length. "
                 f"Received: inputs={inputs} of length {len(inputs)}, and "
                 f"mask={mask} of length {len(mask)}"
             )
-        if all(m is None for m in mask):
+        # Default implementation does an OR between the masks, which works
+        # for `Add`, `Subtract`, `Average`, `Maximum`, `Minimum`, `Multiply`.
+        if any(m is None for m in mask):
             return None
-        masks = [ops.expand_dims(m, axis=0) for m in mask if m is not None]
-        return ops.all(ops.concatenate(masks, axis=0), axis=0, keepdims=False)
+        output_mask = mask[0]
+        for m in mask[1:]:
+            output_mask = ops.logical_or(output_mask, m)
+        return output_mask
 
     def get_config(self):
         return super().get_config()
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/concatenate.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,19 +141,23 @@
         masks = []
         for input_i, mask_i in zip(inputs, mask):
             if mask_i is None:
                 # Input is unmasked. Append all 1s to masks,
                 masks.append(ops.ones_like(input_i, dtype="bool"))
             elif mask_i.ndim < input_i.ndim:
                 # Mask is smaller than the input, expand it
-                masks.append(ops.expand_dims(mask_i, axis=-1))
+                masks.append(
+                    ops.broadcast_to(
+                        ops.expand_dims(mask_i, axis=-1), ops.shape(input_i)
+                    )
+                )
             else:
                 masks.append(mask_i)
         concatenated = ops.concatenate(masks, axis=self.axis)
-        return ops.all(concatenated, axis=-1, keepdims=False)
+        return ops.any(concatenated, axis=-1, keepdims=False)
 
     def get_config(self):
         config = {"axis": self.axis}
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/dot.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/maximum.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/maximum.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,18 +27,15 @@
     >>> y = keras.layers.Maximum()([x1, x2])
     >>> out = keras.layers.Dense(4)(y)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
 
     def _merge_function(self, inputs):
-        output = inputs[0]
-        for i in range(1, len(inputs)):
-            output = ops.maximum(output, inputs[i])
-        return output
+        return self._apply_merge_op_and_or_mask(ops.maximum, inputs)
 
 
 @keras_export("keras.layers.maximum")
 def maximum(inputs, **kwargs):
     """Functional interface to the `keras.layers.Maximum` layer.
 
     Args:
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/minimum.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/minimum.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,15 @@
     >>> y = keras.layers.Minimum()([x1, x2])
     >>> out = keras.layers.Dense(4)(y)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
 
     def _merge_function(self, inputs):
-        output = inputs[0]
-        for i in range(1, len(inputs)):
-            output = ops.minimum(output, inputs[i])
-        return output
+        return self._apply_merge_op_and_or_mask(ops.minimum, inputs)
 
 
 @keras_export("keras.layers.minimum")
 def minimum(inputs, **kwargs):
     """Functional interface to the `keras.layers.Minimum` layer.
 
     Args:
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/multiply.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/merging/subtract.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,82 @@
 from keras.src import ops
 from keras.src.api_export import keras_export
 from keras.src.layers.merging.base_merge import Merge
 
 
-@keras_export("keras.layers.Multiply")
-class Multiply(Merge):
-    """Performs elementwise multiplication.
-
-    It takes as input a list of tensors, all of the same shape,
-    and returns a single tensor (also of the same shape).
+@keras_export("keras.layers.Subtract")
+class Subtract(Merge):
+    """Performs elementwise subtraction.
+
+    It takes as input a list of tensors of size 2 both of the
+    same shape, and returns a single tensor (inputs[0] - inputs[1])
+    of same shape.
 
     Examples:
 
     >>> input_shape = (2, 3, 4)
     >>> x1 = np.random.rand(*input_shape)
     >>> x2 = np.random.rand(*input_shape)
-    >>> y = keras.layers.Multiply()([x1, x2])
+    >>> y = keras.layers.Subtract()([x1, x2])
 
     Usage in a Keras model:
 
     >>> input1 = keras.layers.Input(shape=(16,))
     >>> x1 = keras.layers.Dense(8, activation='relu')(input1)
     >>> input2 = keras.layers.Input(shape=(32,))
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
-    >>> # equivalent to `y = keras.layers.multiply([x1, x2])`
-    >>> y = keras.layers.Multiply()([x1, x2])
-    >>> out = keras.layers.Dense(4)(y)
+    >>> # equivalent to `subtracted = keras.layers.subtract([x1, x2])`
+    >>> subtracted = keras.layers.Subtract()([x1, x2])
+    >>> out = keras.layers.Dense(4)(subtracted)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
 
+    def build(self, input_shape):
+        super().build(input_shape)
+        if len(input_shape) != 2:
+            raise ValueError(
+                "A `Subtract` layer should be called on exactly 2 inputs. "
+                f"Received: input_shape={input_shape}"
+            )
+
     def _merge_function(self, inputs):
-        output = inputs[0]
-        for i in range(1, len(inputs)):
-            output = ops.multiply(output, inputs[i])
-        return output
+        if len(inputs) != 2:
+            raise ValueError(
+                "A `Subtract` layer should be called on exactly 2 inputs. "
+                f"Received: inputs={inputs}"
+            )
+        return ops.subtract(inputs[0], inputs[1])
 
 
-@keras_export("keras.layers.multiply")
-def multiply(inputs, **kwargs):
-    """Functional interface to the `keras.layers.Multiply` layer.
+@keras_export("keras.layers.subtract")
+def subtract(inputs, **kwargs):
+    """Functional interface to the `keras.layers.Subtract` layer.
 
     Args:
-        inputs: A list of input tensors , all of the same shape.
+        inputs: A list of input tensors of size 2, each tensor of
+            the same shape.
         **kwargs: Standard layer keyword arguments.
 
     Returns:
-        A tensor as the elementwise product of the inputs with the same
-        shape as the inputs.
+        A tensor as the difference of the inputs. It has the same shape
+        as the inputs.
 
     Examples:
 
     >>> input_shape = (2, 3, 4)
     >>> x1 = np.random.rand(*input_shape)
     >>> x2 = np.random.rand(*input_shape)
-    >>> y = keras.layers.multiply([x1, x2])
+    >>> y = keras.layers.subtract([x1, x2])
 
     Usage in a Keras model:
 
     >>> input1 = keras.layers.Input(shape=(16,))
     >>> x1 = keras.layers.Dense(8, activation='relu')(input1)
     >>> input2 = keras.layers.Input(shape=(32,))
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
-    >>> y = keras.layers.multiply([x1, x2])
-    >>> out = keras.layers.Dense(4)(y)
+    >>> subtracted = keras.layers.subtract([x1, x2])
+    >>> out = keras.layers.Dense(4)(subtracted)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
-    return Multiply(**kwargs)(inputs)
+    return Subtract(**kwargs)(inputs)
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/average_pooling1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,20 +27,22 @@
             corresponds to inputs with shape `(batch, steps, features)`
             while `"channels_first"` corresponds to inputs with shape
             `(batch, features, steps)`. It defaults to the `image_data_format`
             value found in your Keras config file at `~/.keras/keras.json`.
             If you never set it, then it will be `"channels_last"`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         3D tensor with shape `(batch_size, steps, features)`.
     - If `data_format="channels_first"`:
         3D tensor with shape `(batch_size, features, steps)`.
 
     Output shape:
+
     - If `data_format="channels_last"`:
         3D tensor with shape `(batch_size, downsampled_steps, features)`.
     - If `data_format="channels_first"`:
         3D tensor with shape `(batch_size, features, downsampled_steps)`.
 
     Examples:
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/average_pooling2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,20 +36,22 @@
             while `"channels_first"` corresponds to inputs with shape
             `(batch, channels, height, width)`. It defaults to the
             `image_data_format` value found in your Keras config file at
             `~/.keras/keras.json`. If you never set it, then it will be
             `"channels_last"`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         4D tensor with shape `(batch_size, height, width, channels)`.
     - If `data_format="channels_first"`:
         4D tensor with shape `(batch_size, channels, height, width)`.
 
     Output shape:
+
     - If `data_format="channels_last"`:
         4D tensor with shape
         `(batch_size, pooled_height, pooled_width, channels)`.
     - If `data_format="channels_first"`:
         4D tensor with shape
         `(batch_size, channels, pooled_height, pooled_width)`.
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/average_pooling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,22 +29,24 @@
             `"channels_first"` corresponds to inputs with shape
             `(batch, channels, spatial_dim1, spatial_dim2, spatial_dim3)`.
             It defaults to the `image_data_format` value found in your Keras
             config file at `~/.keras/keras.json`. If you never set it, then it
             will be `"channels_last"`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         5D tensor with shape:
         `(batch_size, spatial_dim1, spatial_dim2, spatial_dim3, channels)`
     - If `data_format="channels_first"`:
         5D tensor with shape:
         `(batch_size, channels, spatial_dim1, spatial_dim2, spatial_dim3)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         5D tensor with shape:
         `(batch_size, pooled_dim1, pooled_dim2, pooled_dim3, channels)`
     - If `data_format="channels_first"`:
         5D tensor with shape:
         `(batch_size, channels, pooled_dim1, pooled_dim2, pooled_dim3)`
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/max_pooling1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,22 @@
             corresponds to inputs with shape `(batch, steps, features)`
             while `"channels_first"` corresponds to inputs with shape
             `(batch, features, steps)`. It defaults to the `image_data_format`
             value found in your Keras config file at `~/.keras/keras.json`.
             If you never set it, then it will be `"channels_last"`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         3D tensor with shape `(batch_size, steps, features)`.
     - If `data_format="channels_first"`:
         3D tensor with shape `(batch_size, features, steps)`.
 
     Output shape:
+
     - If `data_format="channels_last"`:
         3D tensor with shape `(batch_size, downsampled_steps, features)`.
     - If `data_format="channels_first"`:
         3D tensor with shape `(batch_size, features, downsampled_steps)`.
 
     Examples:
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/max_pooling2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,22 @@
             while `"channels_first"` corresponds to inputs with shape
             `(batch, channels, height, width)`. It defaults to the
             `image_data_format` value found in your Keras config file at
             `~/.keras/keras.json`. If you never set it, then it will be
             `"channels_last"`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         4D tensor with shape `(batch_size, height, width, channels)`.
     - If `data_format="channels_first"`:
         4D tensor with shape `(batch_size, channels, height, width)`.
 
     Output shape:
+
     - If `data_format="channels_last"`:
         4D tensor with shape
         `(batch_size, pooled_height, pooled_width, channels)`.
     - If `data_format="channels_first"`:
         4D tensor with shape
         `(batch_size, channels, pooled_height, pooled_width)`.
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/pooling/max_pooling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,22 +29,24 @@
             `"channels_first"` corresponds to inputs with shape
             `(batch, channels, spatial_dim1, spatial_dim2, spatial_dim3)`.
             It defaults to the `image_data_format` value found in your Keras
             config file at `~/.keras/keras.json`. If you never set it, then it
             will be `"channels_last"`.
 
     Input shape:
+
     - If `data_format="channels_last"`:
         5D tensor with shape:
         `(batch_size, spatial_dim1, spatial_dim2, spatial_dim3, channels)`
     - If `data_format="channels_first"`:
         5D tensor with shape:
         `(batch_size, channels, spatial_dim1, spatial_dim2, spatial_dim3)`
 
     Output shape:
+
     - If `data_format="channels_last"`:
         5D tensor with shape:
         `(batch_size, pooled_dim1, pooled_dim2, pooled_dim3, channels)`
     - If `data_format="channels_first"`:
         5D tensor with shape:
         `(batch_size, channels, pooled_dim1, pooled_dim2, pooled_dim3)`
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/gru.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/backend.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/layers.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/losses.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/losses/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/losses/loss.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/losses/losses.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/metric.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/models/cloning.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/models/functional.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/models/model.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/models/sequential.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/models/variable_mapping.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/core.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/function.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/image.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1072,19 +1072,30 @@
         )
     if target_width < 0:
         raise ValueError(
             "target_width must be >= 0. "
             f"Received: target_width={target_width}"
         )
 
+    if isinstance(top_cropping, int) and isinstance(left_cropping, int):
+        start_indices = [0, top_cropping, left_cropping, 0]
+    else:
+        start_indices = backend.numpy.stack([0, top_cropping, left_cropping, 0])
+    if (
+        isinstance(batch, int)
+        and isinstance(target_height, int)
+        and isinstance(target_width, int)
+        and isinstance(depth, int)
+    ):
+        shape = [batch, target_height, target_width, depth]
+    else:
+        shape = backend.numpy.stack([batch, target_height, target_width, depth])
     cropped = ops.slice(
         images,
-        backend.numpy.stack([0, top_cropping, left_cropping, 0]),
-        backend.numpy.stack([batch, target_height, target_width, depth]),
+        start_indices,
+        shape,
     )
 
-    cropped_shape = [batch, target_height, target_width, depth]
-    cropped = backend.numpy.reshape(cropped, cropped_shape)
-
+    cropped = backend.numpy.reshape(cropped, shape)
     if not is_batch:
         cropped = backend.numpy.squeeze(cropped, axis=[0])
     return cropped
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/linalg.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/math.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/nn.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/node.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/numpy.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/operation.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/operation_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adadelta.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adafactor.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adagrad.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adam.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adamax.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adamw.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/ftrl.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/lion.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/nadam.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/optimizer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/sgd.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/quantizers/quantizers.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/random/random.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/random/seed_generator.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/regularizers/regularizers.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/saving/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/saving/keras_saveable.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/saving/keras_saveable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/saving/object_registration.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/saving/saving_api.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/saving/saving_lib.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/saving/serialization_lib.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/testing/test_case.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/testing/test_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/compile_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/trainer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/tree/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/tree/optree_impl.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/tree/tree_api.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/__init__.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/argument_validation.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/backend_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/code_stats.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/dataset_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/dtype_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/file_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/image_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/io_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/jax_layer.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/model_visualization.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/module_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/naming.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/numerical_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/progbar.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/python_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/rng_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/sequence_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/summary_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/tf_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/torch_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/traceback_utils.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras/src/utils/tracking.py` & `keras_nightly-3.3.3.dev2024050803/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.3.3.dev2024050803/keras_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.3.dev2024050703
+Version: 3.3.3.dev2024050803
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.3.3.dev2024050803/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050703/setup.py` & `keras_nightly-3.3.3.dev2024050803/setup.py`

 * *Files identical despite different names*

