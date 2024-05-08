# Comparing `tmp/acceldata_sdk-3.3.0.tar.gz` & `tmp/acceldata_sdk-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acceldata_sdk-3.3.0.tar", last modified: Mon Apr 15 09:07:02 2024, max compression
+gzip compressed data, was "acceldata_sdk-3.4.0.tar", last modified: Wed May  8 11:06:44 2024, max compression
```

## Comparing `acceldata_sdk-3.3.0.tar` & `acceldata_sdk-3.4.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.452101 acceldata_sdk-3.3.0/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       91 2024-04-15 09:06:32.000000 acceldata_sdk-3.3.0/CHANGELOG.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3952 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/DATASOURCE_README.md
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/LICENCE.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/MANIFEST.in
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23642 2024-04-15 09:07:02.451700 acceldata_sdk-3.3.0/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    18890 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/README.md
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/README.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.440179 acceldata_sdk-3.3.0/acceldata_sdk/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1227 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/client.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     7776 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/common.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2098 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      329 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/datetime_utils.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      172 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/errors.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.442022 acceldata_sdk-3.3.0/acceldata_sdk/events/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/events/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      903 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/events/generic_event.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1016 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/events/job_events.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      826 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/events/log_events.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1487 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/events/span_event.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      328 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/initialiser.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.446176 acceldata_sdk-3.3.0/acceldata_sdk/models/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      162 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     6106 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/asset.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      664 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/assetType.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10021 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/connection.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3522 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/create_asset.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     8164 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/datasource.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10268 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/dqrule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4599 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/job.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    24639 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/pipeline.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2015 2024-03-21 11:14:24.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/profile.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    11785 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/reconcillationrule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     5929 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/rule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10102 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/ruleExecutionResult.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2396 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/span.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10582 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/span_context.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3810 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/tags.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    15832 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/torch_client.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    48544 2024-04-15 09:06:32.000000 acceldata_sdk-3.3.0/acceldata_sdk/torch_http_client.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.451055 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23642 2024-04-15 09:07:02.000000 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1923 2024-04-15 09:07:02.000000 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2024-04-15 09:07:02.000000 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      117 2024-04-15 09:07:02.000000 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/requires.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       14 2024-04-15 09:07:02.000000 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.446411 acceldata_sdk-3.3.0/docs/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.435983 acceldata_sdk-3.3.0/docs/_build/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.436046 acceldata_sdk-3.3.0/docs/_build/html/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.448592 acceldata_sdk-3.3.0/docs/_build/html/_sources/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      491 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       72 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       54 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/readme.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       45 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/readme_datasource.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       34 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/readme_pipeline.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      921 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.events.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1731 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.models.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1070 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1946 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/conf.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.450745 acceldata_sdk-3.3.0/integration_tests/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      887 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/integration_tests/test_constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3765 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/integration_tests/test_ds_assets.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    11805 2024-03-21 11:14:17.000000 acceldata_sdk-3.3.0/integration_tests/test_external_integration_default_time.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    15535 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/integration_tests/test_external_integration_explicit_time.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4488 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/integration_tests/test_pipelines.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4386 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/integration_tests/test_policy.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    27169 2024-04-15 09:06:32.000000 acceldata_sdk-3.3.0/integration_tests/test_torch_client.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2024-04-15 09:07:02.452164 acceldata_sdk-3.3.0/setup.cfg
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1238 2024-04-15 09:06:32.000000 acceldata_sdk-3.3.0/setup.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.560537 acceldata_sdk-3.4.0/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      213 2024-05-08 11:01:16.000000 acceldata_sdk-3.4.0/CHANGELOG.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3952 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/DATASOURCE_README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/LICENCE.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/MANIFEST.in
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23764 2024-05-08 11:06:44.559992 acceldata_sdk-3.4.0/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    18890 2024-05-08 11:01:16.000000 acceldata_sdk-3.4.0/README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/README.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.536074 acceldata_sdk-3.4.0/acceldata_sdk/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1227 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     7776 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/common.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2098 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      329 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/datetime_utils.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      172 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/errors.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.538674 acceldata_sdk-3.4.0/acceldata_sdk/events/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/events/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      903 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/events/generic_event.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1016 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/events/job_events.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      826 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/events/log_events.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1487 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/events/span_event.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      328 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/initialiser.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.552034 acceldata_sdk-3.4.0/acceldata_sdk/models/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      162 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6106 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/asset.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      664 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/assetType.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10021 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/connection.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3522 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/create_asset.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     8164 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/datasource.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10268 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/dqrule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4599 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/job.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    24639 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/pipeline.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2015 2024-03-21 11:14:24.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/profile.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    11785 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/reconcillationrule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     5929 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/rule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10102 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/ruleExecutionResult.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2396 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/span.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10582 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/span_context.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3810 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/acceldata_sdk/models/tags.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    15888 2024-05-08 11:01:16.000000 acceldata_sdk-3.4.0/acceldata_sdk/torch_client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    48151 2024-05-08 11:01:16.000000 acceldata_sdk-3.4.0/acceldata_sdk/torch_http_client.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.559519 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23764 2024-05-08 11:06:44.000000 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1923 2024-05-08 11:06:44.000000 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2024-05-08 11:06:44.000000 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      117 2024-05-08 11:06:44.000000 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/requires.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       14 2024-05-08 11:06:44.000000 acceldata_sdk-3.4.0/acceldata_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.552265 acceldata_sdk-3.4.0/docs/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.531315 acceldata_sdk-3.4.0/docs/_build/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.531392 acceldata_sdk-3.4.0/docs/_build/html/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.556143 acceldata_sdk-3.4.0/docs/_build/html/_sources/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      491 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       72 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       54 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/readme.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       45 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/readme_datasource.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       34 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/readme_pipeline.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      921 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.events.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1731 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.models.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1070 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1946 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/docs/conf.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:06:44.558026 acceldata_sdk-3.4.0/integration_tests/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      887 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/integration_tests/test_constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3765 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/integration_tests/test_ds_assets.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    11805 2024-03-21 11:14:17.000000 acceldata_sdk-3.4.0/integration_tests/test_external_integration_default_time.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    15535 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/integration_tests/test_external_integration_explicit_time.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4488 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/integration_tests/test_pipelines.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4386 2024-02-22 04:32:27.000000 acceldata_sdk-3.4.0/integration_tests/test_policy.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    27169 2024-05-02 08:45:58.000000 acceldata_sdk-3.4.0/integration_tests/test_torch_client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2024-05-08 11:06:44.560614 acceldata_sdk-3.4.0/setup.cfg
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1238 2024-05-08 11:01:16.000000 acceldata_sdk-3.4.0/setup.py
```

### Comparing `acceldata_sdk-3.3.0/DATASOURCE_README.md` & `acceldata_sdk-3.4.0/DATASOURCE_README.md`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/LICENCE.txt` & `acceldata_sdk-3.4.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/PKG-INFO` & `acceldata_sdk-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_sdk
-Version: 3.3.0
+Version: 3.4.0
 Summary: Acceldata SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,15 +30,15 @@
 ```bash
 pip install acceldata-sdk
 ```
 
 ## Create Torch Client
 Torch client is used to send data to the torch servers. It consists of various methods to communicate with the torch server. Torch client have access to catalog and pipeline APIs. To create a torch client, torch url and API keys are required. To create torch API keys, go to torch ui’s settings and generate keys for the client.
 
-While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is enabled. If we want we can disable that check by passing `do_version_check` as `False.
+While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is disabled. If we want we can enable that check by passing `do_version_check` as `True`.
 
 
 ```python
 from acceldata_sdk.torch_client import TorchClient
 
 torch_client = TorchClient(url='https://acceldata.host.dev:9999', access_key='******',
                          secret_key='*****************', do_version_check=True)
@@ -519,11 +519,12 @@
 # List all rules
 recon_rules = torch_client.list_all_policies(filter=filter)
 ```
 
 Version Log
 ==========
 
