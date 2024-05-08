# Comparing `tmp/keras_nightly-3.3.3.dev2024050603.tar.gz` & `tmp/keras_nightly-3.3.3.dev2024050703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.3.3.dev2024050603.tar", last modified: Mon May  6 03:21:09 2024, max compression
+gzip compressed data, was "keras_nightly-3.3.3.dev2024050703.tar", last modified: Tue May  7 03:21:51 2024, max compression
```

## Comparing `keras_nightly-3.3.3.dev2024050603.tar` & `keras_nightly-3.3.3.dev2024050703.tar`

### file list

```diff
@@ -1,698 +1,698 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.964171 keras_nightly-3.3.3.dev2024050603/
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-06 03:21:09.964171 keras_nightly-3.3.3.dev2024050603/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.864170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.868170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.872170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-06 03:21:04.000000 keras_nightly-3.3.3.dev2024050603/keras/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.876170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.880170 keras_nightly-3.3.3.dev2024050603/keras/api/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.884170 keras_nightly-3.3.3.dev2024050603/keras/api/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.888170 keras_nightly-3.3.3.dev2024050603/keras/api/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.888170 keras_nightly-3.3.3.dev2024050603/keras/api/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.888170 keras_nightly-3.3.3.dev2024050603/keras/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.888170 keras_nightly-3.3.3.dev2024050603/keras/api/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.888170 keras_nightly-3.3.3.dev2024050603/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.888170 keras_nightly-3.3.3.dev2024050603/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.892170 keras_nightly-3.3.3.dev2024050603/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.892170 keras_nightly-3.3.3.dev2024050603/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.892170 keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.896170 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    28948 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    30999 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.900170 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    28249 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.904170 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    28490 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    78825 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.904170 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    48116 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.908170 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.908170 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.912170 keras_nightly-3.3.3.dev2024050603/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.912170 keras_nightly-3.3.3.dev2024050603/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.912170 keras_nightly-3.3.3.dev2024050603/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.912170 keras_nightly-3.3.3.dev2024050603/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.912170 keras_nightly-3.3.3.dev2024050603/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33588 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.916170 keras_nightly-3.3.3.dev2024050603/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.916170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.916170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.916170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.920170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.924170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25225 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    42009 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    17438 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    63920 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.924170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.924170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.928170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.932170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.936170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.936170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.940170 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    28138 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.940170 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.940170 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.944170 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.944170 keras_nightly-3.3.3.dev2024050603/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    69039 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.944170 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.948171 keras_nightly-3.3.3.dev2024050603/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    32507 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22763 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.948171 keras_nightly-3.3.3.dev2024050603/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15497 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    37275 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    67512 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   196510 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.952170 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.952170 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.952170 keras_nightly-3.3.3.dev2024050603/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.952170 keras_nightly-3.3.3.dev2024050603/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.952170 keras_nightly-3.3.3.dev2024050603/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.952170 keras_nightly-3.3.3.dev2024050603/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/saving/keras_saveable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.956171 keras_nightly-3.3.3.dev2024050603/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.956171 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25904 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.956171 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.956171 keras_nightly-3.3.3.dev2024050603/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/tree/tree_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.960171 keras_nightly-3.3.3.dev2024050603/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16629 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-06 03:19:50.000000 keras_nightly-3.3.3.dev2024050603/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-06 03:21:07.000000 keras_nightly-3.3.3.dev2024050603/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 03:21:09.964171 keras_nightly-3.3.3.dev2024050603/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-06 03:21:09.000000 keras_nightly-3.3.3.dev2024050603/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-05-06 03:21:09.000000 keras_nightly-3.3.3.dev2024050603/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 03:21:09.000000 keras_nightly-3.3.3.dev2024050603/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-06 03:21:09.000000 keras_nightly-3.3.3.dev2024050603/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 03:21:09.000000 keras_nightly-3.3.3.dev2024050603/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 03:21:09.964171 keras_nightly-3.3.3.dev2024050603/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-06 03:21:07.000000 keras_nightly-3.3.3.dev2024050603/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.479807 keras_nightly-3.3.3.dev2024050703/
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-07 03:21:51.479807 keras_nightly-3.3.3.dev2024050703/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.387807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.391807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.395807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-07 03:21:46.000000 keras_nightly-3.3.3.dev2024050703/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.399807 keras_nightly-3.3.3.dev2024050703/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.403807 keras_nightly-3.3.3.dev2024050703/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.407807 keras_nightly-3.3.3.dev2024050703/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.411807 keras_nightly-3.3.3.dev2024050703/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.411807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.415807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.415807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11661 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28948 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30999 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.419807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28249 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.423807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28490 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78825 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.423807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48116 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.427807 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.427807 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.427807 keras_nightly-3.3.3.dev2024050703/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.431807 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.431807 keras_nightly-3.3.3.dev2024050703/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.431807 keras_nightly-3.3.3.dev2024050703/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.431807 keras_nightly-3.3.3.dev2024050703/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33588 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.431807 keras_nightly-3.3.3.dev2024050703/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.435807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.435807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.435807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.439807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.439807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25225 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42009 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17438 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64128 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.443807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.443807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.443807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.451807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.451807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.451807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.455807 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28138 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.455807 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.455807 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.459807 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.459807 keras_nightly-3.3.3.dev2024050703/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69039 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.459807 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.463807 keras_nightly-3.3.3.dev2024050703/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30043 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22763 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.463807 keras_nightly-3.3.3.dev2024050703/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37275 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67512 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196510 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.467807 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.467807 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.467807 keras_nightly-3.3.3.dev2024050703/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.467807 keras_nightly-3.3.3.dev2024050703/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.467807 keras_nightly-3.3.3.dev2024050703/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.471807 keras_nightly-3.3.3.dev2024050703/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/keras_saveable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.471807 keras_nightly-3.3.3.dev2024050703/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.471807 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25904 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.471807 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.475807 keras_nightly-3.3.3.dev2024050703/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/tree/tree_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.479807 keras_nightly-3.3.3.dev2024050703/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16629 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-07 03:20:19.000000 keras_nightly-3.3.3.dev2024050703/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-07 03:21:49.000000 keras_nightly-3.3.3.dev2024050703/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:21:51.479807 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-07 03:21:51.000000 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-05-07 03:21:51.000000 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:21:51.000000 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 03:21:51.000000 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 03:21:51.000000 keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:21:51.479807 keras_nightly-3.3.3.dev2024050703/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-07 03:21:49.000000 keras_nightly-3.3.3.dev2024050703/setup.py
```

### Comparing `keras_nightly-3.3.3.dev2024050603/PKG-INFO` & `keras_nightly-3.3.3.dev2024050703/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.3.dev2024050603
+Version: 3.3.3.dev2024050703
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.3.dev2024050603/README.md` & `keras_nightly-3.3.3.dev2024050703/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/activations/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/applications/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/backend/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/config/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/layers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/losses/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/ops/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/random/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/saving/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/tree/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/api/utils/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/activations/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/activations/activations.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/api_export.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/convnext.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/densenet.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/efficientnet.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/inception_v3.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/mobilenet.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/nasnet.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/resnet.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/resnet_v2.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/vgg16.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/vgg19.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/applications/xception.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/dtypes.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/global_state.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/name_scope.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/common/variables.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/config.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/exports.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/core.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,97 +179,74 @@
                     rec_args.append(args[idx_sym])
                     idx_sym += 1
 
                 i += 1
             with StatelessScope():
                 return fn(*rec_args, **kwargs, **static_kwargs)
 
