# Comparing `tmp/langcheck-0.6.0.tar.gz` & `tmp/langcheck-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langcheck-0.6.0.tar", last modified: Sun Apr  7 14:25:00 2024, max compression
+gzip compressed data, was "langcheck-0.7.0.tar", last modified: Wed May  8 10:39:01 2024, max compression
```

## Comparing `langcheck-0.6.0.tar` & `langcheck-0.7.0.tar`

### file list

```diff
@@ -1,91 +1,133 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:25:00.001309 langcheck-0.6.0/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2023-10-10 09:38:20.000000 langcheck-0.6.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10386 2024-04-07 14:24:59.993419 langcheck-0.6.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6957 2024-04-07 14:19:34.000000 langcheck-0.6.0/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2729 2024-04-07 14:20:39.000000 langcheck-0.6.0/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      160 2024-04-07 14:25:00.018462 langcheck-0.6.0/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:56.856671 langcheck-0.6.0/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:57.329232 langcheck-0.6.0/src/langcheck/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      103 2023-11-06 02:00:48.000000 langcheck-0.6.0/src/langcheck/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      486 2023-11-16 07:47:37.000000 langcheck-0.6.0/src/langcheck/_handle_logs.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:57.587521 langcheck-0.6.0/src/langcheck/augment/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      554 2024-04-03 02:39:44.000000 langcheck-0.6.0/src/langcheck/augment/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:57.835399 langcheck-0.6.0/src/langcheck/augment/en/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      523 2023-12-26 07:19:48.000000 langcheck-0.6.0/src/langcheck/augment/en/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1424 2023-11-16 07:47:37.000000 langcheck-0.6.0/src/langcheck/augment/en/_change_case.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:57.928393 langcheck-0.6.0/src/langcheck/augment/en/_gender/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-12-26 07:19:48.000000 langcheck-0.6.0/src/langcheck/augment/en/_gender/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4173 2024-03-02 07:03:11.000000 langcheck-0.6.0/src/langcheck/augment/en/_gender/_gender.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3851 2023-12-26 07:19:49.000000 langcheck-0.6.0/src/langcheck/augment/en/_gender/_gender_pronouns.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2697 2023-11-16 07:47:37.000000 langcheck-0.6.0/src/langcheck/augment/en/_keyboard_typo.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2364 2023-11-16 07:47:37.000000 langcheck-0.6.0/src/langcheck/augment/en/_ocr_typo.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1364 2023-11-16 07:47:37.000000 langcheck-0.6.0/src/langcheck/augment/en/_remove_punctuation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4448 2023-12-26 07:19:49.000000 langcheck-0.6.0/src/langcheck/augment/en/_rephrase.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1815 2023-11-16 07:47:37.000000 langcheck-0.6.0/src/langcheck/augment/en/_synonym.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:58.006735 langcheck-0.6.0/src/langcheck/augment/ja/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       73 2024-02-29 10:04:37.000000 langcheck-0.6.0/src/langcheck/augment/ja/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2076 2024-04-03 09:30:38.000000 langcheck-0.6.0/src/langcheck/augment/ja/_synonym.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:58.243062 langcheck-0.6.0/src/langcheck/metrics/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2090 2024-04-03 02:39:44.000000 langcheck-0.6.0/src/langcheck/metrics/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5851 2024-04-07 14:19:34.000000 langcheck-0.6.0/src/langcheck/metrics/_pairwise_text_quality_utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9754 2024-04-02 00:47:28.000000 langcheck-0.6.0/src/langcheck/metrics/_validation.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:58.505336 langcheck-0.6.0/src/langcheck/metrics/de/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      905 2024-02-29 10:04:38.000000 langcheck-0.6.0/src/langcheck/metrics/de/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      632 2024-02-29 10:04:38.000000 langcheck-0.6.0/src/langcheck/metrics/de/_tokenizers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2741 2024-03-18 09:06:28.000000 langcheck-0.6.0/src/langcheck/metrics/de/_translation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10321 2024-03-18 09:06:28.000000 langcheck-0.6.0/src/langcheck/metrics/de/reference_based_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    34864 2024-04-01 07:06:32.000000 langcheck-0.6.0/src/langcheck/metrics/de/reference_free_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15159 2024-04-01 07:06:32.000000 langcheck-0.6.0/src/langcheck/metrics/de/source_based_text_quality.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:58.725176 langcheck-0.6.0/src/langcheck/metrics/en/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      858 2024-04-02 00:47:28.000000 langcheck-0.6.0/src/langcheck/metrics/en/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10829 2024-04-07 14:19:34.000000 langcheck-0.6.0/src/langcheck/metrics/en/_openai.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12280 2024-04-07 14:19:34.000000 langcheck-0.6.0/src/langcheck/metrics/en/pairwise_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10402 2024-03-18 09:06:28.000000 langcheck-0.6.0/src/langcheck/metrics/en/reference_based_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    35608 2024-04-01 07:06:32.000000 langcheck-0.6.0/src/langcheck/metrics/en/reference_free_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18411 2024-04-01 07:06:32.000000 langcheck-0.6.0/src/langcheck/metrics/en/source_based_text_quality.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:58.978442 langcheck-0.6.0/src/langcheck/metrics/ja/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      857 2024-04-07 14:19:34.000000 langcheck-0.6.0/src/langcheck/metrics/ja/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3468 2023-11-16 07:47:37.000000 langcheck-0.6.0/src/langcheck/metrics/ja/_tokenizers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12880 2024-04-07 14:19:34.000000 langcheck-0.6.0/src/langcheck/metrics/ja/pairwise_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11042 2024-03-18 09:06:29.000000 langcheck-0.6.0/src/langcheck/metrics/ja/reference_based_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    35325 2024-04-01 07:06:32.000000 langcheck-0.6.0/src/langcheck/metrics/ja/reference_free_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11656 2024-04-01 07:06:32.000000 langcheck-0.6.0/src/langcheck/metrics/ja/source_based_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11027 2024-04-02 00:47:28.000000 langcheck-0.6.0/src/langcheck/metrics/metric_value.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:59.105170 langcheck-0.6.0/src/langcheck/metrics/model_manager/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       70 2024-03-02 07:03:12.000000 langcheck-0.6.0/src/langcheck/metrics/model_manager/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4189 2024-03-18 09:06:29.000000 langcheck-0.6.0/src/langcheck/metrics/model_manager/_model_loader.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11909 2024-03-18 09:06:29.000000 langcheck-0.6.0/src/langcheck/metrics/model_manager/_model_management.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:59.163359 langcheck-0.6.0/src/langcheck/metrics/model_manager/config/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3596 2024-03-18 09:06:29.000000 langcheck-0.6.0/src/langcheck/metrics/model_manager/config/metric_config.yaml
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1814 2023-12-07 09:44:42.000000 langcheck-0.6.0/src/langcheck/metrics/reference_based_text_quality.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:59.276076 langcheck-0.6.0/src/langcheck/metrics/scorer/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4855 2024-04-03 02:48:06.000000 langcheck-0.6.0/src/langcheck/metrics/scorer/_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6481 2024-03-18 09:06:30.000000 langcheck-0.6.0/src/langcheck/metrics/scorer/detoxify_models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5656 2024-03-18 09:06:30.000000 langcheck-0.6.0/src/langcheck/metrics/scorer/hf_models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2248 2024-03-18 09:06:30.000000 langcheck-0.6.0/src/langcheck/metrics/scorer/openai_models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14772 2023-12-07 09:44:42.000000 langcheck-0.6.0/src/langcheck/metrics/text_structure.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:59.474024 langcheck-0.6.0/src/langcheck/metrics/zh/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      547 2024-03-02 07:03:12.000000 langcheck-0.6.0/src/langcheck/metrics/zh/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2560 2024-03-02 07:03:12.000000 langcheck-0.6.0/src/langcheck/metrics/zh/_tokenizers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11629 2024-04-03 09:30:38.000000 langcheck-0.6.0/src/langcheck/metrics/zh/reference_based_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14853 2024-04-01 07:06:32.000000 langcheck-0.6.0/src/langcheck/metrics/zh/reference_free_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5809 2024-04-01 07:06:32.000000 langcheck-0.6.0/src/langcheck/metrics/zh/source_based_text_quality.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:59.746827 langcheck-0.6.0/src/langcheck/plot/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      128 2023-10-10 09:38:20.000000 langcheck-0.6.0/src/langcheck/plot/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      538 2023-10-10 09:38:20.000000 langcheck-0.6.0/src/langcheck/plot/_css.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4112 2023-11-06 02:01:01.000000 langcheck-0.6.0/src/langcheck/plot/_histogram.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15343 2024-04-02 00:47:28.000000 langcheck-0.6.0/src/langcheck/plot/_scatter.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1303 2023-11-06 02:01:01.000000 langcheck-0.6.0/src/langcheck/plot/_utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1940 2023-10-10 09:38:20.000000 langcheck-0.6.0/src/langcheck/stats.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:59.887412 langcheck-0.6.0/src/langcheck/utils/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       66 2023-10-10 09:38:20.000000 langcheck-0.6.0/src/langcheck/utils/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      263 2023-10-10 09:38:20.000000 langcheck-0.6.0/src/langcheck/utils/io.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      460 2023-12-26 05:12:57.000000 langcheck-0.6.0/src/langcheck/utils/progess_bar.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:59.940082 langcheck-0.6.0/src/langcheck.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10386 2024-04-07 14:24:56.000000 langcheck-0.6.0/src/langcheck.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2865 2024-04-07 14:24:56.000000 langcheck-0.6.0/src/langcheck.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-04-07 14:24:56.000000 langcheck-0.6.0/src/langcheck.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      634 2024-04-07 14:24:56.000000 langcheck-0.6.0/src/langcheck.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2024-04-07 14:24:56.000000 langcheck-0.6.0/src/langcheck.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-04-07 14:24:59.914529 langcheck-0.6.0/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1119 2023-10-25 04:25:55.000000 langcheck-0.6.0/tests/test_stats.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.667811 langcheck-0.7.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2023-08-11 13:51:15.000000 langcheck-0.7.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10659 2024-05-08 10:39:01.666169 langcheck-0.7.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6957 2024-04-05 07:29:40.000000 langcheck-0.7.0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2921 2024-05-08 10:37:31.000000 langcheck-0.7.0/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      160 2024-05-08 10:39:01.670547 langcheck-0.7.0/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.129437 langcheck-0.7.0/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.209598 langcheck-0.7.0/src/langcheck/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      103 2023-11-19 15:49:24.000000 langcheck-0.7.0/src/langcheck/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      486 2023-12-05 05:59:04.000000 langcheck-0.7.0/src/langcheck/_handle_logs.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.235411 langcheck-0.7.0/src/langcheck/augment/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      554 2024-04-03 12:24:40.000000 langcheck-0.7.0/src/langcheck/augment/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.262279 langcheck-0.7.0/src/langcheck/augment/en/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      523 2023-12-12 02:12:39.000000 langcheck-0.7.0/src/langcheck/augment/en/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1424 2023-12-05 05:59:05.000000 langcheck-0.7.0/src/langcheck/augment/en/_change_case.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.272201 langcheck-0.7.0/src/langcheck/augment/en/_gender/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-12-12 02:12:39.000000 langcheck-0.7.0/src/langcheck/augment/en/_gender/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4173 2024-03-02 15:56:50.000000 langcheck-0.7.0/src/langcheck/augment/en/_gender/_gender.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3851 2023-12-12 02:12:39.000000 langcheck-0.7.0/src/langcheck/augment/en/_gender/_gender_pronouns.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2697 2023-12-05 05:59:05.000000 langcheck-0.7.0/src/langcheck/augment/en/_keyboard_typo.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2364 2023-12-05 05:59:05.000000 langcheck-0.7.0/src/langcheck/augment/en/_ocr_typo.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1364 2023-12-05 05:59:05.000000 langcheck-0.7.0/src/langcheck/augment/en/_remove_punctuation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4276 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/augment/en/_rephrase.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1815 2023-12-05 05:59:05.000000 langcheck-0.7.0/src/langcheck/augment/en/_synonym.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.278767 langcheck-0.7.0/src/langcheck/augment/ja/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       73 2024-01-11 08:18:01.000000 langcheck-0.7.0/src/langcheck/augment/ja/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2076 2024-04-03 12:24:40.000000 langcheck-0.7.0/src/langcheck/augment/ja/_synonym.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.299612 langcheck-0.7.0/src/langcheck/metrics/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2124 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3798 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/_pairwise_text_quality_utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9754 2024-04-03 12:24:40.000000 langcheck-0.7.0/src/langcheck/metrics/_validation.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.320561 langcheck-0.7.0/src/langcheck/metrics/de/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      905 2024-02-24 16:17:52.000000 langcheck-0.7.0/src/langcheck/metrics/de/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      632 2024-02-24 16:17:52.000000 langcheck-0.7.0/src/langcheck/metrics/de/_tokenizers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2741 2024-03-22 04:27:03.000000 langcheck-0.7.0/src/langcheck/metrics/de/_translation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9336 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/de/reference_based_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    21572 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/de/reference_free_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8115 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/de/source_based_text_quality.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.338243 langcheck-0.7.0/src/langcheck/metrics/en/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      858 2024-04-03 12:24:40.000000 langcheck-0.7.0/src/langcheck/metrics/en/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5046 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/en/pairwise_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9394 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/en/reference_based_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    23239 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/en/reference_free_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11734 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/en/source_based_text_quality.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.359709 langcheck-0.7.0/src/langcheck/metrics/eval_clients/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      620 2024-05-08 10:14:25.000000 langcheck-0.7.0/src/langcheck/metrics/eval_clients/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7348 2024-05-08 10:14:25.000000 langcheck-0.7.0/src/langcheck/metrics/eval_clients/_anthropic.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4902 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/eval_clients/_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9366 2024-05-08 10:14:25.000000 langcheck-0.7.0/src/langcheck/metrics/eval_clients/_gemini.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8454 2024-05-03 02:46:01.000000 langcheck-0.7.0/src/langcheck/metrics/eval_clients/_google.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13970 2024-05-08 10:14:25.000000 langcheck-0.7.0/src/langcheck/metrics/eval_clients/_openai.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.382434 langcheck-0.7.0/src/langcheck/metrics/ja/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      857 2024-04-05 07:29:40.000000 langcheck-0.7.0/src/langcheck/metrics/ja/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3468 2023-11-29 01:09:25.000000 langcheck-0.7.0/src/langcheck/metrics/ja/_tokenizers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5047 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/ja/pairwise_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10028 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/ja/reference_based_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22556 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/ja/reference_free_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10034 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/ja/source_based_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11027 2024-04-03 12:24:40.000000 langcheck-0.7.0/src/langcheck/metrics/metric_value.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.394566 langcheck-0.7.0/src/langcheck/metrics/model_manager/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       70 2024-03-01 06:48:01.000000 langcheck-0.7.0/src/langcheck/metrics/model_manager/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4189 2024-03-22 04:27:03.000000 langcheck-0.7.0/src/langcheck/metrics/model_manager/_model_loader.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11909 2024-03-22 04:27:03.000000 langcheck-0.7.0/src/langcheck/metrics/model_manager/_model_management.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.398822 langcheck-0.7.0/src/langcheck/metrics/model_manager/config/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3596 2024-03-22 04:27:03.000000 langcheck-0.7.0/src/langcheck/metrics/model_manager/config/metric_config.yaml
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.402641 langcheck-0.7.0/src/langcheck/metrics/prompts/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      408 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/_utils.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.157413 langcheck-0.7.0/src/langcheck/metrics/prompts/de/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.411313 langcheck-0.7.0/src/langcheck/metrics/prompts/de/get_score/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2024-05-03 01:56:00.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/de/get_score/anthropic.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/de/get_score/openai.j2
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.436983 langcheck-0.7.0/src/langcheck/metrics/prompts/de/metrics/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      828 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/de/metrics/answer_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      863 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/de/metrics/context_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1041 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/de/metrics/factual_consistency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      849 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/de/metrics/fluency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      589 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/de/metrics/sentiment.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/de/metrics/toxicity.j2
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.163808 langcheck-0.7.0/src/langcheck/metrics/prompts/en/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.457139 langcheck-0.7.0/src/langcheck/metrics/prompts/en/get_score/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      245 2024-05-08 10:14:25.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/en/get_score/function_calling.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      365 2024-05-08 10:14:25.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/en/get_score/plain_text.j2
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.488901 langcheck-0.7.0/src/langcheck/metrics/prompts/en/metrics/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      737 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/en/metrics/answer_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      741 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/en/metrics/context_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      953 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/en/metrics/factual_consistency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      761 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/en/metrics/fluency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2189 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/en/metrics/pairwise_comparison.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      546 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/en/metrics/sentiment.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      336 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/en/metrics/toxicity.j2
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.169329 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.512983 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/get_score/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      397 2024-05-03 01:56:00.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/get_score/anthropic.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      278 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/get_score/openai.j2
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.580876 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/metrics/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      923 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/metrics/answer_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      968 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/metrics/context_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1527 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/metrics/factual_consistency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      968 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/metrics/fluency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2421 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/metrics/pairwise_comparison.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      706 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/metrics/sentiment.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      518 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/prompts/ja/metrics/toxicity.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1814 2023-12-05 05:59:05.000000 langcheck-0.7.0/src/langcheck/metrics/reference_based_text_quality.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.594080 langcheck-0.7.0/src/langcheck/metrics/scorer/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4855 2024-03-22 04:27:03.000000 langcheck-0.7.0/src/langcheck/metrics/scorer/_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6481 2024-03-22 04:27:03.000000 langcheck-0.7.0/src/langcheck/metrics/scorer/detoxify_models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5656 2024-03-22 04:27:03.000000 langcheck-0.7.0/src/langcheck/metrics/scorer/hf_models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14772 2023-12-05 05:59:05.000000 langcheck-0.7.0/src/langcheck/metrics/text_structure.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.616434 langcheck-0.7.0/src/langcheck/metrics/zh/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      547 2024-03-01 06:48:01.000000 langcheck-0.7.0/src/langcheck/metrics/zh/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2560 2024-03-01 06:48:01.000000 langcheck-0.7.0/src/langcheck/metrics/zh/_tokenizers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10273 2024-04-30 05:42:20.000000 langcheck-0.7.0/src/langcheck/metrics/zh/reference_based_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12361 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/zh/reference_free_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4464 2024-04-26 01:26:17.000000 langcheck-0.7.0/src/langcheck/metrics/zh/source_based_text_quality.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.637560 langcheck-0.7.0/src/langcheck/plot/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      128 2023-09-26 12:28:25.000000 langcheck-0.7.0/src/langcheck/plot/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      538 2023-09-26 12:28:25.000000 langcheck-0.7.0/src/langcheck/plot/_css.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4112 2023-11-29 01:09:25.000000 langcheck-0.7.0/src/langcheck/plot/_histogram.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15343 2024-04-03 12:24:40.000000 langcheck-0.7.0/src/langcheck/plot/_scatter.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1303 2023-11-29 01:09:25.000000 langcheck-0.7.0/src/langcheck/plot/_utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1940 2023-09-26 12:28:25.000000 langcheck-0.7.0/src/langcheck/stats.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.652311 langcheck-0.7.0/src/langcheck/utils/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       66 2023-09-26 12:28:25.000000 langcheck-0.7.0/src/langcheck/utils/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      263 2023-09-26 12:28:25.000000 langcheck-0.7.0/src/langcheck/utils/io.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      460 2023-12-05 05:59:05.000000 langcheck-0.7.0/src/langcheck/utils/progess_bar.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.660127 langcheck-0.7.0/src/langcheck.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10659 2024-05-08 10:39:01.000000 langcheck-0.7.0/src/langcheck.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4605 2024-05-08 10:39:01.000000 langcheck-0.7.0/src/langcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-08 10:39:01.000000 langcheck-0.7.0/src/langcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      733 2024-05-08 10:39:01.000000 langcheck-0.7.0/src/langcheck.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2024-05-08 10:39:01.000000 langcheck-0.7.0/src/langcheck.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 10:39:01.656180 langcheck-0.7.0/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1119 2023-11-19 15:49:24.000000 langcheck-0.7.0/tests/test_stats.py
```

### Comparing `langcheck-0.6.0/LICENSE` & `langcheck-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/PKG-INFO` & `langcheck-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langcheck
-Version: 0.6.0
+Version: 0.7.0
 Summary: Simple, Pythonic building blocks to evaluate LLM-based applications
 Author-email: Citadel AI <info@citadel.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Citadel AI
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,14 +29,15 @@
 Keywords: llm,ai,nlp,evaluation,validation,testing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dash>=2.11