-3.3.0 (15/04/2024)
+3.4.0 (08/05/2024)
 -------------------
-- Improved sample data api
+- Incorporated fix for control plane version compatibility check based apis to handle patch version
+- Disable version compatibility check by default
```

### Comparing `acceldata_sdk-3.3.0/README.md` & `acceldata_sdk-3.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ```bash
 pip install acceldata-sdk
 ```
 
 ## Create Torch Client
 Torch client is used to send data to the torch servers. It consists of various methods to communicate with the torch server. Torch client have access to catalog and pipeline APIs. To create a torch client, torch url and API keys are required. To create torch API keys, go to torch ui’s settings and generate keys for the client.
 
-While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is enabled. If we want we can disable that check by passing `do_version_check` as `False.
+While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is disabled. If we want we can enable that check by passing `do_version_check` as `True`.
 
 
 ```python
 from acceldata_sdk.torch_client import TorchClient
 
 torch_client = TorchClient(url='https://acceldata.host.dev:9999', access_key='******',
                          secret_key='*****************', do_version_check=True)
```

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/client.py` & `acceldata_sdk-3.4.0/acceldata_sdk/client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/common.py` & `acceldata_sdk-3.4.0/acceldata_sdk/common.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/constants.py` & `acceldata_sdk-3.4.0/acceldata_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/events/generic_event.py` & `acceldata_sdk-3.4.0/acceldata_sdk/events/generic_event.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/events/job_events.py` & `acceldata_sdk-3.4.0/acceldata_sdk/events/job_events.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/events/log_events.py` & `acceldata_sdk-3.4.0/acceldata_sdk/events/log_events.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/events/span_event.py` & `acceldata_sdk-3.4.0/acceldata_sdk/events/span_event.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/asset.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/asset.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/assetType.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/assetType.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/connection.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/connection.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/create_asset.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/create_asset.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/datasource.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/datasource.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/dqrule.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/dqrule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/job.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/job.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/pipeline.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/profile.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/profile.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/reconcillationrule.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/reconcillationrule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/rule.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/rule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/ruleExecutionResult.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/ruleExecutionResult.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/span.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/span.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/span_context.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/span_context.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/models/tags.py` & `acceldata_sdk-3.4.0/acceldata_sdk/models/tags.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/torch_client.py` & `acceldata_sdk-3.4.0/acceldata_sdk/torch_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 
     """
             Description : Torch user client is used to send data to catalog server.
             :param url: (String) url of the catalog server
             :param timeout_ms: (Integer) timeout of the requests sending to catalog
             :param access_key: (String) Access key of API key. You can generate API key from torch UI's setting
             :param secret_key: (String) Secret key of API key.
-            :param do_version_check: (bool) Enable version compatibility check between sdk and torch.
+            :param do_version_check: (bool) Enable/Disable version compatibility check between sdk and ADOC. By default version checks are disabled.
             Ex.  TorchClient = TorchUserClient(url='https://torch.acceldata.local:5443', access_key='OY2VVIN2N6LJ', secret_key='da6bDBimQfXSMsyyhlPVJJfk7Zc2gs')
     """
 
     def __init__(self, url, timeout_ms=10000, access_key: str = None, secret_key: str = None,
-                 do_version_check: bool = True):
+                 do_version_check: bool = False):
         """
                 Description : Torch user client is used to send data to catalog server.
                 :param url: (String) url of the catalog server
                 :param timeout_ms: (Integer) timeout of the requests sending to catalog
                 :param access_key: (String) Access key of API key. You can generate API key from torch UI's setting
                 :param secret_key: (String) Secret key of API key.
-                :param do_version_check: (bool) Enable version compatibility check between sdk and torch.
+                :param do_version_check: (bool) Enable/Disable version compatibility check between sdk and torch.
                 Ex.  TorchClient = TorchUserClient(url='https://torch.acceldata.local:5443', access_key='OY2VVIN2N6LJ', secret_key='da6bDBimQfXSMsyyhlPVJJfk7Zc2gs')
         """
         if access_key is None and secret_key is None:
             raise Exception('Access key and secret key - required')
         self.client = TorchHttpClient(url=url, access_key=access_key, secret_key=secret_key, timeout_ms=timeout_ms)
         if isinstance(do_version_check, str):
             self.do_version_check = bool(distutils.util.strtobool(do_version_check))
```

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk/torch_http_client.py` & `acceldata_sdk-3.4.0/acceldata_sdk/torch_http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,22 +39,46 @@
 
 _HEADERS = {'User-Agent': 'Acceldata-sdk', 'accessKey': None, 'secretKey': None, 'Content-Type': 'application/json'}
 catalog_api_path = "/catalog-server/api"
 pipeline_api_path = "/torch-pipeline/api"
 admin_api_path = "/admin/api"
 
 import urllib3
