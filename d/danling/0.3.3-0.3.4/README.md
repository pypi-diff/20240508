# Comparing `tmp/danling-0.3.3.tar.gz` & `tmp/danling-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danling-0.3.3.tar", last modified: Tue Feb 27 05:21:19 2024, max compression
+gzip compressed data, was "danling-0.3.4.tar", last modified: Wed May  8 06:30:34 2024, max compression
```

## Comparing `danling-0.3.3.tar` & `danling-0.3.4.tar`

### file list

```diff
@@ -1,149 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.238476 danling-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.210475 danling-0.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-27 05:20:28.000000 danling-0.3.3/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.210475 danling-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-02-27 05:20:28.000000 danling-0.3.3/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-02-27 05:20:28.000000 danling-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-27 05:20:28.000000 danling-0.3.3/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       88 2024-02-27 05:20:28.000000 danling-0.3.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.210475 danling-0.3.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-27 05:20:28.000000 danling-0.3.3/LICENSES/LICENSE.AGPL
--rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-02-27 05:20:28.000000 danling-0.3.3/LICENSES/LICENSE.Apache
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-02-27 05:20:28.000000 danling-0.3.3/LICENSES/LICENSE.BSD
--rwxr-xr-x   0 runner    (1001) docker     (127)    18092 2024-02-27 05:20:28.000000 danling-0.3.3/LICENSES/LICENSE.GPLv2
--rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-02-27 05:20:28.000000 danling-0.3.3/LICENSES/LICENSE.GPLv3
--rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-02-27 05:20:28.000000 danling-0.3.3/LICENSES/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-27 05:20:28.000000 danling-0.3.3/LICENSES/LICENSE.Unlicense
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-02-27 05:21:19.238476 danling-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-27 05:20:28.000000 danling-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-27 05:20:28.000000 danling-0.3.3/anaconda-project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.214475 danling-0.3.3/danling/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-27 05:20:28.000000 danling-0.3.3/danling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-27 05:21:18.000000 danling-0.3.3/danling/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.214475 danling-0.3.3/danling/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-27 05:20:28.000000 danling-0.3.3/danling/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-02-27 05:20:28.000000 danling-0.3.3/danling/metrics/average_meters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-02-27 05:20:28.000000 danling-0.3.3/danling/metrics/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-02-27 05:20:28.000000 danling-0.3.3/danling/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.214475 danling-0.3.3/danling/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.214475 danling-0.3.3/danling/modules/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/mlp/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/mlp/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.214475 danling-0.3.3/danling/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.214475 danling-0.3.3/danling/modules/transformer/attention/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/transformer/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/transformer/attention/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/transformer/attention/simple_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/transformer/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.214475 danling-0.3.3/danling/modules/transformer/ffn/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/transformer/ffn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/transformer/ffn/fcn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.214475 danling-0.3.3/danling/modules/transformer/pos_embed/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/transformer/pos_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-02-27 05:20:28.000000 danling-0.3.3/danling/modules/transformer/pos_embed/pos_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.214475 danling-0.3.3/danling/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-27 05:20:28.000000 danling-0.3.3/danling/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.218475 danling-0.3.3/danling/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-27 05:20:28.000000 danling-0.3.3/danling/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-02-27 05:20:28.000000 danling-0.3.3/danling/optim/lr_scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-27 05:20:28.000000 danling-0.3.3/danling/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.218475 danling-0.3.3/danling/runner/
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-02-27 05:20:28.000000 danling-0.3.3/danling/runner/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-27 05:20:28.000000 danling-0.3.3/danling/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-02-27 05:20:28.000000 danling-0.3.3/danling/runner/accelerate_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    43062 2024-02-27 05:20:28.000000 danling-0.3.3/danling/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-27 05:20:28.000000 danling-0.3.3/danling/runner/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-02-27 05:20:28.000000 danling-0.3.3/danling/runner/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-02-27 05:20:28.000000 danling-0.3.3/danling/runner/torch_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-02-27 05:20:28.000000 danling-0.3.3/danling/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.218475 danling-0.3.3/danling/tensors/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-27 05:20:28.000000 danling-0.3.3/danling/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-27 05:20:28.000000 danling-0.3.3/danling/tensors/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    41933 2024-02-27 05:20:28.000000 danling-0.3.3/danling/tensors/nested_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-02-27 05:20:28.000000 danling-0.3.3/danling/tensors/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-27 05:20:28.000000 danling-0.3.3/danling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.218475 danling-0.3.3/danling/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-27 05:20:28.000000 danling-0.3.3/danling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-27 05:20:28.000000 danling-0.3.3/danling/utils/basex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-27 05:20:28.000000 danling-0.3.3/danling/utils/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-02-27 05:20:28.000000 danling-0.3.3/danling/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-27 05:20:28.000000 danling-0.3.3/danling/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-02-27 05:20:28.000000 danling-0.3.3/danling/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.238476 danling-0.3.3/danling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-02-27 05:21:19.000000 danling-0.3.3/danling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-27 05:21:19.000000 danling-0.3.3/danling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 05:21:19.000000 danling-0.3.3/danling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-27 05:21:19.000000 danling-0.3.3/danling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-27 05:21:19.000000 danling-0.3.3/danling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.206475 danling-0.3.3/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.218475 danling-0.3.3/demo/vision/
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-27 05:20:28.000000 danling-0.3.3/demo/vision/torch_mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.218475 danling-0.3.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.222475 danling-0.3.3/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.222475 danling-0.3.3/docs/docs/blog/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/manifest.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.222475 danling-0.3.3/docs/docs/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/metrics/average_meter.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/metrics/average_meters.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/metrics/metrics.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.222475 danling-0.3.3/docs/docs/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/optim/lr_scheduler.md
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/package.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.222475 danling-0.3.3/docs/docs/runner/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/runner/base_runner.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/runner/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/runner/runner_state.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/runner/torch_runner.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/runner/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.222475 danling-0.3.3/docs/docs/tensors/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/tensors/nested_tensor.md
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/tensors/pn_tensor.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/tensors/torch_func_registry.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.222475 danling-0.3.3/docs/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/utils/basex.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/utils/contextmanagers.md
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/utils/decorators.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-27 05:20:28.000000 danling-0.3.3/docs/docs/utils/io.md
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-02-27 05:20:28.000000 danling-0.3.3/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.222475 danling-0.3.3/docs/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.210475 danling-0.3.3/docs/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.222475 danling-0.3.3/docs/overrides/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-27 05:20:28.000000 danling-0.3.3/docs/overrides/assets/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-27 05:20:28.000000 danling-0.3.3/docs/overrides/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.234476 danling-0.3.3/docs/overrides/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   213368 2024-02-27 05:20:28.000000 danling-0.3.3/docs/overrides/assets/fonts/CascadiaCodePL.woff2
--rw-r--r--   0 runner    (1001) docker     (127)  8530056 2024-02-27 05:20:28.000000 danling-0.3.3/docs/overrides/assets/fonts/HYQiHei.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   118704 2024-02-27 05:20:28.000000 danling-0.3.3/docs/overrides/assets/fonts/HelveticaNowDisplay.otf
--rw-r--r--   0 runner    (1001) docker     (127)   656232 2024-02-27 05:20:28.000000 danling-0.3.3/docs/overrides/assets/fonts/HelveticaWorld.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.234476 danling-0.3.3/docs/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-02-27 05:20:28.000000 danling-0.3.3/docs/overrides/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-02-27 05:20:28.000000 danling-0.3.3/docs/overrides/assets/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.238476 danling-0.3.3/docs/overrides/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-27 05:20:28.000000 danling-0.3.3/docs/overrides/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-27 05:20:28.000000 danling-0.3.3/docs/overrides/javascripts/shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-27 05:20:28.000000 danling-0.3.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-27 05:20:28.000000 danling-0.3.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-27 05:20:28.000000 danling-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-27 05:20:28.000000 danling-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 05:21:19.238476 danling-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 05:20:28.000000 danling-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.210475 danling-0.3.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.238476 danling-0.3.3/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-02-27 05:20:28.000000 danling-0.3.3/tests/metrics/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.238476 danling-0.3.3/tests/optim/
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-02-27 05:20:28.000000 danling-0.3.3/tests/optim/test_lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.238476 danling-0.3.3/tests/runner/
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-02-27 05:20:28.000000 danling-0.3.3/tests/runner/test_base_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-02-27 05:20:28.000000 danling-0.3.3/tests/runner/test_torch_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.238476 danling-0.3.3/tests/tensors/
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-02-27 05:20:28.000000 danling-0.3.3/tests/tensors/test_nested_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:21:19.238476 danling-0.3.3/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-27 05:20:28.000000 danling-0.3.3/tests/utils/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-27 05:20:28.000000 danling-0.3.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.961465 danling-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.929465 danling-0.3.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-08 06:30:31.000000 danling-0.3.4/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.933465 danling-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-08 06:30:31.000000 danling-0.3.4/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-08 06:30:31.000000 danling-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-08 06:30:31.000000 danling-0.3.4/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       88 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.933465 danling-0.3.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.AGPL
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.Apache
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.BSD
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18092 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.GPLv2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.GPLv3
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.Unlicense
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-08 06:30:34.961465 danling-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 06:30:31.000000 danling-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-08 06:30:31.000000 danling-0.3.4/anaconda-project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.933465 danling-0.3.4/danling/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-08 06:30:31.000000 danling-0.3.4/danling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 06:30:34.000000 danling-0.3.4/danling/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-08 06:30:31.000000 danling-0.3.4/danling/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-05-08 06:30:31.000000 danling-0.3.4/danling/metrics/average_meters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-08 06:30:31.000000 danling-0.3.4/danling/metrics/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-05-08 06:30:31.000000 danling-0.3.4/danling/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 06:30:31.000000 danling-0.3.4/danling/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/mlp/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/mlp/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/transformer/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/attention/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/attention/simple_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/transformer/ffn/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/ffn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/ffn/fcn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/transformer/pos_embed/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/pos_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/pos_embed/pos_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 06:30:31.000000 danling-0.3.4/danling/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 06:30:31.000000 danling-0.3.4/danling/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-08 06:30:31.000000 danling-0.3.4/danling/optim/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 06:30:31.000000 danling-0.3.4/danling/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/danling/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19467 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/accelerate_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43863 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/torch_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/danling/tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-08 06:30:31.000000 danling-0.3.4/danling/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-08 06:30:31.000000 danling-0.3.4/danling/tensors/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41934 2024-05-08 06:30:31.000000 danling-0.3.4/danling/tensors/nested_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-08 06:30:31.000000 danling-0.3.4/danling/tensors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-08 06:30:31.000000 danling-0.3.4/danling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/danling/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/basex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.961465 danling-0.3.4/danling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-08 06:30:34.000000 danling-0.3.4/danling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-08 06:30:34.000000 danling-0.3.4/danling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:30:34.000000 danling-0.3.4/danling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-08 06:30:34.000000 danling-0.3.4/danling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 06:30:34.000000 danling-0.3.4/danling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.925465 danling-0.3.4/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/demo/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-08 06:30:31.000000 danling-0.3.4/demo/vision/torch_mnist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/docs/docs/blog/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/manifest.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/docs/docs/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/metrics/average_meter.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/metrics/average_meters.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/metrics/metrics.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/docs/docs/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/optim/lr_scheduler.md
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/package.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.945465 danling-0.3.4/docs/docs/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/runner/accelerate_runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/runner/base_runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/runner/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/runner/state.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/runner/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.945465 danling-0.3.4/docs/docs/tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/tensors/nested_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/tensors/pn_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/tensors/torch_func_registry.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.945465 danling-0.3.4/docs/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/utils/basex.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/utils/contextmanagers.md
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/utils/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/utils/io.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-08 06:30:31.000000 danling-0.3.4/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.945465 danling-0.3.4/docs/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.929465 danling-0.3.4/docs/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.945465 danling-0.3.4/docs/overrides/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/docs/overrides/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   213368 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/fonts/CascadiaCodePL.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)  8530056 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/fonts/HYQiHei.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   118704 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/fonts/HelveticaNowDisplay.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   656232 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/fonts/HelveticaWorld.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/docs/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/docs/overrides/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/javascripts/shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-08 06:30:31.000000 danling-0.3.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-08 06:30:31.000000 danling-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-08 06:30:31.000000 danling-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 06:30:34.961465 danling-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 06:30:31.000000 danling-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.929465 danling-0.3.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-05-08 06:30:31.000000 danling-0.3.4/tests/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/tests/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-08 06:30:31.000000 danling-0.3.4/tests/optim/test_lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/tests/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-08 06:30:31.000000 danling-0.3.4/tests/runner/test_base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-08 06:30:31.000000 danling-0.3.4/tests/runner/test_torch_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/tests/tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-08 06:30:31.000000 danling-0.3.4/tests/tensors/test_nested_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-08 06:30:31.000000 danling-0.3.4/tests/utils/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 06:30:31.000000 danling-0.3.4/tox.ini
```

### Comparing `danling-0.3.3/.github/workflows/push.yaml` & `danling-0.3.4/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/.gitignore` & `danling-0.3.4/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -412,7 +412,10 @@
 
 # version
 danling/_version.py
 
 # pytest
 data
 examples
+
+# experiments
+experiments
```

### Comparing `danling-0.3.3/.pre-commit-config.yaml` & `danling-0.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/LICENSES/LICENSE.AGPL` & `danling-0.3.4/LICENSES/LICENSE.AGPL`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/LICENSES/LICENSE.Apache` & `danling-0.3.4/LICENSES/LICENSE.Apache`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/LICENSES/LICENSE.BSD` & `danling-0.3.4/LICENSES/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/LICENSES/LICENSE.GPLv2` & `danling-0.3.4/LICENSES/LICENSE.GPLv2`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/LICENSES/LICENSE.GPLv3` & `danling-0.3.4/LICENSES/LICENSE.GPLv3`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/LICENSES/LICENSE.MIT` & `danling-0.3.4/LICENSES/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/LICENSES/LICENSE.Unlicense` & `danling-0.3.4/LICENSES/LICENSE.Unlicense`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/PKG-INFO` & `danling-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.3.3
+Version: 0.3.4
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR AGPL-3.0-or-later OR GPL-2.0-or-later OR BSD-4-Clause OR MIT OR Apache-2.0
         
 Project-URL: documentation, https://danling.org
 Project-URL: homepage, https://danling.org
```

### Comparing `danling-0.3.3/README.md` & `danling-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/anaconda-project.yml` & `danling-0.3.4/anaconda-project.yml`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/__init__.py` & `danling-0.3.4/danling/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from danling import metrics, modules, optim, registry, runner, tensors, typing, utils
 
 from .metrics import AverageMeter, AverageMeters
 from .registry import GlobalRegistry, Registry