+Requires-Dist: Jinja2
 Requires-Dist: nlpaug
 Requires-Dist: nltk>=3
 Requires-Dist: openai>=1
 Requires-Dist: pandas>=1
 Requires-Dist: plotly>=5
 Requires-Dist: rouge-score>=0.1.2
 Requires-Dist: sentence-transformers>=2
@@ -56,20 +57,26 @@
 Requires-Dist: unidic-lite>=1.0.1; extra == "ja"
 Provides-Extra: ja-optional
 Requires-Dist: mecab-python3>=1.0.4; extra == "ja-optional"
 Requires-Dist: sudachidict-core; extra == "ja-optional"
 Requires-Dist: sudachipy; extra == "ja-optional"
 Provides-Extra: zh
 Requires-Dist: hanlp>=2.1.0b33; extra == "zh"
+Provides-Extra: anthropic
+Requires-Dist: anthropic; extra == "anthropic"
+Provides-Extra: gemini
+Requires-Dist: google-generativeai; extra == "gemini"
 Provides-Extra: all
 Requires-Dist: langcheck[de]; extra == "all"
 Requires-Dist: langcheck[en]; extra == "all"
 Requires-Dist: langcheck[ja]; extra == "all"
 Requires-Dist: langcheck[ja-optional]; extra == "all"
 Requires-Dist: langcheck[zh]; extra == "all"
+Requires-Dist: langcheck[anthropic]; extra == "all"
+Requires-Dist: langcheck[gemini]; extra == "all"
 Provides-Extra: dev
 Requires-Dist: yapf==0.40.1; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `langcheck-0.6.0/README.md` & `langcheck-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/pyproject.toml` & `langcheck-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langcheck"
-version = "0.6.0"
+version = "0.7.0"
 description = "Simple, Pythonic building blocks to evaluate LLM-based applications"
 readme = "README.md"
 authors = [{ name = "Citadel AI", email = "info@citadel.co.jp" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["llm", "ai", "nlp", "evaluation", "validation", "testing"]
 dependencies = [
     'dash >= 2.11',  # Dash 2.11 introduces a breaking change with Jupyter notebook support
+    'Jinja2',
     'nlpaug',
     'nltk >= 3',
     'openai >= 1',
     'pandas >= 1',
     'plotly >= 5',
     'rouge-score >= 0.1.2',
     'sentence-transformers >= 2',
@@ -46,21 +47,33 @@
     'mecab-python3 >= 1.0.4',
     'sudachidict-core',
     'sudachipy'
 ]
 zh = [
     'hanlp >= 2.1.0b33'
 ]
+
+# Different LLM clients
+anthropic = [
+    'anthropic'
+]
+gemini = [
+    'google-generativeai'
+]
+
 all = [
     'langcheck[de]',
     'langcheck[en]',
     'langcheck[ja]',
     'langcheck[ja-optional]',
-    'langcheck[zh]'
+    'langcheck[zh]',
+    'langcheck[anthropic]',
+    'langcheck[gemini]'
 ]
+
 dev = [
     "yapf==0.40.1",
     "flake8",
     "isort",
     "pyright",
     "pandas-stubs",
     "pytest",
@@ -103,8 +116,8 @@
 ]
 disable_test_id_escaping_and_forfeit_all_rights_to_community_support = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-langcheck = ["metrics/model_manager/config/*.yaml"]
+langcheck = ["metrics/model_manager/config/*.yaml", "metrics/prompts/**/*.j2"]
```

### Comparing `langcheck-0.6.0/src/langcheck/augment/__init__.py` & `langcheck-0.7.0/src/langcheck/augment/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/augment/en/__init__.py` & `langcheck-0.7.0/src/langcheck/augment/en/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/augment/en/_change_case.py` & `langcheck-0.7.0/src/langcheck/augment/en/_change_case.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/augment/en/_gender/_gender.py` & `langcheck-0.7.0/src/langcheck/augment/en/_gender/_gender.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/augment/en/_gender/_gender_pronouns.py` & `langcheck-0.7.0/src/langcheck/augment/en/_gender/_gender_pronouns.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/augment/en/_keyboard_typo.py` & `langcheck-0.7.0/src/langcheck/augment/en/_keyboard_typo.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/augment/en/_ocr_typo.py` & `langcheck-0.7.0/src/langcheck/augment/en/_ocr_typo.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/augment/en/_remove_punctuation.py` & `langcheck-0.7.0/src/langcheck/augment/en/_remove_punctuation.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/augment/en/_rephrase.py` & `langcheck-0.7.0/src/langcheck/augment/en/_rephrase.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,15 @@
     in `"Rethinking Benchmark and Contamination for Language Models with
     Rephrased Samples" <https://arxiv.org/abs/2311.04850>`__ to make an LLM
     rephrase the given text.
 
     We currently support two model types:
 
     1. The 'openai' type, where we use OpenAI's 'gpt-turbo-3.5' model
