# Comparing `tmp/kan_gpt-0.3.0.tar.gz` & `tmp/kan_gpt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kan_gpt-0.3.0.tar", last modified: Tue May  7 19:30:44 2024, max compression
+gzip compressed data, was "kan_gpt-0.4.0.tar", last modified: Wed May  8 17:43:45 2024, max compression
```

## Comparing `kan_gpt-0.3.0.tar` & `kan_gpt-0.4.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.092052 kan_gpt-0.3.0/kan_gpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.092052 kan_gpt-0.3.0/kan_gpt/efficient_kan/
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/efficient_kan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.096052 kan_gpt-0.3.0/kan_gpt/kan/
--rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/KAN.py
--rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/LBFGS.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/Symbolic_KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.096052 kan_gpt-0.3.0/kan_gpt/kan/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_2_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_3_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_4_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/kan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/kan_gpt/mingpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/mingpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/mingpt/bpe.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/mingpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/mingpt/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/mingpt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/kan_gpt/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/kan_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 19:30:44.000000 kan_gpt-0.3.0/kan_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:44.100051 kan_gpt-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_efficient_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_gpt_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_gpt_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-07 19:30:35.000000 kan_gpt-0.3.0/tests/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.184074 kan_gpt-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-08 17:43:45.184074 kan_gpt-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.176074 kan_gpt-0.4.0/kan_gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/download_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.176074 kan_gpt-0.4.0/kan_gpt/efficient_kan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/efficient_kan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/efficient_kan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.180074 kan_gpt-0.4.0/kan_gpt/kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/KAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/LBFGS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/Symbolic_KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.180074 kan_gpt-0.4.0/kan_gpt/kan/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_2_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/kan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.180074 kan_gpt-0.4.0/kan_gpt/mingpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/mingpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/mingpt/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/mingpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/mingpt/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/mingpt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/kan_gpt/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.184074 kan_gpt-0.4.0/kan_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 17:43:45.000000 kan_gpt-0.4.0/kan_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:43:45.184074 kan_gpt-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:45.184074 kan_gpt-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_dataset_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_efficient_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_gpt_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_gpt_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-08 17:43:36.000000 kan_gpt-0.4.0/tests/test_train.py
```

### Comparing `kan_gpt-0.3.0/HISTORY.md` & `kan_gpt-0.4.0/HISTORY.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Version increment. [Aditya NG]
+- Fix(kan_gpt/efficient_kan/__init__.py): missing init file. [Aditya NG]
+- Feat(README.md): results added. [Aditya NG]
+- Docs(mkdocs): documentation for mkdocs. [Aditya NG]
+- Feat(sweep): slower learning rate. [Aditya NG]
+- Fix(sweep): max_iters. [Aditya NG]
+- Fix(sweep): cuda device. [Aditya NG]
+- Ci(main): disabled wandb in ci. [Aditya NG]
+- Test(tests/test_train.py): disable wandb during testing. [Aditya NG]
+- Fix(sweep): added cuda clean. [Aditya NG]
+- Feat(sweep): reduced batch size. [Aditya NG]
+- Feat(download_dataset): functions to download tinyshakespeare and
+  webtext. [Aditya NG]
+
+
+0.3.0 (2024-05-07)
+------------------
+- Release: version 0.3.0 🚀 [Aditya NG]
 - Docs(README.md): dataset mention. [Aditya NG]
 - Feat(sweep): sweep script for getting a vast hyperparam sweep. [Aditya
   NG]
 - Feat(tinyshakespeare): support for another dataset. [Aditya NG]
 - Test(tests/test_prompt.py): eval code. [Aditya NG]
 - Test(efficient_kan,original_kan): coverage. [Aditya NG]
```

### Comparing `kan_gpt-0.3.0/LICENSE` & `kan_gpt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/PKG-INFO` & `kan_gpt-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.3.0
+Version: 0.4.0
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -25,19 +25,22 @@
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
 Requires-Dist: lark; extra == "test"
 Requires-Dist: types-requests; extra == "test"