-from .runner import BaseRunner, TorchRunner
+from .runner import AccelerateRunner, BaseRunner, TorchRunner
 from .tensors import NestedTensor, PNTensor
 from .utils import catch, debug, ensure_dir, flexible_decorator, is_json_serializable, load, method_cache, save
 
 __all__ = [
     "metrics",
     "modules",
     "optim",
     "registry",
     "runner",
     "tensors",
     "utils",
     "typing",
     "BaseRunner",
+    "AccelerateRunner",
     "TorchRunner",
     "Registry",
     "GlobalRegistry",
     "Metrics",
     "AverageMeter",
     "AverageMeters",
     "NestedTensor",
```

### Comparing `danling-0.3.3/danling/metrics/__init__.py` & `danling-0.3.4/danling/metrics/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 from functools import partial
 
 from lazy_imports import try_import
 
 from .average_meters import AverageMeter, AverageMeters
 
 with try_import():
-    from .functional import accuracy, auprc, auroc, pearson, r2_score, rmse, spearman
+    from .functional import accuracy, auprc, auroc, matthews_corrcoef, pearson, r2_score, rmse, spearman
     from .metrics import Metrics
 
 __all__ = [
     "Metrics",
     "AverageMeter",
     "AverageMeters",
     "regression_metrics",
     "binary_metrics",
     "multiclass_metrics",
     "multilabel_metrics",
 ]
 
 
 def binary_metrics(**kwargs):
-    return Metrics(auroc=auroc, auprc=auprc, acc=accuracy, **kwargs)
+    return Metrics(auroc=auroc, auprc=auprc, acc=accuracy, mcc=matthews_corrcoef, **kwargs)
 
 
 def multiclass_metrics(num_classes: int, **kwargs):
+    p_mcc = partial(matthews_corrcoef, num_classes=num_classes)
     p_auroc = partial(auroc, num_classes=num_classes)
     p_auprc = partial(auprc, num_classes=num_classes)
     p_acc = partial(accuracy, num_classes=num_classes)
-    return Metrics(auroc=p_auroc, auprc=p_auprc, acc=p_acc, **kwargs)
+    return Metrics(auroc=p_auroc, auprc=p_auprc, acc=p_acc, mcc=p_mcc, **kwargs)
 
 
 def multilabel_metrics(num_labels: int, **kwargs):
+    p_mcc = partial(matthews_corrcoef, num_labels=num_labels)
     p_auroc = partial(auroc, num_labels=num_labels)
     p_auprc = partial(auprc, num_labels=num_labels)
-    return Metrics(auroc=p_auroc, auprc=p_auprc, acc=accuracy, **kwargs)
+    p_acc = partial(accuracy, num_labels=num_labels)
+    return Metrics(auroc=p_auroc, auprc=p_auprc, acc=p_acc, mcc=p_mcc, **kwargs)
 
 
 def regression_metrics(**kwargs):
     return Metrics(
         pearson=pearson,
         spearman=spearman,
         r2=r2_score,
```

### Comparing `danling-0.3.3/danling/metrics/functional.py` & `danling-0.3.4/danling/metrics/functional.py`

 * *Files 15% similar despite different names*

```diff
@@ -105,14 +105,39 @@
     if isinstance(input, NestedTensor):
         input = torch.cat(input.storage())
     if isinstance(target, NestedTensor):
         target = torch.cat(target.storage())
     return tmf.spearman_corrcoef(input, target)
 
 
+def matthews_corrcoef(
+    input: Tensor | NestedTensor,
+    target: Tensor | NestedTensor,
+    threshold: float = 0.5,
+    average: str | None = "micro",
+    num_labels: int | None = None,
+    num_classes: int | None = None,
+):
+    lazy_import.check()
+    if num_classes and num_labels:
+        raise ValueError("Only one of num_classes or num_labels can be specified, but not both")
+    task = "binary"
+    if num_classes:
+        task = "multiclass"
+    if num_labels:
+        task = "multilabel"
+    if isinstance(input, NestedTensor):
+        input = torch.cat(input.storage())
+    if isinstance(target, NestedTensor):
+        target = torch.cat(target.storage())
+    return tmf.matthews_corrcoef(
+        input, target, task, threshold=threshold, num_classes=num_classes, num_labels=num_labels
+    )
+
+
 def r2_score(
     input: Tensor | NestedTensor,
     target: Tensor | NestedTensor,
 ):
     if isinstance(input, NestedTensor):
         input = torch.cat(input.storage())
     if isinstance(target, NestedTensor):
```

### Comparing `danling-0.3.3/danling/metrics/metrics.py` & `danling-0.3.4/danling/metrics/metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,47 +9,37 @@
 from chanfig import DefaultDict, FlatDict
 from torch import Tensor
 from torch import distributed as dist
 from torcheval.metrics import Metric
 
 from danling.tensors import NestedTensor
 
+from .utils import flist, get_world_size
+
 try:
     from typing import Self  # type: ignore[attr-defined]
 except ImportError:
     from typing_extensions import Self
 
 
-def world_size() -> int:
-    r"""Return the number of processes in the current process group."""
-    if dist.is_available() and dist.is_initialized():
-        return dist.get_world_size()
-    return 1
-
-
-class flist(list):
-    def to(self, *args, **kwargs):
-        return flist(i.to(*args, **kwargs) for i in self)
-
-    def __format__(self, *args, **kwargs):
-        return " ".join([x.__format__(*args, **kwargs) for x in self])
-
-
 class Metrics(Metric):
     r"""
     Metric class wraps around multiple metrics that share the same states.
 
     Typically, there are many metrics that we want to compute for a single task.
     For example, we usually needs to compute `accuracy`, `auroc`, `auprc` for a classification task.
     Computing them one by one is inefficient, especially when evaluating in a distributed environment.
 
     To solve this problem, Metrics maintains a shared state for multiple metric functions.
 
     Attributes:
         metrics: A dictionary of metrics to be computed.
+        val: Metric results of current batch on current device.
+        bat: Metric results of current batch on all devices.
+        avg: Metric results of all results on all devices.
         input: The input tensor of latest batch.
         target: The target tensor of latest batch.
         inputs: All input tensors.
         targets: All target tensors.
 
     Args:
         *args: A single mapping of metrics.
@@ -65,20 +55,20 @@
         tensor([0.2000, 0.3000, 0.5000, 0.7000])
         >>> metrics.target  # ground truth of current batch
         tensor([0, 1, 0, 1])
         >>> metrics.inputs  # predicted values of all data
         tensor([0.2000, 0.3000, 0.5000, 0.7000])
         >>> metrics.targets  # ground truth of all data
         tensor([0, 1, 0, 1])
-        >>> metrics.comp  # Metrics of current batch on current device
+        >>> metrics.val  # Metrics of current batch on current device
         FlatDict(
           ('auroc'): 0.75
           ('auprc'): 0.8333333730697632
         )
-        >>> metrics.val  # Metrics of current batch on all devices
+        >>> metrics.bat  # Metrics of current batch on all devices
         FlatDict(
           ('auroc'): 0.75
           ('auprc'): 0.8333333730697632
         )
         >>> metrics.avg  # Metrics of all data on all devices
         FlatDict(
           ('auroc'): 0.75
@@ -89,20 +79,20 @@
         tensor([0.1000, 0.4000, 0.6000, 0.8000])
         >>> metrics.target  # ground truth of current batch
         tensor([0, 0, 1, 0])
         >>> metrics.inputs  # predicted values of all data
         tensor([0.2000, 0.3000, 0.5000, 0.7000, 0.1000, 0.4000, 0.6000, 0.8000])
         >>> metrics.targets  # ground truth of all data
         tensor([0, 1, 0, 1, 0, 0, 1, 0])
-        >>> metrics.comp  # Metrics of current batch on current device
+        >>> metrics.val  # Metrics of current batch on current device
         FlatDict(
           ('auroc'): 0.6666666666666666
           ('auprc'): 0.5
         )
-        >>> metrics.val  # Metrics of current batch on all devices
+        >>> metrics.bat  # Metrics of current batch on all devices
         FlatDict(
           ('auroc'): 0.6666666666666666
           ('auprc'): 0.5
         )
         >>> metrics.avg  # Metrics of all data on all devices
         FlatDict(
           ('auroc'): 0.6666666666666666
@@ -162,33 +152,36 @@
         else:
             if not isinstance(target, torch.Tensor):
                 target = torch.tensor(target)
             self._target = target
             self._target_buffer.append(target.cpu())
 
     def compute(self) -> FlatDict[str, float]:
-        return self.comp
+        return self.calculate(self.inputs.to(self.device), self.targets.to(self.device))
 
     def value(self) -> FlatDict[str, float]:
-        return self.val
+        return self.calculate(self._input, self._target)
+
+    def batch(self) -> FlatDict[str, float]:
+        return self.calculate(self.input, self.target)
 
     def average(self) -> FlatDict[str, float]:
-        return self.avg
+        return self.calculate(self.inputs.to(self.device), self.targets.to(self.device))
 
     @property
-    def comp(self) -> FlatDict[str, float]:
-        return self.calculate(self._input, self._target)
+    def val(self) -> FlatDict[str, float]:
+        return self.value()
 
     @property
-    def val(self) -> FlatDict[str, float]:
-        return self.calculate(self.input, self.target)
+    def bat(self) -> FlatDict[str, float]:
+        return self.batch()
 
     @property
     def avg(self) -> FlatDict[str, float]:
-        return self.calculate(self.inputs.to(self.device), self.targets.to(self.device))
+        return self.average()
 
     @torch.inference_mode()
     def calculate(self, input: Tensor, target: Tensor) -> flist | float:
         if (
             isinstance(input, (Tensor, NestedTensor))
             and input.numel() == 0 == target.numel()
             or isinstance(input, (list, dict))
@@ -220,42 +213,48 @@
         raise NotImplementedError()
 
     # Due to an issue with PyTorch, we cannot decorate input/target with @torch.inference_mode()
     # Otherwise, we will encounter the following error when using "gloo" backend:
     # Inplace update to inference tensor outside InferenceMode is not allowed
     @property
     def input(self):
-        if world_size() == 1:
+        world_size = get_world_size()
+        if world_size == 1:
+            if isinstance(self._input, NestedTensor) and not self.return_nested:
+                return torch.cat(self._input.storage(), 0)
             return self._input
         if isinstance(self._input, Tensor):
-            synced_tensor = [torch.zeros_like(self._input) for _ in range(dist.get_world_size())]
+            synced_tensor = [torch.zeros_like(self._input) for _ in range(world_size)]
             dist.all_gather(synced_tensor, self._input)
             return torch.cat(synced_tensor, 0)
         if isinstance(self._input, NestedTensor):
-            synced_tensors = [None for _ in range(dist.get_world_size())]
+            synced_tensors = [None for _ in range(world_size)]
             dist.all_gather_object(synced_tensors, self._input.storage())
             synced_tensors = flist(i.to(self.device) for j in synced_tensors for i in j)
             try:
                 return torch.cat(synced_tensors, 0)
             except RuntimeError:
                 if self.return_nested:
                     return NestedTensor(synced_tensor)
                 return synced_tensors
         raise ValueError(f"Expected _input to be a Tensor or a NestedTensor, but got {type(self._input)}")
 
     @property
     def target(self):
-        if world_size() == 1:
+        world_size = get_world_size()
+        if world_size == 1:
+            if isinstance(self._target, NestedTensor) and not self.return_nested:
+                return torch.cat(self._target.storage(), 0)
             return self._target
         if isinstance(self._target, Tensor):
-            synced_tensor = [torch.zeros_like(self._target) for _ in range(dist.get_world_size())]
+            synced_tensor = [torch.zeros_like(self._target) for _ in range(world_size)]
             dist.all_gather(synced_tensor, self._target)
             return torch.cat(synced_tensor, 0)
         if isinstance(self._target, NestedTensor):
-            synced_tensors = [None for _ in range(dist.get_world_size())]
+            synced_tensors = [None for _ in range(world_size)]
             dist.all_gather_object(synced_tensors, self._target.storage())
             synced_tensors = flist(i.to(self.device) for j in synced_tensors for i in j)
             try:
                 return torch.cat(synced_tensors, 0)
             except RuntimeError:
                 if self.return_nested:
                     return NestedTensor(synced_tensor)
@@ -263,16 +262,17 @@
         raise ValueError(f"Expected _target to be a Tensor or a NestedTensor, but got {type(self._target)}")
 
     @property
     def inputs(self):
         if not self._inputs and not self._input_buffer:
             return torch.empty(0)
         if self._input_buffer:
-            if world_size() > 1:
-                synced_tensors = [None for _ in range(dist.get_world_size())]
+            world_size = get_world_size()
+            if world_size > 1:
+                synced_tensors = [None for _ in range(world_size)]
                 dist.all_gather_object(synced_tensors, self._input_buffer)
                 self._inputs.extend([i for j in synced_tensors for i in j])
             else:
                 self._inputs.extend(self._input_buffer)
             self._input_buffer = flist()
         try:
             return torch.cat(self._inputs, 0)
@@ -282,16 +282,17 @@
             return self._inputs
 
     @property
     def targets(self):
         if not self._targets and not self._target_buffer:
             return torch.empty(0)
         if self._target_buffer:
-            if world_size() > 1:
-                synced_tensors = [None for _ in range(dist.get_world_size())]
+            world_size = get_world_size()
+            if world_size > 1:
+                synced_tensors = [None for _ in range(world_size)]
                 dist.all_gather_object(synced_tensors, self._target_buffer)
                 self._targets.extend([i for j in synced_tensors for i in j])
             else:
                 self._targets.extend(self._target_buffer)
             self._target_buffer = flist()
         try:
             return torch.cat(self._targets, 0)
@@ -301,15 +302,15 @@
             return self._targets
 
     def __repr__(self):
         keys = tuple(i for i in self.metrics.keys())
         return f"{self.__class__.__name__}{keys}"
 
     def __format__(self, format_spec):
-        val, avg = self.compute(), self.average()
+        val, avg = self.value(), self.average()
         return "\n".join(
             [f"{key}: {val[key].__format__(format_spec)} ({avg[key].__format__(format_spec)})" for key in self.metrics]
         )
 
     def reset(self: Self) -> Self:  # pragma: no cover
         """
         Reset the metric state variables to their default value.
```

### Comparing `danling-0.3.3/danling/modules/__init__.py` & `danling-0.3.4/danling/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/modules/mlp/dense.py` & `danling-0.3.4/danling/modules/mlp/dense.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/modules/mlp/mlp.py` & `danling-0.3.4/danling/modules/mlp/mlp.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/modules/transformer/__init__.py` & `danling-0.3.4/danling/modules/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/modules/transformer/attention/multihead_attention.py` & `danling-0.3.4/danling/modules/transformer/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/modules/transformer/attention/simple_attention.py` & `danling-0.3.4/danling/modules/transformer/attention/simple_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/modules/transformer/decoder.py` & `danling-0.3.4/danling/modules/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/modules/transformer/encoder.py` & `danling-0.3.4/danling/modules/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/modules/transformer/ffn/fcn.py` & `danling-0.3.4/danling/modules/transformer/ffn/fcn.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/modules/transformer/pos_embed/pos_embed.py` & `danling-0.3.4/danling/modules/transformer/pos_embed/pos_embed.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/optim/lr_scheduler/lr_scheduler.py` & `danling-0.3.4/danling/optim/lr_scheduler/lr_scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,26 @@
     You can alternate by passing `warmup_steps` and `cooldown_steps`, or disable them by setting them to 0.
 
     Args:
         optimizer: Wrapped optimizer.
         total_steps: Total number of steps.
         final_lr_ratio: Final learning rate ratio to initial learning rate.
             Defaults to 1e-3.
-        final_lr: Final learning rate. Deprecated, use `final_lr_ratio` instead.
-            Defaults to None.
+        final_lr: Final learning rate.
         min_lr: Minimal learning rate.
             Defaults to 1e-9.
         strategy: Scaling strategy.
             Defaults to "cosine".
         warmup_steps: Number of warmup steps.
             Defaults to `steps // 20`.
         cooldown_steps: Number of cooldown steps.
             Defaults to `steps // 5`.
         last_epoch: The index of last epoch.
             Defaults to -1.
-        method: Method to calculate learning rate given ratio, should be one of "percentile" or "linear".
+        method: Method to calculate learning rate given ratio, should be one of "percentile" or "numerical".
             Defaults to "percentile".
 
     Examples:
         >>> from danling.optim import LRScheduler
         >>> import torch
         >>> from torch import optim
         >>> optimizer = optim.SGD([{'params': torch.tensor([0])}], lr=1, momentum=0.9)
@@ -59,15 +58,15 @@
         [0.3330753446, 0.0187302031, 0.000533897, 3.00232e-05, 1e-09]
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
         total_steps: int,
-        final_lr_ratio: float = 1e-3,
+        final_lr_ratio: Optional[float] = None,
         final_lr: Optional[float] = None,
         min_lr: float = 1e-9,
         strategy: str = "cosine",
         warmup_steps: Optional[int] = None,
         cooldown_steps: Optional[int] = None,
         last_epoch: int = -1,
         method: str = "percentile",
@@ -82,32 +81,36 @@
             raise ValueError(f"Warmup steps must be positive, but got {warmup_steps}")
         if cooldown_steps is None:
             cooldown_steps = total_steps // 5
         elif cooldown_steps > total_steps:
             raise ValueError(f"Cooldown steps must be less than total steps, but got {cooldown_steps} > {total_steps}")
         elif cooldown_steps < 0:
             raise ValueError(f"Cooldown steps must be positive, but got {cooldown_steps}")
-        if final_lr_ratio < 0:
+        if final_lr_ratio is not None and final_lr is not None:
+            raise ValueError("Only one of `final_lr_ratio` and `final_lr` should be set, but not both")
+        if final_lr_ratio is not None and final_lr_ratio < 0:
             raise ValueError(f"`final_lr_ratio` must be positive, but got {final_lr_ratio}")
+        if final_lr is not None and final_lr < 0:
+            raise ValueError(f"`final_lr` must be positive, but got {final_lr}")
         if min_lr < 0:
             raise ValueError(f"`min_lr` must be positive, but got {min_lr}")
         self.strategies = {
             k: v for k, v in self.__class__.__dict__.items() if callable(v) and (not k.startswith("_") or k in "get_lr")
         }
         if strategy not in self.strategies:
             raise ValueError(f"Scaling strategy must be one of {self.strategies.keys()}, but got {strategy}")
-        self.total_steps = total_steps
+
+        if final_lr_ratio is None and final_lr is None:
+            final_lr_ratio = 1e-3
+        if final_lr is not None and min_lr > final_lr:
+            min_lr = final_lr
+
         self.final_lr_ratio = final_lr_ratio
-        if final_lr is not None:
-            warn(
-                "Argument `final_lr` is deprecated, use `final_lr_ratio` instead",
-                category=DeprecationWarning,
-                stacklevel=2,
-            )
         self.final_lr = final_lr
+        self.total_steps = total_steps
         self.min_lr = min_lr
         self.strategy = strategy
         self.method = method
         self.warmup_steps = warmup_steps
         self.cooldown_steps = cooldown_steps
         self.cooldown_steps_begin = self.total_steps - self.cooldown_steps
         super().__init__(optimizer, last_epoch)
@@ -130,15 +133,15 @@
         warmup_ratio: Optional[float] = None,
         cooldown_ratio: Optional[float] = None,
         method: Optional[str] = None,
     ) -> float:
         method = method or self.method
         step_count = step_count or self._step_count
         progress = progress or min(max(step_count / self.total_steps, 0.0), 1.0)
-        final_lr = self.final_lr or lr * self.final_lr_ratio
+        final_lr = self.final_lr if self.final_lr is not None else lr * self.final_lr_ratio  # type: ignore[operator]
         ratio = getattr(self, self.strategy)(progress)
         if method == "percentile":
             lr *= pow(final_lr / lr, ratio)
         elif method == "numerical":
             lr = (1 - ratio) * (lr - final_lr) + final_lr
         else:
             raise ValueError(f"Method must be one of ['percentile', 'numerical'], but got {method}")
```

### Comparing `danling-0.3.3/danling/runner/README.md` & `danling-0.3.4/danling/runner/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ### PlatformRunner
 
 PlatformRunner implements platform-specific features like `step` and `prepare`.
 
 The Runner contains all runtime information that is irrelevant to the checkpoint (e.g. `world_size`, `rank`, etc.). All other information should be saved in `RunnerState`.
 
-Currently, only [`TorchRunner`][danling.runner.TorchRunner] is supported.
+Currently, only [`AccelerateRunner`][danling.runner.AccelerateRunner] is supported.
 
 ### [`BaseRunner`][danling.runner.BaseRunner]
 
 [`BaseRunner`](danling.runner.BaseRunner) defines shared attributes and implements platform-agnostic features, including `init_logging`, `results` and `scores`.
 
 ### [`RunnerState`][danling.runner.RunnerState]
```

### Comparing `danling-0.3.3/danling/runner/accelerate_runner.py` & `danling-0.3.4/danling/runner/accelerate_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import random
 from collections.abc import Callable, Mapping
 from contextlib import suppress
 from time import time
 from typing import Any
 from warnings import warn
 
+# pylint: disable=redefined-builtin
 import torch
 from accelerate import Accelerator
 from accelerate.utils import DeepSpeedPlugin
 from chanfig import NestedDict
 from torch import distributed as dist
 from torch import nn, optim, utils
 from torch.backends import cudnn
@@ -21,18 +22,18 @@
     from numpy import random as np_random
 except ImportError:
     np_random = None
 
 from danling.utils import catch
 
 from .base_runner import BaseRunner
-from .utils import on_main_process
+from .utils import RunnerMode, on_main_process
 
 
-class AccelerateRunner(BaseRunner):
+class AccelerateRunner(BaseRunner):  # pylint: disable=too-many-public-methods
     r"""
     Set up everything for running a job.
 
     `AccelerateRunner` uses [`accelerate`][accelerate] as distributed backend to
     provide seamless distributed training experience.
 
     `AccelerateRunner` will automatically [`prepare`][accelerate.Accelerator.prepare] everything,
@@ -45,16 +46,14 @@
     automatically set `shuffle`.
 
     Attributes:
         accelerator (Accelerator):
         accelerate: Arguments to pass when building accelerator. Defaults to `{}`.
     """
 
-    # pylint: disable=R0902
-
     accelerator: Accelerator
     accelerate: dict
 
     model: nn.Module
     criterion: nn.Module
     optimizer: optim.Optimizer
     scheduler: optim.lr_scheduler._LRScheduler
@@ -70,36 +69,28 @@
         else:
             config = args[0]
         if "accelerate" not in self:  # class attributes
             self.accelerate = {}
         self.accelerate.update(config.get("accelerate", {}))
         super().__init__(config)
 
-    def __post_init__(self, *args, **kwargs) -> None:
-        self._prepare()
-
-    def _prepare(self):
+    def __post_init__(self) -> None:
+        self.model, self.criterion, self.optimizer = self.prepare(self.model, self.criterion, self.optimizer)
+        self.scheduler = self.prepare(self.scheduler)
         if self.datasets:
             datasets = {k: d for k, d in self.datasets.items() if k not in self.dataloaders}
-            dataloader_kwargs = self.state.get("dataloader", {})
+            default_kwargs = self.state.get("dataloader", NestedDict)
+            dataloader_kwargs = NestedDict({k: default_kwargs.pop(k) for k in self.datasets if k in default_kwargs})
             for k, d in datasets.items():
-                shuffle = dataloader_kwargs.shuffle if "shuffle" in dataloader_kwargs else getattr(d, "train", True)
-                self.dataloaders[k] = utils.data.DataLoader(d, shuffle=shuffle, **dataloader_kwargs)
-        objects = [self.model, self.criterion, self.optimizer, self.scheduler]
-        num_objects = len(objects)
-        dataloader_names = []
-        for name, dataloader in self.dataloaders.items():
-            dataloader_names.append(name)
-            objects.append(dataloader)
-        objects = self.prepare(*objects)
-        self.model, self.criterion, self.optimizer, self.scheduler = objects[:num_objects]
-        if len(objects) != len(dataloader_names) + num_objects:
-            raise ValueError("Number of dataloaders does not match.")
-        for name, dataloader in zip(dataloader_names, objects[num_objects:]):
-            self.dataloaders[name] = dataloader
+                dataloader_kwargs.setdefault(k, NestedDict())
+                dataloader_kwargs[k].merge(default_kwargs, overwrite=False)
+                dataloader_kwargs[k].setdefault("shuffle", getattr(d, "train", True))
+                dataloader_kwargs[k].setdefault("drop_last", not getattr(d, "train", True))
+                self.dataloaders[k] = self.prepare(utils.data.DataLoader(d, **dataloader_kwargs[k]))
+            default_kwargs.update(dataloader_kwargs)
 
     @property
     def deepspeed(self) -> dict | None:
         if "accelerator" not in self:
             raise ValueError("accelerator is not used")
         if self.accelerator.state.deepspeed_plugin is not None:
             return self.accelerator.state.deepspeed_plugin.deepspeed_config
@@ -137,37 +128,38 @@
                 result[split] = self.train_epoch(split)
             for split in eval_splits:
                 result[split] = self.evaluate_epoch(split)
             self.append_result(result)
             print(self.format_epoch_result(result))
             self.save_result()
             self.save_checkpoint()
-            """@nni.report_intermediate_result(self.latest_score)"""  # pylint: disable=W0105
+            """@nni.report_intermediate_result(self.latest_score)"""
             early_stop_counter = 0 if self.is_best else early_stop_counter + 1
             if early_stop_counter > patience:
                 print("early stop")
                 break
-        """@nni.report_final_result(self.latest_score)"""  # pylint: disable=W0105
+        """@nni.report_final_result(self.latest_score)"""
         return self.results
 
     def train_epoch(self, split: str = "train") -> NestedDict:
         r"""
         Train one epoch on `split`.
 
         Args:
             split (str): split to run train
 
         Return:
             NestedDict: train result
         """
 
-        # pylint: disable=E1101, E1102, W0622
         self.mode = "train"  # type: ignore
+        self.split = split
         loader = self.dataloaders[split]
         length = len(loader) - 1
+        last_print_iteration = -1
         self.meters.reset()
         if self.metrics is not None:
             self.metrics.reset()
         batch_time = time()
         if hasattr(loader.batch_sampler, "set_epoch"):
             loader.batch_sampler.set_epoch(self.epochs)
         if hasattr(loader.sampler, "set_epoch"):
@@ -179,26 +171,30 @@
                 target = data["target"] if isinstance(data, Mapping) else data[1]
                 pred = self.model(**input) if isinstance(input, Mapping) else self.model(input)
                 loss = self.criterion(pred, target)
                 if self.metrics is not None:
                     self.metrics.update(pred, target)
                 self.step(loss)
 
-            if self.print_interval > 0 and iteration % self.print_interval == 0:
+            if self.print_interval > 0 and (
+                iteration > 0 and iteration % self.print_interval == 0 or iteration == length
+            ):
+                interval = iteration - last_print_iteration
                 if self.device == torch.device("cuda"):
                     torch.cuda.synchronize()
-                self.meters.time.update((time() - batch_time) / self.print_interval)
+                self.meters.time.update((time() - batch_time) / interval)
                 batch_time = time()
                 reduced_loss = self.reduce(loss).item()
                 self.meters.loss.update(reduced_loss)
                 self.step_log(split, iteration, length)
+                last_print_iteration = iteration
 
-        result = self.meters.avg
+        result = self.meters.average()
         if self.metrics is not None:
-            result.merge(self.metrics.avg)
+            result.merge(self.metrics.average())
         return result
 
     def evaluate(self, eval_splits: list[str] | None = None) -> NestedDict:
         r"""
         Perform evaluation on `eval_splits`.
 
         Args:
@@ -229,43 +225,48 @@
         Args:
             split (str): split to run evaluate
 
         Return:
             NestedDict: evaluation result
         """
 
-        # pylint: disable=E1101, E1102, W0622
         self.mode = "eval"  # type: ignore
+        self.split = split
         loader = self.dataloaders[split]
         length = len(loader) - 1
+        last_print_iteration = -1
         self.meters.reset()
         if self.metrics is not None:
             self.metrics.reset()
         batch_time = time()
 
         for iteration, data in enumerate(loader):
             input = data["input"] if isinstance(data, Mapping) else data[0]
             target = data["target"] if isinstance(data, Mapping) else data[1]
             pred = self.model(**input) if isinstance(input, Mapping) else self.model(input)
             loss = self.criterion(pred, target)
             if self.metrics is not None:
                 self.metrics.update(pred, target)
 
-            if self.print_interval > 0 and iteration % self.print_interval == 0:
+            if self.print_interval > 0 and (
+                iteration > 0 and iteration % self.print_interval == 0 or iteration == length
+            ):
+                interval = iteration - last_print_iteration
                 if self.device == torch.device("cuda"):
                     torch.cuda.synchronize()
-                self.meters.time.update((time() - batch_time) / self.print_interval)
+                self.meters.time.update((time() - batch_time) / interval)
                 batch_time = time()
                 reduced_loss = self.reduce(loss).item()
                 self.meters.loss.update(reduced_loss)
                 self.step_log(split, iteration, length)
+                last_print_iteration = iteration
 
-        result = self.meters.avg
+        result = self.meters.average()
         if self.metrics is not None:
-            result.merge(self.metrics.avg)
+            result.merge(self.metrics.average())
         self.write_result(result, split, self.state.epochs)
         return result
 
     @torch.inference_mode()
     def inference(self, split: str = "inf") -> list:
         r"""
         Perform inference on `split`.
@@ -302,107 +303,29 @@
         if os.environ.get("ACCELERATE_USE_DEEPSPEED", "false").lower() == "true":
             deepspeed_config = self.state.get("deepspeed", os.environ.get("ACCELERATE_DEEPSPEED_CONFIG_FILE"))
             self.accelerate["deepspeed_plugin"] = DeepSpeedPlugin(hf_ds_config=self.init_deepspeed(deepspeed_config))
         self.accelerator = Accelerator(**self.accelerate)
         if self.distributed:
             object_list = [self.id, self.timestamp]
             dist.broadcast_object_list(object_list)
-            self.id, self.timestamp = object_list[0]
+            self.id, self.timestamp = object_list
 
     @on_main_process
     def init_tensorboard(self, *args, **kwargs) -> None:
         r"""
         Set up Tensoraoard SummaryWriter.
         """
         from torch.utils.tensorboard.writer import SummaryWriter  # pylint: disable=C0415
 
         if "log_dir" not in kwargs:
             kwargs["log_dir"] = self.dir
 
         self.writer = SummaryWriter(*args, **kwargs)
         self.writer.add_scalar = catch(OSError, verbose=False)(self.writer.add_scalar)
 
-    def init_deepspeed(self, config: dict = None) -> dict:  # type: ignore # pylint: disable=R0912,R0915
-        r"""
-        Preprocess DeepSpeed config.
-        """
-
-        if config is None:
-            config = self.state.get("deepspeed")
-        if config is None:
-            return {}
-        if isinstance(config, str):
-            config = NestedDict.load(config)
-        if config.get("steps_per_print", "auto") == "auto":
-            config["steps_per_print"] = self.print_interval
-        if config.get("train_micro_batch_size_per_gpu", "auto") == "auto":
-            config["train_micro_batch_size_per_gpu"] = self.batch_size
-        if "amp" in config:
-            amp = config["amp"]
-            if amp.get("enabled", "auto") == "auto":
-                amp["enabled"] = "true"
-            if amp.get("opt_level", "auto") == "auto":
-                amp["opt_level"] = "O1"
-        if "zero_optimization" in config:
-            zero = config["zero_optimization"]
-            if zero.get("allgather_bucket_size") == "auto":
-                zero["allgather_bucket_size"] = 1e6
-            if zero.get("reduce_bucket_size") == "auto":
-                zero["reduce_bucket_size"] = 1e6
-            if zero.get("stage3_max_live_parameters") == "auto":
-                zero["stage3_max_live_parameters"] = 1e8
-            if zero.get("stage3_max_live_gradients") == "auto":
-                zero["stage3_max_live_gradients"] = 1e8
-            if zero.get("stage3_max_reuse_distance") == "auto":
-                zero["stage3_max_reuse_distance"] = 1e8
-            if zero.get("stage3_prefetch_bucket_size") == "auto":
-                zero["stage3_prefetch_bucket_size"] = 1e6
-            if zero.get("stage3_param_persistence_threshold") == "auto":
-                zero["stage3_param_persistence_threshold"] = 1e8
-            if "amp" in config:
-                if "fp16" not in config:
-                    config["fp16"] = {}
-                if config["fp16"].get("enabled", "auto"):
-                    config["fp16"]["enabled"] = config["amp"]["enabled"]
-                warn(
-                    f"AMP is not compatible with ZeRO. Automatically set 'fp16' to {config['amp']['enabled']}",
-                    stacklevel=2,
-                )
-                del config["amp"]
-        if "optimizer" in config:
-            if "params" not in config["optimizer"]:
-                config["optimizer"]["params"] = {}
-            optimizer = config["optimizer"]["params"]
-            if optimizer.get("lr", "auto") == "auto":
-                optimizer["lr"] = self.state.get("optim.lr", 1e-3)
-            if optimizer.get("weight_decay", "auto") == "auto":
-                optimizer["weight_decay"] = self.state.get("optim.weight_decay", 1e-2)
-            if optimizer.get("betas") == "auto":
-                optimizer["betas"] = (0.9, 0.999)
-            if optimizer.get("eps") == "auto":
-                optimizer["eps"] = 1e-8
-        if "scheduler" in config:
-            if "params" not in config["scheduler"]:
-                config["scheduler"]["params"] = {}
-            scheduler = config["scheduler"]["params"]
-            if scheduler.get("total_num_steps", "auto") == "auto":
-                scheduler["total_num_steps"] = self.total_steps
-            if scheduler.get("warmup_num_steps", "auto") == "auto":
-                scheduler["warmup_num_steps"] = scheduler["total_num_steps"] // 20
-            if scheduler.get("warmup_max_lr", "auto") == "auto":
-                if self.optimizer:
-                    scheduler["warmup_max_lr"] = self.optimizer.param_groups[0]["lr"]
-                elif "optimizer" in config:
-                    scheduler["warmup_max_lr"] = config["optimizer"]["params"]["lr"]
-                else:
-                    raise ValueError("warmup_max_lr is not defined and cannot be inferred")
-            if scheduler.get("warmup_min_lr", "auto") == "auto":
-                scheduler["warmup_min_lr"] = 1e-7
-        return config
-
     def set_seed(self, seed: int | None = None, bias: int | None = None) -> None:
         r"""
         Set up random seed.
 
         Args:
             seed: Random seed to set.
                 Defaults to `self.state.seed` (`config.seed`).
@@ -449,17 +372,17 @@
         Args:
             zero_grad: Whether to zero the gradients.
         """
 
         self.accelerator.backward(loss)
         if self.sync_gradients:
             if self.state.get("max_grad_value") is not None:
-                self.clip_grad_value_(self.model.parameters(), self.state.get("max_grad_value"))  # type: ignore
+                self.clip_grad_value_(self.model.parameters(), self.state.get("max_grad_value"))
             if self.state.get("max_grad_norm") is not None:
-                self.clip_grad_norm_(self.model.parameters(), self.state.get("max_grad_norm"))  # type: ignore
+                self.clip_grad_norm_(self.model.parameters(), self.state.get("max_grad_norm"))
         if self.optimizer is not None:
             self.optimizer.step()
             if zero_grad:
                 self.optimizer.zero_grad()
         if self.scheduler is not None:
             self.scheduler.step()
         self.state.steps += 1
@@ -480,15 +403,15 @@
         return cls(
             runner=self.state.dict(),
             model=model.state_dict(),
             optimizer=self.optimizer.state_dict() if self.optimizer else None,
             scheduler=self.scheduler.state_dict() if self.scheduler else None,
         )
 
-    def prepare(self, *args, device_placement: list[bool] | None = None) -> None:
+    def prepare(self, *args: list[Any], device_placement: list[bool] | None = None) -> list[Any]:
         r"""
         Prepare all objects passed in `args` for distributed training and mixed precision,
         then return them in the same order.
         """
 
         return self.accelerator.prepare(*args, device_placement=device_placement)
 
@@ -528,27 +451,39 @@
         if self.accelerator is not None:
             return self.accelerator.unwrap_model(model)
         if self.distributed:
             return model.module
         return model
 
     @property
+    def mode(self) -> RunnerMode:
+        return self._mode
+
+    @mode.setter
+    def mode(self, mode: str | RunnerMode) -> None:
+        if isinstance(mode, str):
+            mode = RunnerMode(mode)
+        self._mode = mode
+        if self.model is not None:
+            self.model.train(mode == RunnerMode.train)
+
+    @property
     def batch_size(self) -> int:
         r"""
         Batch size.
 
         Notes:
             If `train` is in `dataloaders`, then `batch_size` is the batch size of `train`.
             Otherwise, `batch_size` is the batch size of the first dataloader.
 
         Returns:
             (int):
         """
 
-        batch_size = self.state.get("batch_size")
+        batch_size = self.state.get("dataloader.batch_size")
         if batch_size:
             return batch_size
         if self.dataloaders:
             loader = self.dataloaders.get("train", next(iter(self.dataloaders.values())))
             if loader.batch_size:
                 return loader.batch_size
             batch_sampler = loader.batch_sampler if loader.batch_sampler is not None else loader.sampler
@@ -563,15 +498,15 @@
         Returns:
             (int):
         """
 
         return self.accelerator.gradient_accumulation_steps
 
     @property
-    def device(self) -> torch.device:  # pylint: disable=E1101
+    def device(self) -> torch.device:
         r"""
         Device of runner.
         """
 
         return self.accelerator.device
 
     @property
```

### Comparing `danling-0.3.3/danling/runner/base_runner.py` & `danling-0.3.4/danling/runner/base_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,16 @@
     Attributes: Data:
         datasets (FlatDict): All datasets, should be in the form of ``{subset: dataset}``.
             Initialised to `FlatDict` by default.
         datasamplers (FlatDict): All datasamplers, should be in the form of ``{subset: datasampler}``.
             Initialised to `FlatDict` by default.
         dataloaders (FlatDict): All dataloaders, should be in the form of ``{subset: dataloader}``.
             Initialised to `FlatDict` by default.
-        batch_size (int, property): Number of samples per batch in train dataloader or the first dataloader.
+        split (str): Current running split.
+        batch_size (int, property): Number of samples per batch in current running split.
         batch_size_equivalent (int, property): Total batch_size (`batch_size * world_size * accum_steps`).
 
     `datasets`, `datasamplers`, `dataloaders` should be a dict with the same keys.
     Their keys should be `split` (e.g. `train`, `val`, `test`).
 
     Attributes: Progress:
         progress (float, property): Running Progress, in `range(0, 1)`.
@@ -90,14 +91,37 @@
         best_score (float, property): Best score, should be in the form of `score`.
         score_set (Optional[str]): The subset to calculate the score.
             If is `None`, will use the last set of the result.
         score_name (str): The metric name of score.
             Defaults to `"loss"`.
         is_best (bool, property): If `latest_score == best_score`.
 
+    A `result` is a dict with the same `split` as keys, like `dataloaders`.
+    A typical `result` shall look like this:
+    ```python
+    {
+        "train": {
+            "loss": 0.1,
+            "accuracy": 0.9,
+        },
+        "val": {
+            "loss": 0.2,
+            "accuracy": 0.8,
+        },
+        "test": {
+            "loss": 0.3,
+            "accuracy": 0.7,
+        },
+    }
+    ```
+
+    `scores` are dynamically extracted from `results` by `score_set` and `score_name`.
+    They represent the core metric that is used in comparing the performance against different models and settings.
+    For the above `results`, If `score_set = "val"`, `score_name = "accuracy"`, then `scores = 0.9`.
+
     Attributes: IO:
         dir (str, property): Directory of the run.
             Defaults to `${self.project_root}/${self.name}-${self.id}/${self.timestamp})`.
         checkpoint_dir (str, property): Directory of checkpoints.
         log_path (str, property):  Path of log file.
         checkpoint_dir_name (str): The name of the directory under `runner.dir` to save checkpoints.
             Defaults to `"checkpoints"`.
@@ -123,556 +147,66 @@
     """
 
     # DO NOT set default value in class, as they won't be stored in `__dict__`.
 
     timestamp: str
 
     _mode: RunnerMode
-    state: RunnerState
+    _state: RunnerState
+    inited: bool = False
 
     model: Callable | None = None
     criterion: Callable | None = None
     optimizer: Any | None = None
     scheduler: Any | None = None
 
     datasets: FlatDict
     datasamplers: FlatDict
     dataloaders: FlatDict
+    split: str
 
+    results: NestedDict
     meters: AverageMeters
     metrics: Metrics | None = None
     logger: logging.Logger | None = None
     writer: Any | None = None
 
     def __init__(self, config: NestedDict) -> None:
         self.timestamp = get_time_str()
         if "datasets" not in self.__dict__:
             self.datasets = FlatDict()
         if "datasamplers" not in self.__dict__:
             self.datasamplers = FlatDict()
         if "dataloaders" not in self.__dict__:
             self.dataloaders = FlatDict()
-        self._mode = RunnerMode.train  # type: ignore[assignment]
+        if "results" not in self.__dict__:
+            self.results = NestedDict()
         self.meters = AverageMeters()
-        self.metrics = None
-        # must init state at last to avoid conflict names
-        self.state = RunnerState(config)
+        self._mode = RunnerMode.train  # type: ignore[assignment]
+        # must init state at last to avoid name conflicts
+        self._state = RunnerState(config)
+        self.inited = True
         self.init_distributed()
         if self.state.seed is not None:
             self.set_seed()
         if self.state.deterministic:
             self.set_deterministic()
         if self.state.log:
             self.init_logging()
         self.init_print()
         if self.state.tensorboard:
             self.init_tensorboard()
 
-    def __post_init__(self, *args, **kwargs) -> None:
-        pass
-
-    @property
-    def mode(self) -> RunnerMode:
-        return self._mode
-
-    @mode.setter
-    def mode(self, mode: str | RunnerMode) -> None:
-        if isinstance(mode, str):
-            mode = RunnerMode(mode)
-        self._mode = mode
-
-    @cached_property
-    def batch_size(self) -> int:
-        r"""
-        Batch size.
-
-        Notes:
-            If `train` is in `dataloaders`, then `batch_size` is the batch size of `train`.
-            Otherwise, `batch_size` is the batch size of the first dataloader.
-
-        Returns:
-            (int):
-        """
-
-        batch_size = self.state.get("dataloader.batch_size")
-        if batch_size:
-            return batch_size
-        if self.dataloaders:
-            loader = self.dataloaders["train"] if "train" in self.dataloaders else next(iter(self.dataloaders.values()))
-            return loader.batch_size
-        raise AttributeError("batch_size could not be inferred, since no dataloader found.")
-
-    @property
-    def batch_size_equivalent(self) -> int:
-        r"""
-        Actual batch size.
-
-        Returns:
-            (int): `batch_size` * `world_size` * `accum_steps`
-        """
-
-        return self.batch_size * self.world_size * self.accum_steps
-
-    @cached_property
-    def total_epochs(self) -> int:
-        if self.state.epoch_end:
-            return self.state.epoch_end - self.state.epoch_begin
-        raise ValueError("epoch_end is not specified")
-
-    @cached_property
-    def total_steps(self) -> int:
-        if self.state.step_end:
-            return self.state.step_end - self.state.step_begin
-        dataset = self.datasets.get("train", next(iter(self.datasets.values())))
-        return self.total_epochs * ceil(len(dataset) / self.batch_size)
-
-    @cached_property
-    def accum_steps(self) -> int:
-        r"""
-        Accumulated steps.
-
-        Returns:
-            (int):
-        """
-
-        return self.state.get("accum_steps", 1)
-
     def init_distributed(self) -> None:
         r"""
         Initialise distributed running environment.
         """
 
         raise NotImplementedError
 
-    @property
-    def device(self) -> Any:
-        r"""
-        Device of runner.
-        """
-
-        return "cpu"
-
-    @property
-    def world_size(self) -> int:
-        r"""
-        Number of processes.
-        """
-
-        return 1
-
-    @property
-    def rank(self) -> int:
-        r"""
-        Process index of all processes.
-        """
-
-        return 0
-
-    @property
-    def local_rank(self) -> int:
-        r"""
-        Process index of local processes.
-        """
-
-        return 0
-
-    @property
-    def distributed(self) -> bool:
-        r"""
-        If runner is running in distributed mode.
-        """
-
-        return self.world_size > 1
-
-    @property
-    def is_main_process(self) -> bool:
-        r"""
-        If current process is the main process of all processes.
-        """
-
-        return self.rank == 0
-
-    @property
-    def is_local_main_process(self) -> bool:
-        r"""
-        If current process is the main process of local processes.
-        """
-
-        return self.local_rank == 0
-
-    @catch
-    def save(self, obj: Any, file: PathStr, main_process_only: bool = True, *args, **kwargs) -> File:
-        r"""
-        Save any file with supported extensions.
-
-        `Runner.save` internally calls `dl.save`,
-        but with additional arguments to allow it save only on the main process.
-        Moreover, any error raised by `Runner.save` will be caught and logged.
-        """
-
-        if main_process_only and self.is_main_process or not main_process_only:
-            return save(obj, file, *args, **kwargs)
-        return file
-
-    @staticmethod
-    def load(file: PathStr, *args, **kwargs) -> Any:
-        r"""
-        Load any file with supported extensions.
-
-        `Runner.load` is identical to `dl.load`.
-        """
-
-        return load(file, *args, **kwargs)
-
-    def dict(self, cls: Callable = dict) -> Mapping:
-        r"""
-        Convert state to Mapping.
-
-        Args:
-            cls: Target `clc to convert to.
-        """
-
-        return self.state.dict(cls)
-
-    @catch
-    def json(self, file: File, main_process_only: bool = True, *args, **kwargs) -> None:  # pylint: disable=R1710
-        r"""
-        Dump Runner State to json file.
-        """
-
-        if main_process_only and self.is_main_process or not main_process_only:
-            return self.state.json(file, *args, **kwargs)
-
-    @classmethod
-    def from_json(cls, file: File, *args, **kwargs) -> BaseRunner:
-        r"""
-        Construct Runner from json file.
-
-        This function calls `self.from_jsons()` to construct object from json string.
-        You may overwrite `from_jsons` in case something is not json serializable.
-        """
-
-        with FlatDict.open(file) as fp:
-            return cls.from_jsons(fp.read(), *args, **kwargs)
-
-    def jsons(self, *args, **kwargs) -> str:
-        r"""
-        Dump Runner State to json string.
-        """
-
-        return self.state.jsons(*args, **kwargs)
-
-    @classmethod
-    def from_jsons(cls, string: str, *args, **kwargs) -> BaseRunner:
-        r"""
-        Construct Runner from json string.
-        """
-
-        return cls(Config.from_jsons(string, *args, **kwargs))
-
-    @catch
-    def yaml(self, file: File, main_process_only: bool = True, *args, **kwargs) -> None:  # pylint: disable=R1710
-        r"""
-        Dump Runner State to yaml file.
-        """
-
-        if main_process_only and self.is_main_process or not main_process_only:
-            return self.state.yaml(file, *args, **kwargs)
-
-    @classmethod
-    def from_yaml(cls, file: File, *args, **kwargs) -> BaseRunner:
-        r"""
-        Construct Runner from yaml file.
-
-        This function calls `self.from_yamls()` to construct object from yaml string.
-        You may overwrite `from_yamls` in case something is not yaml serializable.
-        """
-
-        with FlatDict.open(file) as fp:
-            return cls.from_yamls(fp.read(), *args, **kwargs)
-
-    def yamls(self, *args, **kwargs) -> str:
-        r"""
-        Dump Runner State to yaml string.
-        """
-
-        return self.state.yamls(*args, **kwargs)
-
-    @classmethod
-    def from_yamls(cls, string: str, *args, **kwargs) -> BaseRunner:
-        r"""
-        Construct Runner from yaml string.
-        """
-
-        return cls(Config.from_yamls(string, *args, **kwargs))
-
-    @property
-    def progress(self) -> float:
-        r"""
-        Training Progress.
-
-        Returns:
-            (float):
-
-        Raises:
-            RuntimeError: If no terminal is defined.
-        """
-
-        return self.steps / self.total_steps
-
-    @property
-    def best_fn(self) -> Callable:
-        r"""
-        Function to determine the best score from a list of scores.
-
-        By default, the `best_fn` returns `min` if `self.state.score_name` is `loss`,
-        otherwise, returns `max`.
-
-        Subclass can override this method to accommodate needs, such as `min`.
-
-        Returns:
-            (callable):
-        """
-
-        return max if self.state.score_name != "loss" else min
-
-    @property
-    def best_index(self) -> int:
-        r"""
-        Find the best index from all scores.
-
-        Returns:
-            (int):
-        """
-
-        if not self.scores:
-            return 0
-        values = list(self.scores.values())
-        return self.best_fn(range(len(values)), key=values.__getitem__)
-
-    @property
-    def latest_result(self) -> NestedDict | None:
-        r"""
-        Latest result.
-        """
-
-        if not self.state.results:
-            return None
-        latest_index = next(reversed(self.state.results if PY38_PLUS else list(self.state.results)))  # type: ignore
-        ret = self.state.results[latest_index].clone()
-        ret["index"] = latest_index
-        return ret
-
-    @property
-    def best_result(self) -> NestedDict | None:
-        r"""
-        Best result.
-        """
-
-        if not self.state.results:
-            return None
-        best_index = self.best_index
-        ret = self.state.results[best_index].clone()
-        ret["index"] = best_index
-        return ret
-
-    @property
-    def scores(self) -> FlatDict | None:
-        r"""
-        All scores.
-
-        Scores are extracted from results by `score_set` and `runner.state.score_name`,
-        following `[r[score_set][self.state.score_name] for r in self.state.results]`.
-
-        Scores are considered as the index of the performance of the model.
-        It is useful to determine the best model and the best hyper-parameters.
-
-        `score_set` is defined in `self.state.score_set`.
-        If it is not set, `DanLing` will use `val` or `validate` if they appear in the `latest_result`.
-        If `DanLing` still could not find, it will fall back to the second key in the `latest_result`
-        if it contains more that one element, or the first key.
-
-        Note that certain keys are ignored when falling back, they are defined in {IGNORED_SET_NAMES}.
-        """
-
-        if not self.state.results:
-            return None
-        subsets = [i for i in self.latest_result.keys() if i not in IGNORED_SET_NAMES]  # type: ignore
-        score_set = self.state.get("score_set")
-        if score_set is None and "val" in subsets:
-            score_set = "val"
-        if score_set is None and "validate" in subsets:
-            score_set = "validate"
-        if score_set is None:
-            score_set = subsets[1] if len(subsets) > 1 else subsets[0]
-        return FlatDict({k: v[score_set][self.state.score_name] for k, v in self.state.results.items()})
-
-    @property
-    def latest_score(self) -> float | None:
-        r"""
-        Latest score.
-        """
-
-        if not self.state.results:
-            return None
-        if not PY38_PLUS:
-            return next(reversed(list(self.scores.values())))  # type: ignore
-        return next(reversed(self.scores.values()))  # type: ignore
-
-    @property
-    def best_score(self) -> float | None:
-        r"""
-        Best score.
-        """
-
-        if not self.state.results:
-            return None
-        return self.scores[self.best_index]  # type: ignore
-
-    @property
-    def is_best(self) -> bool:
-        r"""
-        If current epoch is the best epoch.
-        """
-
-        if not self.state.results:
-            return True
-        try:
-            return abs(self.latest_score - self.best_score) < 1e-7  # type: ignore
-        except TypeError:
-            return True
-
-    @property
-    @ensure_dir
-    def dir(self) -> str:
-        r"""
-        Directory of the run.
-        """
-
-        if "dir" in self.state:
-            return self.state.dir
-        return os.path.join(self.project_root, f"{self.name}-{self.id}", self.timestamp)
-
-    @cached_property
-    def log_path(self) -> str:
-        r"""
-        Path of log file.
-        """
-
-        if "log_path" in self.state:
-            return self.state.log_path
-        return os.path.join(self.dir, "run.log")
-
-    @property
-    @ensure_dir
-    def checkpoint_dir(self) -> str:
-        r"""
-        Directory of checkpoints.
-        """
-
-        if "checkpoint_dir" in self.state:
-            return self.state.checkpoint_dir
-        return os.path.join(self.dir, self.checkpoint_dir_name)
-
-    # def __getattribute__(self, name) -> Any:
-    #     if name in ("__class__", "__dict__"):
-    #         return super().__getattribute__(name)
-    #     if name in self.__dict__:
-    #         return self.__dict__[name]
-    #     if name in dir(self):
-    #         return super().__getattribute__(name)
-    #     if "state" in self and name in self.state:
-    #         return self.state[name]
-    #     return super().__getattribute__(name)
-
-    def __getattr__(self, name) -> Any:
-        if "state" in self:
-            if name in self.state:
-                return self.state[name]
-            if name in dir(self.state):
-                return getattr(self.state, name)
-        return super().__getattribute__(name)
-
-    def __setattr__(self, name, value) -> None:
-        if name in self.__dict__:
-            if isinstance(self.__dict__[name], Variable):
-                self.__dict__[name].set(value)
-            else:
-                self.__dict__[name] = value
-            return
-        if name in dir(self):
-            if isinstance(super().__getattribute__(name), Variable):
-                super().__getattribute__(name).set(value)
-            else:
-                object.__setattr__(self, name, value)
-            return
-        if "state" in self:
-            if name in self.state:
-                if isinstance(self.state[name], Variable):
-                    self.state[name].set(value)
-                else:
-                    self.state[name] = value
-                return
-            if name in dir(self.state):
-                setattr(self.state, name, value)
-                return
-        object.__setattr__(self, name, value)
-
-    def __contains__(self, name) -> bool:
-        return name in dir(self) or ("state" in self.__dict__ and name in dir(self.state))
-
-    def __repr__(self):
-        lines = []
-        for key, value in self.__dict__.items():
-            value_str = repr(value)
-            value_str = self._add_indent(value_str)
-            lines.append("(" + key + "): " + value_str)
-
-        main_str = self.__class__.__name__ + "("
-        if lines:
-            main_str += "\n  " + "\n  ".join(lines) + "\n"
-
-        main_str += ")"
-        return main_str
-
-    def _add_indent(self, text):
-        lines = text.split("\n")
-        # don't do anything for single-line stuff
-        if len(lines) == 1:
-            return text
-        first = lines.pop(0)
-        # add 2 spaces to each line but the first
-        lines = [(2 * " ") + line for line in lines]
-        lines = "\n".join(lines)
-        lines = first + "\n" + lines
-        return lines
-
-    def check_dir(self, action: str = "warn") -> bool:
-        r"""
-        Check if `self.dir` is not empty.
-
-        Args:
-            action (str): The action to perform if `self.dir` is not empty.
-            Can be one of ("warn", "raise", "ignore"), default is "warn".
-        """
-
-        if action and action not in ("warn", "raise", "ignore"):
-            raise ValueError(f"Directory `{self.dir}`")
-        if os.listdir(self.dir):
-            if action == "warn":
-                warn(
-                    f"Directory `{self.dir}` is not empty",
-                    category=RuntimeWarning,
-                    stacklevel=2,
-                )
-            if action == "raise":
-                raise RuntimeError(f"Directory `{self.dir}` is not empty")
-            return False
-        return True
-
     def init_deepspeed(  # pylint: disable=too-many-branches, too-many-statements
         self, config: Dict = None  # type: ignore
     ) -> Dict:
         r"""
         Preprocess DeepSpeed config.
         """
 
@@ -905,14 +439,143 @@
     def state_dict(self, cls: Callable = dict) -> Mapping:
         r"""
         Return dict of all attributes for checkpoint.
         """
 
         return cls(self.state)
 
+    def dict(self, cls: Callable = dict) -> Mapping:
+        r"""
+        Convert state to Mapping.
+
+        Args:
+            cls: Target `clc to convert to.
+        """
+
+        return self.state.dict(cls)
+
+    @catch
+    def save(self, obj: Any, file: PathStr, main_process_only: bool = True, *args, **kwargs) -> File:
+        r"""
+        Save any file with supported extensions.
+
+        `Runner.save` internally calls `dl.save`,
+        but with additional arguments to allow it save only on the main process.
+        Moreover, any error raised by `Runner.save` will be caught and logged.
+        """
+
+        if main_process_only and self.is_main_process or not main_process_only:
+            return save(obj, file, *args, **kwargs)
+        return file
+
+    @staticmethod
+    def load(file: PathStr, *args, **kwargs) -> Any:
+        r"""
+        Load any file with supported extensions.
+
+        `Runner.load` is identical to `dl.load`.
+        """
+
+        return load(file, *args, **kwargs)
+
+    @catch
+    def json(self, file: File, main_process_only: bool = True, *args, **kwargs) -> None:  # pylint: disable=R1710
+        r"""
+        Dump Runner State to json file.
+        """
+
+        if main_process_only and self.is_main_process or not main_process_only:
+            return self.state.json(file, *args, **kwargs)
+
+    @classmethod
+    def from_json(cls, file: File, *args, **kwargs) -> BaseRunner:
+        r"""
+        Construct Runner from json file.
+
+        This function calls `self.from_jsons()` to construct object from json string.
+        You may overwrite `from_jsons` in case something is not json serializable.
+        """
+
+        with FlatDict.open(file) as fp:
+            return cls.from_jsons(fp.read(), *args, **kwargs)
+
+    def jsons(self, *args, **kwargs) -> str:
+        r"""
+        Dump Runner State to json string.
+        """
+
+        return self.state.jsons(*args, **kwargs)
+
+    @classmethod
+    def from_jsons(cls, string: str, *args, **kwargs) -> BaseRunner:
+        r"""
+        Construct Runner from json string.
+        """
+
+        return cls(Config.from_jsons(string, *args, **kwargs))
+
+    @catch
+    def yaml(self, file: File, main_process_only: bool = True, *args, **kwargs) -> None:  # pylint: disable=R1710
+        r"""
+        Dump Runner State to yaml file.
+        """
+
+        if main_process_only and self.is_main_process or not main_process_only:
+            return self.state.yaml(file, *args, **kwargs)
+
+    @classmethod
+    def from_yaml(cls, file: File, *args, **kwargs) -> BaseRunner:
+        r"""
+        Construct Runner from yaml file.
+
+        This function calls `self.from_yamls()` to construct object from yaml string.
+        You may overwrite `from_yamls` in case something is not yaml serializable.
+        """
+
+        with FlatDict.open(file) as fp:
+            return cls.from_yamls(fp.read(), *args, **kwargs)
+
+    def yamls(self, *args, **kwargs) -> str:
+        r"""
+        Dump Runner State to yaml string.
+        """
+
+        return self.state.yamls(*args, **kwargs)
+
+    @classmethod
+    def from_yamls(cls, string: str, *args, **kwargs) -> BaseRunner:
+        r"""
+        Construct Runner from yaml string.
+        """
+
+        return cls(Config.from_yamls(string, *args, **kwargs))
+
+    def check_dir(self, action: str = "warn") -> bool:
+        r"""
+        Check if `self.dir` is not empty.
+
+        Args:
+            action (str): The action to perform if `self.dir` is not empty.
+            Can be one of ("warn", "raise", "ignore"), default is "warn".
+        """
+
+        if action and action not in ("warn", "raise", "ignore"):
+            raise ValueError(f"action should be one of warn, raise or ignore, but got {action}")
+        if os.listdir(self.dir):
+            if action == "warn":
+                warn(
+                    f"Directory `{self.dir}` is not empty",
+                    category=RuntimeWarning,
+                    stacklevel=2,
+                )
+            if action == "raise":
+                raise RuntimeError(f"Directory `{self.dir}` is not empty")
+            return False
+        return True
+
     @catch
     @on_main_process
     def save_checkpoint(self) -> None:
         r"""
         Save checkpoint to `self.checkpoint_dir`.
 
         The checkpoint will be saved to `self.checkpoint_dir/latest.pth`.
@@ -975,21 +638,21 @@
                 warn(
                     "latest checkpoint is preempted by value specified in checkpoint",
                     RuntimeWarning,
                     stacklevel=2,
                 )
             if isinstance(checkpoint, (bytes, str, os.PathLike)):
                 if not os.path.exists(checkpoint):
-                    raise FileNotFoundError(f"checkpoint is set to {checkpoint!r} but does not exist.")
+                    raise FileNotFoundError(f"checkpoint is set to {checkpoint!r} but does not exist")
                 self.state.checkpoint = checkpoint
                 ckpt = self.load(checkpoint, *args, **kwargs)
             elif isinstance(checkpoint, Mapping):
                 ckpt = checkpoint
             else:
-                raise ValueError(f"pretrained is set to {checkpoint!r} but is not a valid checkpoint.")
+                raise ValueError(f"pretrained is set to {checkpoint!r} but is not a valid checkpoint")
         elif auto_resume:
             checkpoint = os.path.join(self.checkpoint_dir, "latest.pth")
             if os.path.exists(checkpoint):
                 self.state.checkpoint = checkpoint
                 ckpt = self.load(checkpoint, *args, **kwargs)
             else:
                 warn("latest checkpoint does not exits", category=RuntimeWarning, stacklevel=2)
@@ -1025,15 +688,15 @@
         """
 
         if isinstance(checkpoint, (bytes, str, os.PathLike)):
             ckpt = cls.load(checkpoint, *args, **kwargs)
         elif isinstance(checkpoint, Mapping):
             ckpt = checkpoint
         else:
-            raise ValueError(f"checkpoint is set to {checkpoint} but is not a valid checkpoint.")
+            raise ValueError(f"checkpoint is set to {checkpoint} but is not a valid checkpoint")
         runner = cls(**ckpt["runner"])
         runner.load_checkpoint(ckpt, override_state=False)
         return runner
 
     def load_pretrained(self, checkpoint: Mapping | bytes | str | os.PathLike | None = None, *args, **kwargs) -> None:
         """
         Load parameters from pretrained checkpoint.
@@ -1055,31 +718,32 @@
 
         # TODO: Support loading checkpoints in other format
         checkpoint = checkpoint if checkpoint is not None else self.state.get("pretrained")
         if checkpoint is None:
             raise ValueError("pretrained is not specified")
         if isinstance(checkpoint, (bytes, str, os.PathLike)):
             if not os.path.exists(checkpoint):
-                raise FileNotFoundError(f"pretrained is set to {checkpoint!r} but does not exist.")
+                raise FileNotFoundError(f"pretrained is set to {checkpoint!r} but does not exist")
             ckpt = self.load(checkpoint, *args, **kwargs)
         elif isinstance(checkpoint, Mapping):
             ckpt = checkpoint
         else:
-            raise ValueError(f"pretrained is set to {checkpoint!r} but is not a valid checkpoint.")
-        ckpt = ckpt.get("model", ckpt)
-        ckpt = ckpt.get("state_dict", ckpt)
-        model = self.unwrap_model(self.model)
-        model.load_state_dict(ckpt)
+            raise ValueError(f"pretrained is set to {checkpoint!r} but is not a valid checkpoint")
+        if self.model is not None and "model" in ckpt:
+            model = self.unwrap_model(self.model)
+            model.load_state_dict(ckpt["model"])
+        else:
+            raise ValueError(f"Unable to find model weights in {checkpoint!r}")
 
     def append_result(self, result: NestedDict, index: int | None = None) -> None:
         r"""
-        Append result to `self.state.results`.
+        Append result to `self.results`.
 
         Warnings:
-            `self.state.results` is heavily relied upon for computing metrics.
+            `self.results` is heavily relied upon for computing metrics.
 
             Failed to use this method may lead to unexpected behavior.
         """
 
         if index is None:
             index = self.state.epochs
             global __APPEND_RESULT_COUNTER__  # pylint: disable=global-statement
@@ -1089,25 +753,25 @@
                     """
                     Automatically set index to `self.state.epochs`.
                     Please ensure `self.state.epochs` updates before calling `append_result`
                     """,
                     category=RuntimeWarning,
                     stacklevel=2,
                 )