-    by default. See `this page
-    <https://langcheck.readthedocs.io/en/latest/metrics.html#computing-metrics-with-openai-models>`__
-    for examples on setting up the OpenAI API key.
+    by default.
 
     2. The 'azure_openai' type. Essentially the same as the 'openai' type,
     except that it uses the AzureOpenAI client. Note that you must specify the
     model to use in ``openai_args``, e.g.
     ``openai_args={'model': 'YOUR_DEPLOYMENT_NAME'}``
 
     Args:
@@ -42,15 +40,15 @@
         openai_args: Dict of additional args to pass in to the
             ``client.chat.completions.create`` function, default None
 
     Returns:
         A list of rephrased instances.
     '''
     # Initialize the openai object if openai_client is None
-    # TODO: Refactor this into OpenAIBasedEvaluator?
+    # TODO: Refactor this into OpenAIEvalClient?
     if openai_client is None:
         if model_type == 'openai':
             openai_client = OpenAI()
         elif model_type == 'azure_openai':
             if not openai_args:
                 raise AssertionError(
                     'The model deployment must be specified in `openai_args` '
```

### Comparing `langcheck-0.6.0/src/langcheck/augment/en/_synonym.py` & `langcheck-0.7.0/src/langcheck/augment/en/_synonym.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/augment/ja/_synonym.py` & `langcheck-0.7.0/src/langcheck/augment/ja/_synonym.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/__init__.py` & `langcheck-0.7.0/src/langcheck/metrics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langcheck.metrics import en
+from langcheck.metrics import en, eval_clients
 from langcheck.metrics.en.pairwise_text_quality import pairwise_comparison
 from langcheck.metrics.en.reference_based_text_quality import (
     rouge1, rouge2, rougeL, semantic_similarity)
 from langcheck.metrics.en.reference_free_text_quality import (
     ai_disclaimer_similarity, answer_relevance, flesch_kincaid_grade,
     flesch_reading_ease, fluency, sentiment, toxicity)
 from langcheck.metrics.en.source_based_text_quality import (context_relevance,
@@ -20,14 +20,15 @@
     'answer_relevance',
     'contains_all_strings',
     'contains_any_strings',
     'contains_regex',
     'context_relevance',
     'MetricValue',
     'en',
+    'eval_clients',
     'exact_match',
     'factual_consistency',
     'flesch_kincaid_grade',
     'flesch_reading_ease',
     'fluency',
     'is_float',
     'is_int',
```

### Comparing `langcheck-0.6.0/src/langcheck/metrics/_validation.py` & `langcheck-0.7.0/src/langcheck/metrics/_validation.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/de/__init__.py` & `langcheck-0.7.0/src/langcheck/metrics/de/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/de/_tokenizers.py` & `langcheck-0.7.0/src/langcheck/metrics/de/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/de/_translation.py` & `langcheck-0.7.0/src/langcheck/metrics/de/_translation.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/de/reference_based_text_quality.py` & `langcheck-0.7.0/src/langcheck/metrics/ja/reference_based_text_quality.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,157 +1,128 @@
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional
+from typing import List, Optional
 
-from openai import OpenAI
 from rouge_score import rouge_scorer
+from rouge_score.tokenizers import Tokenizer
 
 from langcheck.metrics._validation import validate_parameters_reference_based
-from langcheck.metrics.de._tokenizers import DeTokenizer
+from langcheck.metrics.eval_clients import EvalClient
+from langcheck.metrics.ja._tokenizers import JanomeTokenizer
 from langcheck.metrics.metric_value import MetricValue
 from langcheck.metrics.scorer.hf_models import \
     SentenceTransformerSimilarityScorer
-from langcheck.metrics.scorer.openai_models import OpenAISimilarityScorer
 from langcheck.utils.progess_bar import tqdm_wrapper
 
-LANG = "de"
-
 
 def semantic_similarity(
-    generated_outputs: List[str] | str,
-    reference_outputs: List[str] | str,
-    prompts: Optional[List[str] | str] = None,
-    model_type: str = "local",
-    openai_client: Optional[OpenAI] = None,
-    openai_args: Optional[Dict[str, Any]] = None,
-) -> MetricValue[float]:
-    """Calculates the semantic similarities between the generated outputs and
+        generated_outputs: List[str] | str,
+        reference_outputs: List[str] | str,
+        prompts: Optional[List[str] | str] = None,
+        eval_model: str | EvalClient = 'local') -> MetricValue[float]:
+    '''Calculates the semantic similarities between the generated outputs and
     the reference outputs. The similarities are computed as the cosine
     similarities between the generated and reference embeddings. This metric
     takes on float values between [-1, 1], but typically ranges between 0 and 1
     where 0 is minimum similarity and 1 is maximum similarity.
 
-    We currently support three embedding model types:
+    We currently support two embedding model types:
+
+    1. The 'local' type, where the 'paraphrase-multilingual-mpnet-base-v2' model
+    is downloaded from HuggingFace and run locally. This is the default model
+    type and there is no setup needed to run this.
+
+    2. The EvalClient type, where you can use a similarlity scorer returned by
+    the given EvalClient. The scorer is typically implemented using the
+    embedding APIs of cloud services. The implementation details are explained
+    in each of the concrete EvalClient classes.
 
-    1. The 'local' type, where the MODEL_NAME model is downloaded
-    from HuggingFace and run locally. This is the default model type and
-    there is no setup needed to run this.
-
-    2. The 'openai' type, where we use OpenAI's 'text-embedding-3-small' model
-    by default (this is configurable). See
-    `this page <https://langcheck.readthedocs.io/en/latest/metrics.html
-    #computing-metrics-with-openai-models>`__
-    on setting up the OpenAI API key.
-
-    3. The 'azure_openai' type. Essentially the same as the 'openai' type,
-    except that it uses the AzureOpenAI client. Note that you must specify your
-    model deployment to use in ``openai_args``, e.g.
-    ``openai_args={'model': 'YOUR_DEPLOYMENT_NAME'}``
 
     Ref:
         https://huggingface.co/tasks/sentence-similarity
         https://www.sbert.net/docs/usage/semantic_textual_similarity.html
-        https://openai.com/blog/new-embedding-models-and-api-updates
 
     Args:
         generated_outputs: The model generated output(s) to evaluate
         reference_outputs: The reference output(s)
         prompts: The prompts used to generate the output(s). Prompts are
             optional metadata and not used to calculate the metric.
-        model_type: The type of embedding model to use ('local', 'openai', or
-            'azure_openai'), default 'local'
-        openai_client: OpenAI or AzureOpenAI client, default None. If this is
-            None but ``model_type`` is 'openai' or 'azure_openai', we will
-            attempt to create a default client.
-        openai_args: Dict of additional args to pass in to the
-            ``client.embeddings.create`` function, default None
+        eval_model: The type of model to use ('local' or the EvalClient instance
+            used for the evaluation). default 'local'
 
     Returns:
         An :class:`~langcheck.metrics.metric_value.MetricValue` object
-    """
-    (
-        generated_outputs,
-        reference_outputs,
-        prompts,
-    ) = validate_parameters_reference_based(  # NOQA: E501
+    '''
+    generated_outputs, reference_outputs, prompts = validate_parameters_reference_based(  # NOQA: E501
         generated_outputs, reference_outputs, prompts)
-    assert model_type in [
-        "local", "openai", "azure_openai"
-    ], ("Unsupported embedding model type. "
-        'The supported ones are ["local", "openai", "azure_openai"]')
-
-    if model_type == 'local':
-        scorer = SentenceTransformerSimilarityScorer(language=LANG)
-    else:  # openai or azure_openai
-        scorer = OpenAISimilarityScorer(model_type=model_type,
-                                        openai_client=openai_client,
-                                        openai_args=openai_args)
+    if eval_model == 'local':
+        scorer = SentenceTransformerSimilarityScorer(language='ja')
+    else:  # EvalClient
+        assert isinstance(
+            eval_model, EvalClient
+        ), 'An EvalClient must be provided for non-local model types.'
+        scorer = eval_model.similarity_scorer()
+
     scores = scorer.score(generated_outputs, reference_outputs)
 
-    return MetricValue(
-        metric_name="semantic_similarity",
-        prompts=prompts,
-        generated_outputs=generated_outputs,
-        reference_outputs=reference_outputs,
-        sources=None,
-        explanations=None,
-        metric_values=scores,
-        language=LANG,
-    )
-
-
-def rouge1(
-    generated_outputs: List[str] | str,
-    reference_outputs: List[str] | str,
-    prompts: Optional[List[str] | str] = None,
-) -> MetricValue[float]:
-    """Calculates the F1 metrics of the ROUGE-1 scores between the generated
-    outputs and the reference outputs. It evaluates the overlap of unigrams
+    return MetricValue(metric_name='semantic_similarity',
+                       prompts=prompts,
+                       generated_outputs=generated_outputs,
+                       reference_outputs=reference_outputs,
+                       sources=None,
+                       explanations=None,
+                       metric_values=scores,
+                       language='ja')
+
+
+def rouge1(generated_outputs: List[str] | str,
+           reference_outputs: List[str] | str,
+           prompts: Optional[List[str] | str] = None,
+           *,
+           tokenizer: Optional[Tokenizer] = None) -> MetricValue[float]:
+    '''Calculates the F1 metrics of the ROUGE-1 scores between the generated
     (single tokens) between the generated outputs and the reference outputs.
     This metric takes on float values between [0, 1], where 0 is no overlap and
     1 is complete overlap.
 
     Ref:
         https://github.com/google-research/google-research/tree/master/rouge
 
     Args:
         generated_outputs: The model generated output(s) to evaluate
         reference_outputs: The reference output(s)
         prompts: The prompts used to generate the output(s). Prompts are
             optional metadata and not used to calculate the metric.
 
     Returns:
-        An :class:`~langcheck.metrics.metric_value.MetricValue` object
-    """
-    (
-        generated_outputs,
-        reference_outputs,
-        prompts,
-    ) = validate_parameters_reference_based(  # NOQA: E501
+        An MetricValue object
+    '''
+    generated_outputs, reference_outputs, prompts = validate_parameters_reference_based(  # NOQA: E501
         generated_outputs, reference_outputs, prompts)
 