+import re
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
+def _has_leading_zero(value):
+    return (value
+            and value[0] == '0'
+            and value.isdigit()
+            and value != '0')
+
 
 def extract_actual_version(torch_version) -> str:
     if torch_version.buildVersion:
-        parsed_version = Version(torch_version.buildVersion)
-        actual_version = f'{parsed_version.major}.{parsed_version.minor}.{parsed_version.patch}'
+        version_string =torch_version.buildVersion
+        version_re = re.compile(r'^(\d+)(?:\.(\d+)(?:\.(\d+))?)?(?:-(.*))?$')
+        match = version_re.match(version_string)
+        if not match:
+            raise ValueError('Invalid version string: %r' % version_string)
+
+        major, minor, patch, others = match.groups()
+
+        if _has_leading_zero(major):
+            raise ValueError("Invalid leading zero in major: %r" % version_string)
+        if _has_leading_zero(minor):
+            raise ValueError("Invalid leading zero in minor: %r" % version_string)
+        if _has_leading_zero(patch):
+            raise ValueError("Invalid leading zero in patch: %r" % version_string)
+
+        major = int(major)
+        minor = int(minor)
+        patch = int(patch)
+        actual_version = f'{major}.{minor}.{patch}'
         return actual_version
     else:
         raise TorchSdkException(f'Torch version is not available.')
 
 
 def validate_torch_version(actual_version):
     if Version(MIN_TORCH_BACKEND_VERSION_FOR_RULE_ID_API) not in SimpleSpec(f'<={actual_version}'):