-        if index in self.state.results:
-            self.state.results[index].merge(result)
+        if index in self.results:
+            self.results[index].merge(result)
         else:
-            self.state.results[index] = result
+            self.results[index] = result
 
     def print_result(self) -> None:
         r"""
         Print latest and best result.
         """
 
-        print(f"results: {self.state.results}")
+        print(f"results: {self.results}")
         print(f"latest result: {self.latest_result}")
         print(f"best result: {self.best_result}")
 
     def step_log(self, split: str, iteration: int, length: int | None = None):
         if length is None:
             length = len(self.dataloaders[split]) - 1
         result = self.meters.val
@@ -1171,23 +835,23 @@
         This method will save latest and best result to
         `self.dir/latest.json` and `self.dir/best.json` respectively.
         """
 
         results_path = os.path.join(self.dir, "results.json")
         self.save(
             {
-                "id": self.id,
                 "name": self.name,
+                "id": self.id,
                 "timestamp": self.timestamp,
-                "results": self.state.results,
+                "results": self.results,
             },
             results_path,
             indent=4,
         )
-        ret = {"id": self.id, "name": self.name, "timestamp": self.timestamp}
+        ret = {"name": self.name, "id": self.id, "timestamp": self.timestamp}
         result = self.latest_result
         if isinstance(result, FlatDict):
             result = result.dict()
         # This is slower but ensure id is the first key
         if result is not None:
             ret.update(result)
         latest_path = os.path.join(self.dir, "latest.json")
@@ -1207,7 +871,373 @@
     @cached_property
     def uuid(self) -> UUID:
         r"""
         UUID of the state.
         """
 
         return uuid5(self.run_uuid, self.id)
+
+    @property
+    def mode(self) -> RunnerMode:
+        return self._mode
+
+    @mode.setter
+    def mode(self, mode: str | RunnerMode) -> None:
+        if isinstance(mode, str):
+            mode = RunnerMode(mode)
+        self._mode = mode
+
+    @property
+    def state(self) -> RunnerState:
+        return self._state
+
+    @property
+    def batch_size(self) -> int:
+        r"""
+        Batch size.
+
+        Notes:
+            If `train` is in `dataloaders`, then `batch_size` is the batch size of `train`.
+            Otherwise, `batch_size` is the batch size of the first dataloader.
+
+        Returns:
+            (int):
+        """
+
+        if self.dataloaders and self.split:
+            return self.dataloaders[self.split].batch_size
+        batch_size = self.state.get("dataloader.batch_size")
+        if batch_size:
+            return batch_size
+        raise AttributeError("batch_size could not be inferred and is not in config")
+
+    @property
+    def batch_size_equivalent(self) -> int:
+        r"""
+        Actual batch size.
+
+        Returns:
+            (int): `batch_size` * `world_size` * `accum_steps`
+        """
+
+        return self.batch_size * self.world_size * self.accum_steps
+
+    @cached_property
+    def total_epochs(self) -> int:
+        if self.state.epoch_end:
+            return self.state.epoch_end - self.state.epoch_begin + 1
+        raise ValueError("epoch_end is not specified")
+
+    @cached_property
+    def total_steps(self) -> int:
+        if self.state.step_end:
+            return self.state.step_end - self.state.step_begin
+        dataset = self.datasets.get("train", next(iter(self.datasets.values())))
+        return self.total_epochs * ceil(len(dataset) / self.batch_size) + 1
+
+    @cached_property
+    def accum_steps(self) -> int:
+        r"""
+        Accumulated steps.
+
+        Returns:
+            (int):
+        """
+
+        return self.state.get("accum_steps", 1)
+
+    @property
+    def progress(self) -> float:
+        r"""
+        Training Progress.
+
+        Returns:
+            (float):
+
+        Raises:
+            RuntimeError: If no terminal is defined.
+        """
+
+        return self.steps / self.total_steps
+
+    @property
+    def device(self) -> Any:
+        r"""
+        Device of runner.
+        """
+
+        return "cpu"
+
+    @property
+    def world_size(self) -> int:
+        r"""
+        Number of processes.
+        """
+
+        return 1
+
+    @property
+    def rank(self) -> int:
+        r"""
+        Process index of all processes.
+        """
+
+        return 0
+
+    @property
+    def local_rank(self) -> int:
+        r"""
+        Process index of local processes.
+        """
+
+        return 0
+
+    @property
+    def distributed(self) -> bool:
+        r"""
+        If runner is running in distributed mode.
+        """
+
+        return self.world_size > 1
+
+    @property
+    def is_main_process(self) -> bool:
+        r"""
+        If current process is the main process of all processes.
+        """
+
+        return self.rank == 0
+
+    @property
+    def is_local_main_process(self) -> bool:
+        r"""
+        If current process is the main process of local processes.
+        """
+
+        return self.local_rank == 0
+
+    @property
+    def best_fn(self) -> Callable:
+        r"""
+        Function to determine the best score from a list of scores.
+
+        By default, the `best_fn` returns `min` if `self.state.score_name` is `loss`,
+        otherwise, returns `max`.
+
+        Subclass can override this method to accommodate needs, such as `min`.
+
+        Returns:
+            (callable):
+        """
+
+        return max if self.state.score_name != "loss" else min
+
+    @property
+    def best_index(self) -> int:
+        r"""
+        Find the best index from all scores.
+
+        Returns:
+            (int):
+        """
+
+        if not self.scores:
+            return 0
+        values = list(self.scores.values())
+        return self.best_fn(range(len(values)), key=values.__getitem__)
+
+    @property
+    def latest_result(self) -> NestedDict | None:
+        r"""
+        Latest result.
+        """
+
+        if not self.results:
+            return None
+        latest_index = next(reversed(self.results if PY38_PLUS else list(self.results)))  # type: ignore
+        ret = self.results[latest_index].clone()
+        ret["index"] = latest_index
+        return ret
+
+    @property
+    def best_result(self) -> NestedDict | None:
+        r"""
+        Best result.
+        """
+
+        if not self.results:
+            return None
+        best_index = self.best_index
+        ret = self.results[best_index].clone()
+        ret["index"] = best_index
+        return ret
+
+    @property
+    def scores(self) -> FlatDict | None:
+        r"""
+        All scores.
+
+        Scores are extracted from results by `score_set` and `runner.state.score_name`,
+        following `[r[score_set][self.state.score_name] for r in self.results]`.
+
+        Scores are considered as the index of the performance of the model.
+        It is useful to determine the best model and the best hyper-parameters.
+
+        `score_set` is defined in `self.state.score_set`.
+        If it is not set, `DanLing` will use `val` or `validate` if they appear in the `latest_result`.
+        If `DanLing` still could not find, it will fall back to the second key in the `latest_result`
+        if it contains more that one element, or the first key.
+
+        Note that certain keys are ignored when falling back, they are defined in {IGNORED_SET_NAMES}.
+        """
+
+        if not self.results:
+            return None
+        subsets = [i for i in self.latest_result.keys() if i not in IGNORED_SET_NAMES]  # type: ignore
+        score_set = self.state.get("score_set")
+        if score_set is None and "val" in subsets:
+            score_set = "val"
+        if score_set is None and "validate" in subsets:
+            score_set = "validate"
+        if score_set is None:
+            score_set = subsets[1] if len(subsets) > 1 else subsets[0]
+        return FlatDict({k: v[score_set][self.state.score_name] for k, v in self.results.items()})
+
+    @property
+    def latest_score(self) -> float | None:
+        r"""
+        Latest score.
+        """
+
+        if not self.results:
+            return None
+        if not PY38_PLUS:
+            return next(reversed(list(self.scores.values())))  # type: ignore
+        return next(reversed(self.scores.values()))  # type: ignore
+
+    @property
+    def best_score(self) -> float | None:
+        r"""
+        Best score.
+        """
+
+        if not self.results:
+            return None
+        return self.scores[self.best_index]  # type: ignore
+
+    @property
+    def is_best(self) -> bool:
+        r"""
+        If current epoch is the best epoch.
+        """
+
+        if not self.results:
+            return True
+        try:
+            return abs(self.latest_score - self.best_score) < 1e-7  # type: ignore
+        except TypeError:
+            return True
+
+    @property
+    @ensure_dir
+    def dir(self) -> str:
+        r"""
+        Directory of the run.
+        """
+
+        if "dir" in self.state:
+            return self.state.dir
+        return os.path.join(self.project_root, f"{self.name}-{self.id}", self.timestamp)
+
+    @cached_property
+    def log_path(self) -> str:
+        r"""
+        Path of log file.
+        """
+
+        if "log_path" in self.state:
+            return self.state.log_path
+        return os.path.join(self.dir, "run.log")
+
+    @property
+    @ensure_dir
+    def checkpoint_dir(self) -> str:
+        r"""
+        Directory of checkpoints.
+        """
+
+        if "checkpoint_dir" in self.state:
+            return self.state.checkpoint_dir
+        return os.path.join(self.dir, self.checkpoint_dir_name)
+
+    # def __getattribute__(self, name) -> Any:
+    #     if name in ("__class__", "__dict__"):
+    #         return super().__getattribute__(name)
+    #     if name in self.__dict__:
+    #         return self.__dict__[name]
+    #     if name in dir(self):
+    #         return super().__getattribute__(name)
+    #     if "state" in self and name in self.state:
+    #         return self.state[name]
+    #     return super().__getattribute__(name)
+
+    def __getattr__(self, name) -> Any:
+        if self.inited:
+            if name in self._state:
+                return self.state[name]
+            if name in dir(self.state):
+                return getattr(self.state, name)
+        return super().__getattribute__(name)
+
+    def __setattr__(self, name, value) -> None:
+        if name in self.__dict__:
+            if isinstance(self.__dict__[name], Variable):
+                self.__dict__[name].set(value)
+            else:
+                self.__dict__[name] = value
+            return
+        if name in dir(self):
+            if isinstance(super().__getattribute__(name), Variable):
+                super().__getattribute__(name).set(value)
+            else:
+                object.__setattr__(self, name, value)
+            return
+        if self.inited:
+            if name in self.state:
+                if isinstance(self.state[name], Variable):
+                    self.state[name].set(value)
+                else:
+                    self.state[name] = value
+                return
+            if name in dir(self.state):
+                setattr(self.state, name, value)
+                return
+        object.__setattr__(self, name, value)
+
+    def __contains__(self, name) -> bool:
+        return name in dir(self) or ("state" in self.__dict__ and name in dir(self.state))
+
+    def __repr__(self):
+        lines = []
+        for key, value in self.__dict__.items():
+            value_str = repr(value)
+            value_str = self._add_indent(value_str)
+            lines.append("(" + key + "): " + value_str)
+
+        main_str = self.__class__.__name__ + "("
+        if lines:
+            main_str += "\n  " + "\n  ".join(lines) + "\n"
+
+        main_str += ")"
+        return main_str
+
+    def _add_indent(self, text):
+        lines = text.split("\n")
+        # don't do anything for single-line stuff
+        if len(lines) == 1:
+            return text
+        first = lines.pop(0)
+        # add 2 spaces to each line but the first
+        lines = [(2 * " ") + line for line in lines]
+        lines = "\n".join(lines)
+        lines = first + "\n" + lines
+        return lines
```

### Comparing `danling-0.3.3/danling/runner/state.py` & `danling-0.3.4/danling/runner/state.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,41 +49,14 @@
         step_end (int): End running steps.
             Note that `step_end` not initialised since this variable may not apply to some Runners.
         epoch_end (int): End running epochs.
             Note that `epoch_end` not initialised since this variable may not apply to some Runners.
 
     In general you should only use one of `iter_end`, `step_end`, `epoch_end` to indicate the length of running.
 
-    Attributes: Results:
-        results (dict): All results, should be in the form of `{step: {subset: {score_name: score}}}`.
-
-    `results` should be a list of `result`.
-    `result` should be a dict with the same `split` as keys, like `dataloaders`.
-    A typical `result` might look like this:
-    ```python
-    {
-        "train": {
-            "loss": 0.1,
-            "accuracy": 0.9,
-        },
-        "val": {
-            "loss": 0.2,
-            "accuracy": 0.8,
-        },
-        "test": {
-            "loss": 0.3,
-            "accuracy": 0.7,
-        },
-    }
-    ```
-
-    `scores` are dynamically extracted from `results` by `score_set` and `score_name`.
-    They represent the core metric that is used in comparing the performance against different models and settings.
-    For the above `results`, If `score_set = "val"`, `score_name = "accuracy"`, then `scores = 0.9`.
-
     Attributes: IO:
         project_root (str): The root directory for all experiments.
             Defaults to `"experiments"`.
 
     `project_root` is the root directory of all **Experiments**, and should be consistent across the **Project**.
 
     `dir` is the directory of a certain **Run**.
@@ -127,15 +100,14 @@
     iter_begin: int = 0
     step_begin: int = 0
     epoch_begin: int = 0
     iter_end: Optional[int] = None
     step_end: Optional[int] = None
     epoch_end: Optional[int] = None
 
-    results: dict
     score_set: Optional[str] = None
     score_name: str = "loss"
 
     project_root: str = "experiments"
     checkpoint_dir_name: str = "checkpoints"
     log: bool = True
     tensorboard: bool = False
@@ -149,15 +121,14 @@
     master_port: Optional[int] = None
 
     def __init__(self, *args, **kwargs):
         for k, v in self.__class__.__dict__.items():
             if not (k.startswith("__") and k.endswith("__")) and (not (isinstance(v, property) or callable(v))):
                 self.set(k, v)
         self.seed = randint(0, 2**32 - 1)
-        self.results = NestedDict()
         super().__init__(*args, **kwargs)
         if "experiment_id" not in self:
             self.experiment_id = get_git_hash() or defaults.DEFAULT_EXPERIMENT_ID
         if "run_id" not in self:
             self.run_id = self.run_uuid.hex
         self.setattr("ignored_keys_in_hash", defaults.DEFAULT_IGNORED_KEYS_IN_HASH)
```

### Comparing `danling-0.3.3/danling/runner/utils.py` & `danling-0.3.4/danling/runner/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/tensors/functional.py` & `danling-0.3.4/danling/tensors/functional.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/tensors/nested_tensor.py` & `danling-0.3.4/danling/tensors/nested_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,36 +33,36 @@
         Identical to `self`.
 
         Returns:
             (torch.Tensor):
 
         Examples:
             >>> tensor = torch.tensor([1, 2, 3])
-            >>> pn_tensor = PNTensor(tensor)
-            >>> (tensor == pn_tensor).all()
-            PNTensor(True)
-            >>> (tensor == pn_tensor.tensor).all()
-            PNTensor(True)
+            >>> pn_tensor = PNTensor([1, 2, 3])
+            >>> bool((tensor == pn_tensor).all())
+            True
+            >>> bool((tensor == pn_tensor.tensor).all())
+            True
         """
 
         return self
 
     @property
     def mask(self) -> Tensor:
         r"""
         Identical to `torch.ones_like(self)`.
 
         Returns:
             (torch.Tensor):
 
         Examples:
             >>> tensor = torch.tensor([1, 2, 3])
-            >>> pn_tensor = PNTensor(tensor)
-            >>> (pn_tensor.mask == torch.ones_like(pn_tensor)).all()
-            PNTensor(True)
+            >>> pn_tensor = PNTensor([1, 2, 3])
+            >>> bool((pn_tensor.mask == torch.ones_like(pn_tensor)).all().item())
+            True
         """
 
         return torch.ones_like(self)
 
     def new_empty(self, *args, **kwargs):
         return PNTensor(super().new_empty(*args, **kwargs))