-    scores = _rouge(generated_outputs, reference_outputs, "rouge1")
-    return MetricValue(
-        metric_name="rouge1",
-        prompts=prompts,
-        generated_outputs=generated_outputs,
-        reference_outputs=reference_outputs,
-        sources=None,
-        explanations=None,
-        metric_values=scores,
-        language=LANG,
-    )
-
-
-def rouge2(
-    generated_outputs: List[str] | str,
-    reference_outputs: List[str] | str,
-    prompts: Optional[List[str] | str] = None,
-) -> MetricValue[float]:
-    """Calculates the F1 metrics of the ROUGE-2 scores between the generated
+    scores = _rouge(generated_outputs,
+                    reference_outputs,
+                    'rouge1',
+                    tokenizer=tokenizer)
+    return MetricValue(metric_name='rouge1',
+                       prompts=prompts,
+                       generated_outputs=generated_outputs,
+                       reference_outputs=reference_outputs,
+                       sources=None,
+                       explanations=None,
+                       metric_values=scores,
+                       language='ja')
+
+
+def rouge2(generated_outputs: List[str] | str,
+           reference_outputs: List[str] | str,
+           prompts: Optional[List[str] | str] = None,
+           *,
+           tokenizer: Optional[Tokenizer] = None) -> MetricValue[float]:
+    '''Calculates the F1 metrics of the ROUGE-2 scores between the generated
     outputs and the reference outputs. It evaluates the overlap of bigrams
     (two adjacent tokens) between the generated outputs and the reference
     outputs. This metric takes on float values between [0, 1], where 0 is no
     overlap and 1 is complete overlap.
 
     Ref:
         https://github.com/google-research/google-research/tree/master/rouge
@@ -159,42 +130,39 @@
     Args:
         generated_outputs: The model generated output(s) to evaluate
         reference_outputs: The reference output(s)
         prompts: The prompts used to generate the output(s). Prompts are
             optional metadata and not used to calculate the metric.
 
     Returns:
-        An :class:`~langcheck.metrics.metric_value.MetricValue` object
-    """
-    (
-        generated_outputs,
-        reference_outputs,
-        prompts,
-    ) = validate_parameters_reference_based(  # NOQA: E501
+        An MetricValue object
+    '''
+    generated_outputs, reference_outputs, prompts = validate_parameters_reference_based(  # NOQA: E501
         generated_outputs, reference_outputs, prompts)
 
-    scores = _rouge(generated_outputs, reference_outputs, "rouge2")
-    return MetricValue(
-        metric_name="rouge2",
-        prompts=prompts,
-        generated_outputs=generated_outputs,
-        reference_outputs=reference_outputs,
-        sources=None,
-        explanations=None,
-        metric_values=scores,
-        language=LANG,
-    )
-
-
-def rougeL(
-    generated_outputs: List[str] | str,
-    reference_outputs: List[str] | str,
-    prompts: Optional[List[str] | str] = None,
-) -> MetricValue[float]:
-    """Calculates the F1 metrics of the ROUGE-L scores between the generated
+    scores = _rouge(generated_outputs,
+                    reference_outputs,
+                    'rouge2',
+                    tokenizer=tokenizer)
+    return MetricValue(metric_name='rouge2',
+                       prompts=prompts,
+                       generated_outputs=generated_outputs,
+                       reference_outputs=reference_outputs,
+                       sources=None,
+                       explanations=None,
+                       metric_values=scores,
+                       language='ja')
+
+
+def rougeL(generated_outputs: List[str] | str,
+           reference_outputs: List[str] | str,
+           prompts: Optional[List[str] | str] = None,
+           *,
+           tokenizer: Optional[Tokenizer] = None) -> MetricValue[float]:
+    '''Calculates the F1 metrics of the ROUGE-L scores between the generated
     outputs and the reference outputs. It evaluates the longest common
     subsequence (LCS) between the generated outputs and the reference outputs.
     This metric takes on float values between [0, 1], where 0 means that the LCS
     is empty and 1 means that the reference and generated outputs are the same.
 
     Ref:
         https://github.com/google-research/google-research/tree/master/rouge
@@ -202,63 +170,64 @@
     Args:
         generated_outputs: The model generated output(s) to evaluate
         reference_outputs: The reference output(s)
         prompts: The prompts used to generate the output(s). Prompts are
             optional metadata and not used to calculate the metric.
 
     Returns:
-        An :class:`~langcheck.metrics.metric_value.MetricValue` object
-    """
-    (
-        generated_outputs,
-        reference_outputs,
-        prompts,
-    ) = validate_parameters_reference_based(  # NOQA: E501
+        An MetricValue object
+    '''
+    generated_outputs, reference_outputs, prompts = validate_parameters_reference_based(  # NOQA: E501
         generated_outputs, reference_outputs, prompts)
 
     # The `rouge_score` package has two flavors of ROUGE-L [1]:
     # - 1) sentence-level, where newline characters are ignored
     # - 2) summary-level, where newline characters are interpreted as sentence
     #      boundaries
     #
     # We use (2) here (i.e. `rougeLsum`) because this is how `pyrouge` computes
     # the ROUGE-L score (https://github.com/bheinzerling/pyrouge), which is a
     # Python wrapper around original perl script implementation.
     #
     # [1] https://github.com/google-research/google-research/tree/master/rouge#two-flavors-of-rouge-l # NOQA: E501
-    scores = _rouge(generated_outputs, reference_outputs, "rougeLsum")
-    return MetricValue(
-        metric_name="rougeL",
-        prompts=prompts,
-        generated_outputs=generated_outputs,
-        reference_outputs=reference_outputs,
-        sources=None,
-        explanations=None,
-        metric_values=scores,
-        language=LANG,
-    )
-
-
-def _rouge(generated_outputs: List[str], reference_outputs: List[str],
-           rouge_type: str) -> List[float]:
-    """Helper function for computing the rouge1, rouge2, and rougeL metrics.
+    scores = _rouge(generated_outputs,
+                    reference_outputs,
+                    'rougeLsum',
+                    tokenizer=tokenizer)
+    return MetricValue(metric_name='rougeL',
+                       prompts=prompts,
+                       generated_outputs=generated_outputs,
+                       reference_outputs=reference_outputs,
+                       sources=None,
+                       explanations=None,
+                       metric_values=scores,
+                       language='ja')
+
+
+def _rouge(generated_outputs: List[str],
+           reference_outputs: List[str],
+           rouge_type: str,
+           *,
+           tokenizer: Optional[Tokenizer] = None) -> List[float]:
+    '''Helper function for computing the rouge1, rouge2, and rougeL metrics.
     This uses Google Research's implementation of ROUGE:
     https://github.com/google-research/google-research/tree/master/rouge
 
     Args:
         generated_outputs: A list of model generated outputs to evaluate
         reference_outputs: A list of reference outputs
         rouge_type: rouge1, rouge2, or rougeLsum
 
     Returns:
         A list of F1 values of the ROUGE scores
-    """
-    assert rouge_type in ["rouge1", "rouge2", "rougeLsum"]
+    '''
+    assert rouge_type in ['rouge1', 'rouge2', 'rougeLsum']
 
-    tokenizer = DeTokenizer()
+    # The tokenizer is default to JanomeTokenizer
+    tokenizer = tokenizer or JanomeTokenizer()
     scorer = rouge_scorer.RougeScorer([rouge_type],
                                       use_stemmer=True,
                                       tokenizer=tokenizer)
     scores = []
     for gen, ref in tqdm_wrapper(zip(generated_outputs, reference_outputs),
                                  total=len(generated_outputs)):
         score = scorer.score(gen, ref)
```

### Comparing `langcheck-0.6.0/src/langcheck/metrics/en/__init__.py` & `langcheck-0.7.0/src/langcheck/metrics/en/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/en/_openai.py` & `langcheck-0.7.0/src/langcheck/metrics/eval_clients/_gemini.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,251 +1,228 @@
 from __future__ import annotations
 
-import asyncio
-import json
 import os
-from collections.abc import Callable, Iterable
-from typing import Any
+from typing import Any, Iterable
 
-from openai import AsyncAzureOpenAI, AsyncOpenAI, AzureOpenAI, OpenAI
+import google.ai.generativelanguage as glm
+import google.generativeai as genai
+import torch
 
 from langcheck.utils.progess_bar import tqdm_wrapper
 
+from ..prompts._utils import get_template
+from ..scorer._base import BaseSimilarityScorer
+from ._base import EvalClient
 
-class OpenAIBasedEvaluator:
-    '''Evaluator class based on OpenAI's API.'''
+
+class GeminiEvalClient(EvalClient):
+    '''EvalClient defined for the Gemini model.
+    '''
 
     def __init__(self,
-                 assessment_to_score_mapping: dict[str, float],
-                 function_name: str,
-                 function_description: str,
-                 argument_name: str,
-                 argument_description: str,
-                 client_type: str,
-                 client: OpenAI | None,
-                 openai_args: dict[str, str] | None,
-                 *,
-                 use_async: bool = False) -> None:
+                 model: genai.GenerativeModel | None = None,
+                 model_args: dict[str, Any] | None = None,
+                 generate_content_args: dict[str, Any] | None = None,
+                 embed_model_name: str | None = None):
         '''
-        Initialize the OpenAIBasedEvaluator with given parameters.
+        Initialize the Gemini evaluation client. The authentication
+        information is automatically read from the environment variables,
+        so please make sure GOOGLE_API_KEY is set.
+
+        TODO: Allow the user to specify the use of async. There currently
+        seems to be an issue with `generate_content_async()` that is blocking
+        this: https://github.com/google-gemini/generative-ai-python/issues/207
+
+        Ref:
+            https://ai.google.dev/api/python/google/generativeai/GenerativeModel
 
         Args:
-            assessment_to_score_mapping: Mapping from an assessment (str) to a
-                numeric score (float)
-            function_name: Name of the function that we force the OpenAI API to
-                call
-            function_description: Description of the function
-            argument_name: Name of the argument to the function. This should be
-                the name of the metric to evaluate (e.g. sentiment).
-            argument_description: Description of the argument
-            client_type: The type of OpenAI client ('openai' or 'azure_openai')
-            client: (Optional) OpenAI, AzureOpenAI, AsyncOpenAI or
-                AsyncAzureOpenAI client. If this is None, we will attempt to
-                create a default client depending on the ``client_type``.
-            openai_args: (Optional) dict of additional args to pass in to the
-                ``client.chat.completions.create`` function
-            use_async: (Optional) If True, the async client will be used.
+            model: (Optional) The Gemini model to use. If not provided, the
+                model will be created using the model_args.
+            model_args: (Optional) Dict of args to create the Gemini model.
+            generate_content_args: (Optional) Dict of args to pass in to the
+                ``generate_content`` function.
+            embed_model_name: (Optional) The name of the embedding model to use.
+                If not provided, the models/embedding-001 model will be used.
         '''
-        self._client_type = client_type
-        if self._client_type == 'azure_openai' and not openai_args:
-            raise AssertionError(
-                'The model deployment must be specified in `openai_args` for '
-                'the azure_openai type, e.g. '
-                '`openai_args={"model": "YOUR_DEPLOYMENT_NAME"}`')
-
-        if client:
-            self._client = client
-        elif self._client_type == 'openai':
-            if use_async:
-                self._client = AsyncOpenAI()
-            else:
-                self._client = OpenAI()
-        elif self._client_type == 'azure_openai':
-            # https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/migration?tabs=python-new%2Cdalle-fix#completions
-            kargs = {
-                "api_key": os.getenv("AZURE_OPENAI_KEY"),
-                "api_version": os.getenv("OPENAI_API_VERSION"),
-                "azure_endpoint": os.getenv("AZURE_OPENAI_ENDPOINT"),
-            }
-            if use_async:
-                self._client = AsyncAzureOpenAI(**kargs)  # type: ignore
-            else:
-                self._client = AzureOpenAI(**kargs)  # type: ignore
+        if model:
+            self._model = model
         else:
-            raise AssertionError(f'Unexpected client type "{client_type}"')
+            genai.configure(api_key=os.getenv('GOOGLE_API_KEY'))
+            model_args = model_args or {}
+            self._model = genai.GenerativeModel(**model_args)
+
+        self._generate_content_args = generate_content_args or {}
+        self._embed_model_name = embed_model_name
+
+    def _call_api(self,
+                  prompts: Iterable[str | None],
+                  config: dict[str, Any],
+                  *,
+                  tqdm_description: str | None = None) -> list[Any]:
+        # A helper function to call the API with exception filter for alignment
+        # of exception handling with the async version.
+        def _call_api_with_exception_filter(prompt: str) -> Any:
+            try:
+                return self._model.generate_content(prompt, **config)
+            except Exception as e:
+                return e
 
-        self._assessment_to_score_mapping = assessment_to_score_mapping
-        self._function_name = function_name
-        self._function_description = function_description
-        self._argument_name = argument_name
-        self._argument_description = argument_description
-        self._openai_args = openai_args
-        self._use_async = use_async
-
-    def get_score(
-        self,
-        prompts: str | Iterable[str],
-        function_call_prompt_template: Callable,
-        *,
-        intermediate_tqdm_description: str | None = None,
-        score_tqdm_description: str | None = None
-    ) -> tuple[list[float | None], list[str | None]]:
+        responses = [
+            _call_api_with_exception_filter(prompt)
+            for prompt in tqdm_wrapper(prompts, desc=tqdm_description)
+        ]
+
+        # Filter out exceptions and print them out. Also filter out responses
+        # that are blocked by safety settings and print out the safety ratings.
+        for i, response in enumerate(responses):
+            if isinstance(response, Exception):
+                print('Gemini failed to return an assessment corresponding to '
+                      f'{i}th prompt: {response}')
+                responses[i] = None
+            elif response.candidates[0].finish_reason == 3:
+                print(
+                    f"Gemini's safety settings blocked the {i}th prompt:\n {response.candidates[0].safety_ratings}"  # NOQA: E501
+                )
+                responses[i] = None
+        return responses
+
+    def get_text_responses(
+            self,
+            prompts: Iterable[str],
+            *,
+            tqdm_description: str | None = None) -> list[str | None]:
+        '''The function that gets resonses to the given prompt texts.
+
+        Args:
+            prompts: The prompts you want to get the responses for.
+        Returns:
+            A list of responses to the prompts. The responses can be None if the
+            evaluation fails.
         '''