-        output_spec = None
         if has_none:
-            try:
-                ms_args_1, ms_kwargs_1 = tree.map_structure(
-                    lambda x: convert_keras_tensor_to_jax(x, fill_value=83),
-                    (maybe_symbolic_args, maybe_symbolic_kwargs),
-                )
-                _, jax_out_1 = jax.make_jaxpr(wrapped_fn, return_shape=True)(
-                    *ms_args_1, **ms_kwargs_1
-                )
-
-                ms_args_2, ms_kwargs_2 = tree.map_structure(
-                    lambda x: convert_keras_tensor_to_jax(x, fill_value=89),
-                    (maybe_symbolic_args, maybe_symbolic_kwargs),
-                )
-                _, jax_out_2 = jax.make_jaxpr(wrapped_fn, return_shape=True)(
-                    *ms_args_2, **ms_kwargs_2
-                )
-
-                def merge_shapes(shape1, shape2):
-                    return tuple(
-                        [
-                            d1 if d1 == d2 else None
-                            for d1, d2 in zip(shape1, shape2)
-                        ]
-                    )
-
-                def convert_jax_specs_to_keras_tensor(x1, x2):
-                    if isinstance(x1, jax.ShapeDtypeStruct):
-                        if not isinstance(x2, jax.ShapeDtypeStruct):
-                            raise ValueError("Indeterministic output ordering.")
-                        return KerasTensor(
-                            merge_shapes(x1.shape, x2.shape), dtype=x1.dtype
-                        )
-                    elif isinstance(x1, jax_sparse.BCOO):
-                        if not isinstance(x2, jax_sparse.BCOO):
-                            raise ValueError("Indeterministic output ordering.")
-                        return KerasTensor(
-                            merge_shapes(x1.shape, x2.shape),
-                            dtype=x1.dtype,
-                            sparse=True,
-                        )
-                    else:
-                        return x1
+            ms_args_1, ms_kwargs_1 = tree.map_structure(
+                lambda x: convert_keras_tensor_to_jax(x, fill_value=83),
+                (maybe_symbolic_args, maybe_symbolic_kwargs),
+            )
+            _, jax_out_1 = jax.make_jaxpr(wrapped_fn, return_shape=True)(
+                *ms_args_1, **ms_kwargs_1
+            )
 