```

### Comparing `danling-0.3.3/danling/tensors/utils.py` & `danling-0.3.4/danling/tensors/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/utils/__init__.py` & `danling-0.3.4/danling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/utils/basex.py` & `danling-0.3.4/danling/utils/basex.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/utils/contextmanagers.py` & `danling-0.3.4/danling/utils/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/utils/decorators.py` & `danling-0.3.4/danling/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling/utils/io.py` & `danling-0.3.4/danling/utils/io.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/danling.egg-info/PKG-INFO` & `danling-0.3.4/danling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.3.3
+Version: 0.3.4
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR AGPL-3.0-or-later OR GPL-2.0-or-later OR BSD-4-Clause OR MIT OR Apache-2.0
         
 Project-URL: documentation, https://danling.org
 Project-URL: homepage, https://danling.org
```

### Comparing `danling-0.3.3/danling.egg-info/SOURCES.txt` & `danling-0.3.4/danling.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 danling.egg-info/dependency_links.txt
 danling.egg-info/requires.txt
 danling.egg-info/top_level.txt
 danling/metrics/__init__.py
 danling/metrics/average_meters.py
 danling/metrics/functional.py
 danling/metrics/metrics.py
+danling/metrics/utils.py
 danling/modules/__init__.py
 danling/modules/mlp/__init__.py
 danling/modules/mlp/dense.py
 danling/modules/mlp/mlp.py
 danling/modules/transformer/__init__.py
 danling/modules/transformer/decoder.py
 danling/modules/transformer/encoder.py