+Requires-Dist: requests-mock; extra == "test"
 
 # KAN-GPT
 
 [![codecov](https://codecov.io/gh/AdityaNG/kan-gpt/branch/main/graph/badge.svg?token=kan-gpt_token_here)](https://codecov.io/gh/AdityaNG/kan-gpt)
 [![CI](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml/badge.svg)](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml)
+![PyPI - Version](https://img.shields.io/pypi/v/kan-gpt)
+![GitHub License](https://img.shields.io/github/license/AdityaNG/kan-gpt)
 
 The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
@@ -84,14 +87,15 @@
 # Download Repo
 git clone https://github.com/AdityaNG/kan-gpt
 cd kan-gpt
 git pull
 
 # Download Dataset
 ./scripts/download_webtext.sh
+./scripts/download_tinyshakespeare.sh
 
 # Install dependencies for development
 pip install -r requirements.txt
 pip install -e .
 ```
 
 ## Train
@@ -110,14 +114,20 @@
 ## Prompt
 
 You can prompt the model to produce text as follows
 ```bash
 python -m kan_gpt.prompt --prompt "Bangalore is often described as the " --model_path (checkpoint)
 ```
 
+## Results
+
+We train and compare KAN-GPT with an equivalent MLP-GPT model on the Tiny Shakespeare dataset. We observe that the KAN-GPT performs slightly better than the MLP-GPT. We are looking into further experiments to dive deeper. The results are shown below:
+
+<img src="media/results.png">
+
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
 - [x] Mini training POC for KAN-GPT
@@ -128,15 +138,19 @@
 - [x] Train KAN-GPT on the webtext dataset as a baseline
 - [ ] Metrics comparing KAN-GPT and MLP-GPT
 - [x] Auto Save checkpoints
 - [x] Auto Save checkpoints to W&B
 - [ ] Auto Download model weights from git / huggingface
 - [x] W&B hyperparam sweep script
 - [x] Script to load checkpoint in interactive mode
+- [ ] Reduce requrements.txt constraints
+- [ ] Define pydantic model for training and sweep args
+- [ ] Pruning the package, get rid of unused code
 - [ ] Training script to PyTorch Lighting
+- [x] Documentation: `mkdocs gh-deploy`
 - [x] Integrate with [efficient-kan](https://github.com/Blealtan/efficient-kan/blob/master/src/efficient_kan/kan.py)
 - [x] Test Cases
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
   - [x] EFFICIENT_KAN: Forward-Backward test
```

### Comparing `kan_gpt-0.3.0/README.md` & `kan_gpt-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # KAN-GPT
 
 [![codecov](https://codecov.io/gh/AdityaNG/kan-gpt/branch/main/graph/badge.svg?token=kan-gpt_token_here)](https://codecov.io/gh/AdityaNG/kan-gpt)
 [![CI](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml/badge.svg)](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml)
+![PyPI - Version](https://img.shields.io/pypi/v/kan-gpt)
+![GitHub License](https://img.shields.io/github/license/AdityaNG/kan-gpt)
 
 The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
@@ -52,14 +54,15 @@
 # Download Repo
 git clone https://github.com/AdityaNG/kan-gpt
 cd kan-gpt
 git pull
 
 # Download Dataset
 ./scripts/download_webtext.sh
+./scripts/download_tinyshakespeare.sh
 
 # Install dependencies for development
 pip install -r requirements.txt
 pip install -e .
 ```
 
 ## Train
@@ -78,14 +81,20 @@
 ## Prompt
 
 You can prompt the model to produce text as follows
 ```bash
 python -m kan_gpt.prompt --prompt "Bangalore is often described as the " --model_path (checkpoint)
 ```
 
+## Results
+
+We train and compare KAN-GPT with an equivalent MLP-GPT model on the Tiny Shakespeare dataset. We observe that the KAN-GPT performs slightly better than the MLP-GPT. We are looking into further experiments to dive deeper. The results are shown below:
+
+<img src="media/results.png">
+
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
 - [x] Mini training POC for KAN-GPT
@@ -96,15 +105,19 @@
 - [x] Train KAN-GPT on the webtext dataset as a baseline
 - [ ] Metrics comparing KAN-GPT and MLP-GPT
 - [x] Auto Save checkpoints
 - [x] Auto Save checkpoints to W&B
 - [ ] Auto Download model weights from git / huggingface
 - [x] W&B hyperparam sweep script
 - [x] Script to load checkpoint in interactive mode
+- [ ] Reduce requrements.txt constraints
+- [ ] Define pydantic model for training and sweep args
+- [ ] Pruning the package, get rid of unused code
 - [ ] Training script to PyTorch Lighting
+- [x] Documentation: `mkdocs gh-deploy`
 - [x] Integrate with [efficient-kan](https://github.com/Blealtan/efficient-kan/blob/master/src/efficient_kan/kan.py)
 - [x] Test Cases
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
   - [x] EFFICIENT_KAN: Forward-Backward test
```

### Comparing `kan_gpt-0.3.0/kan_gpt/cli.py` & `kan_gpt-0.4.0/kan_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/dataset.py` & `kan_gpt-0.4.0/kan_gpt/dataset.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/efficient_kan/model.py` & `kan_gpt-0.4.0/kan_gpt/efficient_kan/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/KAN.py` & `kan_gpt-0.4.0/kan_gpt/kan/KAN.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/KANLayer.py` & `kan_gpt-0.4.0/kan_gpt/kan/KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/LBFGS.py` & `kan_gpt-0.4.0/kan_gpt/kan/LBFGS.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/Symbolic_KANLayer.py` & `kan_gpt-0.4.0/kan_gpt/kan/Symbolic_KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_0.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_1.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_2.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_3.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_0_4.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_0_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_0.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_1.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_2.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_3.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_0_1_4.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_0_1_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_0_0.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_1_0.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_2_0.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_2_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_3_0.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_3_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/figures/sp_1_4_0.png` & `kan_gpt-0.4.0/kan_gpt/kan/figures/sp_1_4_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/spline.py` & `kan_gpt-0.4.0/kan_gpt/kan/spline.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/kan/utils.py` & `kan_gpt-0.4.0/kan_gpt/kan/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/mingpt/bpe.py` & `kan_gpt-0.4.0/kan_gpt/mingpt/bpe.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/mingpt/model.py` & `kan_gpt-0.4.0/kan_gpt/mingpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/mingpt/trainer.py` & `kan_gpt-0.4.0/kan_gpt/mingpt/trainer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/mingpt/utils.py` & `kan_gpt-0.4.0/kan_gpt/mingpt/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/model.py` & `kan_gpt-0.4.0/kan_gpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt/prompt.py` & `kan_gpt-0.4.0/kan_gpt/prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,20 +48,20 @@
     print(result)
 
 
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser("KAN-GPT Trainer")
-    parser.add_argument("--model_type", default="gpt-mini")
+    parser.add_argument("--model_type", default="gpt-micro")
     parser.add_argument("--model_path", default=None)
     parser.add_argument("--max_tokens", default=100)
 
     parser.add_argument(
-        "--prompt", default="Bangalore is often described as the "
+        "--prompt", default="Out of thy sleep. What is it thou didst say?"
     )
     parser.add_argument(
         "--architecture", choices=["MLP", "KAN"], default="KAN"
     )
     parser.add_argument(
         "--device", choices=["auto", "cpu", "cuda"], default="auto"
     )
```

### Comparing `kan_gpt-0.3.0/kan_gpt/sweep.py` & `kan_gpt-0.4.0/kan_gpt/sweep.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import torch
+
 import wandb
 from kan_gpt.train import main
 
 
 def wandb_sweep():
     run = wandb.init(resume="allow", anonymous="must")
 
@@ -14,16 +16,22 @@
         batch_size = wandb.config.batch_size
         dataset = wandb.config.dataset
         architecture = wandb.config.architecture
         device = wandb.config.device
 
     run_args = Args()
 
+    if "cuda" in run_args.device:
+        torch.cuda.empty_cache()
+
     main(args=run_args, run=run)
 
+    if "cuda" in run_args.device:
+        torch.cuda.empty_cache()
+
 
 def sweep(args):
     sweep_configuration = {
         "method": "random",
         "name": "sweep",
         "metric": {"goal": "minimize", "name": "test_loss"},
         "parameters": {
@@ -44,28 +52,28 @@
 
     wandb.agent(sweep_id, function=wandb_sweep)
 
 
 if __name__ == "__main__":
 
     class SweepArgs:
-        model_type = ["gpt-mini", "gpt-nano", "gpt2"]
+        model_type = ["gpt-mini", "gpt-micro", "gpt-nano", "gpt-pico"]
         dummy_dataset = [
             False,
         ]
-        learning_rate = [5e-3, 5e-4, 5e-5, 5e-6]
+        learning_rate = [5e-5, 5e-6, 5e-7]
         max_iters = [
-            1000,
+            8000,
         ]
         num_workers = [
             0,
         ]
-        batch_size = [1, 2, 4, 8, 12, 16]
+        batch_size = [1, 2, 3, 4]
         dataset = [
             "tinyshakespeare",
         ]
         architecture = ["MLP", "KAN"]
         device = [
-            "auto",
+            "cuda",
         ]
 
     sweep(SweepArgs())
```

### Comparing `kan_gpt-0.3.0/kan_gpt/train.py` & `kan_gpt-0.4.0/kan_gpt/train.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/kan_gpt.egg-info/PKG-INFO` & `kan_gpt-0.4.0/kan_gpt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 0.3.0
+Version: 0.4.0
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -25,19 +25,22 @@
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
 Requires-Dist: lark; extra == "test"
 Requires-Dist: types-requests; extra == "test"
+Requires-Dist: requests-mock; extra == "test"
 
 # KAN-GPT
 
 [![codecov](https://codecov.io/gh/AdityaNG/kan-gpt/branch/main/graph/badge.svg?token=kan-gpt_token_here)](https://codecov.io/gh/AdityaNG/kan-gpt)
 [![CI](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml/badge.svg)](https://github.com/AdityaNG/kan-gpt/actions/workflows/main.yml)
+![PyPI - Version](https://img.shields.io/pypi/v/kan-gpt)
+![GitHub License](https://img.shields.io/github/license/AdityaNG/kan-gpt)
 
 The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
@@ -84,14 +87,15 @@
 # Download Repo
 git clone https://github.com/AdityaNG/kan-gpt
 cd kan-gpt
 git pull
 
 # Download Dataset
 ./scripts/download_webtext.sh
+./scripts/download_tinyshakespeare.sh
 
 # Install dependencies for development
 pip install -r requirements.txt
 pip install -e .
 ```
 
 ## Train
@@ -110,14 +114,20 @@
 ## Prompt
 
 You can prompt the model to produce text as follows
 ```bash
 python -m kan_gpt.prompt --prompt "Bangalore is often described as the " --model_path (checkpoint)
 ```
 
+## Results
+
+We train and compare KAN-GPT with an equivalent MLP-GPT model on the Tiny Shakespeare dataset. We observe that the KAN-GPT performs slightly better than the MLP-GPT. We are looking into further experiments to dive deeper. The results are shown below:
+
+<img src="media/results.png">
+
 ## TODOs
 
 - [x] Integrate [minGPT](https://github.com/karpathy/minGPT) and [pykan](https://github.com/KindXiaoming/pykan)
 - [x] Dataset downloading script for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [WebText](https://github.com/openai/gpt-2-output-dataset)
 - [x] PyTorch Dataset parser for [tinyshakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)
 - [x] Mini training POC for KAN-GPT
@@ -128,15 +138,19 @@
 - [x] Train KAN-GPT on the webtext dataset as a baseline
 - [ ] Metrics comparing KAN-GPT and MLP-GPT
 - [x] Auto Save checkpoints
 - [x] Auto Save checkpoints to W&B
 - [ ] Auto Download model weights from git / huggingface
 - [x] W&B hyperparam sweep script
 - [x] Script to load checkpoint in interactive mode
+- [ ] Reduce requrements.txt constraints
+- [ ] Define pydantic model for training and sweep args
+- [ ] Pruning the package, get rid of unused code
 - [ ] Training script to PyTorch Lighting
+- [x] Documentation: `mkdocs gh-deploy`
 - [x] Integrate with [efficient-kan](https://github.com/Blealtan/efficient-kan/blob/master/src/efficient_kan/kan.py)
 - [x] Test Cases
   - [x] KAN: Forward-Backward test
   - [x] GPT: Forward-Backward test
   - [x] KAN_GPT: Forward-Backward test
   - [x] EFFICIENT_KAN: Forward-Backward test
```

### Comparing `kan_gpt-0.3.0/kan_gpt.egg-info/SOURCES.txt` & `kan_gpt-0.4.0/kan_gpt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 setup.py
 kan_gpt/VERSION
 kan_gpt/__init__.py
 kan_gpt/__main__.py
 kan_gpt/base.py
 kan_gpt/cli.py
 kan_gpt/dataset.py
+kan_gpt/download_dataset.py
 kan_gpt/model.py
 kan_gpt/prompt.py
 kan_gpt/settings.py
 kan_gpt/sweep.py
 kan_gpt/train.py
 kan_gpt.egg-info/PKG-INFO
 kan_gpt.egg-info/SOURCES.txt
 kan_gpt.egg-info/dependency_links.txt
 kan_gpt.egg-info/entry_points.txt
 kan_gpt.egg-info/requires.txt
 kan_gpt.egg-info/top_level.txt
+kan_gpt/efficient_kan/__init__.py
 kan_gpt/efficient_kan/model.py
 kan_gpt/kan/KAN.py
 kan_gpt/kan/KANLayer.py
 kan_gpt/kan/LBFGS.py
 kan_gpt/kan/Symbolic_KANLayer.py
 kan_gpt/kan/__init__.py
 kan_gpt/kan/spline.py
@@ -48,13 +50,14 @@
 kan_gpt/mingpt/bpe.py
 kan_gpt/mingpt/model.py
 kan_gpt/mingpt/trainer.py
 kan_gpt/mingpt/utils.py
 tests/__init__.py
 tests/conftest.py
 tests/test_base.py
+tests/test_dataset_download.py
 tests/test_efficient_kan.py
 tests/test_gpt_kan.py
 tests/test_gpt_mlp.py
 tests/test_kan.py
 tests/test_prompt.py
 tests/test_train.py
```

### Comparing `kan_gpt-0.3.0/setup.py` & `kan_gpt-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/tests/test_efficient_kan.py` & `kan_gpt-0.4.0/tests/test_efficient_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/tests/test_gpt_kan.py` & `kan_gpt-0.4.0/tests/test_gpt_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/tests/test_gpt_mlp.py` & `kan_gpt-0.4.0/tests/test_gpt_mlp.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/tests/test_kan.py` & `kan_gpt-0.4.0/tests/test_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-0.3.0/tests/test_train.py` & `kan_gpt-0.4.0/tests/test_train.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 import torch
+
 from kan_gpt.mingpt.model import GPT as MLP_GPT
 from kan_gpt.train import save_model, main
+from kan_gpt.download_dataset import download_tinyshakespeare
 
 VOCAB_SIZE = 8
 BLOCK_SIZE = 16
 MODEL_TYPE = "gpt-pico"
 
 
 def get_gpt_model() -> MLP_GPT:
@@ -31,23 +33,25 @@
         for name, param in model.named_parameters():
             assert torch.equal(param, model_loaded.state_dict()[name]), (
                 f"Model not saved correctly at {save_path}, parameter "
                 f"{name} does not match original model"
             )
 
 
-# def test_train():
+def test_train():
+    download_tinyshakespeare()
 
-#     # TODO: Download mini dataset for testing
+    class Args:
+        model_type = MODEL_TYPE
+        dummy_dataset = True
+        learning_rate = 5e-3
+        max_iters = 1
+        num_workers = 0
+        batch_size = 1
+        dataset = "tinyshakespeare"
+        architecture = "MLP"
+        device = "cpu"
 
-#     class Args:
-#         model_type = MODEL_TYPE
-#         dummy_dataset = True
-#         learning_rate = 5e-3
-#         max_iters = 1
-#         num_workers = 0
-#         batch_size = 1
-#         architecture = "KAN"
-#         device = "cpu"
+    os.environ["WANDB_DISABLED"] = "true"
 
-#     args = Args()
-#     main(args)
+    args = Args()
+    main(args)
```