-        Retrieves the score and unstructured assessment for a given prompt using
-        the OpenAI API. The first API call is a "normal" call, where the API
-        will return unstructured text. The second call leverages the function
-        calling API, where the API should return a structured response. If the
-        API fails to return a response, or the response is not in the expected
-        format, `None` is returned for both the score and the unstructured
-        assessment.
+        config = {"generation_config": {"temperature": 0.0}}
+        config.update(self._generate_content_args or {})
+        tqdm_description = tqdm_description or 'Intermediate assessments (1/2)'  # NOQA: E501
+        responses = self._call_api(prompts=prompts,
+                                   config=config,
+                                   tqdm_description=tqdm_description)
+        response_texts = [
+            response.text if response else None for response in responses
+        ]
+
+        return response_texts
+
+    def get_float_score(
+            self,
+            metric_name: str,
+            language: str,
+            unstructured_assessment_result: list[str | None],
+            score_map: dict[str, float],
+            *,
+            tqdm_description: str | None = None) -> list[float | None]:
+        '''The function that transforms the unstructured assessments (i.e. long
+        texts that describe the evaluation results) into scores. We leverage the
+        function calling API to extract the short assessment results from the
+        unstructured assessments, so please make sure that the model you use
+        supports function calling
+        (https://ai.google.dev/gemini-api/docs/function-calling#supported-models).
+
+        Ref:
+            https://ai.google.dev/gemini-api/docs/function-calling
 
         Args:
-            prompts: :List of prompt that asks the OpenAI API for the
-                unstructured assessment response
-            function_call_prompt_template: Prompt template used to construct the
-                prompt that asks the OpenAI API for the structured assessment
-                response
-            intermediate_tqdm_description: (Optional) Description for the
-                progress bar for the intermediate assessments
-            score_tqdm_description: (Optional) Description for the progress bar
-                for the scores
+            metric_name: The name of the metric to be used. (e.g. "toxicity")
+            language: The language of the prompts. (e.g. "en")
+            unstructured_assessment_result: The unstructured assessment results
+                for the given assessment prompts.
+            score_map: The mapping from the short assessment results
+                (e.g. "Good") to the scores.
+            tqdm_description: The description to be shown in the tqdm bar.
 
         Returns:
-            scores: List of scores associated with the corresponding prompts
-                based on the resulting structured assessment. If a score cannot
-                be computed for a prompt, it will be represented as `None`.
-            unstructured_assessments: List of unstructured assessment text,
-                which also serves as the explanation of the score. If a score
-                cannot be computed for a prompt, it will be represented as
-                `None`.
+            A list of scores for the given prompts. The scores can be None if
+            the evaluation fails.
         '''
-        if isinstance(prompts, str):
-            prompts = [prompts]
-
-        # First, call the API to get an unstructured assessment. The response
-        # should include both the assessment itself and the model's reasoning
-        # for that assessment.
-        config_unstructured_assessments = {
-            "model": "gpt-3.5-turbo",
-            "seed": 123
-        }
-        config_unstructured_assessments.update(self._openai_args or {})
+        if language not in ['en', 'ja', 'de']:
+            raise ValueError(f'Unsupported language: {language}')
 
-        intermediate_tqdm_description = intermediate_tqdm_description or 'Intermediate assessments (1/2)'  # NOQA: E501
-        responses = self._call_api(
-            prompts=prompts,
-            config=config_unstructured_assessments,
-            tqdm_description=intermediate_tqdm_description)
-        unstructured_assessments = [
-            response.choices[0].message.content if response else None
-            for response in responses
-        ]
+        fn_call_template = get_template(
+            f'{language}/get_score/function_calling.j2')
 
-        # Next, call the API leveraging function calling to get a structured
-        # assessment.
-        # Construct the prompt for the function calling API, filled with None
-        # for the failed unstructured assessment.
+        options = list(score_map.keys())
         fn_call_messages = [
-            function_call_prompt_template(unstructured_assessment)
-            if unstructured_assessment else None
-            for unstructured_assessment in unstructured_assessments
+            fn_call_template.render({
+                'metric': metric_name,
+                'unstructured_assessment': unstructured_assessment,
+                'options': options,
+            }) if unstructured_assessment else None
+            for unstructured_assessment in unstructured_assessment_result
         ]
-        argument_options = list(self._assessment_to_score_mapping.keys())
-        functions = [{
-            "name": self._function_name,
-            "description": self._function_description,
-            "parameters": {
-                "type": "object",
-                "properties": {
-                    self._argument_name: {
-                        "type": "string",
-                        "enum": argument_options,
-                        "description": self._argument_description,
-                    },
-                },
-                "required": [self._argument_name],
-            },
-        }]
+
+        assessment_schema = glm.Schema(type=glm.Type.STRING, enum=options)
+
+        save_assessment = glm.FunctionDeclaration(
+            name='save_assessment',
+            description=f'Save the assessment of {metric_name}.',
+            parameters=glm.Schema(type=glm.Type.OBJECT,
+                                  properties={'assessment': assessment_schema}))
         config_structured_assessments = {
-            "seed": 123,
-            "functions": functions,
-            "function_call": {
-                "name": self._function_name
+            "tools": [save_assessment],
+            "tool_config": {
+                'function_calling_config': 'ANY'
             },
-            "model": "gpt-3.5-turbo"
+            "generation_config": {
+                "temperature": 0.0
+            }
         }
-        config_structured_assessments.update(self._openai_args or {})
+        config_structured_assessments.update(self._generate_content_args or {})
 
-        score_tqdm_description = score_tqdm_description or 'Scores (2/2)'
+        tqdm_description = tqdm_description or 'Scores (2/2)'
         responses = self._call_api(prompts=fn_call_messages,
                                    config=config_structured_assessments,
-                                   tqdm_description=score_tqdm_description)
-        function_args = [
-            json.loads(response.choices[0].message.function_call.arguments)
-            if response else None for response in responses
-        ]
-        assessments = [
-            function_arg.get(self._argument_name) if function_arg else None
-            for function_arg in function_args
-        ]
-
+                                   tqdm_description=tqdm_description)
+        assessments = []
+        for response in responses:
+            if response is None:
+                assessments.append(None)
+                continue
+            function_call = response.candidates[0].content.parts[
+                0].function_call
+            fc_dict = type(function_call).to_dict(function_call)
+            assessments.append(fc_dict.get('args', {}).get('assessment'))
         # Check if any of the assessments are not recognized.
         for assessment in assessments:
-            if (assessment is None) or (assessment
-                                        in self._assessment_to_score_mapping):
+            if (assessment is None) or (assessment in options):
                 continue
             # By leveraging the function calling API, this should be pretty
             # rare, but we're dealing with LLMs here so nothing is absolute!
-            print(f'OpenAI returned an unrecognized assessment: "{assessment}"')
+            print(f'Gemini returned an unrecognized assessment: "{assessment}"')
 
         return [
-            self._assessment_to_score_mapping[assessment]
-            if assessment else None for assessment in assessments
-        ], unstructured_assessments
+            score_map[assessment] if assessment else None
+            for assessment in assessments
+        ]
 
-    def _call_api(self,
-                  prompts: Iterable[str | None],
-                  config: dict[str, str],
-                  tqdm_description: str | None = None) -> list[Any]:
-        # A helper function to call the API with exception filter for alignment
-        # of exception handling with the async version.
-        def _call_api_with_exception_filter(model_input: dict[str, Any]) -> Any:
-            if model_input is None:
-                return None
-            try:
-                return self._client.chat.completions.create(**model_input)
-            except Exception as e:
-                return e
+    def similarity_scorer(self) -> GeminiSimilarityScorer:
+        return GeminiSimilarityScorer(embed_model_name=self._embed_model_name)
 
-        model_inputs = [{
-            "messages": [{
-                "role": "user",
-                "content": prompt
-            }],
-            **config
-        } for prompt in prompts]
-
-        if self._use_async:
-            # A helper function to call the async API.
-            async def _call_async_api() -> list[Any]:
-                responses = await asyncio.gather(*map(
-                    lambda model_input: self._client.chat.completions.create(
-                        **model_input), model_inputs),
-                                                 return_exceptions=True)
-                return responses
 
-            responses = asyncio.run(_call_async_api())
-        else:
-            responses = [
-                _call_api_with_exception_filter(model_input)
-                for model_input in tqdm_wrapper(model_inputs,
-                                                desc=tqdm_description)
-            ]
+class GeminiSimilarityScorer(BaseSimilarityScorer):
+    '''Similarity scorer that uses the Gemini API to embed the inputs.
+    In the current version of langcheck, the class is only instantiated within
+    EvalClients.
+    '''
 
-        # Filter out exceptions and print them out.
-        for i, response in enumerate(responses):
-            if not isinstance(response, Exception):
-                continue
-            print('OpenAI failed to return an assessment corresponding to '
-                  f'{i}th prompt: {response}')
-            responses[i] = None
-        return responses
+    def __init__(self, embed_model_name: str | None):
+
+        super().__init__()
+
+        self.embed_model_name = embed_model_name or 'models/embedding-001'
+
+    def _embed(self, inputs: list[str]) -> torch.Tensor:
+        '''Embed the inputs using the Gemini API.
+        '''
+        # Embed the inputs
+        embed_response = genai.embed_content(model=self.embed_model_name,
+                                             content=inputs)
+
+        return torch.Tensor([item for item in embed_response['embedding']])
```

### Comparing `langcheck-0.6.0/src/langcheck/metrics/en/reference_based_text_quality.py` & `langcheck-0.7.0/src/langcheck/metrics/en/reference_based_text_quality.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,67 @@
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional
+from typing import List, Optional
 
-from openai import OpenAI
 from rouge_score import rouge_scorer
 
 from langcheck.metrics._validation import validate_parameters_reference_based
+from langcheck.metrics.eval_clients import EvalClient
 from langcheck.metrics.metric_value import MetricValue
 from langcheck.metrics.scorer.hf_models import \
     SentenceTransformerSimilarityScorer
-from langcheck.metrics.scorer.openai_models import OpenAISimilarityScorer
 from langcheck.utils.progess_bar import tqdm_wrapper
 
 
 def semantic_similarity(
         generated_outputs: List[str] | str,
         reference_outputs: List[str] | str,
         prompts: Optional[List[str] | str] = None,
-        model_type: str = 'local',
-        openai_client: Optional[OpenAI] = None,
-        openai_args: Optional[Dict[str, Any]] = None) -> MetricValue[float]:
+        eval_model: str | EvalClient = 'local') -> MetricValue[float]:
     '''Calculates the semantic similarities between the generated outputs and
     the reference outputs. The similarities are computed as the cosine
     similarities between the generated and reference embeddings. This metric
     takes on float values between [-1, 1], but typically ranges between 0 and 1
     where 0 is minimum similarity and 1 is maximum similarity.
 
-    We currently support three embedding model types:
+    We currently support two embedding model types:
 
     1. The 'local' type, where the 'all-mpnet-base-v2' model is downloaded
     from HuggingFace and run locally. This is the default model type and
     there is no setup needed to run this.
 
-    2. The 'openai' type, where we use OpenAI's 'text-embedding-3-small' model
-    by default (this is configurable). See
-    `this page <https://langcheck.readthedocs.io/en/latest/metrics.html
-    #computing-metrics-with-openai-models>`__
-    on setting up the OpenAI API key.
-
-    3. The 'azure_openai' type. Essentially the same as the 'openai' type,
-    except that it uses the AzureOpenAI client. Note that you must specify your
-    model deployment to use in ``openai_args``, e.g.
-    ``openai_args={'model': 'YOUR_DEPLOYMENT_NAME'}``
+    2. The EvalClient type, where you can use a similarlity scorer returned by
+    the given EvalClient. The scorer is typically implemented using the
+    embedding APIs of cloud services. The implementation details are explained
+    in each of the concrete EvalClient classes.
 
     Ref:
         https://huggingface.co/tasks/sentence-similarity
         https://www.sbert.net/docs/usage/semantic_textual_similarity.html
-        https://openai.com/blog/new-embedding-models-and-api-updates
 
     Args:
         generated_outputs: The model generated output(s) to evaluate
         reference_outputs: The reference output(s)
         prompts: The prompts used to generate the output(s). Prompts are
             optional metadata and not used to calculate the metric.
-        model_type: The type of embedding model to use ('local', 'openai', or
-            'azure_openai'), default 'local'
-        openai_client: OpenAI or AzureOpenAI client, default None. If this is
-            None but ``model_type`` is 'openai' or 'azure_openai', we will
-            attempt to create a default client.
-        openai_args: Dict of additional args to pass in to the
-            ``client.embeddings.create`` function, default None
+        eval_model: The type of model to use ('local' or the EvalClient instance
+            used for the evaluation). default 'local'
 
     Returns:
         An :class:`~langcheck.metrics.metric_value.MetricValue` object
     '''
     generated_outputs, reference_outputs, prompts = validate_parameters_reference_based(  # NOQA: E501
         generated_outputs, reference_outputs, prompts)