@@ -72,18 +73,18 @@
 docs/docs/manifest.webmanifest
 docs/docs/package.md
 docs/docs/blog/index.md
 docs/docs/metrics/average_meter.md
 docs/docs/metrics/average_meters.md
 docs/docs/metrics/metrics.md
 docs/docs/optim/lr_scheduler.md
+docs/docs/runner/accelerate_runner.md
 docs/docs/runner/base_runner.md
 docs/docs/runner/index.md
-docs/docs/runner/runner_state.md
-docs/docs/runner/torch_runner.md
+docs/docs/runner/state.md
 docs/docs/runner/utils.md
 docs/docs/tensors/nested_tensor.md
 docs/docs/tensors/pn_tensor.md
 docs/docs/tensors/torch_func_registry.md
 docs/docs/utils/basex.md
 docs/docs/utils/contextmanagers.md
 docs/docs/utils/decorators.md
```

### Comparing `danling-0.3.3/demo/vision/torch_mnist.py` & `danling-0.3.4/demo/vision/torch_mnist.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         self.datasets.val = torchvision.datasets.MNIST(train=False, **self.dataset)
 
         self.model = getattr(torchvision.models, self.network.name)(pretrained=False, num_classes=10)
         self.model.conv1 = nn.Conv2d(1, 64, 1, bias=False)
         self.optimizer = OPTIMIZERS.build(params=self.model.parameters(), **self.optim)
         self.criterion = nn.CrossEntropyLoss()
 