-                output_spec = tree.map_structure(
-                    convert_jax_specs_to_keras_tensor, jax_out_1, jax_out_2
-                )
-            except Exception as e:
-                if "[JAX RNG]" in str(e):
-                    raise e
-                # Errors can happen when the filled dimensions
-                # are not compatible with the function
-                # (or when the function contains a bug).
-                # In such cases we don't want to confuse users
-                # with random filled dimensions and the like,
-                # so we rerun a pass on the dynamic shapes,
-                # which will likely error out when JAX tries to
-                # validate shapes as fully static.
-                # The error message will be much easier to understand.
-                pass
-
-        if output_spec is None:
-            maybe_symbolic_args, maybe_symbolic_kwargs = tree.map_structure(
-                convert_keras_tensor_to_jax,
+            ms_args_2, ms_kwargs_2 = tree.map_structure(
+                lambda x: convert_keras_tensor_to_jax(x, fill_value=89),
                 (maybe_symbolic_args, maybe_symbolic_kwargs),
             )
-            _, jax_out = jax.make_jaxpr(wrapped_fn, return_shape=True)(
-                *maybe_symbolic_args, **maybe_symbolic_kwargs
+            _, jax_out_2 = jax.make_jaxpr(wrapped_fn, return_shape=True)(
+                *ms_args_2, **ms_kwargs_2
             )
 
-            def convert_jax_spec_to_keras_tensor(x):
-                if isinstance(x, jax.ShapeDtypeStruct):
-                    return KerasTensor(x.shape, x.dtype)
-                elif isinstance(x, jax_sparse.BCOO):
-                    return KerasTensor(x.shape, x.dtype, sparse=True)
-                return x
+            def merge_shapes(shape1, shape2):
+                return tuple(
+                    [d1 if d1 == d2 else None for d1, d2 in zip(shape1, shape2)]
+                )
+
+            def convert_jax_specs_to_keras_tensor(x1, x2):
+                if isinstance(x1, jax.ShapeDtypeStruct):
+                    if not isinstance(x2, jax.ShapeDtypeStruct):
+                        raise ValueError("Indeterministic output ordering.")
+                    return KerasTensor(
+                        merge_shapes(x1.shape, x2.shape), dtype=x1.dtype
+                    )
+                elif isinstance(x1, jax_sparse.BCOO):
+                    if not isinstance(x2, jax_sparse.BCOO):
+                        raise ValueError("Indeterministic output ordering.")
+                    return KerasTensor(
+                        merge_shapes(x1.shape, x2.shape),
+                        dtype=x1.dtype,
+                        sparse=True,
+                    )
+                else:
+                    return x1
 
-            output_spec = tree.map_structure(
-                convert_jax_spec_to_keras_tensor, jax_out
+            return tree.map_structure(
+                convert_jax_specs_to_keras_tensor, jax_out_1, jax_out_2
             )
 
-    return output_spec
+        maybe_symbolic_args, maybe_symbolic_kwargs = tree.map_structure(
+            convert_keras_tensor_to_jax,
+            (maybe_symbolic_args, maybe_symbolic_kwargs),
+        )
+        _, jax_out = jax.make_jaxpr(wrapped_fn, return_shape=True)(
+            *maybe_symbolic_args, **maybe_symbolic_kwargs
+        )
+
+        def convert_jax_spec_to_keras_tensor(x):
+            if isinstance(x, jax.ShapeDtypeStruct):
+                return KerasTensor(x.shape, x.dtype)
+            elif isinstance(x, jax_sparse.BCOO):
+                return KerasTensor(x.shape, x.dtype, sparse=True)
+            return x
+
+        return tree.map_structure(convert_jax_spec_to_keras_tensor, jax_out)
 
 
 def cond(pred, true_fn, false_fn):
     return jax.lax.cond(pred, true_fun=true_fn, false_fun=false_fn)
 
 
 def vectorized_map(function, elements):
```

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/image.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/linalg.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/math.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/nn.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/numpy.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/random.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/rnn.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/sparse.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/jax/trainer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/core.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/image.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/math.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/nn.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/random.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/core.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/image.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/layer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/linalg.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/math.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/nn.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/numpy.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/random.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/rnn.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/backend/torch/trainer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/callback.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/callback_list.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/history.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/constraints/constraints.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/datasets/boston_housing.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/datasets/california_housing.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/datasets/cifar.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/datasets/cifar10.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/datasets/cifar100.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/datasets/imdb.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/datasets/mnist.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/datasets/reuters.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/export/export_lib.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/initializers/initializer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/initializers/random_initializers.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/activation.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/elu.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/prelu.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/relu.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/activations/softmax.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/attention/attention.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/dense.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/embedding.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/identity.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/input_layer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/input_layer.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         self,
         shape=None,
         batch_size=None,
         dtype=None,
         sparse=None,
         batch_shape=None,
         input_tensor=None,
+        optional=False,
         name=None,
         **kwargs,
     ):
         # TODO: support for ragged.
         super().__init__(name=name)
         if "input_shape" in kwargs:
             warnings.warn(
@@ -65,14 +66,15 @@
         else:
             input_tensor = backend.KerasTensor(
                 shape=batch_shape, dtype=dtype, sparse=sparse, name=name
             )
         self._input_tensor = input_tensor
         Node(operation=self, call_args=(), call_kwargs={}, outputs=input_tensor)
         self.built = True
+        self.optional = optional
 
     def call(self):
         return
 
     @property
     def dtype(self):
         return self._dtype
@@ -91,14 +93,15 @@
     shape=None,
     batch_size=None,
     dtype=None,
     sparse=None,
     batch_shape=None,
     name=None,
     tensor=None,
+    optional=False,
 ):
     """Used to instantiate a Keras tensor.
 
     A Keras tensor is a symbolic tensor-like object, which we augment with
     certain attributes that allow us to build a Keras model just by knowing the
     inputs and outputs of the model.
 
@@ -123,14 +126,16 @@
             backend. Defaults to `False`.
         name: Optional name string for the layer.
             Should be unique in a model (do not reuse the same name twice).
             It will be autogenerated if it isn't provided.
         tensor: Optional existing tensor to wrap into the `Input` layer.
             If set, the layer will use this tensor rather
             than creating a new placeholder tensor.
+        optional: Boolean, whether the input is optional or not.
+            An optional input can accept `None` values.
 
     Returns:
       A Keras tensor.
 
     Example:
 
     ```python
@@ -144,9 +149,10 @@
         shape=shape,
         batch_size=batch_size,
         dtype=dtype,
         sparse=sparse,
         batch_shape=batch_shape,
         name=name,
         input_tensor=tensor,
+        optional=optional,
     )
     return layer.output
```

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/masking.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/core/wrapper.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/input_spec.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/input_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         axes: Dictionary mapping integer axes to
             a specific dimension value.
         allow_last_axis_squeeze: If `True`, allow inputs of rank N+1 as long
             as the last axis of the input is 1, as well as inputs of rank N-1
             as long as the last axis of the spec is 1.
         name: Expected key corresponding to this input when passing data as
             a dictionary.
+        optional: Boolean, whether the input is optional or not.
+            An optional input can accept `None` values.
 
     Example:
 
     ```python
     class MyLayer(Layer):
         def __init__(self):
             super().__init__()
@@ -52,27 +54,29 @@
         shape=None,
         ndim=None,
         max_ndim=None,
         min_ndim=None,
         axes=None,
         allow_last_axis_squeeze=False,
         name=None,
+        optional=False,
     ):
         self.dtype = (
             backend.standardize_dtype(dtype) if dtype is not None else None
         )
         if shape is not None:
             self.shape = backend.standardize_shape(shape)
             self.ndim = len(shape)
         else:
             self.ndim = ndim
             self.shape = None
         self.max_ndim = max_ndim
         self.min_ndim = min_ndim
         self.name = name
+        self.optional = optional
         self.allow_last_axis_squeeze = allow_last_axis_squeeze
         try:
             axes = axes or {}
             self.axes = {int(k): axes[k] for k in axes}
         except (ValueError, TypeError):
             raise TypeError(
                 "Argument `axes` must be a dict with integer keys. "
@@ -148,40 +152,36 @@
                         f"{list(inputs.keys())}. "
                         f"Expected the following keys: {names}"
                     )
                 list_inputs.append(inputs[name])
             inputs = list_inputs
 
     inputs = tree.flatten(inputs)
-    if len(input_spec) != len(inputs):
+    if len(inputs) != len(input_spec):
         raise ValueError(
-            f"Layer '{layer_name}' expected {len(input_spec)} input(s). "
-            f"Received {len(inputs)} instead."
+            f'Layer "{layer_name}" expects {len(input_spec)} input(s),'
+            f" but it received {len(inputs)} input tensors. "
+            f"Inputs received: {inputs}"
         )
-    for x in inputs:
+    for input_index, (x, spec) in enumerate(zip(inputs, input_spec)):
+        if spec is None:
+            continue
+        if x is None and spec.optional:
+            continue
+
         # Having a shape/dtype is the only commonality of the various
         # tensor-like objects that may be passed. The most common kind of
         # invalid type we are guarding for is a Layer instance (Functional API),
         # which does not have a `shape` attribute.
         if not hasattr(x, "shape"):
             raise ValueError(
                 f"Inputs to a layer should be tensors. Got '{x}' "
                 f"(of type {type(x)}) as input for layer '{layer_name}'."
             )
 
-    if len(inputs) != len(input_spec):
-        raise ValueError(
-            f'Layer "{layer_name}" expects {len(input_spec)} input(s),'
-            f" but it received {len(inputs)} input tensors. "
-            f"Inputs received: {inputs}"
-        )
-    for input_index, (x, spec) in enumerate(zip(inputs, input_spec)):
-        if spec is None:
-            continue
-
         shape = backend.standardize_shape(x.shape)
         ndim = len(shape)
         # Check ndim.
         if spec.ndim is not None and not spec.allow_last_axis_squeeze:
             if ndim != spec.ndim:
                 raise ValueError(
                     f'Input {input_index} of layer "{layer_name}" '
```

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/layer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -743,16 +743,18 @@
             args = tree.map_structure(maybe_convert, args)
             kwargs = tree.map_structure(maybe_convert, kwargs)
 
         ##########################################################
         # 2. Enforce that only tensors can be passed positionally.
         if not self._allow_non_tensor_positional_args:
             for arg in tree.flatten(args):
-                if not isinstance(arg, KerasTensor) and not backend.is_tensor(
-                    arg
+                if (
+                    not isinstance(arg, KerasTensor)
+                    and not backend.is_tensor(arg)
+                    and arg is not None
                 ):
                     raise ValueError(
                         "Only input tensors may be passed as "
                         "positional arguments. The following argument value "
                         f"should be passed as a keyword argument: {arg} "
                         f"(of type {type(arg)})"
                     )
@@ -1444,15 +1446,17 @@
 
     def _open_name_scope(self):
         if self._parent_path is None:
             self._parent_path = current_path()
         return backend.name_scope(self.name, caller=self)
 
 
-def is_backend_tensor_or_symbolic(x):
+def is_backend_tensor_or_symbolic(x, allow_none=False):
+    if allow_none and x is None:
+        return True
     return backend.is_tensor(x) or isinstance(x, backend.KerasTensor)
 
 
 class CallSpec:
     def __init__(self, signature, args, kwargs):
         # `training` and `mask` are special kwargs that are always available in
         # a layer, if user specifies them in their call without adding to spec,
@@ -1479,15 +1483,18 @@
             arg_names.append(name)
             if is_backend_tensor_or_symbolic(value):
                 tensor_args.append(value)
                 tensor_arg_names.append(name)
                 tensor_arg_dict[name] = value
             elif tree.is_nested(value) and len(value) > 0:
                 flat_values = tree.flatten(value)
-                if all(is_backend_tensor_or_symbolic(x) for x in flat_values):
+                if all(
+                    is_backend_tensor_or_symbolic(x, allow_none=True)
+                    for x in flat_values
+                ):
                     tensor_args.append(value)
                     tensor_arg_names.append(name)
                     tensor_arg_dict[name] = value
                     nested_tensor_arg_names.append(name)
                 elif any(is_backend_tensor_or_symbolic(x) for x in flat_values):
                     raise ValueError(
                         "In a nested call() argument, "
```

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/add.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/average.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/dot.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/maximum.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/minimum.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/multiply.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/merging/subtract.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/string_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,39 +188,39 @@
     >>> data = ["a", "b", "c", "d", "z"]
     >>> layer = StringLookup(vocabulary=vocab, output_mode='one_hot')
     >>> layer(data)
     array([[0., 1., 0., 0., 0.],
            [0., 0., 1., 0., 0.],
            [0., 0., 0., 1., 0.],
            [0., 0., 0., 0., 1.],
-           [1., 0., 0., 0., 0.]], dtype=float32)
+           [1., 0., 0., 0., 0.]], dtype=int64)
 
     **Multi-hot output**
 
     Configure the layer with `output_mode='multi_hot'`. Note that the first
     `num_oov_indices` dimensions in the multi_hot encoding represent OOV values.
 
     >>> vocab = ["a", "b", "c", "d"]
     >>> data = [["a", "c", "d", "d"], ["d", "z", "b", "z"]]
     >>> layer = StringLookup(vocabulary=vocab, output_mode='multi_hot')
     >>> layer(data)
     array([[0., 1., 0., 1., 1.],
-           [1., 0., 1., 0., 1.]], dtype=float32)
+           [1., 0., 1., 0., 1.]], dtype=int64)
 
     **Token count output**
 
     Configure the layer with `output_mode='count'`. As with multi_hot output,
     the first `num_oov_indices` dimensions in the output represent OOV values.
 
     >>> vocab = ["a", "b", "c", "d"]
     >>> data = [["a", "c", "d", "d"], ["d", "z", "b", "z"]]
     >>> layer = StringLookup(vocabulary=vocab, output_mode='count')
     >>> layer(data)
     array([[0., 1., 0., 1., 2.],
-           [2., 0., 1., 0., 1.]], dtype=float32)
+           [2., 0., 1., 0., 1.]], dtype=int64)
 
     **TF-IDF output**
 
     Configure the layer with `output_mode="tf_idf"`. As with multi_hot output,
     the first `num_oov_indices` dimensions in the output represent OOV values.
 
     Each token bin will output `token_count * idf_weight`, where the idf weights