@@ -117,19 +141,19 @@
     :param months_before: Number of months to subtract from the current month.
     :return: A tuple containing two datetime objects -
              the starting time before the given months from the beginning of the current month and
              the ending time as the beginning of the current month.
     """
     now = datetime.now()
     first_day_of_months_before = (now - relativedelta(months=months_before)).replace(day=1, hour=0, minute=0, second=0,
-                                                                       microsecond=0)
+                                                                                     microsecond=0)
     last_day_of_prev_month = now.replace(day=1, hour=0, minute=0, second=0, microsecond=0)
     started_after_time = first_day_of_months_before
     finished_before_time = last_day_of_prev_month
-    return started_after_time,finished_before_time
+    return started_after_time, finished_before_time
 
 
 def calculate_time_range(filter):
     if filter.period is not None:
         now = datetime.now()
         finished_before_time = now
         started_after_time = None  # Initialize to None
@@ -382,46 +406,26 @@
             Description:
                 To get pipeline run with particular id or continuation id of any pipeline
         :param pipeline_run_id: run id of the pipeline run
         :param continuation_id: continuation id of the pipeline run
         :param pipeline_id: id of the pipeline. This is a mandatory parameter when run is being queried using continuation_id
         :return: PipelineRun instance
         """
-        payload = dict()
-        return_run = dict()
         if pipeline_run_id is not None:
             url = f'{self._pipeline_api_base}/pipelines/runs/{pipeline_run_id}'
             response = self._get(url)
             return_run = response['run']
         elif continuation_id is not None and pipeline_id is not None:
-            supported_versions = self.get_supported_sdk_versions()
-            torch_version: str = self.get_torch_version()
-            if torch_version.buildVersion is not None and torch_version.buildVersion != "":
-                # Parse the semantic version string
-                parsed_version = semantic_version.Version(torch_version.buildVersion)
-                actual_version = f'{parsed_version.major}.{parsed_version.minor}.{parsed_version.patch}'
+            url = f'{self._pipeline_api_base}/pipelines/{pipeline_id}/runs'
+            payload = {"continuationId": continuation_id}
+            response = self._get(url, params=payload)
+            if response["runs"] is not None and len(response["runs"]) > 0:
+                return_run = response["runs"][0]
             else:
-                actual_version = supported_versions.maxVersion
-            ver_comparator = SimpleSpec(f'<={actual_version}')
-            if Version('2.5.0') in ver_comparator:
-                url = f'{self._pipeline_api_base}/pipelines/{pipeline_id}/runs'
-                payload = {"continuationId": continuation_id}
-                response = self._get(url, params=payload)
-                if response["runs"] is not None and len(response["runs"]) > 0:
-                    return_run = response["runs"][0]
-                else:
-                    raise TorchSdkException('No runs found against the given continuation_id.')
-            else:
-                # For torch versions lower than 2.5.0 use old call for continuation_id
-                if continuation_id.isdigit() is False:
-                    url = f'{self._pipeline_api_base}/pipelines/runs/{continuation_id}'
-                    response = self._get(url)
-                    return_run = response['run']
-                else:
-                    raise TorchSdkException('Please provide continuation_id which is not a valid number.')
+                raise TorchSdkException('No runs found against the given continuation_id.')
         else:
             raise TorchSdkException('Please provide either continuation_id and pipeline_id or pipeline_run_id')
 
         return_run['client'] = self
         return PipelineRun(**return_run)
 
     # get pipeline runs for a pipeline