+        self.metrics = dl.metrics.multiclass_metrics(num_classes=10)
         self.meters.loss.reset()
         self.meters.time.reset()
 
 
 if __name__ == "__main__":
     config = MNISTConfig()
     config.parse()
```

### Comparing `danling-0.3.3/docs/mkdocs.yml` & `danling-0.3.4/docs/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 nav:
   - DanLing: index.md
   - Runner:
       - runner/index.md
       - RunnerState: runner/runner_state.md
       - BaseRunner: runner/base_runner.md
-      - TorchRunner: runner/torch_runner.md
+      - AccelerateRunner: runner/accelerate_runner.md
       - Utilities: runner/utils.md
   - Tensors:
       - NestedTensor: tensors/nested_tensor.md
       - PNTensor: tensors/pn_tensor.md
       - TorchFuncRegistry: tensors/torch_func_registry.md
   - Optim:
       - LRScheduler: optim/lr_scheduler.md
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 site_name: DanLing site_url: https://danling.org site_author: DanLing
 Contributors site_description: Scaffold for experienced Machine Learning
 Researchers copyright: All rights reserved © 2021-2023, DanLing Contributors
 repo_name: DanLing repo_url: https://github.com/ZhiyuanChen/DanLing nav: -
 DanLing: index.md - Runner: - runner/index.md - RunnerState: runner/