```

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/gru.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/legacy/backend.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/legacy/layers.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/legacy/losses.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/losses/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/losses/loss.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/losses/losses.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/metrics/metric.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/models/cloning.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/models/functional.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/models/functional.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,69 +98,42 @@
     def __new__(cls, *args, **kwargs):
         return typing.cast(Functional, super().__new__(cls))
 
     @tracking.no_automatic_dependency_tracking
     def __init__(self, inputs, outputs, name=None, **kwargs):
         if isinstance(inputs, dict):
             for k, v in inputs.items():
-                if not isinstance(v, backend.KerasTensor):
-                    raise ValueError(
-                        "When providing `inputs` as a dict, all values in the "
-                        f"dict must be KerasTensors. Received: inputs={inputs} "
-                        f"including invalid value {v} of type {type(v)}"
-                    )
-                if k != v.name:
+                if isinstance(v, backend.KerasTensor) and k != v.name:
                     warnings.warn(
                         "When providing `inputs` as a dict, all keys in the "
                         "dict must match the names of the corresponding "
                         f"tensors. Received key '{k}' mapping to value {v} "
                         f"which has name '{v.name}'. Change the tensor name to "
                         f"'{k}' (via `Input(..., name='{k}')`)"
                     )
-        elif isinstance(inputs, (list, tuple)):
-            for x in inputs:
-                if not isinstance(x, backend.KerasTensor):
-                    raise ValueError(
-                        "When providing `inputs` as a list/tuple, all values "
-                        f"in the list/tuple must be KerasTensors. Received: "
-                        f"inputs={inputs} including invalid value {x} of type "
-                        f"{type(x)}"
-                    )
-        elif not isinstance(inputs, backend.KerasTensor):
-            raise ValueError(
-                f"Unrecognized type for `inputs`: {inputs} "
-                f"(of type {type(inputs)})"
-            )
-        if isinstance(outputs, dict):
-            for k, v in outputs.items():
-                if not isinstance(v, backend.KerasTensor):
-                    raise ValueError(
-                        "When providing `outputs` as a dict, all values in the "
-                        f"dict must be KerasTensors. Received: "
-                        f"outputs={outputs} including invalid value {v} of "
-                        f"type {type(v)}"
-                    )
-        elif isinstance(outputs, (list, tuple)):
-            for x in outputs:
-                if not isinstance(x, backend.KerasTensor):
-                    raise ValueError(
-                        "When providing `outputs` as a list/tuple, all values "
-                        f"in the list/tuple must be KerasTensors. Received: "
-                        f"outputs={outputs} including invalid value {x} of "
-                        f"type {type(x)}"
-                    )
-        elif not isinstance(outputs, backend.KerasTensor):
-            raise ValueError(
-                f"Unrecognized type for `outputs`: {outputs} "
-                f"(of type {type(outputs)})"
-            )
 
         trainable = kwargs.pop("trainable", None)
+        flat_inputs = tree.flatten(inputs)
+        flat_outputs = tree.flatten(outputs)
+        for x in flat_inputs:
+            if not isinstance(x, backend.KerasTensor):
+                raise ValueError(
+                    "All `inputs` values must be KerasTensors. Received: "
+                    f"inputs={inputs} including invalid value {x} of "
+                    f"type {type(x)}"
+                )
+        for x in flat_outputs:
+            if not isinstance(x, backend.KerasTensor):
+                raise ValueError(
+                    "All `outputs` values must be KerasTensors. Received: "
+                    f"outputs={outputs} including invalid value {x} of "
+                    f"type {type(x)}"
+                )
 
-        if not all([is_input_keras_tensor(t) for t in tree.flatten(inputs)]):
+        if not all(is_input_keras_tensor(t) for t in flat_inputs):
             inputs, outputs = clone_graph_nodes(inputs, outputs)
 
         Function.__init__(self, inputs, outputs, name=name, **kwargs)
 
         if trainable is not None:
             self.trainable = trainable
 
@@ -224,58 +197,37 @@
         if isinstance(output_shapes, list) and len(output_shapes) == 1:
             return output_shapes[0]
         return output_shapes
 
     def _assert_input_compatibility(self, *args):
         return super(Model, self)._assert_input_compatibility(*args)
 
-    def _flatten_to_reference_inputs(self, inputs, allow_extra_keys=True):
-        if isinstance(inputs, dict):
-            ref_inputs = self._inputs_struct
-            if not tree.is_nested(ref_inputs):
-                ref_inputs = [self._inputs_struct]
-            if isinstance(ref_inputs, dict):
-                # In the case that the graph is constructed with dict input
-                # tensors, We will use the original dict key to map with the
-                # keys in the input data. Note that the model.inputs is using
-                # tree.flatten to process the input tensors, which means the
-                # dict input tensors are ordered by their keys.
-                ref_input_names = sorted(ref_inputs.keys())
-            else:
-                ref_input_names = [
-                    inp._keras_history.operation.name for inp in ref_inputs
-                ]
-            # Raise an warning if there are more input data comparing to input
-            # tensor
-            if not allow_extra_keys and len(inputs) > len(ref_input_names):
-                warnings.warn(
-                    "Input dict contained keys {} which did not match any "
-                    "model input. They will be ignored by the model.".format(
-                        [n for n in inputs.keys() if n not in ref_input_names]
-                    ),
-                    stacklevel=2,
-                )
-            # Flatten in the order `Input`s were passed during Model
-            # construction.
-            return [inputs[n] for n in ref_input_names]
-        # Otherwise both ref inputs and inputs will already be in same order.
+    def _flatten_to_reference_inputs(self, inputs):
         return tree.flatten(inputs)
 
     def _convert_inputs_to_tensors(self, flat_inputs):
         converted = []
         for x, input in zip(flat_inputs, self._inputs):
-            converted.append(
-                ops.convert_to_tensor(x, dtype=input.dtype, sparse=input.sparse)
-            )
+            if x is None:  # TODO: check if optional
+                converted.append(x)
+            else:
+                converted.append(
+                    ops.convert_to_tensor(
+                        x, dtype=input.dtype, sparse=input.sparse
+                    )
+                )
         return converted
 
     def _adjust_input_rank(self, flat_inputs):
         flat_ref_shapes = [x.shape for x in self._inputs]
         adjusted = []
         for x, ref_shape in zip(flat_inputs, flat_ref_shapes):
+            if x is None:
+                adjusted.append(x)
+                continue
             x_rank = len(x.shape)
             ref_rank = len(ref_shape)
             if x_rank == ref_rank:
                 adjusted.append(x)
                 continue
             if x_rank == ref_rank + 1:
                 if x.shape[-1] == 1:
@@ -324,38 +276,45 @@
 
         def shape_with_no_batch_size(x):
             x = list(x)
             if x:
                 x[0] = None
             return tuple(x)
 
+        def make_spec_for_tensor(x):
+            optional = False
+            if isinstance(x._keras_history[0], InputLayer):
+                if x._keras_history[0].optional:
+                    optional = True
+            return InputSpec(
+                shape=shape_with_no_batch_size(x.shape),
+                allow_last_axis_squeeze=True,
+                name=x._keras_history[0].name,
+                optional=optional,
+            )
+
         if isinstance(self._inputs_struct, dict):
-            # Case where `_nested_inputs` is a plain dict of Inputs.
-            names = sorted(self._inputs_struct.keys())
-            return [
-                InputSpec(
-                    shape=shape_with_no_batch_size(
-                        self._inputs_struct[name].shape
-                    ),
-                    allow_last_axis_squeeze=True,
-                    name=name,
-                )
-                for name in names
-            ]
-        else:
-            # Single input, or list/tuple of inputs.
-            # The data may be passed as a dict keyed by input name.
-            return [
-                InputSpec(
-                    shape=shape_with_no_batch_size(x.shape),
-                    allow_last_axis_squeeze=True,
-                    name=x._keras_history[0].name,
-                )
-                for x in self._inputs
-            ]
+            if all(
+                isinstance(x, backend.KerasTensor)
+                for x in self._inputs_struct.values()
+            ):
+                # Case where `_nested_inputs` is a plain dict of Inputs.
+                names = sorted(self._inputs_struct.keys())
+                return [
+                    InputSpec(
+                        shape=shape_with_no_batch_size(
+                            self._inputs_struct[name].shape
+                        ),
+                        allow_last_axis_squeeze=True,
+                        name=name,
+                    )
+                    for name in names
+                ]
+            return None  # Deeply nested dict: skip checks.
+        return [make_spec_for_tensor(x) for x in self.inputs]
 
     @input_spec.setter
     def input_spec(self, value):
         self._manual_input_spec = value
 
     def get_config(self):
         if not functional_like_constructor(self.__class__):
@@ -420,20 +379,17 @@
             tensor_index = tensor._keras_history[2]
             node_key = make_node_key(operation, node_index)
             assert node_key in self._nodes
             new_node_index = node_reindexing_map[node_key]
             return [operation.name, new_node_index, tensor_index]
 
         def map_tensors(tensors):
-            if isinstance(tensors, dict):
-                return {k: get_tensor_config(v) for k, v in tensors.items()}
-            if isinstance(tensors, (list, tuple)):
-                return [get_tensor_config(v) for v in tensors]
-            else:
+            if isinstance(tensors, backend.KerasTensor):
                 return [get_tensor_config(tensors)]
+            return tree.map_structure(get_tensor_config, tensors)
 
         config["input_layers"] = map_tensors(self._inputs_struct)
         config["output_layers"] = map_tensors(self._outputs_struct)
         return copy.deepcopy(config)
 
 
 def functional_from_config(cls, config, custom_objects=None):
@@ -559,24 +515,28 @@
         if isinstance(layer, Functional):
             # Functional models start out with a built-in node.
             node_index -= 1
         layer_output_tensors = layer._inbound_nodes[node_index].output_tensors
         return layer_output_tensors[tensor_index]
 
     def map_tensors(tensors):
+        if (
+            isinstance(tensors, list)
+            and len(tensors) == 3
+            and isinstance(tensors[0], str)
+        ):
+            # Leaf
+            return get_tensor(*tensors)
         if isinstance(tensors, dict):
-            return {k: get_tensor(*v) for k, v in tensors.items()}
-        else:
-            tensor_list = [get_tensor(*v) for v in tensors]
-            if len(tensor_list) == 1:
-                return tensor_list[0]
-            return tensor_list
+            return {k: map_tensors(v) for k, v in tensors.items()}
+        return [map_tensors(v) for v in tensors]
 
     input_tensors = map_tensors(config["input_layers"])
     output_tensors = map_tensors(config["output_layers"])
+
     return cls(
         inputs=input_tensors,
         outputs=output_tensors,
         name=name,
         trainable=trainable,
     )
```

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/models/model.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/models/sequential.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/models/variable_mapping.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/core.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/function.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,18 +84,20 @@
 
     @property
     def operations(self):
         return self._operations[:]
 
     @property
     def inputs(self):