-    assert model_type in [
-        'local', 'openai', 'azure_openai'
-    ], ('Unsupported embedding model type. '
-        'The supported ones are ["local", "openai", "azure_openai"]')
-    if model_type == 'local':
+    if eval_model == 'local':
         scorer = SentenceTransformerSimilarityScorer(language='en')
-    else:  # openai or azure_openai
-        scorer = OpenAISimilarityScorer(model_type=model_type,
-                                        openai_client=openai_client,
-                                        openai_args=openai_args)
+    else:  # EvalClient
+        assert isinstance(
+            eval_model, EvalClient
+        ), 'An EvalClient must be provided for non-local model types.'
+        scorer = eval_model.similarity_scorer()
 
     scores = scorer.score(generated_outputs, reference_outputs)
     return MetricValue(metric_name='semantic_similarity',
                        prompts=prompts,
                        generated_outputs=generated_outputs,
                        reference_outputs=reference_outputs,
                        sources=None,
```

### Comparing `langcheck-0.6.0/src/langcheck/metrics/ja/__init__.py` & `langcheck-0.7.0/src/langcheck/metrics/ja/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/ja/_tokenizers.py` & `langcheck-0.7.0/src/langcheck/metrics/ja/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/ja/reference_based_text_quality.py` & `langcheck-0.7.0/src/langcheck/metrics/zh/reference_based_text_quality.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,97 +1,86 @@
 from __future__ import annotations
 
-from typing import Dict, List, Optional
+from typing import List, Optional
 
-from openai import OpenAI
 from rouge_score import rouge_scorer
 from rouge_score.tokenizers import Tokenizer
 
 from langcheck.metrics._validation import validate_parameters_reference_based
-from langcheck.metrics.ja._tokenizers import JanomeTokenizer
+from langcheck.metrics.eval_clients import EvalClient
 from langcheck.metrics.metric_value import MetricValue
 from langcheck.metrics.scorer.hf_models import \
     SentenceTransformerSimilarityScorer
-from langcheck.metrics.scorer.openai_models import OpenAISimilarityScorer
-from langcheck.utils.progess_bar import tqdm_wrapper
+from langcheck.metrics.zh._tokenizers import HanLPTokenizer
 
 
 def semantic_similarity(
         generated_outputs: List[str] | str,
         reference_outputs: List[str] | str,
         prompts: Optional[List[str] | str] = None,
-        model_type: str = 'local',
-        openai_client: Optional[OpenAI] = None,
-        openai_args: Optional[Dict[str, str]] = None) -> MetricValue[float]:
-    '''Calculates the semantic similarities between the generated outputs and
+        eval_model: str | EvalClient = 'local') -> MetricValue[float]:
+    '''
+    Calculates the semantic similarities between the generated outputs and
     the reference outputs. The similarities are computed as the cosine
     similarities between the generated and reference embeddings. This metric
     takes on float values between [-1, 1], but typically ranges between 0 and 1
-    where 0 is minimum similarity and 1 is maximum similarity.
+    where 0 is minimum similarity and 1 is maximum similarity. (NOTE: when using
+    OpenAI embeddings, the cosine similarities tend to be skewed quite heavily
+    towards higher numbers.)
 
-    We currently support three embedding model types:
+    We currently support two embedding model types:
 
-    1. The 'local' type, where the 'paraphrase-multilingual-mpnet-base-v2' model
-    is downloaded from HuggingFace and run locally. This is the default model
-    type and there is no setup needed to run this.
 
-    2. The 'openai' type, where we use OpenAI's 'text-embedding-3-small' model
-    by default (this is configurable). See
-    `this page <https://langcheck.readthedocs.io/en/latest/metrics.html
-    #computing-metrics-with-openai-models>`__
-    for examples on setting up the OpenAI API key.
-
-    3. The 'azure_openai' type. Essentially the same as the 'openai' type,
-    except that it uses the AzureOpenAI client. Note that you must specify your
-    model deployment to use in ``openai_args``, e.g.
-    ``openai_args={'model': 'YOUR_DEPLOYMENT_NAME'}``
+    1. The 'local' type, where the 'BAAI/bge-base-zh-v1.5' model
+    is downloaded from HuggingFace and run locally. This is the default model
+    type and there is no setup needed to run this. This model will return cosine
+    similarities around 0.3 when sentences have no semantic similarity. Sentences # NOQA: E501
+    with missing punctuation/different punctuation (one is declarative sentence,
+    one is question) would lower the value to 0.2 ~ 0.3.
+
+    2. The EvalClient type, where you can use a similarlity scorer returned by
+    the given EvalClient. The scorer is typically implemented using the
+    embedding APIs of cloud services. The implementation details are explained
+    in each of the concrete EvalClient classes.
 
     Ref:
         https://huggingface.co/tasks/sentence-similarity
         https://www.sbert.net/docs/usage/semantic_textual_similarity.html
-        https://openai.com/blog/new-embedding-models-and-api-updates
 
     Args:
         generated_outputs: The model generated output(s) to evaluate
         reference_outputs: The reference output(s)
         prompts: The prompts used to generate the output(s). Prompts are
             optional metadata and not used to calculate the metric.
-        model_type: The type of embedding model to use ('local', 'openai', or
-            'azure_openai'), default 'local'
-        openai_client: OpenAI or AzureOpenAI client, default None. If this is
-            None but ``model_type`` is 'openai' or 'azure_openai', we will
-            attempt to create a default client.
-        openai_args: Dict of additional args to pass in to the
-            ``client.embeddings.create`` function, default None
+        eval_model: The type of model to use ('local' or the EvalClient instance
+            used for the evaluation). default 'local'
 
     Returns:
         An :class:`~langcheck.metrics.metric_value.MetricValue` object
     '''
     generated_outputs, reference_outputs, prompts = validate_parameters_reference_based(  # NOQA: E501
         generated_outputs, reference_outputs, prompts)
-    assert model_type in [
-        'local', 'openai', 'azure_openai'
-    ], ('Unsupported embedding model type. '
-        'The supported ones are ["local", "openai", "azure_openai"]')
-    if model_type == 'local':
-        scorer = SentenceTransformerSimilarityScorer(language='ja')
-    else:  # openai or azure_openai
-        scorer = OpenAISimilarityScorer(model_type=model_type,
-                                        openai_client=openai_client,
-                                        openai_args=openai_args)
+
+    if eval_model == 'local':
+        scorer = SentenceTransformerSimilarityScorer(language='zh')
+    else:  # EvalClient
+        assert isinstance(
+            eval_model, EvalClient
+        ), 'An EvalClient must be provided for non-local model types.'
+        scorer = eval_model.similarity_scorer()
     scores = scorer.score(generated_outputs, reference_outputs)
 
     return MetricValue(metric_name='semantic_similarity',
                        prompts=prompts,
                        generated_outputs=generated_outputs,
                        reference_outputs=reference_outputs,
                        sources=None,
                        explanations=None,
                        metric_values=scores,
-                       language='ja')
+                       language='zh')
 
 
 def rouge1(generated_outputs: List[str] | str,
            reference_outputs: List[str] | str,
            prompts: Optional[List[str] | str] = None,
            *,
            tokenizer: Optional[Tokenizer] = None) -> MetricValue[float]:
@@ -122,25 +111,25 @@
     return MetricValue(metric_name='rouge1',
                        prompts=prompts,
                        generated_outputs=generated_outputs,
                        reference_outputs=reference_outputs,
                        sources=None,
                        explanations=None,
                        metric_values=scores,
-                       language='ja')
+                       language='zh')
 
 
 def rouge2(generated_outputs: List[str] | str,
            reference_outputs: List[str] | str,
            prompts: Optional[List[str] | str] = None,
            *,
            tokenizer: Optional[Tokenizer] = None) -> MetricValue[float]:
     '''Calculates the F1 metrics of the ROUGE-2 scores between the generated
     outputs and the reference outputs. It evaluates the overlap of bigrams
-    (two adjacent tokens) between the generated outputs and the reference
+    (two adzhcent tokens) between the generated outputs and the reference
     outputs. This metric takes on float values between [0, 1], where 0 is no
     overlap and 1 is complete overlap.
 
     Ref:
         https://github.com/google-research/google-research/tree/master/rouge
 
     Args:
@@ -162,15 +151,15 @@
     return MetricValue(metric_name='rouge2',
                        prompts=prompts,
                        generated_outputs=generated_outputs,
                        reference_outputs=reference_outputs,
                        sources=None,
                        explanations=None,
                        metric_values=scores,
-                       language='ja')
+                       language='zh')
 
 
 def rougeL(generated_outputs: List[str] | str,
            reference_outputs: List[str] | str,
            prompts: Optional[List[str] | str] = None,
            *,
            tokenizer: Optional[Tokenizer] = None) -> MetricValue[float]:
@@ -212,15 +201,15 @@
     return MetricValue(metric_name='rougeL',
                        prompts=prompts,
                        generated_outputs=generated_outputs,
                        reference_outputs=reference_outputs,
                        sources=None,
                        explanations=None,
                        metric_values=scores,
-                       language='ja')
+                       language='zh')
 
 
 def _rouge(generated_outputs: List[str],
            reference_outputs: List[str],
            rouge_type: str,
            *,
            tokenizer: Optional[Tokenizer] = None) -> List[float]:
@@ -234,18 +223,17 @@
         rouge_type: rouge1, rouge2, or rougeLsum
 
     Returns:
         A list of F1 values of the ROUGE scores
     '''
     assert rouge_type in ['rouge1', 'rouge2', 'rougeLsum']
 
-    # The tokenizer is default to JanomeTokenizer
-    tokenizer = tokenizer or JanomeTokenizer()
+    # The tokenizer is default to HanLPTokenizer
+    tokenizer = tokenizer or HanLPTokenizer()
     scorer = rouge_scorer.RougeScorer([rouge_type],
                                       use_stemmer=True,
                                       tokenizer=tokenizer)
     scores = []
-    for gen, ref in tqdm_wrapper(zip(generated_outputs, reference_outputs),
-                                 total=len(generated_outputs)):
+    for gen, ref in zip(generated_outputs, reference_outputs):
         score = scorer.score(gen, ref)
         scores.append(score[rouge_type].fmeasure)
     return scores
```

### Comparing `langcheck-0.6.0/src/langcheck/metrics/metric_value.py` & `langcheck-0.7.0/src/langcheck/metrics/metric_value.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/model_manager/_model_loader.py` & `langcheck-0.7.0/src/langcheck/metrics/model_manager/_model_loader.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/model_manager/_model_management.py` & `langcheck-0.7.0/src/langcheck/metrics/model_manager/_model_management.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/model_manager/config/metric_config.yaml` & `langcheck-0.7.0/src/langcheck/metrics/model_manager/config/metric_config.yaml`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/reference_based_text_quality.py` & `langcheck-0.7.0/src/langcheck/metrics/reference_based_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/scorer/_base.py` & `langcheck-0.7.0/src/langcheck/metrics/scorer/_base.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/scorer/detoxify_models.py` & `langcheck-0.7.0/src/langcheck/metrics/scorer/detoxify_models.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/scorer/hf_models.py` & `langcheck-0.7.0/src/langcheck/metrics/scorer/hf_models.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/text_structure.py` & `langcheck-0.7.0/src/langcheck/metrics/text_structure.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/zh/__init__.py` & `langcheck-0.7.0/src/langcheck/metrics/zh/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/zh/_tokenizers.py` & `langcheck-0.7.0/src/langcheck/metrics/zh/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/metrics/zh/reference_based_text_quality.py` & `langcheck-0.7.0/src/langcheck/metrics/zh/reference_free_text_quality.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,262 +1,283 @@
 from __future__ import annotations
 
-from typing import Dict, List, Optional
+from typing import List, Optional
 
-from openai import OpenAI
-from rouge_score import rouge_scorer
-from rouge_score.tokenizers import Tokenizer
+import hanlp
+from transformers.pipelines import pipeline
 
-from langcheck.metrics._validation import validate_parameters_reference_based
+from langcheck.metrics._validation import validate_parameters_reference_free
+from langcheck.metrics.en.reference_free_text_quality import \
+    _toxicity_eval_client
+from langcheck.metrics.en.reference_free_text_quality import \
+    sentiment as en_sentiment
+from langcheck.metrics.eval_clients import EvalClient
 from langcheck.metrics.metric_value import MetricValue
-from langcheck.metrics.scorer.hf_models import \
-    SentenceTransformerSimilarityScorer
-from langcheck.metrics.scorer.openai_models import OpenAISimilarityScorer
-from langcheck.metrics.zh._tokenizers import HanLPTokenizer
 
 
-def semantic_similarity(
-        generated_outputs: List[str] | str,
-        reference_outputs: List[str] | str,
-        prompts: Optional[List[str] | str] = None,
-        model_type: str = 'local',
-        openai_client: Optional[OpenAI] = None,
-        openai_args: Optional[Dict[str, str]] = None) -> MetricValue[float]:
-    '''
-    Calculates the semantic similarities between the generated outputs and
-    the reference outputs. The similarities are computed as the cosine
-    similarities between the generated and reference embeddings. This metric
-    takes on float values between [-1, 1], but typically ranges between 0 and 1
-    where 0 is minimum similarity and 1 is maximum similarity. (NOTE: when using
-    OpenAI embeddings, the cosine similarities tend to be skewed quite heavily
-    towards higher numbers.)
-
-    We currently support three embedding model types:
-
-    1. The 'local' type, where the 'BAAI/bge-base-zh-v1.5' model
-    is downloaded from HuggingFace and run locally. This is the default model
-    type and there is no setup needed to run this. This model will return cosine
-    similarities around 0.3 when sentences have no semantic similarity. Sentences # NOQA: E501
-    with missing punctuation/different punctuation (one is declarative sentence,
-    one is question) would lower the value to 0.2 ~ 0.3.
-
-    2. The 'openai' type, where we use OpenAI's 'text-embedding-ada-002' model
-    by default (this is configurable). See
-    `this example <https://langcheck.readthedocs.io/en/latest/metrics.html
-    #computing-metrics-with-openai-models>`__
-    for examples on setting up the OpenAI API key.
-
-    3. The 'azure_openai' type. Essentially the same as the 'openai' type,
-    except that it uses the AzureOpenAI client. Note that you must specify your
-    model deployment to use in ``openai_args``, e.g.
-    ``openai_args={'model': 'YOUR_DEPLOYMENT_NAME'}``
+def sentiment(
+    generated_outputs: List[str] | str,
+    prompts: Optional[List[str] | str] = None,
+    eval_model: str | EvalClient = 'local',
+) -> MetricValue[Optional[float]]:
+    '''Calculates the sentiment scores of generated outputs. This metric takes
+    on float values between [0, 1], where 0 is negative sentiment and 1 is
+    positive sentiment. (NOTE: when using an EvalClient, the sentiment scores
+    are either 0.0 (negative), 0.5 (neutral), or 1.0 (positive). The score may
+    also be `None` if it could not be computed.)
+
+    We currently support two evaluation model types:
+
+    1. The 'local' type, where the IDEA-CCNL/Erlangshen-Roberta-110M-Sentiment
+    model is downloaded from HuggingFace and run locally. This is the default
+    model type and there is no setup needed to run this.
+
+    2. The EvalClient type, where you can use an EvalClient typically
+    implemented with an LLM. The implementation details are explained in each of
+    the concrete EvalClient classes.
 
     Ref:
-        https://huggingface.co/tasks/sentence-similarity
-        https://www.sbert.net/docs/usage/semantic_textual_similarity.html
-        https://openai.com/blog/new-and-improved-embedding-model
+        https://huggingface.co/IDEA-CCNL/Erlangshen-Roberta-110M-Sentiment
 
     Args:
         generated_outputs: The model generated output(s) to evaluate
-        reference_outputs: The reference output(s)
         prompts: The prompts used to generate the output(s). Prompts are
             optional metadata and not used to calculate the metric.
-        model_type: The type of embedding model to use ('local', 'openai', or
-            'azure_openai'), default 'local'
-        openai_client: OpenAI or AzureOpenAI client, default None. If this is
-            None but ``model_type`` is 'openai' or 'azure_openai', we will
-            attempt to create a default client.
-        openai_args: Dict of additional args to pass in to the
-            ``client.embeddings.create`` function, default None
+        eval_model: The type of model to use ('local' or the EvalClient instance
+            used for the evaluation). default 'local'
 
     Returns:
         An :class:`~langcheck.metrics.metric_value.MetricValue` object
     '''
-    generated_outputs, reference_outputs, prompts = validate_parameters_reference_based(  # NOQA: E501
-        generated_outputs, reference_outputs, prompts)
-    assert model_type in [
-        'local', 'openai', 'azure_openai'
-    ], ('Unsupported embedding model type. '
-        'The supported ones are ["local", "openai", "azure_openai"]')
-    generated_outputs, reference_outputs, prompts = validate_parameters_reference_based(  # NOQA: E501
-        generated_outputs, reference_outputs, prompts)
-    assert model_type in [
-        'local', 'openai', 'azure_openai'
-    ], ('Unsupported embedding model type. '
-        'The supported ones are ["local", "openai", "azure_openai"]')
-
-    if model_type == 'local':
-        scorer = SentenceTransformerSimilarityScorer(language='zh')
-    else:  # openai or azure_openai
-        scorer = OpenAISimilarityScorer(model_type=model_type,
-                                        openai_client=openai_client,
-                                        openai_args=openai_args)
-    scores = scorer.score(generated_outputs, reference_outputs)
+    generated_outputs, prompts = validate_parameters_reference_free(
+        generated_outputs, prompts)
 
-    return MetricValue(metric_name='semantic_similarity',
-                       prompts=prompts,
-                       generated_outputs=generated_outputs,
-                       reference_outputs=reference_outputs,
-                       sources=None,
-                       explanations=None,
-                       metric_values=scores,
-                       language='zh')
+    if eval_model != 'local':  # EvalClient
+        assert isinstance(
+            eval_model, EvalClient
+        ), 'An EvalClient must be provided for non-local model types.'
+
+        # This reuses the English prompt.
+        # TODO: Update this to use a Chinese prompt.
+        metric_value = en_sentiment(generated_outputs, prompts, eval_model)
+        metric_value.language = 'zh'
+        return metric_value
+
+    # {0:"Negative", 1:'Positive'}
+    from langcheck.metrics.model_manager import manager
+    tokenizer, model = manager.fetch_model(language='zh', metric='sentiment')
+    _sentiment_pipeline = pipeline(
+        'sentiment-analysis',
+        model=model,  # type: ignore[reportGeneralTypeIssues]
+        tokenizer=tokenizer  # type: ignore[reportGeneralTypeIssues]
+    )
+    _model_id2label = _sentiment_pipeline.model.config.id2label
+    _predict_result = _sentiment_pipeline(
+        generated_outputs
+    )  # type: ignore[reportGeneralTypeIssues]  # NOQA: E501
+    # if predicted result is 'Positive', use the score directly
+    # else, use 1 - score as the sentiment score
+    # yapf: disable
+    scores = [
+        1 - x['score'] if x['label'] == _model_id2label[0] else x['score']  # type: ignore[reportGeneralTypeIssues]  # NOQA: E501
+        for x in _predict_result   # type: ignore[reportGeneralTypeIssues]  # NOQA: E501
+    ]
+    # yapf: enable
+    return MetricValue(
+        metric_name='sentiment',
+        prompts=prompts,
+        generated_outputs=generated_outputs,
+        reference_outputs=None,
+        sources=None,
+        explanations=None,
+        metric_values=scores,  # type: ignore[reportGeneralTypeIssues]
+        language='zh')
 
 
-def rouge1(generated_outputs: List[str] | str,
-           reference_outputs: List[str] | str,
-           prompts: Optional[List[str] | str] = None,
-           *,
-           tokenizer: Optional[Tokenizer] = None) -> MetricValue[float]:
-    '''Calculates the F1 metrics of the ROUGE-1 scores between the generated
-    (single tokens) between the generated outputs and the reference outputs.
-    This metric takes on float values between [0, 1], where 0 is no overlap and
-    1 is complete overlap.
+def toxicity(
+        generated_outputs: List[str] | str,
+        prompts: Optional[List[str] | str] = None,
+        eval_model: str | EvalClient = 'local') -> MetricValue[Optional[float]]:
+    '''Calculates the toxicity scores of generated outputs. This metric takes on
+    float values between [0, 1], where 0 is low toxicity and 1 is high toxicity.
+    (NOTE: when using an EvalClient, the toxicity scores are in steps of
+    0.25. The score may also be `None` if it could not be computed.)
+
+    We currently support two evaluation model types:
+
+    1. The 'local' type, where a model file is downloaded from HuggingFace and
+    run locally. This is the default model type and there is no setup needed to
+    run this.
+    The model (alibaba-pai/pai-bert-base-zh-llm-risk-detection) is a
+    risky detection model for LLM generated content released by Alibaba group.
+
+    2. The EvalClient type, where you can use an EvalClient typically
+    implemented with an LLM. The implementation details are explained in each of
+    the concrete EvalClient classes.
 
     Ref:
-        https://github.com/google-research/google-research/tree/master/rouge
+        https://huggingface.co/alibaba-pai/pai-bert-base-zh-llm-risk-detection
 
     Args:
         generated_outputs: The model generated output(s) to evaluate
-        reference_outputs: The reference output(s)
         prompts: The prompts used to generate the output(s). Prompts are
             optional metadata and not used to calculate the metric.
+        eval_model: The type of model to use ('local' or the EvalClient instance
+            used for the evaluation). default 'local'
 
     Returns:
-        An MetricValue object
+        An :class:`~langcheck.metrics.metric_value.MetricValue` object
     '''
-    generated_outputs, reference_outputs, prompts = validate_parameters_reference_based(  # NOQA: E501
-        generated_outputs, reference_outputs, prompts)
+    generated_outputs, prompts = validate_parameters_reference_free(
+        generated_outputs, prompts)
+
+    if eval_model == 'local':
+        scores = _toxicity_local(generated_outputs)
+        explanations = None
+    else:
+        assert isinstance(
+            eval_model, EvalClient
+        ), 'An EvalClient must be provided for non-local model types.'
+
+        # This reuses the English prompt.
+        # TODO: Update this to use a Chinese prompt.
+        scores, explanations = _toxicity_eval_client(generated_outputs,
+                                                     eval_model)
 
-    scores = _rouge(generated_outputs,
-                    reference_outputs,
-                    'rouge1',
-                    tokenizer=tokenizer)
-    return MetricValue(metric_name='rouge1',
+    return MetricValue(metric_name='toxicity',
                        prompts=prompts,
                        generated_outputs=generated_outputs,
-                       reference_outputs=reference_outputs,
+                       reference_outputs=None,
                        sources=None,
-                       explanations=None,
+                       explanations=explanations,
                        metric_values=scores,
                        language='zh')
 
 
-def rouge2(generated_outputs: List[str] | str,
-           reference_outputs: List[str] | str,
-           prompts: Optional[List[str] | str] = None,
-           *,
-           tokenizer: Optional[Tokenizer] = None) -> MetricValue[float]:
-    '''Calculates the F1 metrics of the ROUGE-2 scores between the generated
-    outputs and the reference outputs. It evaluates the overlap of bigrams
-    (two adzhcent tokens) between the generated outputs and the reference
-    outputs. This metric takes on float values between [0, 1], where 0 is no
-    overlap and 1 is complete overlap.
+def _toxicity_local(generated_outputs: List[str]) -> List[float]:
+    '''Calculates the toxicity scores of generated outputs using a fine-tuned
+    model from `alibaba-pai/pai-bert-base-zh-llm-risk-detection`. This metric
+    takes on float values between [0, 1], where 0 is low toxicity and 1 is high
+    toxicity.
 
     Ref:
-        https://github.com/google-research/google-research/tree/master/rouge
+        https://huggingface.co/alibaba-pai/pai-bert-base-zh-llm-risk-detection
 
     Args:
-        generated_outputs: The model generated output(s) to evaluate
-        reference_outputs: The reference output(s)
-        prompts: The prompts used to generate the output(s). Prompts are
-            optional metadata and not used to calculate the metric.
+        generated_outputs: A list of model generated outputs to evaluate
 
     Returns:
-        An MetricValue object
+        A list of scores
     '''