@@ -756,19 +760,19 @@
 
             return sample_data_result
         else:
             return response
 
 
     def get_sample_data_result(self, request_id: str):
-            url = f'{self._catalog_api_base}/assets/sample/result/{request_id}'
-            response = self._get(
-                url=url
-            )
-            return response
+        url = f'{self._catalog_api_base}/assets/sample/result/{request_id}'
+        response = self._get(
+            url=url
+        )
+        return response
 
     def get_profile_request_details(self, asset_id: int, req_id: int):
         url = f'{self._catalog_api_base}/assets/{asset_id}/profile/{req_id}'
         response = self._get(
             url=url
         )
         return response
```

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk.egg-info/PKG-INFO` & `acceldata_sdk-3.4.0/acceldata_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_sdk
-Version: 3.3.0
+Version: 3.4.0
 Summary: Acceldata SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,15 +30,15 @@
 ```bash
 pip install acceldata-sdk
 ```
 
 ## Create Torch Client
 Torch client is used to send data to the torch servers. It consists of various methods to communicate with the torch server. Torch client have access to catalog and pipeline APIs. To create a torch client, torch url and API keys are required. To create torch API keys, go to torch ui’s settings and generate keys for the client.
 
-While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is enabled. If we want we can disable that check by passing `do_version_check` as `False.
+While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is disabled. If we want we can enable that check by passing `do_version_check` as `True`.
 
 
 ```python
 from acceldata_sdk.torch_client import TorchClient
 
 torch_client = TorchClient(url='https://acceldata.host.dev:9999', access_key='******',
                          secret_key='*****************', do_version_check=True)
@@ -519,11 +519,12 @@
 # List all rules
 recon_rules = torch_client.list_all_policies(filter=filter)
 ```
 
 Version Log
 ==========
 
-3.3.0 (15/04/2024)
+3.4.0 (08/05/2024)
 -------------------
-- Improved sample data api
+- Incorporated fix for control plane version compatibility check based apis to handle patch version
+- Disable version compatibility check by default
```

### Comparing `acceldata_sdk-3.3.0/acceldata_sdk.egg-info/SOURCES.txt` & `acceldata_sdk-3.4.0/acceldata_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.events.rst.txt` & `acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.events.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.models.rst.txt` & `acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.models.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.rst.txt` & `acceldata_sdk-3.4.0/docs/_build/html/_sources/torch_sdk.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/docs/conf.py` & `acceldata_sdk-3.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/integration_tests/test_constants.py` & `acceldata_sdk-3.4.0/integration_tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/integration_tests/test_ds_assets.py` & `acceldata_sdk-3.4.0/integration_tests/test_ds_assets.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/integration_tests/test_external_integration_default_time.py` & `acceldata_sdk-3.4.0/integration_tests/test_external_integration_default_time.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/integration_tests/test_external_integration_explicit_time.py` & `acceldata_sdk-3.4.0/integration_tests/test_external_integration_explicit_time.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/integration_tests/test_pipelines.py` & `acceldata_sdk-3.4.0/integration_tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/integration_tests/test_policy.py` & `acceldata_sdk-3.4.0/integration_tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/integration_tests/test_torch_client.py` & `acceldata_sdk-3.4.0/integration_tests/test_torch_client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.3.0/setup.py` & `acceldata_sdk-3.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # except (IOError, ImportError):
 #     description = open('README.md').read()
 
 # Change MIN_TORCH_BACKEND_VERSION_SUPPORTED in constants as well if needed while updating version here
 
 setup(
     name='acceldata_sdk',
-    version='3.3.0',
+    version='3.4.0',
     description='Acceldata SDK.' + '\n\n' + open('README.txt').read(),
     long_description=open('README.md').read() + '\n\n' + open('DATASOURCE_README.md').read() + '\n\n'  + open('CHANGELOG.txt').read(),
     long_description_content_type="text/markdown",
     url='',
     author='acceldata',
     author_email='apisupport@acceldata.io',
     license='MIT License',
```