+        """Flat list of the symbolic inputs of the Function."""
         return self._inputs
 
     @property
     def outputs(self):
+        """Flat list of the symbolic outputs of the Function."""
         return self._outputs
 
     def compute_output_spec(self, inputs):
         self._assert_input_compatibility(inputs)
         # Check if input shapes are identical to ref input shapes,
         # if so take a shortcut.
         shortcut = True
```

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/image.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/linalg.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/math.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/nn.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/node.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/numpy.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/operation.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,27 +75,24 @@
     def quantized_call(self, *args, **kwargs):
         raise NotImplementedError
 
     def compute_output_spec(self, *args, **kwargs):
         try:
             return backend.compute_output_spec(self.call, *args, **kwargs)
         except Exception as e:
-            if isinstance(e, TypeError):
-                raise e
-            else:
-                new_e = RuntimeError(
-                    "Could not automatically infer the output shape / dtype of "
-                    f"'{self.name}' (of type {self.__class__.__name__}). "
-                    f"Either the `{self.__class__.__name__}.call()` method "
-                    f"is incorrect, or you need to implement the "
-                    f"`{self.__class__.__name__}.compute_output_spec() / "
-                    "compute_output_shape()` method. "
-                    f"Error encountered:\n\n{e}"
-                )
-                raise new_e.with_traceback(e.__traceback__) from None
+            new_e = e.__class__(
+                "Could not automatically infer the output shape / dtype of "
+                f"'{self.name}' (of type {self.__class__.__name__}). "
+                f"Either the `{self.__class__.__name__}.call()` method "
+                f"is incorrect, or you need to implement the "
+                f"`{self.__class__.__name__}.compute_output_spec() / "
+                "compute_output_shape()` method. "
+                f"Error encountered:\n\n{e}"
+            )
+            raise new_e.with_traceback(e.__traceback__) from None
 
     def __new__(cls, *args, **kwargs):
         """We override __new__ to saving serializable constructor arguments.
 
         These arguments are used to auto-generate an object serialization
         config, which enables user-created subclasses to be serializable
         out of the box in most cases without forcing the user
```

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/operation_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/ops/symbolic_arguments.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,13 +36,11 @@
         if self._single_positional_tensor is not None:
             # Performance optimization for most common case.
             # Approx. 70x faster.
             return (tensor_dict[id(self._single_positional_tensor)],), {}
 
         def switch_fn(x):
             if isinstance(x, KerasTensor):
-                val = tensor_dict.get(id(x), None)
-                if val is not None:
-                    return val
+                return tensor_dict.get(id(x), None)
             return x
 
         return self.convert(switch_fn)
```

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adadelta.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adafactor.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adagrad.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adam.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adamax.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/adamw.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/ftrl.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/lion.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/nadam.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/optimizer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/optimizers/sgd.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/quantizers/quantizers.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/random/random.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/random/seed_generator.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/regularizers/regularizers.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/saving/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/saving/keras_saveable.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/saving/keras_saveable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/saving/object_registration.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/saving/saving_api.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/saving/saving_lib.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/saving/serialization_lib.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/testing/test_case.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/testing/test_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/compile_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/trainers/trainer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/tree/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/tree/optree_impl.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/tree/tree_api.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/__init__.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/argument_validation.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/backend_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/code_stats.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/dataset_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/dtype_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/file_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/image_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/io_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/jax_layer.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/model_visualization.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/module_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/naming.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/numerical_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/progbar.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/python_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/rng_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/sequence_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/summary_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/tf_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/torch_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/traceback_utils.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras/src/utils/tracking.py` & `keras_nightly-3.3.3.dev2024050703/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.3.dev2024050603
+Version: 3.3.3.dev2024050703
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.3.dev2024050603/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.3.3.dev2024050703/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050603/setup.py` & `keras_nightly-3.3.3.dev2024050703/setup.py`

 * *Files identical despite different names*