-    generated_outputs, reference_outputs, prompts = validate_parameters_reference_based(  # NOQA: E501
-        generated_outputs, reference_outputs, prompts)
-
-    scores = _rouge(generated_outputs,
-                    reference_outputs,
-                    'rouge2',
-                    tokenizer=tokenizer)
-    return MetricValue(metric_name='rouge2',
-                       prompts=prompts,
-                       generated_outputs=generated_outputs,
-                       reference_outputs=reference_outputs,
-                       sources=None,
-                       explanations=None,
-                       metric_values=scores,
-                       language='zh')
+    # this pipeline output predict probability for each text on each label.
+    # the output format is List[List[Dict(str)]]
+    from langcheck.metrics.model_manager import manager
+    tokenizer, model = manager.fetch_model(language='zh', metric="toxicity")
+    _toxicity_pipeline = pipeline(
+        'text-classification',
+        model=model,  # type: ignore[reportOptionalIterable]
+        tokenizer=tokenizer,  # type: ignore[reportOptionalIterable]
+        top_k=5)
+    # {'Normal': 0, 'Pulp': 1, 'Sex': 2, 'Other Risk': 3, 'Adult': 4}
+    _model_id2label = _toxicity_pipeline.model.config.id2label
+    _predict_results = _toxicity_pipeline(
+        generated_outputs  # type: ignore[reportGeneralTypeIssues]
+    )
+    # labels except Normal are all risky, toxicity_score = 1-score['Normal']
+    toxicity_scores = []
+    for item_predict_proba in _predict_results:  # type: ignore[reportOptionalIterable]  # NOQA: E501
+        for label_proba in item_predict_proba:  # type: ignore[reportGeneralTypeIssues]  # NOQA: E501
+            # yapf: disable
+            if label_proba['label'] == _model_id2label[0]:  # type: ignore[reportGeneralTypeIssues]  # NOQA: E501
+                toxicity_scores.append(1 - label_proba['score'])  # type: ignore[reportGeneralTypeIssues]  # NOQA: E501
+            # yapf: enable
+    return toxicity_scores  # type: ignore[reportGeneralTypeIssues]
 
 
-def rougeL(generated_outputs: List[str] | str,
-           reference_outputs: List[str] | str,
-           prompts: Optional[List[str] | str] = None,
-           *,
-           tokenizer: Optional[Tokenizer] = None) -> MetricValue[float]:
-    '''Calculates the F1 metrics of the ROUGE-L scores between the generated
-    outputs and the reference outputs. It evaluates the longest common
-    subsequence (LCS) between the generated outputs and the reference outputs.
-    This metric takes on float values between [0, 1], where 0 means that the LCS
-    is empty and 1 means that the reference and generated outputs are the same.
+def xuyaochen_report_readability(
+        generated_outputs: List[str] | str,
+        prompts: Optional[List[str] | str] = None) -> MetricValue[float]:
+    '''Calculates the readability scores of generated outputs introduced in
+    "中文年报可读性"(Chinese annual report readability). This metric calculates
+    average words per sentence as r1, average of the sum of the numbers of
+    adverbs and coordinating conjunction words in a sentence in given generated
+    outputs as r2, then, refer to the Fog Index that combine r1 with r2 by
+    arithmetic mean as the final outputs. This function uses HanLP Tokenizer and
+    POS at the same time, POS in CTB style
+    https://hanlp.hankcs.com/docs/annotations/pos/ctb.html.
+    The lower the score is, the better the readability. The score is mainly
+    influenced by r1, the average number of words in sentences.
 
     Ref:
-        https://github.com/google-research/google-research/tree/master/rouge
+        Refer Chinese annual report readability: measurement and test
+        Link: https://www.tandfonline.com/doi/full/10.1080/21697213.2019.1701259
 
     Args:
-        generated_outputs: The model generated output(s) to evaluate
-        reference_outputs: The reference output(s)
+        generated_outputs: A list of model generated outputs to evaluate
         prompts: The prompts used to generate the output(s). Prompts are
             optional metadata and not used to calculate the metric.
 
     Returns:
-        An MetricValue object
+        A list of scores
     '''
-    generated_outputs, reference_outputs, prompts = validate_parameters_reference_based(  # NOQA: E501
-        generated_outputs, reference_outputs, prompts)
-
-    # The `rouge_score` package has two flavors of ROUGE-L [1]:
-    # - 1) sentence-level, where newline characters are ignored
-    # - 2) summary-level, where newline characters are interpreted as sentence
-    #      boundaries
-    #
-    # We use (2) here (i.e. `rougeLsum`) because this is how `pyrouge` computes
-    # the ROUGE-L score (https://github.com/bheinzerling/pyrouge), which is a
-    # Python wrapper around original perl script implementation.
-    #
-    # [1] https://github.com/google-research/google-research/tree/master/rouge#two-flavors-of-rouge-l # NOQA: E501
-    scores = _rouge(generated_outputs,
-                    reference_outputs,
-                    'rougeLsum',
-                    tokenizer=tokenizer)
-    return MetricValue(metric_name='rougeL',
+    # split generated_outputs into sentence
+    generated_outputs, prompts = validate_parameters_reference_free(
+        generated_outputs, prompts=prompts)
+    # yapf: disable
+    tokenizer = hanlp.load(
+        hanlp.pretrained.tok.FINE_ELECTRA_SMALL_ZH  # type: ignore[reportGeneralTypeIssues] # NOQA: E501
+    )
+    postagger = hanlp.load(
+        hanlp.pretrained.pos.CTB9_POS_RADICAL_ELECTRA_SMALL   # type: ignore[reportGeneralTypeIssues] # NOQA: E501
+    )
+
+    pos_pipeline = hanlp.pipeline().\
+        append(hanlp.utils.rules.split_sentence)  # type: ignore[reportGeneralTypeIssues] # NOQA: E501
+    pos_pipeline = pos_pipeline.append(tokenizer).append(postagger)
+
+    tokenize_pipeline = hanlp.pipeline().\
+        append(hanlp.utils.rules.split_sentence)  # type: ignore[reportGeneralTypeIssues] # NOQA: E501
+    tokenize_pipeline = tokenize_pipeline.append(tokenizer)
+    # OUTPUT: List[List[List[TOKEN]]]
+    output_tokens = list(map(tokenize_pipeline, generated_outputs))
+    # List[List[List[POS]]]
+    output_pos = list(map(pos_pipeline, generated_outputs))
+
+    def count_tokens(sent_tokens: List[str]) -> int:
+        count = sum([
+            not hanlp.utils.string_util.ispunct(token) for token in   # type: ignore[reportGeneralTypeIssues] # NOQA: E501
+            sent_tokens
+        ])
+        return count
+
+    def count_postags(sent_poses: List[str]) -> int:
+        # AD: adverb, CC: coordinating conjunction,
+        # CS: subordinating conjunction
+        count = sum([pos in ['AD', 'CC', 'CS'] for pos in sent_poses])
+        return count
+
+    def calc_r1(content: List[List[str]]) -> float:
+        token_count_by_sentence = list(map(count_tokens, content))
+        if len(token_count_by_sentence) == 0:
+            return 0
+        else:
+            return sum(token_count_by_sentence) / len(token_count_by_sentence)
+
+    def calc_r2(content: List[List[str]]) -> float:
+        pos_count_by_sentence = list(map(count_postags, content))
+        if len(pos_count_by_sentence) == 0:
+            return 0
+        else:
+            return sum(pos_count_by_sentence) / len(pos_count_by_sentence)
+
+    r1 = list(map(calc_r1, output_tokens))   # type: ignore[reportGeneralTypeIssues] # NOQA: E501
+    r2 = list(map(calc_r2, output_pos))   # type: ignore[reportGeneralTypeIssues] # NOQA: E501
+    r3 = [(r1_score + r2_score) * 0.5 for r1_score, r2_score in zip(r1, r2)]
+    # yapf: enable
+    return MetricValue(metric_name='readability',
                        prompts=prompts,
                        generated_outputs=generated_outputs,
-                       reference_outputs=reference_outputs,
                        sources=None,
+                       reference_outputs=None,
                        explanations=None,
-                       metric_values=scores,
+                       metric_values=r3,
                        language='zh')
-
-
-def _rouge(generated_outputs: List[str],
-           reference_outputs: List[str],
-           rouge_type: str,
-           *,
-           tokenizer: Optional[Tokenizer] = None) -> List[float]:
-    '''Helper function for computing the rouge1, rouge2, and rougeL metrics.
-    This uses Google Research's implementation of ROUGE:
-    https://github.com/google-research/google-research/tree/master/rouge
-
-    Args:
-        generated_outputs: A list of model generated outputs to evaluate
-        reference_outputs: A list of reference outputs
-        rouge_type: rouge1, rouge2, or rougeLsum
-
-    Returns:
-        A list of F1 values of the ROUGE scores
-    '''
-    assert rouge_type in ['rouge1', 'rouge2', 'rougeLsum']
-
-    # The tokenizer is default to HanLPTokenizer
-    tokenizer = tokenizer or HanLPTokenizer()
-    scorer = rouge_scorer.RougeScorer([rouge_type],
-                                      use_stemmer=True,
-                                      tokenizer=tokenizer)
-    scores = []
-    for gen, ref in zip(generated_outputs, reference_outputs):
-        score = scorer.score(gen, ref)
-        scores.append(score[rouge_type].fmeasure)
-    return scores
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `langcheck-0.6.0/src/langcheck/plot/_css.py` & `langcheck-0.7.0/src/langcheck/plot/_css.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/plot/_histogram.py` & `langcheck-0.7.0/src/langcheck/plot/_histogram.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/plot/_scatter.py` & `langcheck-0.7.0/src/langcheck/plot/_scatter.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/plot/_utils.py` & `langcheck-0.7.0/src/langcheck/plot/_utils.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck/stats.py` & `langcheck-0.7.0/src/langcheck/stats.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.6.0/src/langcheck.egg-info/PKG-INFO` & `langcheck-0.7.0/src/langcheck.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langcheck
-Version: 0.6.0
+Version: 0.7.0
 Summary: Simple, Pythonic building blocks to evaluate LLM-based applications
 Author-email: Citadel AI <info@citadel.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Citadel AI
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,14 +29,15 @@
 Keywords: llm,ai,nlp,evaluation,validation,testing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dash>=2.11
+Requires-Dist: Jinja2
 Requires-Dist: nlpaug
 Requires-Dist: nltk>=3
 Requires-Dist: openai>=1
 Requires-Dist: pandas>=1
 Requires-Dist: plotly>=5
 Requires-Dist: rouge-score>=0.1.2
 Requires-Dist: sentence-transformers>=2
@@ -56,20 +57,26 @@
 Requires-Dist: unidic-lite>=1.0.1; extra == "ja"
 Provides-Extra: ja-optional
 Requires-Dist: mecab-python3>=1.0.4; extra == "ja-optional"
 Requires-Dist: sudachidict-core; extra == "ja-optional"
 Requires-Dist: sudachipy; extra == "ja-optional"
 Provides-Extra: zh
 Requires-Dist: hanlp>=2.1.0b33; extra == "zh"
+Provides-Extra: anthropic
+Requires-Dist: anthropic; extra == "anthropic"
+Provides-Extra: gemini
+Requires-Dist: google-generativeai; extra == "gemini"
 Provides-Extra: all
 Requires-Dist: langcheck[de]; extra == "all"
 Requires-Dist: langcheck[en]; extra == "all"
 Requires-Dist: langcheck[ja]; extra == "all"
 Requires-Dist: langcheck[ja-optional]; extra == "all"
 Requires-Dist: langcheck[zh]; extra == "all"
+Requires-Dist: langcheck[anthropic]; extra == "all"
+Requires-Dist: langcheck[gemini]; extra == "all"
 Provides-Extra: dev
 Requires-Dist: yapf==0.40.1; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `langcheck-0.6.0/src/langcheck.egg-info/requires.txt` & `langcheck-0.7.0/src/langcheck.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 dash>=2.11
+Jinja2
 nlpaug
 nltk>=3
 openai>=1
 pandas>=1
 plotly>=5
 rouge-score>=0.1.2
 sentence-transformers>=2
@@ -20,14 +21,19 @@
 
 [all]
 langcheck[de]
 langcheck[en]
 langcheck[ja]
 langcheck[ja-optional]
 langcheck[zh]
+langcheck[anthropic]
+langcheck[gemini]
+
+[anthropic]
+anthropic
 
 [de]
 
 [dev]
 yapf==0.40.1
 flake8
 isort
@@ -38,14 +44,17 @@
 sphinx-book-theme
 myst-parser
 ipykernel
 sphinxcontrib-youtube
 
 [en]
 
+[gemini]
+google-generativeai
+
 [ja]
 chikkarpy
 fugashi
 janome>=0.3.1
 unidic-lite>=1.0.1
 
 [ja-optional]
```

### Comparing `langcheck-0.6.0/tests/test_stats.py` & `langcheck-0.7.0/tests/test_stats.py`

 * *Files identical despite different names*