-runner_state.md - BaseRunner: runner/base_runner.md - TorchRunner: runner/
-torch_runner.md - Utilities: runner/utils.md - Tensors: - NestedTensor:
+runner_state.md - BaseRunner: runner/base_runner.md - AccelerateRunner: runner/
+accelerate_runner.md - Utilities: runner/utils.md - Tensors: - NestedTensor:
 tensors/nested_tensor.md - PNTensor: tensors/pn_tensor.md - TorchFuncRegistry:
 tensors/torch_func_registry.md - Optim: - LRScheduler: optim/lr_scheduler.md -
 Metrics: - metrics: metrics/metrics.md - AverageMeters: metrics/
 average_meters.md - Utilities: - Decorator: utils/decorators.md - Context
 Manager: utils/contextmanagers.md - IO: utils/io.md - basex: utils/basex.md -
 package: package.md # - Blog: blog/index.md theme: name: material custom_dir:
 overrides language: "zh" palette: - media: "(prefers-color-scheme: dark)"
```

### Comparing `danling-0.3.3/docs/overrides/assets/fonts/CascadiaCodePL.woff2` & `danling-0.3.4/docs/overrides/assets/fonts/CascadiaCodePL.woff2`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/docs/overrides/assets/fonts/HYQiHei.ttf` & `danling-0.3.4/docs/overrides/assets/fonts/HYQiHei.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/docs/overrides/assets/fonts/HelveticaNowDisplay.otf` & `danling-0.3.4/docs/overrides/assets/fonts/HelveticaNowDisplay.otf`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/docs/overrides/assets/fonts/HelveticaWorld.ttf` & `danling-0.3.4/docs/overrides/assets/fonts/HelveticaWorld.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/docs/overrides/assets/images/favicon.ico` & `danling-0.3.4/docs/overrides/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/docs/overrides/assets/images/logo.png` & `danling-0.3.4/docs/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/docs/overrides/main.html` & `danling-0.3.4/docs/overrides/main.html`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/pyproject.toml` & `danling-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/tests/metrics/test_metrics.py` & `danling-0.3.4/tests/metrics/test_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,31 +63,32 @@
         for _ in range(10):
             pred = torch.randn(8).sigmoid()
             target = torch.randint(0, 2, (8,))
             preds.append(pred)
             targets.append(target)
             metrics.update(pred, target)
             merge_metrics.update(pred, target)
-            assert (pred == metrics.input).all()
-            assert (target == metrics.target).all()
             auc.update(pred, target)
             prc.update(pred, target)
             acc.update(pred, target)
-            assert metrics.compute()["auroc"] - binary_auroc(pred, target) < self.epsilon
-            assert metrics.compute()["auprc"] - binary_auprc(pred, target) < self.epsilon
-            assert metrics.value()["acc"] - binary_accuracy(pred, target) < self.epsilon
-            assert metrics.average()["auroc"] - auc.compute() < self.epsilon
-            assert metrics.average()["auprc"] - prc.compute() < self.epsilon
-            assert metrics.average()["acc"] - acc.compute() < self.epsilon
+            value, average = metrics.value(), metrics.average()
+            assert (pred == metrics.input).all()
+            assert (target == metrics.target).all()
+            assert value["auroc"] - binary_auroc(pred, target) < self.epsilon
+            assert value["auprc"] - binary_auprc(pred, target) < self.epsilon
+            assert value["acc"] - binary_accuracy(pred, target) < self.epsilon
+            assert average["auroc"] - auc.compute() < self.epsilon
+            assert average["auprc"] - prc.compute() < self.epsilon
+            assert average["acc"] - acc.compute() < self.epsilon
             assert metrics.avg == merge_metrics.avg
         assert (torch.cat(preds) == metrics.inputs).all()
         assert (torch.cat(targets) == metrics.targets).all()
-        assert metrics.average()["auroc"] - auc.compute() < self.epsilon
-        assert metrics.average()["auprc"] - prc.compute() < self.epsilon
-        assert metrics.average()["acc"] - acc.compute() < self.epsilon
+        assert average["auroc"] - auc.compute() < self.epsilon
+        assert average["auprc"] - prc.compute() < self.epsilon
+        assert average["acc"] - acc.compute() < self.epsilon
         assert metrics.avg == merge_metrics.avg
 
     def test_single_nested_tensor_binary(self):
         random.seed(0)
         torch.random.manual_seed(0)
         metrics = Metrics(auroc=auroc, auprc=auprc, acc=accuracy)
         dict_metrics = Metrics(func=demo_dict_metric_func, merge_dict=False)
@@ -98,33 +99,40 @@
             pred_list, target_list = [], []
             for length in lengths:
                 pred_list.append(torch.randn(length).sigmoid())
                 target_list.append(torch.randint(0, 2, (length,)))
             preds.extend(pred_list)
             targets.extend(target_list)
             pred_nt, target_nt = NestedTensor(pred_list), NestedTensor(target_list)
-            metrics.update(pred_nt, target_nt)
-            dict_metrics.update(pred_nt, target_nt)
-            assert (pred_nt == metrics.input).all()
-            assert (target_nt == metrics.target).all()
             pred, target = torch.cat(pred_list), torch.cat(target_list)
+            metrics.update(pred_nt, target_nt)
             auc.update(pred, target)
             prc.update(pred, target)
             acc.update(pred, target)
-            assert metrics.compute()["auroc"] - binary_auroc(pred, target) < self.epsilon
-            assert metrics.compute()["auprc"] - binary_auprc(pred, target) < self.epsilon
-            assert metrics.compute()["acc"] - binary_accuracy(pred, target) < self.epsilon
-            assert metrics.average()["auroc"] - auc.compute() < self.epsilon
-            assert metrics.average()["auprc"] - prc.compute() < self.epsilon
-            assert metrics.average()["acc"] - acc.compute() < self.epsilon
+            value, batch, average = metrics.value(), metrics.batch(), metrics.average()
+            assert (pred_nt == metrics._input).all()
+            assert (target_nt == metrics._target).all()
+            dict_metrics.update(pred_nt, target_nt)
+            assert value["auroc"] - binary_auroc(pred, target) < self.epsilon
+            assert value["auprc"] - binary_auprc(pred, target) < self.epsilon
+            assert value["acc"] - binary_accuracy(pred, target) < self.epsilon
+            pred = torch.cat(pred_list)
+            target = torch.cat(target_list)
+            assert batch["auroc"] - binary_auroc(pred, target) < self.epsilon
+            assert batch["auprc"] - binary_auprc(pred, target) < self.epsilon
+            assert batch["acc"] - binary_accuracy(pred, target) < self.epsilon
+            assert average["auroc"] - auc.compute() < self.epsilon
+            assert average["auprc"] - prc.compute() < self.epsilon
+            assert average["acc"] - acc.compute() < self.epsilon
+        average = metrics.average()
         assert (torch.cat(preds) == metrics.inputs).all()
         assert (torch.cat(targets) == metrics.targets).all()
-        assert metrics.average()["auroc"] - auc.compute() < self.epsilon
-        assert metrics.average()["auprc"] - prc.compute() < self.epsilon
-        assert metrics.average()["acc"] - acc.compute() < self.epsilon
+        assert average["auroc"] - auc.compute() < self.epsilon
+        assert average["auprc"] - prc.compute() < self.epsilon
+        assert average["acc"] - acc.compute() < self.epsilon
         ret, dict_ret = metrics.average(), dict_metrics.average()
         for key, value in ret.items():
             assert dict_ret[f"func.{key}"] == value
 
     def test_distributed(self, world_size: int = 8):
         self._test_distributed(self._test_distributed_tensor_binary, world_size)
         self._test_distributed(self._test_distributed_nested_tensor_binary, world_size)
@@ -144,27 +152,27 @@
             target = torch.randint(0, 2, (length,), dtype=torch.float, requires_grad=True)
             preds.append(pred)
             targets.append(target)
             metrics.update(pred, target)
             auc.update(pred, target)
             prc.update(pred, target)
             acc.update(pred, target)
+            value = metrics.value()
             assert (pred == metrics.input[length * rank : length * (rank + 1)]).all()  # noqa: E203
             assert (target == metrics.target[length * rank : length * (rank + 1)]).all()  # noqa: E203
-            assert metrics.compute()["auroc"] - binary_auroc(pred, target) < self.epsilon
-            assert metrics.compute()["auprc"] - binary_auprc(pred, target) < self.epsilon
-            assert metrics.compute()["acc"] - binary_accuracy(pred, target) < self.epsilon
+            assert value["auroc"] - binary_auroc(pred, target) < self.epsilon
+            assert value["auprc"] - binary_auprc(pred, target) < self.epsilon
+            assert value["acc"] - binary_accuracy(pred, target) < self.epsilon
 
         pred = torch.cat(self._all_gather(preds, world_size))
         target = torch.cat(self._all_gather(targets, world_size))
-        assert (pred == metrics.inputs).all()
-        assert (target == metrics.targets).all()
-        assert metrics.average()["auroc"] - binary_auroc(pred, target) < self.epsilon
-        assert metrics.average()["auprc"] - binary_auprc(pred, target) < self.epsilon
-        assert metrics.average()["acc"] - binary_accuracy(pred, target) < self.epsilon
+        average = metrics.average()
+        assert average["auroc"] - binary_auroc(pred, target) < self.epsilon
+        assert average["auprc"] - binary_auprc(pred, target) < self.epsilon
+        assert average["acc"] - binary_accuracy(pred, target) < self.epsilon
 
         dist.destroy_process_group()
 
     def _test_distributed_nested_tensor_binary(self, rank, world_size):
         dist.init_process_group("gloo", rank=rank, world_size=world_size)
 
         # cum_length = 0
@@ -179,37 +187,41 @@
             pred_list, target_list = [], []
             for length in lengths:
                 pred_list.append(torch.randn(length).sigmoid())
                 target_list.append(torch.randint(0, 2, (length,)))
             preds.extend(pred_list)
             targets.extend(target_list)
             pred_nt, target_nt = NestedTensor(pred_list), NestedTensor(target_list)
-            metrics.update(pred_nt, target_nt)
             pred, target = torch.cat(pred_list), torch.cat(target_list)
-            # assert (pred == metrics.input[cum_length * rank : cum_length * (rank + 1)]).all()
-            # assert (target == metrics.target[cum_length * rank : cum_length * (rank + 1)]).all()
-            assert metrics.compute()["auroc"] - binary_auroc(pred, target) < self.epsilon
-            assert metrics.compute()["auprc"] - binary_auprc(pred, target) < self.epsilon
-            assert metrics.compute()["acc"] - binary_accuracy(pred, target) < self.epsilon
-            pred = torch.cat(self._all_gather(pred_list, world_size))
-            target = torch.cat(self._all_gather(target_list, world_size))
+            metrics.update(pred_nt, target_nt)
             auc.update(pred, target)
             prc.update(pred, target)
             acc.update(pred, target)
-            assert metrics.value()["auroc"] - binary_auroc(pred, target) < self.epsilon
-            assert metrics.value()["auprc"] - binary_auprc(pred, target) < self.epsilon
-            assert metrics.value()["acc"] - binary_accuracy(pred, target) < self.epsilon
+            value, batch = metrics.value(), metrics.batch()
+            assert (pred_nt == metrics._input).all()
+            assert (target_nt == metrics._target).all()
+            assert value["auroc"] - binary_auroc(pred, target) < self.epsilon
+            assert value["auprc"] - binary_auprc(pred, target) < self.epsilon
+            assert value["acc"] - binary_accuracy(pred, target) < self.epsilon
+            pred = torch.cat(self._all_gather(pred_list, world_size))
+            target = torch.cat(self._all_gather(target_list, world_size))
+            assert batch["auroc"] - binary_auroc(pred, target) < self.epsilon
+            assert batch["auprc"] - binary_auprc(pred, target) < self.epsilon
+            assert batch["acc"] - binary_accuracy(pred, target) < self.epsilon
+            # assert (pred == metrics.input[cum_length * rank : cum_length * (rank + 1)]).all()
+            # assert (target == metrics.target[cum_length * rank : cum_length * (rank + 1)]).all()
 
         pred = torch.cat(self._all_gather(preds, world_size))
         target = torch.cat(self._all_gather(targets, world_size))
+        average = metrics.average()
         assert (pred == metrics.inputs).all()
         assert (target == metrics.targets).all()
-        assert metrics.average()["auroc"] - binary_auroc(pred, target) < self.epsilon
-        assert metrics.average()["auprc"] - binary_auprc(pred, target) < self.epsilon
-        assert metrics.average()["acc"] - binary_accuracy(pred, target) < self.epsilon
+        assert average["auroc"] - binary_auroc(pred, target) < self.epsilon
+        assert average["auprc"] - binary_auprc(pred, target) < self.epsilon
+        assert average["acc"] - binary_accuracy(pred, target) < self.epsilon
 
         dist.destroy_process_group()
 
     def _test_distributed_nested_tensor_regression(self, rank, world_size):
         dist.init_process_group("gloo", rank=rank, world_size=world_size)
 
         # cum_length = 0
@@ -223,32 +235,36 @@
             pred_list, target_list = [], []
             for length in lengths:
                 pred_list.append(torch.randn(length))
                 target_list.append(torch.randn(length))
             preds.extend(pred_list)
             targets.extend(target_list)
             pred_nt, target_nt = NestedTensor(pred_list), NestedTensor(target_list)
-            metrics.update(pred_nt, target_nt)
             pred, target = torch.cat(pred_list), torch.cat(target_list)
-            assert metrics.compute()["pearson"] - pearson(pred, target) < self.epsilon
-            assert metrics.compute()["spearman"] - spearman(pred, target) < self.epsilon
-            assert metrics.compute()["rmse"] - rmse(pred, target) < self.epsilon
+            metrics.update(pred_nt, target_nt)
+            value, batch = metrics.value(), metrics.batch()
+            assert (pred_nt == metrics._input).all()
+            assert (target_nt == metrics._target).all()
+            assert value["pearson"] - pearson(pred, target) < self.epsilon
+            assert value["spearman"] - spearman(pred, target) < self.epsilon
+            assert value["rmse"] - rmse(pred, target) < self.epsilon
             pred = torch.cat(self._all_gather(pred_list, world_size))
             target = torch.cat(self._all_gather(target_list, world_size))
-            assert metrics.value()["pearson"] - pearson(pred, target) < self.epsilon
-            assert metrics.value()["spearman"] - spearman(pred, target) < self.epsilon
-            assert metrics.value()["rmse"] - rmse(pred, target) < self.epsilon
+            assert batch["pearson"] - pearson(pred, target) < self.epsilon
+            assert batch["spearman"] - spearman(pred, target) < self.epsilon
+            assert batch["rmse"] - rmse(pred, target) < self.epsilon
 
         pred = torch.cat(self._all_gather(preds, world_size))
         target = torch.cat(self._all_gather(targets, world_size))
+        average = metrics.compute()
         assert (pred == metrics.inputs).all()
         assert (target == metrics.targets).all()
-        assert metrics.average()["pearson"] - pearson(pred, target) < self.epsilon
-        assert metrics.average()["spearman"] - spearman(pred, target) < self.epsilon
-        assert metrics.average()["rmse"] - rmse(pred, target) < self.epsilon
+        assert average["pearson"] - pearson(pred, target) < self.epsilon
+        assert average["spearman"] - spearman(pred, target) < self.epsilon
+        assert average["rmse"] - rmse(pred, target) < self.epsilon
 
         dist.destroy_process_group()
 
     def _test_distributed_nested_tensor_multi_regression(self, rank, world_size):
         dist.init_process_group("gloo", rank=rank, world_size=world_size)
 
         # cum_length = 0
@@ -263,32 +279,36 @@
             pred_list, target_list = [], []
             for length in lengths:
                 pred_list.append(torch.randn(length, channels))
                 target_list.append(torch.randn(length, channels))
             preds.extend(pred_list)
             targets.extend(target_list)
             pred_nt, target_nt = NestedTensor(pred_list), NestedTensor(target_list)
-            metrics.update(pred_nt, target_nt)
             pred, target = torch.cat(pred_list), torch.cat(target_list)
-            assert sum(torch.tensor(metrics.compute()["pearson"]) - pearson(pred, target)) < self.epsilon
-            assert sum(torch.tensor(metrics.compute()["spearman"]) - spearman(pred, target)) < self.epsilon
-            assert metrics.compute()["rmse"] - rmse(pred, target) < self.epsilon
+            metrics.update(pred_nt, target_nt)
+            value, batch = metrics.value(), metrics.batch()
+            assert (pred_nt == metrics._input).all()
+            assert (target_nt == metrics._target).all()
+            assert sum(torch.tensor(value["pearson"]) - pearson(pred, target)) < self.epsilon
+            assert sum(torch.tensor(value["spearman"]) - spearman(pred, target)) < self.epsilon
+            assert value["rmse"] - rmse(pred, target) < self.epsilon
             pred = torch.cat(self._all_gather(pred_list, world_size))
             target = torch.cat(self._all_gather(target_list, world_size))
-            assert sum(torch.tensor(metrics.value()["pearson"]) - pearson(pred, target)) < self.epsilon
-            assert sum(torch.tensor(metrics.value()["spearman"]) - spearman(pred, target)) < self.epsilon
-            assert metrics.value()["rmse"] - rmse(pred, target) < self.epsilon
+            assert sum(torch.tensor(batch["pearson"]) - pearson(pred, target)) < self.epsilon
+            assert sum(torch.tensor(batch["spearman"]) - spearman(pred, target)) < self.epsilon
+            assert batch["rmse"] - rmse(pred, target) < self.epsilon
 
         pred = torch.cat(self._all_gather(preds, world_size))
         target = torch.cat(self._all_gather(targets, world_size))
+        average = metrics.average()
         assert (pred == metrics.inputs).all()
         assert (target == metrics.targets).all()
-        assert sum(torch.tensor(metrics.average()["pearson"]) - pearson(pred, target)) < self.epsilon
-        assert sum(torch.tensor(metrics.average()["spearman"]) - spearman(pred, target)) < self.epsilon
-        assert metrics.average()["rmse"] - rmse(pred, target) < self.epsilon
+        assert sum(torch.tensor(average["pearson"]) - pearson(pred, target)) < self.epsilon
+        assert sum(torch.tensor(average["spearman"]) - spearman(pred, target)) < self.epsilon
+        assert average["rmse"] - rmse(pred, target) < self.epsilon
 
         dist.destroy_process_group()
 
     def _test_distributed(self, func: callable, world_size: int = 8):
         random.seed(0)
         torch.random.manual_seed(0)
         os.environ["MASTER_ADDR"] = "localhost"
```

