# Comparing `tmp/imodelsx-1.0.4.tar.gz` & `tmp/imodelsx-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imodelsx-1.0.4.tar", last modified: Mon May  6 13:35:00 2024, max compression
+gzip compressed data, was "imodelsx-1.0.5.tar", last modified: Wed May  8 13:22:01 2024, max compression
```

## Comparing `imodelsx-1.0.4.tar` & `imodelsx-1.0.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 13:35:00.084609 imodelsx-1.0.4/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-05-06 13:35:00.084609 imodelsx-1.0.4/PKG-INFO
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 13:35:00.080609 imodelsx-1.0.4/imodelsx/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      653 2024-05-06 13:13:22.000000 imodelsx-1.0.4/imodelsx/__init__.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 13:35:00.080609 imodelsx-1.0.4/imodelsx/auglinear/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 23:40:44.000000 imodelsx-1.0.4/imodelsx/auglinear/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17684 2024-02-13 16:34:50.000000 imodelsx-1.0.4/imodelsx/auglinear/auglinear.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7082 2024-02-13 16:36:25.000000 imodelsx-1.0.4/imodelsx/auglinear/embed.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 13:35:00.080609 imodelsx-1.0.4/imodelsx/augtree/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-24 23:36:41.000000 imodelsx-1.0.4/imodelsx/augtree/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11437 2023-04-07 17:36:23.000000 imodelsx-1.0.4/imodelsx/augtree/augtree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1273 2023-11-02 14:39:42.000000 imodelsx-1.0.4/imodelsx/augtree/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6465 2023-11-02 14:40:10.000000 imodelsx-1.0.4/imodelsx/augtree/embed.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2234 2023-02-06 22:48:13.000000 imodelsx-1.0.4/imodelsx/augtree/ensemble.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2380 2023-04-07 16:31:41.000000 imodelsx-1.0.4/imodelsx/augtree/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16783 2023-04-07 05:20:42.000000 imodelsx-1.0.4/imodelsx/augtree/stump.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3260 2023-11-02 14:40:40.000000 imodelsx-1.0.4/imodelsx/augtree/utils.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2120 2024-03-24 12:39:14.000000 imodelsx-1.0.4/imodelsx/cache_save_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 13:35:00.080609 imodelsx-1.0.4/imodelsx/d3/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 21:38:29.000000 imodelsx-1.0.4/imodelsx/d3/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4312 2023-04-07 05:02:55.000000 imodelsx-1.0.4/imodelsx/d3/d3.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7246 2022-10-04 22:03:12.000000 imodelsx-1.0.4/imodelsx/d3/step1_get_extreme.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7194 2022-10-04 22:27:59.000000 imodelsx-1.0.4/imodelsx/d3/step2_proposer.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8982 2022-10-04 22:12:36.000000 imodelsx-1.0.4/imodelsx/d3/step3_verifier.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6130 2023-07-28 21:36:15.000000 imodelsx-1.0.4/imodelsx/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      282 2023-02-16 23:25:53.000000 imodelsx-1.0.4/imodelsx/dummy_script.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2516 2023-09-13 00:14:38.000000 imodelsx-1.0.4/imodelsx/embeddings.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 13:35:00.080609 imodelsx-1.0.4/imodelsx/iprompt/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      195 2022-10-15 16:18:36.000000 imodelsx-1.0.4/imodelsx/iprompt/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    36551 2023-06-07 16:00:03.000000 imodelsx-1.0.4/imodelsx/iprompt/api.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11285 2023-06-07 16:00:03.000000 imodelsx-1.0.4/imodelsx/iprompt/autoprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      624 2023-02-07 19:15:27.000000 imodelsx-1.0.4/imodelsx/iprompt/data.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2371 2022-10-15 16:18:36.000000 imodelsx-1.0.4/imodelsx/iprompt/gumbel.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14226 2023-05-25 18:26:24.000000 imodelsx-1.0.4/imodelsx/iprompt/hotflip.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    19376 2023-06-07 16:00:03.000000 imodelsx-1.0.4/imodelsx/iprompt/ipromptx.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12909 2023-06-07 16:01:30.000000 imodelsx-1.0.4/imodelsx/iprompt/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1751 2022-10-15 16:18:36.000000 imodelsx-1.0.4/imodelsx/iprompt/prompt_tune.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24166 2023-02-14 20:42:53.000000 imodelsx-1.0.4/imodelsx/iprompt/utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 13:35:00.084609 imodelsx-1.0.4/imodelsx/kan/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 12:53:34.000000 imodelsx-1.0.4/imodelsx/kan/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12031 2024-05-06 13:10:10.000000 imodelsx-1.0.4/imodelsx/kan/kan_modules.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6024 2024-05-06 13:13:18.000000 imodelsx-1.0.4/imodelsx/kan/kan_sklearn.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8220 2024-04-22 20:35:21.000000 imodelsx-1.0.4/imodelsx/linear_finetune.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5618 2023-11-02 14:37:02.000000 imodelsx-1.0.4/imodelsx/linear_ngram.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22977 2024-04-25 16:47:27.000000 imodelsx-1.0.4/imodelsx/llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1577 2023-04-24 18:43:24.000000 imodelsx-1.0.4/imodelsx/metrics.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6214 2024-05-05 15:40:12.000000 imodelsx-1.0.4/imodelsx/process_results.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 13:35:00.084609 imodelsx-1.0.4/imodelsx/sasc/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-05-15 21:34:39.000000 imodelsx-1.0.4/imodelsx/sasc/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5670 2023-06-27 00:56:11.000000 imodelsx-1.0.4/imodelsx/sasc/api.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4951 2023-05-15 20:33:55.000000 imodelsx-1.0.4/imodelsx/sasc/m1_ngrams.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4957 2023-06-27 00:10:16.000000 imodelsx-1.0.4/imodelsx/sasc/m2_summarize.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3543 2023-06-27 00:10:23.000000 imodelsx-1.0.4/imodelsx/sasc/m3_generate.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14860 2024-05-05 12:34:12.000000 imodelsx-1.0.4/imodelsx/submit_utils.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 13:35:00.084609 imodelsx-1.0.4/imodelsx/treeprompt/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-08-30 17:20:13.000000 imodelsx-1.0.4/imodelsx/treeprompt/__init__.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13430 2023-10-10 15:55:49.000000 imodelsx-1.0.4/imodelsx/treeprompt/stump.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6709 2024-04-15 14:14:26.000000 imodelsx-1.0.4/imodelsx/treeprompt/treeprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6342 2023-12-14 18:21:43.000000 imodelsx-1.0.4/imodelsx/util.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8794 2024-01-19 23:29:14.000000 imodelsx-1.0.4/imodelsx/viz.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 13:35:00.080609 imodelsx-1.0.4/imodelsx.egg-info/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12670 2024-05-06 13:35:00.000000 imodelsx-1.0.4/imodelsx.egg-info/PKG-INFO
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1643 2024-05-06 13:35:00.000000 imodelsx-1.0.4/imodelsx.egg-info/SOURCES.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-05-06 13:35:00.000000 imodelsx-1.0.4/imodelsx.egg-info/dependency_links.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      114 2024-05-06 13:35:00.000000 imodelsx-1.0.4/imodelsx.egg-info/requires.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        9 2024-05-06 13:35:00.000000 imodelsx-1.0.4/imodelsx.egg-info/top_level.txt
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-05-06 13:35:00.084609 imodelsx-1.0.4/setup.cfg
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1323 2024-05-06 13:34:38.000000 imodelsx-1.0.4/setup.py
-drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 13:35:00.084609 imodelsx-1.0.4/tests/
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      146 2023-12-13 21:39:12.000000 imodelsx-1.0.4/tests/test_auglinear.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1685 2023-12-13 21:40:29.000000 imodelsx-1.0.4/tests/test_auglinear_pipeline.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5451 2023-04-07 16:34:10.000000 imodelsx-1.0.4/tests/test_augtree.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1099 2023-02-07 19:05:22.000000 imodelsx-1.0.4/tests/test_iprompt.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      917 2024-03-23 14:38:38.000000 imodelsx-1.0.4/tests/test_llm.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1451 2023-04-07 03:36:08.000000 imodelsx-1.0.4/tests/test_ngram_list.py
--rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      786 2023-05-15 21:35:21.000000 imodelsx-1.0.4/tests/test_sasc.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.449416 imodelsx-1.0.5/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13830 2024-05-08 13:22:01.445417 imodelsx-1.0.5/PKG-INFO
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.389415 imodelsx-1.0.5/imodelsx/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      653 2024-05-06 13:13:22.000000 imodelsx-1.0.5/imodelsx/__init__.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.421416 imodelsx-1.0.5/imodelsx/auglinear/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 23:40:44.000000 imodelsx-1.0.5/imodelsx/auglinear/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    17684 2024-02-13 16:34:50.000000 imodelsx-1.0.5/imodelsx/auglinear/auglinear.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7082 2024-02-13 16:36:25.000000 imodelsx-1.0.5/imodelsx/auglinear/embed.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.437416 imodelsx-1.0.5/imodelsx/augtree/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-01-24 23:36:41.000000 imodelsx-1.0.5/imodelsx/augtree/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11437 2023-04-07 17:36:23.000000 imodelsx-1.0.5/imodelsx/augtree/augtree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1273 2023-11-02 14:39:42.000000 imodelsx-1.0.5/imodelsx/augtree/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6465 2023-11-02 14:40:10.000000 imodelsx-1.0.5/imodelsx/augtree/embed.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2234 2023-02-06 22:48:13.000000 imodelsx-1.0.5/imodelsx/augtree/ensemble.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2380 2023-04-07 16:31:41.000000 imodelsx-1.0.5/imodelsx/augtree/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    16783 2023-04-07 05:20:42.000000 imodelsx-1.0.5/imodelsx/augtree/stump.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3260 2023-11-02 14:40:40.000000 imodelsx-1.0.5/imodelsx/augtree/utils.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2120 2024-03-24 12:39:14.000000 imodelsx-1.0.5/imodelsx/cache_save_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.441416 imodelsx-1.0.5/imodelsx/d3/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2022-10-04 21:38:29.000000 imodelsx-1.0.5/imodelsx/d3/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4312 2023-04-07 05:02:55.000000 imodelsx-1.0.5/imodelsx/d3/d3.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7246 2022-10-04 22:03:12.000000 imodelsx-1.0.5/imodelsx/d3/step1_get_extreme.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     7194 2022-10-04 22:27:59.000000 imodelsx-1.0.5/imodelsx/d3/step2_proposer.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8982 2022-10-04 22:12:36.000000 imodelsx-1.0.5/imodelsx/d3/step3_verifier.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6130 2023-07-28 21:36:15.000000 imodelsx-1.0.5/imodelsx/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      282 2023-02-16 23:25:53.000000 imodelsx-1.0.5/imodelsx/dummy_script.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2516 2023-09-13 00:14:38.000000 imodelsx-1.0.5/imodelsx/embeddings.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.441416 imodelsx-1.0.5/imodelsx/iprompt/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      195 2022-10-15 16:18:36.000000 imodelsx-1.0.5/imodelsx/iprompt/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    36551 2023-06-07 16:00:03.000000 imodelsx-1.0.5/imodelsx/iprompt/api.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    11285 2023-06-07 16:00:03.000000 imodelsx-1.0.5/imodelsx/iprompt/autoprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      624 2023-02-07 19:15:27.000000 imodelsx-1.0.5/imodelsx/iprompt/data.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     2371 2022-10-15 16:18:36.000000 imodelsx-1.0.5/imodelsx/iprompt/gumbel.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14226 2023-05-25 18:26:24.000000 imodelsx-1.0.5/imodelsx/iprompt/hotflip.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    19376 2023-06-07 16:00:03.000000 imodelsx-1.0.5/imodelsx/iprompt/ipromptx.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12909 2023-06-07 16:01:30.000000 imodelsx-1.0.5/imodelsx/iprompt/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1751 2022-10-15 16:18:36.000000 imodelsx-1.0.5/imodelsx/iprompt/prompt_tune.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    24166 2023-02-14 20:42:53.000000 imodelsx-1.0.5/imodelsx/iprompt/utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.441416 imodelsx-1.0.5/imodelsx/kan/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-06 12:53:34.000000 imodelsx-1.0.5/imodelsx/kan/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    12031 2024-05-06 13:10:10.000000 imodelsx-1.0.5/imodelsx/kan/kan_modules.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6580 2024-05-08 13:19:10.000000 imodelsx-1.0.5/imodelsx/kan/kan_sklearn.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8220 2024-04-22 20:35:21.000000 imodelsx-1.0.5/imodelsx/linear_finetune.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5618 2023-11-02 14:37:02.000000 imodelsx-1.0.5/imodelsx/linear_ngram.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    22977 2024-04-25 16:47:27.000000 imodelsx-1.0.5/imodelsx/llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1577 2023-04-24 18:43:24.000000 imodelsx-1.0.5/imodelsx/metrics.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6214 2024-05-05 15:40:12.000000 imodelsx-1.0.5/imodelsx/process_results.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.445417 imodelsx-1.0.5/imodelsx/sasc/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-05-15 21:34:39.000000 imodelsx-1.0.5/imodelsx/sasc/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5670 2023-06-27 00:56:11.000000 imodelsx-1.0.5/imodelsx/sasc/api.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4951 2023-05-15 20:33:55.000000 imodelsx-1.0.5/imodelsx/sasc/m1_ngrams.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     4957 2023-06-27 00:10:16.000000 imodelsx-1.0.5/imodelsx/sasc/m2_summarize.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     3543 2023-06-27 00:10:23.000000 imodelsx-1.0.5/imodelsx/sasc/m3_generate.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    14932 2024-05-07 20:58:56.000000 imodelsx-1.0.5/imodelsx/submit_utils.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.445417 imodelsx-1.0.5/imodelsx/treeprompt/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2023-08-30 17:20:13.000000 imodelsx-1.0.5/imodelsx/treeprompt/__init__.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13430 2023-10-10 15:55:49.000000 imodelsx-1.0.5/imodelsx/treeprompt/stump.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6709 2024-04-15 14:14:26.000000 imodelsx-1.0.5/imodelsx/treeprompt/treeprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     6342 2023-12-14 18:21:43.000000 imodelsx-1.0.5/imodelsx/util.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     8794 2024-01-19 23:29:14.000000 imodelsx-1.0.5/imodelsx/viz.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.409415 imodelsx-1.0.5/imodelsx.egg-info/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)    13830 2024-05-08 13:22:01.000000 imodelsx-1.0.5/imodelsx.egg-info/PKG-INFO
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1643 2024-05-08 13:22:01.000000 imodelsx-1.0.5/imodelsx.egg-info/SOURCES.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        1 2024-05-08 13:22:01.000000 imodelsx-1.0.5/imodelsx.egg-info/dependency_links.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      114 2024-05-08 13:22:01.000000 imodelsx-1.0.5/imodelsx.egg-info/requires.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        9 2024-05-08 13:22:01.000000 imodelsx-1.0.5/imodelsx.egg-info/top_level.txt
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)       38 2024-05-08 13:22:01.449416 imodelsx-1.0.5/setup.cfg
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1323 2024-05-08 13:11:33.000000 imodelsx-1.0.5/setup.py
+drwxr-xr-x   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)        0 2024-05-08 13:22:01.445417 imodelsx-1.0.5/tests/
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      146 2023-12-13 21:39:12.000000 imodelsx-1.0.5/tests/test_auglinear.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1685 2023-12-13 21:40:29.000000 imodelsx-1.0.5/tests/test_auglinear_pipeline.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     5451 2023-04-07 16:34:10.000000 imodelsx-1.0.5/tests/test_augtree.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1099 2023-02-07 19:05:22.000000 imodelsx-1.0.5/tests/test_iprompt.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      917 2024-03-23 14:38:38.000000 imodelsx-1.0.5/tests/test_llm.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)     1451 2023-04-07 03:36:08.000000 imodelsx-1.0.5/tests/test_ngram_list.py
+-rw-r--r--   0 REDMOND.chansingh (560039895) REDMOND.domain users (500000513)      786 2023-05-15 21:35:21.000000 imodelsx-1.0.5/tests/test_sasc.py
```

### Comparing `imodelsx-1.0.4/PKG-INFO` & `imodelsx-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodelsx
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to explain a dataset in natural language.
 Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng
 Author-email: chansingh@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,15 @@
 | Tree-Prompt            | [🗂️](http://csinva.io/imodelsX/treeprompt/treeprompt.html), [🔗](https://github.com/csinva/tree-prompt/tree/main), [📄](https://arxiv.org/abs/2310.14034), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/tree_prompt.ipynb),  | Explanation<br/>+ Steering | Generates a tree of prompts to<br/>steer an LLM (*Official*) |
 | iPrompt            | [🗂️](http://csinva.io/imodelsX/iprompt/api.html#imodelsx.iprompt.api.explain_dataset_iprompt), [🔗](https://github.com/csinva/interpretable-autoprompting), [📄](https://arxiv.org/abs/2210.01848), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/iprompt.ipynb) | Explanation<br/>+ Steering | Generates a prompt that<br/>explains patterns in data (*Official*) |
 | AutoPrompt            | ㅤㅤ[🗂️](), [🔗](https://github.com/ucinlp/autoprompt), [📄](https://arxiv.org/abs/2010.15980) | Explanation<br/>+ Steering | Find a natural-language prompt<br/>using input-gradients (⌛ In progress)|
 | D3            | [🗂️](http://csinva.io/imodelsX/d3/d3.html#imodelsx.d3.d3.explain_dataset_d3), [🔗](https://github.com/ruiqi-zhong/DescribeDistributionalDifferences), [📄](https://arxiv.org/abs/2201.12323), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/d3.ipynb) | Explanation | Explain the difference between two distributions |
 | SASC            |   ㅤㅤ[🗂️](https://csinva.io/imodelsX/sasc/api.html), [🔗](https://github.com/microsoft/automated-explanations), [📄](https://arxiv.org/abs/2305.09863) | Explanation | Explain a black-box text module<br/>using an LLM (*Official*) |
 | Aug-Linear            | [🗂️](https://csinva.io/imodelsX/auglinear/auglinear.html), [🔗](https://github.com/microsoft/aug-models), [📄](https://www.nature.com/articles/s41467-023-43713-1), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/aug_imodels.ipynb) | Linear model | Fit better linear model using an LLM<br/>to extract embeddings (*Official*) |
 | Aug-Tree            | [🗂️](https://csinva.io/imodelsX/augtree/augtree.html), [🔗](https://github.com/microsoft/aug-models), [📄](https://www.nature.com/articles/s41467-023-43713-1), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/aug_imodels.ipynb) | Decision tree | Fit better decision tree using an LLM<br/>to expand features (*Official*) |
+| KAN            | [🗂️](https://csinva.io/imodelsX/kan/kan_sklearn.html), [🔗](https://github.com/Blealtan/efficient-kan/tree/master), [📄](https://arxiv.org/abs/2404.19756), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/kan.ipynb) | 2-layer<br/>network | Fit 2-layer Kolmogorov-Arnold network |
 
 <p align="center">
 <a href="https://github.com/csinva/imodelsX/tree/master/demo_notebooks">📖</a>Demo notebooks &emsp; <a href="https://csinva.io/imodelsX/">🗂️</a> Doc &emsp; 🔗 Reference code &emsp; 📄 Research paper
 </br>
 ⌛ We plan to support other interpretable algorithms like <a href="https://arxiv.org/abs/2205.12548">RLPrompt</a>, <a href="https://arxiv.org/abs/2007.04612">CBMs</a>, and <a href="https://arxiv.org/abs/2004.00221">NBDT</a>. If you want to contribute an algorithm, feel free to open a PR 😄
 </p>
 
@@ -207,14 +208,38 @@
 for k, v in sorted(m.coefs_dict_.items(), key=lambda item: item[1], reverse=True)[:8]:
     print('\t', k, round(v, 2))
 print('Most negative ngrams')
 for k, v in sorted(m.coefs_dict_.items(), key=lambda item: item[1])[:8]:
     print('\t', k, round(v, 2))
 ```
 
+# KAN
+```python
+import imodelsx
+from sklearn.datasets import make_classification, make_regression
+from sklearn.metrics import accuracy_score
+import numpy as np
+
+X, y = make_classification(n_samples=5000, n_features=5, n_informative=3)
+model = imodelsx.KANClassifier(hidden_layer_size=64, device='cpu',
+                               regularize_activation=1.0, regularize_entropy=1.0)
+model.fit(X, y)
+y_pred = model.predict(X)
+print('Test acc', accuracy_score(y, y_pred))
+
+# now try regression
+X, y = make_regression(n_samples=5000, n_features=5, n_informative=3)
+model = imodelsx.kan.KANRegressor(hidden_layer_size=64, device='cpu',
+                                  regularize_activation=1.0, regularize_entropy=1.0)
+model.fit(X, y)
+y_pred = model.predict(X)
+print('Test correlation', np.corrcoef(y, y_pred.flatten())[0, 1])
+```
+
+
 # General utilities
 
 ### Easy baselines
 Easy-to-fit baselines that follow the sklearn API.
 
 ```python
 from imodelsx import LinearFinetuneClassifier, LinearNgramClassifier
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodelsx Version: 1.0.4 Summary: Library to explain
+Metadata-Version: 2.1 Name: imodelsx Version: 1.0.5 Summary: Library to explain
 a dataset in natural language. Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah
 Hsu, Yuntian Deng Author-email: chansingh@microsoft.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown
   [https://microsoft.github.io/aug-models/embgam_gif.gif][https://csinva.io/
@@ -46,15 +46,19 @@
 (https://github.com/csinva/imodelsX/blob/master/demo_notebooks/
 aug_imodels.ipynb) | Linear model | Fit better linear model using an LLM
 to extract embeddings (*Official*) | | Aug-Tree | [ðï¸](https://csinva.io/
 imodelsX/augtree/augtree.html), [ð](https://github.com/microsoft/aug-
 models), [ð](https://www.nature.com/articles/s41467-023-43713-1), [ð]
 (https://github.com/csinva/imodelsX/blob/master/demo_notebooks/
 aug_imodels.ipynb) | Decision tree | Fit better decision tree using an LLM
-to expand features (*Official*) |
+to expand features (*Official*) | | KAN | [ðï¸](https://csinva.io/imodelsX/
+kan/kan_sklearn.html), [ð](https://github.com/Blealtan/efficient-kan/tree/
+master), [ð](https://arxiv.org/abs/2404.19756), [ð](https://github.com/
+csinva/imodelsX/blob/master/demo_notebooks/kan.ipynb) | 2-layer
+network | Fit 2-layer Kolmogorov-Arnold network |
  _ð___Demo notebooks   _ð____ï_¸_ Doc   ð Reference code   ð Research paper
 â We plan to support other interpretable algorithms like _R_L_P_r_o_m_p_t, _C_B_M_s, and
    _N_B_D_T. If you want to contribute an algorithm, feel free to open a PR ð
 **General utilities** | Model | Reference | | :-------------------------- | ---
 --------------------------------------------------------- | | [ðï¸](https:/
 /csinva.io/imodelsX/llm.html) LLM wrapper| Easily call different LLMs | |
 [ðï¸](https://csinva.io/imodelsX/data.html) Dataset wrapper| Download
@@ -118,17 +122,28 @@
 ( checkpoint='textattack/distilbert-base-uncased-rotten-tomatoes', ngrams=2, #
 use bigrams ) m.fit(dset['text'], dset['label']) # predict preds = m.predict
 (dset_val['text']) print('acc_val', np.mean(preds == dset_val['label'])) #
 interpret print('Total ngram coefficients: ', len(m.coefs_dict_)) print('Most
 positive ngrams') for k, v in sorted(m.coefs_dict_.items(), key=lambda item:
 item[1], reverse=True)[:8]: print('\t', k, round(v, 2)) print('Most negative
 ngrams') for k, v in sorted(m.coefs_dict_.items(), key=lambda item: item[1])[:
-8]: print('\t', k, round(v, 2)) ``` # General utilities ### Easy baselines
-Easy-to-fit baselines that follow the sklearn API. ```python from imodelsx
-import LinearFinetuneClassifier, LinearNgramClassifier # fit a simple one-layer
+8]: print('\t', k, round(v, 2)) ``` # KAN ```python import imodelsx from
+sklearn.datasets import make_classification, make_regression from
+sklearn.metrics import accuracy_score import numpy as np X, y =
+make_classification(n_samples=5000, n_features=5, n_informative=3) model =
+imodelsx.KANClassifier(hidden_layer_size=64, device='cpu',
+regularize_activation=1.0, regularize_entropy=1.0) model.fit(X, y) y_pred =
+model.predict(X) print('Test acc', accuracy_score(y, y_pred)) # now try
+regression X, y = make_regression(n_samples=5000, n_features=5,
+n_informative=3) model = imodelsx.kan.KANRegressor(hidden_layer_size=64,
+device='cpu', regularize_activation=1.0, regularize_entropy=1.0) model.fit(X,
+y) y_pred = model.predict(X) print('Test correlation', np.corrcoef(y,
+y_pred.flatten())[0, 1]) ``` # General utilities ### Easy baselines Easy-to-fit
+baselines that follow the sklearn API. ```python from imodelsx import
+LinearFinetuneClassifier, LinearNgramClassifier # fit a simple one-layer
 finetune on top of LLM embeddings m = LinearFinetuneClassifier
 ( checkpoint='distilbert-base-uncased', ) m.fit(dset['text'], dset['label'])
 preds = m.predict(dset_val['text']) acc = (preds == dset_val['label']).mean()
 print('validation acc', acc) ``` ### LLM wrapper Easy API for calling different
 language models with caching (much more lightweight than [langchain](https://
 github.com/langchain-ai/langchain)). ```python import imodelsx.llm # supports
 any huggingface checkpoint or openai checkpoint (including chat models) llm =
```

### Comparing `imodelsx-1.0.4/imodelsx/__init__.py` & `imodelsx-1.0.5/imodelsx/__init__.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/auglinear/auglinear.py` & `imodelsx-1.0.5/imodelsx/auglinear/auglinear.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/auglinear/embed.py` & `imodelsx-1.0.5/imodelsx/auglinear/embed.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/augtree/augtree.py` & `imodelsx-1.0.5/imodelsx/augtree/augtree.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/augtree/data.py` & `imodelsx-1.0.5/imodelsx/augtree/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/augtree/embed.py` & `imodelsx-1.0.5/imodelsx/augtree/embed.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/augtree/ensemble.py` & `imodelsx-1.0.5/imodelsx/augtree/ensemble.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/augtree/llm.py` & `imodelsx-1.0.5/imodelsx/augtree/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/augtree/stump.py` & `imodelsx-1.0.5/imodelsx/augtree/stump.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/augtree/utils.py` & `imodelsx-1.0.5/imodelsx/augtree/utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/cache_save_utils.py` & `imodelsx-1.0.5/imodelsx/cache_save_utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/d3/d3.py` & `imodelsx-1.0.5/imodelsx/d3/d3.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/d3/step1_get_extreme.py` & `imodelsx-1.0.5/imodelsx/d3/step1_get_extreme.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/d3/step2_proposer.py` & `imodelsx-1.0.5/imodelsx/d3/step2_proposer.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/d3/step3_verifier.py` & `imodelsx-1.0.5/imodelsx/d3/step3_verifier.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/data.py` & `imodelsx-1.0.5/imodelsx/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/embeddings.py` & `imodelsx-1.0.5/imodelsx/embeddings.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/iprompt/api.py` & `imodelsx-1.0.5/imodelsx/iprompt/api.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/iprompt/autoprompt.py` & `imodelsx-1.0.5/imodelsx/iprompt/autoprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/iprompt/data.py` & `imodelsx-1.0.5/imodelsx/iprompt/data.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/iprompt/gumbel.py` & `imodelsx-1.0.5/imodelsx/iprompt/gumbel.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/iprompt/hotflip.py` & `imodelsx-1.0.5/imodelsx/iprompt/hotflip.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/iprompt/ipromptx.py` & `imodelsx-1.0.5/imodelsx/iprompt/ipromptx.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/iprompt/llm.py` & `imodelsx-1.0.5/imodelsx/iprompt/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/iprompt/prompt_tune.py` & `imodelsx-1.0.5/imodelsx/iprompt/prompt_tune.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/iprompt/utils.py` & `imodelsx-1.0.5/imodelsx/iprompt/utils.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/kan/kan_modules.py` & `imodelsx-1.0.5/imodelsx/kan/kan_modules.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/kan/kan_sklearn.py` & `imodelsx-1.0.5/imodelsx/kan/kan_sklearn.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,28 +10,43 @@
 from imodelsx.kan.kan_modules import KANModule, KANGAMModule
 from sklearn.datasets import make_classification, make_regression
 from sklearn.metrics import accuracy_score
 
 
 class KAN(BaseEstimator):
     def __init__(self, hidden_layer_size=64, device='cpu',
-                 regularize_activation=1.0, regularize_entropy=1.0, regularize_ridge=0.0):
+                 regularize_activation=1.0, regularize_entropy=1.0, regularize_ridge=0.0,
+                 **kwargs):
         '''
         Params
         ------
         hidden_layer_size : int
             Number of neurons in the hidden layer.
+        regularize_activation: float
+            Activation regularization parameter
+        regularize_entropy: float
+            Entropy regularization parameter
         regularize_ridge: float
             Ridge regularization parameter (only applies to KANGAM)
+        kwargs can be any of these more detailed KAN parameters
+            grid_size=5,
+            spline_order=3,
+            scale_noise=0.1,
+            scale_base=1.0,
+            scale_spline=1.0,
+            base_activation=torch.nn.SiLU,
+            grid_eps=0.02,
+            grid_range=[-1, 1],
         '''
         self.hidden_layer_size = hidden_layer_size
         self.device = device
         self.regularize_activation = regularize_activation
         self.regularize_entropy = regularize_entropy
         self.regularize_ridge = regularize_ridge
+        self.kwargs = kwargs
 
     def fit(self, X, y, batch_size=512, lr=1e-3, weight_decay=1e-4, gamma=0.8):
         if isinstance(self, ClassifierMixin):
             check_classification_targets(y)
             self.classes_, y = np.unique(y, return_inverse=True)
             num_outputs = len(self.classes_)
             y = torch.tensor(y, dtype=torch.long)
@@ -41,14 +56,15 @@
         X = torch.tensor(X, dtype=torch.float32)
         num_features = X.shape[1]
         if isinstance(self, (KANGAMClassifier, KANGAMRegressor)):
             self.model = KANGAMModule(
                 num_features=num_features,
                 hidden_layer_size=self.hidden_layer_size,
                 n_classes=num_outputs,
+                **self.kwargs
             ).to(self.device)
         else:
             self.model = KANModule(
                 layers_hidden=[num_features,
                                self.hidden_layer_size, num_outputs]
             ).to(self.device)
```

### Comparing `imodelsx-1.0.4/imodelsx/linear_finetune.py` & `imodelsx-1.0.5/imodelsx/linear_finetune.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/linear_ngram.py` & `imodelsx-1.0.5/imodelsx/linear_ngram.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/llm.py` & `imodelsx-1.0.5/imodelsx/llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/metrics.py` & `imodelsx-1.0.5/imodelsx/metrics.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/process_results.py` & `imodelsx-1.0.5/imodelsx/process_results.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/sasc/api.py` & `imodelsx-1.0.5/imodelsx/sasc/api.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/sasc/m1_ngrams.py` & `imodelsx-1.0.5/imodelsx/sasc/m1_ngrams.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/sasc/m2_summarize.py` & `imodelsx-1.0.5/imodelsx/sasc/m2_summarize.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/sasc/m3_generate.py` & `imodelsx-1.0.5/imodelsx/sasc/m3_generate.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/submit_utils.py` & `imodelsx-1.0.5/imodelsx/submit_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,17 +112,18 @@
             run_slurm(param_str, slurm_kwargs=slurm_kwargs)
         return
     elif amlt_kwargs is not None:
         assert 'amlt_file' in amlt_kwargs
         sku = amlt_kwargs.get('sku', 'G1')
         process_count_per_node = amlt_kwargs.get('process_count_per_node', 1)
         amlt_dir = dirname(amlt_kwargs['amlt_file'])
+        repo_dir = dirname(amlt_dir)
         amlt_text = open(amlt_kwargs['amlt_file'], 'r').read()
         assert amlt_text.endswith('jobs:'), 'amlt file must end with jobs:'
-        script_name = script_name.replace(amlt_dir, '').strip('/')
+        script_name = script_name.replace(repo_dir, '').strip('/')
         param_str_list = [_param_str_from_args(
             args, cmd_python, script_name) for args in args_list]
         if 'mnt_rename' in amlt_kwargs:
             param_str_list = [
                 param_str.replace(
                     amlt_kwargs['mnt_rename'][0], amlt_kwargs['mnt_rename'][1])
                 for param_str in param_str_list
@@ -132,14 +133,15 @@
         logs_dir = join(amlt_dir, 'logs')
         os.makedirs(logs_dir, exist_ok=True)
         job_template = '''
 - name: {name}
   process_count_per_node: {process_count_per_node}
   sku: {sku}
   command:
+  - echo "{param_str}"
   - {param_str}'''
         out_file = join(logs_dir, sha256({'s': str(param_str_list)}) + '.yaml')
         s = amlt_text
         for i, param_str in enumerate(param_str_list):
             job_text = job_template.format(
                 name=f'{sku}_job_{i}',
                 process_count_per_node=process_count_per_node,
@@ -278,17 +280,18 @@
             gpu_str = ','.join([str(x) for x in gpu_id])
         else:
             gpu_str = str(gpu_id)
         prefix = f'CUDA_VISIBLE_DEVICES={gpu_str} '
         param_str = prefix + param_str
         print(
             f'\n\n-------------------{i + 1}/{n}--------------------\n' + param_str)
-        output = subprocess.run(
-            param_str, shell=True, check=True,
+        subprocess.run(
+            param_str, check=True, shell=True
         )
+        print('here')
     except KeyboardInterrupt:
         print('Keyboard interrupt, exiting...')
         exit(0)
     except subprocess.CalledProcessError as e:
         print('CalledProcessError', e)
         print(f'{ident}: Finished on GPU(s) {gpu_id}')
         failed_job = (i, param_str)
```

### Comparing `imodelsx-1.0.4/imodelsx/treeprompt/stump.py` & `imodelsx-1.0.5/imodelsx/treeprompt/stump.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/treeprompt/treeprompt.py` & `imodelsx-1.0.5/imodelsx/treeprompt/treeprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/util.py` & `imodelsx-1.0.5/imodelsx/util.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx/viz.py` & `imodelsx-1.0.5/imodelsx/viz.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/imodelsx.egg-info/PKG-INFO` & `imodelsx-1.0.5/imodelsx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imodelsx
-Version: 1.0.4
+Version: 1.0.5
 Summary: Library to explain a dataset in natural language.
 Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng
 Author-email: chansingh@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,15 @@
 | Tree-Prompt            | [🗂️](http://csinva.io/imodelsX/treeprompt/treeprompt.html), [🔗](https://github.com/csinva/tree-prompt/tree/main), [📄](https://arxiv.org/abs/2310.14034), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/tree_prompt.ipynb),  | Explanation<br/>+ Steering | Generates a tree of prompts to<br/>steer an LLM (*Official*) |
 | iPrompt            | [🗂️](http://csinva.io/imodelsX/iprompt/api.html#imodelsx.iprompt.api.explain_dataset_iprompt), [🔗](https://github.com/csinva/interpretable-autoprompting), [📄](https://arxiv.org/abs/2210.01848), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/iprompt.ipynb) | Explanation<br/>+ Steering | Generates a prompt that<br/>explains patterns in data (*Official*) |
 | AutoPrompt            | ㅤㅤ[🗂️](), [🔗](https://github.com/ucinlp/autoprompt), [📄](https://arxiv.org/abs/2010.15980) | Explanation<br/>+ Steering | Find a natural-language prompt<br/>using input-gradients (⌛ In progress)|
 | D3            | [🗂️](http://csinva.io/imodelsX/d3/d3.html#imodelsx.d3.d3.explain_dataset_d3), [🔗](https://github.com/ruiqi-zhong/DescribeDistributionalDifferences), [📄](https://arxiv.org/abs/2201.12323), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/d3.ipynb) | Explanation | Explain the difference between two distributions |
 | SASC            |   ㅤㅤ[🗂️](https://csinva.io/imodelsX/sasc/api.html), [🔗](https://github.com/microsoft/automated-explanations), [📄](https://arxiv.org/abs/2305.09863) | Explanation | Explain a black-box text module<br/>using an LLM (*Official*) |
 | Aug-Linear            | [🗂️](https://csinva.io/imodelsX/auglinear/auglinear.html), [🔗](https://github.com/microsoft/aug-models), [📄](https://www.nature.com/articles/s41467-023-43713-1), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/aug_imodels.ipynb) | Linear model | Fit better linear model using an LLM<br/>to extract embeddings (*Official*) |
 | Aug-Tree            | [🗂️](https://csinva.io/imodelsX/augtree/augtree.html), [🔗](https://github.com/microsoft/aug-models), [📄](https://www.nature.com/articles/s41467-023-43713-1), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/aug_imodels.ipynb) | Decision tree | Fit better decision tree using an LLM<br/>to expand features (*Official*) |
+| KAN            | [🗂️](https://csinva.io/imodelsX/kan/kan_sklearn.html), [🔗](https://github.com/Blealtan/efficient-kan/tree/master), [📄](https://arxiv.org/abs/2404.19756), [📖](https://github.com/csinva/imodelsX/blob/master/demo_notebooks/kan.ipynb) | 2-layer<br/>network | Fit 2-layer Kolmogorov-Arnold network |
 
 <p align="center">
 <a href="https://github.com/csinva/imodelsX/tree/master/demo_notebooks">📖</a>Demo notebooks &emsp; <a href="https://csinva.io/imodelsX/">🗂️</a> Doc &emsp; 🔗 Reference code &emsp; 📄 Research paper
 </br>
 ⌛ We plan to support other interpretable algorithms like <a href="https://arxiv.org/abs/2205.12548">RLPrompt</a>, <a href="https://arxiv.org/abs/2007.04612">CBMs</a>, and <a href="https://arxiv.org/abs/2004.00221">NBDT</a>. If you want to contribute an algorithm, feel free to open a PR 😄
 </p>
 
@@ -207,14 +208,38 @@
 for k, v in sorted(m.coefs_dict_.items(), key=lambda item: item[1], reverse=True)[:8]:
     print('\t', k, round(v, 2))
 print('Most negative ngrams')
 for k, v in sorted(m.coefs_dict_.items(), key=lambda item: item[1])[:8]:
     print('\t', k, round(v, 2))
 ```
 
+# KAN
+```python
+import imodelsx
+from sklearn.datasets import make_classification, make_regression
+from sklearn.metrics import accuracy_score
+import numpy as np
+
+X, y = make_classification(n_samples=5000, n_features=5, n_informative=3)
+model = imodelsx.KANClassifier(hidden_layer_size=64, device='cpu',
+                               regularize_activation=1.0, regularize_entropy=1.0)
+model.fit(X, y)
+y_pred = model.predict(X)
+print('Test acc', accuracy_score(y, y_pred))
+
+# now try regression
+X, y = make_regression(n_samples=5000, n_features=5, n_informative=3)
+model = imodelsx.kan.KANRegressor(hidden_layer_size=64, device='cpu',
+                                  regularize_activation=1.0, regularize_entropy=1.0)
+model.fit(X, y)
+y_pred = model.predict(X)
+print('Test correlation', np.corrcoef(y, y_pred.flatten())[0, 1])
+```
+
+
 # General utilities
 
 ### Easy baselines
 Easy-to-fit baselines that follow the sklearn API.
 
 ```python
 from imodelsx import LinearFinetuneClassifier, LinearNgramClassifier
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: imodelsx Version: 1.0.4 Summary: Library to explain
+Metadata-Version: 2.1 Name: imodelsx Version: 1.0.5 Summary: Library to explain
 a dataset in natural language. Home-page: https://github.com/csinva/imodelsX
 Author: Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah
 Hsu, Yuntian Deng Author-email: chansingh@microsoft.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown
   [https://microsoft.github.io/aug-models/embgam_gif.gif][https://csinva.io/
@@ -46,15 +46,19 @@
 (https://github.com/csinva/imodelsX/blob/master/demo_notebooks/
 aug_imodels.ipynb) | Linear model | Fit better linear model using an LLM
 to extract embeddings (*Official*) | | Aug-Tree | [ðï¸](https://csinva.io/
 imodelsX/augtree/augtree.html), [ð](https://github.com/microsoft/aug-
 models), [ð](https://www.nature.com/articles/s41467-023-43713-1), [ð]
 (https://github.com/csinva/imodelsX/blob/master/demo_notebooks/
 aug_imodels.ipynb) | Decision tree | Fit better decision tree using an LLM
-to expand features (*Official*) |
+to expand features (*Official*) | | KAN | [ðï¸](https://csinva.io/imodelsX/
+kan/kan_sklearn.html), [ð](https://github.com/Blealtan/efficient-kan/tree/
+master), [ð](https://arxiv.org/abs/2404.19756), [ð](https://github.com/
+csinva/imodelsX/blob/master/demo_notebooks/kan.ipynb) | 2-layer
+network | Fit 2-layer Kolmogorov-Arnold network |
  _ð___Demo notebooks   _ð____ï_¸_ Doc   ð Reference code   ð Research paper
 â We plan to support other interpretable algorithms like _R_L_P_r_o_m_p_t, _C_B_M_s, and
    _N_B_D_T. If you want to contribute an algorithm, feel free to open a PR ð
 **General utilities** | Model | Reference | | :-------------------------- | ---
 --------------------------------------------------------- | | [ðï¸](https:/
 /csinva.io/imodelsX/llm.html) LLM wrapper| Easily call different LLMs | |
 [ðï¸](https://csinva.io/imodelsX/data.html) Dataset wrapper| Download
@@ -118,17 +122,28 @@
 ( checkpoint='textattack/distilbert-base-uncased-rotten-tomatoes', ngrams=2, #
 use bigrams ) m.fit(dset['text'], dset['label']) # predict preds = m.predict
 (dset_val['text']) print('acc_val', np.mean(preds == dset_val['label'])) #
 interpret print('Total ngram coefficients: ', len(m.coefs_dict_)) print('Most
 positive ngrams') for k, v in sorted(m.coefs_dict_.items(), key=lambda item:
 item[1], reverse=True)[:8]: print('\t', k, round(v, 2)) print('Most negative
 ngrams') for k, v in sorted(m.coefs_dict_.items(), key=lambda item: item[1])[:
-8]: print('\t', k, round(v, 2)) ``` # General utilities ### Easy baselines
-Easy-to-fit baselines that follow the sklearn API. ```python from imodelsx
-import LinearFinetuneClassifier, LinearNgramClassifier # fit a simple one-layer
+8]: print('\t', k, round(v, 2)) ``` # KAN ```python import imodelsx from
+sklearn.datasets import make_classification, make_regression from
+sklearn.metrics import accuracy_score import numpy as np X, y =
+make_classification(n_samples=5000, n_features=5, n_informative=3) model =
+imodelsx.KANClassifier(hidden_layer_size=64, device='cpu',
+regularize_activation=1.0, regularize_entropy=1.0) model.fit(X, y) y_pred =
+model.predict(X) print('Test acc', accuracy_score(y, y_pred)) # now try
+regression X, y = make_regression(n_samples=5000, n_features=5,
+n_informative=3) model = imodelsx.kan.KANRegressor(hidden_layer_size=64,
+device='cpu', regularize_activation=1.0, regularize_entropy=1.0) model.fit(X,
+y) y_pred = model.predict(X) print('Test correlation', np.corrcoef(y,
+y_pred.flatten())[0, 1]) ``` # General utilities ### Easy baselines Easy-to-fit
+baselines that follow the sklearn API. ```python from imodelsx import
+LinearFinetuneClassifier, LinearNgramClassifier # fit a simple one-layer
 finetune on top of LLM embeddings m = LinearFinetuneClassifier
 ( checkpoint='distilbert-base-uncased', ) m.fit(dset['text'], dset['label'])
 preds = m.predict(dset_val['text']) acc = (preds == dset_val['label']).mean()
 print('validation acc', acc) ``` ### LLM wrapper Easy API for calling different
 language models with caching (much more lightweight than [langchain](https://
 github.com/langchain-ai/langchain)). ```python import imodelsx.llm # supports
 any huggingface checkpoint or openai checkpoint (including chat models) llm =
```

### Comparing `imodelsx-1.0.4/imodelsx.egg-info/SOURCES.txt` & `imodelsx-1.0.5/imodelsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/setup.py` & `imodelsx-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # 'InstructorEmbedding', # embeddings for emb_diff_module
     # 'sentence-transformers', # embeddings for emb_diff_module
     # pdoc3 # for generating docs
 ]
 
 setuptools.setup(
     name="imodelsx",
-    version="1.0.4",
+    version="1.0.5",
     author="Chandan Singh, John X. Morris, Armin Askari, Divyanshu Aggarwal, Aliyah Hsu, Yuntian Deng",
     author_email="chansingh@microsoft.com",
     description="Library to explain a dataset in natural language.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/csinva/imodelsX",
     packages=setuptools.find_packages(
```

### Comparing `imodelsx-1.0.4/tests/test_auglinear_pipeline.py` & `imodelsx-1.0.5/tests/test_auglinear_pipeline.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/tests/test_augtree.py` & `imodelsx-1.0.5/tests/test_augtree.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/tests/test_iprompt.py` & `imodelsx-1.0.5/tests/test_iprompt.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/tests/test_llm.py` & `imodelsx-1.0.5/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/tests/test_ngram_list.py` & `imodelsx-1.0.5/tests/test_ngram_list.py`

 * *Files identical despite different names*

### Comparing `imodelsx-1.0.4/tests/test_sasc.py` & `imodelsx-1.0.5/tests/test_sasc.py`

 * *Files identical despite different names*