### Comparing `danling-0.3.3/tests/optim/test_lr_scheduler.py` & `danling-0.3.4/tests/optim/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/tests/runner/test_base_runner.py` & `danling-0.3.4/tests/runner/test_base_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,26 @@
         self.optim.weight_decay = 1e-4
         self.log = False
         self.tensorboard = False
         self.gradient_clip = False
         self.print_interval = 10
         self.train_iterations_per_epoch = 64
         self.val_iterations_per_epoch = 16
-        self.index_set = "val"
-        self.index = "loss"
+        self.score_set = "val"
+        self.score = "loss"
         self.conflict = 1
 
 
 class Test:
     config = Config()
     runner = Runner(config)
 
     def test_results(self):
         runner = self.runner
-        state = runner.state
-        state.results = NestedDict(
+        runner.results = NestedDict(
             {
                 0: {
                     "val": {
                         "loss": 1.0,
                         "acc": 0.0,
                     },
                 },
```

### Comparing `danling-0.3.3/tests/runner/test_torch_runner.py` & `danling-0.3.4/tests/runner/test_torch_runner.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.3/tests/tensors/test_nested_tensor.py` & `danling-0.3.4/tests/tensors/test_nested_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         assert torch.sum(a * i - i / (1 / a)) < self.epsilon
         assert torch.sum(a / (1 / i) - i * a) < self.epsilon
         assert torch.sum(a * i - i * a) < self.epsilon
         a *= i
         b /= 1 / i
         assert torch.sum(a - b) < self.epsilon
 
+    @pytest.mark.skipif(torch.__version__ < "1.12", reason="requires PyTorch 1.12 or higher")
     @pytest.mark.parametrize(
         "i",
         [
             NestedTensor([[6, 5, 4], [3, 2]]),
             torch.tensor([[6, 5, 4], [3, 2, 1]]),
             torch.randn(2, 3),
             1,
```

### Comparing `danling-0.3.3/tests/utils/test_decorators.py` & `danling-0.3.4/tests/utils/test_decorators.py`

 * *Files identical despite different names*

