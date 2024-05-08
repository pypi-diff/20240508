# Comparing `tmp/acceldata_airflow_sdk-3.3.0.tar.gz` & `tmp/acceldata_airflow_sdk-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acceldata_airflow_sdk-3.3.0.tar", last modified: Mon Apr 15 09:08:25 2024, max compression
+gzip compressed data, was "acceldata_airflow_sdk-3.4.0.tar", last modified: Wed May  8 11:07:31 2024, max compression
```

## Comparing `acceldata_airflow_sdk-3.3.0.tar` & `acceldata_airflow_sdk-3.4.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.265374 acceldata_airflow_sdk-3.3.0/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      309 2024-04-15 09:06:32.000000 acceldata_airflow_sdk-3.3.0/CHANGELOG.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/LICENCE.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/MANIFEST.in
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23486 2024-04-15 09:08:25.264983 acceldata_airflow_sdk-3.3.0/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    22515 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/README.md
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/README.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.253032 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3065 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/dag.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.255233 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/decorators/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/decorators/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1100 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/decorators/handle_callback.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3935 2024-03-21 11:14:17.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/decorators/job.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4254 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/decorators/span.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1297 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/initialiser.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.256823 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/operators/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/operators/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4229 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/operators/execute_policy_operator.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     6446 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/operators/job_operator.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     6143 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/operators/span_operator.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     7017 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.257769 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/utils/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/utils/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2270 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/utils/callback.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3477 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/utils/constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3812 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/utils/torch_client.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.264390 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk.egg-info/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23486 2024-04-15 09:08:25.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2029 2024-04-15 09:08:25.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2024-04-15 09:08:25.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       82 2024-04-15 09:08:25.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk.egg-info/requires.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       22 2024-04-15 09:08:25.000000 acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.257957 acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2323 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/README.md
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.258272 acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/__init__.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.259442 acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/listener/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:28.000000 acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/listener/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      867 2024-02-22 04:32:28.000000 acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/listener/constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     5955 2024-03-28 09:04:23.000000 acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/listener/events_listener.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    18561 2024-03-28 09:04:23.000000 acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/listener/utils.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1215 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/listener_plugin.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.259965 acceldata_airflow_sdk-3.3.0/docs/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.249275 acceldata_airflow_sdk-3.3.0/docs/_build/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.249391 acceldata_airflow_sdk-3.3.0/docs/_build/html/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.261838 acceldata_airflow_sdk-3.3.0/docs/_build/html/_sources/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      492 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       96 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      858 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      720 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      707 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      623 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1950 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/docs/conf.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.262037 acceldata_airflow_sdk-3.3.0/openlineage/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1050 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/openlineage/airflow_local_settings.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.262241 acceldata_airflow_sdk-3.3.0/openlineage/config/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/openlineage/config/__init__.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.262996 acceldata_airflow_sdk-3.3.0/openlineage/extractors/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/openlineage/extractors/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3993 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/openlineage/extractors/bigquery_insert_job_extractor.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     6291 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/openlineage/extractors/gcs_bigquery_extractor.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.263513 acceldata_airflow_sdk-3.3.0/openlineage/policy/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/openlineage/policy/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4179 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/openlineage/policy/config_helper.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:08:25.264019 acceldata_airflow_sdk-3.3.0/openlineage/tokenproviders/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/openlineage/tokenproviders/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10427 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.3.0/openlineage/tokenproviders/access_key_secret_token_provider.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2024-04-15 09:08:25.265456 acceldata_airflow_sdk-3.3.0/setup.cfg
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      842 2024-04-15 09:06:32.000000 acceldata_airflow_sdk-3.3.0/setup.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.894420 acceldata_airflow_sdk-3.4.0/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      307 2024-05-08 11:01:16.000000 acceldata_airflow_sdk-3.4.0/CHANGELOG.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/LICENCE.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/MANIFEST.in
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23484 2024-05-08 11:07:31.894071 acceldata_airflow_sdk-3.4.0/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    22515 2024-05-08 11:01:16.000000 acceldata_airflow_sdk-3.4.0/README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/README.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.882429 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3065 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/dag.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.884568 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1100 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/handle_callback.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3935 2024-03-21 11:14:17.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/job.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4254 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/span.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1298 2024-05-08 11:01:16.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/initialiser.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.886524 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4229 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/execute_policy_operator.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6446 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/job_operator.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6143 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/span_operator.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     7017 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.887781 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2270 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/callback.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3477 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3812 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/torch_client.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.893601 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23484 2024-05-08 11:07:31.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2029 2024-05-08 11:07:31.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2024-05-08 11:07:31.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       82 2024-05-08 11:07:31.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/requires.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       22 2024-05-08 11:07:31.000000 acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.888012 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2323 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/README.md
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.888409 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/__init__.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.889415 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:28.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      867 2024-02-22 04:32:28.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     5955 2024-05-08 04:50:53.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/events_listener.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    18561 2024-05-08 04:50:53.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/utils.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1215 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener_plugin.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.889859 acceldata_airflow_sdk-3.4.0/docs/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.879725 acceldata_airflow_sdk-3.4.0/docs/_build/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.879796 acceldata_airflow_sdk-3.4.0/docs/_build/html/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.891320 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      492 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       96 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      858 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      720 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      707 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      623 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1950 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/docs/conf.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.891511 acceldata_airflow_sdk-3.4.0/openlineage/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1050 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/airflow_local_settings.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.891693 acceldata_airflow_sdk-3.4.0/openlineage/config/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/config/__init__.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.892305 acceldata_airflow_sdk-3.4.0/openlineage/extractors/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/extractors/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3993 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/extractors/bigquery_insert_job_extractor.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6291 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/extractors/gcs_bigquery_extractor.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.892750 acceldata_airflow_sdk-3.4.0/openlineage/policy/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/policy/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4179 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/policy/config_helper.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-05-08 11:07:31.893195 acceldata_airflow_sdk-3.4.0/openlineage/tokenproviders/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/tokenproviders/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10427 2024-02-22 04:32:27.000000 acceldata_airflow_sdk-3.4.0/openlineage/tokenproviders/access_key_secret_token_provider.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2024-05-08 11:07:31.894482 acceldata_airflow_sdk-3.4.0/setup.cfg
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      842 2024-05-08 11:01:16.000000 acceldata_airflow_sdk-3.4.0/setup.py
```

### Comparing `acceldata_airflow_sdk-3.3.0/LICENCE.txt` & `acceldata_airflow_sdk-3.4.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/PKG-INFO` & `acceldata_airflow_sdk-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_airflow_sdk
-Version: 3.3.0
+Version: 3.4.0
 Summary: Acceldata Airflow SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-airflow
 Classifier: Development Status :: 5 - Production/Stable
@@ -53,15 +53,15 @@
 ```
 
 
 Read more about acceldata-airflow-sdk from [here](https://pypi.org/project/acceldata-airflow-sdk/)
 
 ## Create TorchClient
 
-While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is enabled. If we want we can disable that check by passing `do_version_check` as `False
+While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is disabled. If we want we can Enable that check by passing `do_version_check` as `True`
 
 
 ```python
 from acceldata-sdk.torch_client import TorchClient
 torchClient = TorchClient(
     url="https://torch.acceldata.local:5443",
     access_key="OY2VVIN2N6LJ",
@@ -438,14 +438,14 @@
             print("Policy execution encountered an error.")
 
 ```
 
 Version Log
 ==========
 
-3.3.0 (15/04/2024)
+3.4.0 (08/05/2024)
 -------------------
 - Acceldata airflow sdk - Wrapper on apache airflow
-- Acceldata airflow sdk provides support for observability of airflow dags in torch catalog. With the use of acceldata airflow SDK, user can e2e observability on airflow dag run in torch UI.
+- Acceldata airflow sdk provides support for observability of airflow dags in ADOC catalog. With the use of acceldata airflow SDK, user can e2e observability on airflow dag run in ADOC UI.
```

### Comparing `acceldata_airflow_sdk-3.3.0/README.md` & `acceldata_airflow_sdk-3.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ```
 
 
 Read more about acceldata-airflow-sdk from [here](https://pypi.org/project/acceldata-airflow-sdk/)
 
 ## Create TorchClient
 
-While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is enabled. If we want we can disable that check by passing `do_version_check` as `False
+While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is disabled. If we want we can Enable that check by passing `do_version_check` as `True`
 
 
 ```python
 from acceldata-sdk.torch_client import TorchClient
 torchClient = TorchClient(
     url="https://torch.acceldata.local:5443",
     access_key="OY2VVIN2N6LJ",
```

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/dag.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/dag.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/decorators/handle_callback.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/handle_callback.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/decorators/job.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/job.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/decorators/span.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/decorators/span.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/initialiser.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/initialiser.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 # setup these 4 env vars in your airflow environment. You can create api keys from torch ui's setting page.
 def torch_credentials(conn_id=None):
     if conn_id is None:
         creds = {
             'url': os.getenv('TORCH_CATALOG_URL', 'https://torch.acceldata.local:5443'),
             'access_key': os.getenv('TORCH_ACCESS_KEY', 'OY2VVIN2N6LJ'),
             'secret_key': os.getenv('TORCH_SECRET_KEY', 'da6bDBimQfXSMsyyhlPVJJfk7Zc2gs'),
-            'do_version_check': os.getenv('ENABLE_VERSION_CHECK', True)
+            'do_version_check': os.getenv('ENABLE_VERSION_CHECK', False)
         }
     else:
         creds = Credentials(conn_id).__dict__
     return creds
```

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/operators/execute_policy_operator.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/execute_policy_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/operators/job_operator.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/job_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/operators/span_operator.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/span_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/operators/torch_initialiser_operator.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/utils/callback.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/callback.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/utils/constants.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk/utils/torch_client.py` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk/utils/torch_client.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk.egg-info/PKG-INFO` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_airflow_sdk
-Version: 3.3.0
+Version: 3.4.0
 Summary: Acceldata Airflow SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-airflow
 Classifier: Development Status :: 5 - Production/Stable
@@ -53,15 +53,15 @@
 ```
 
 
 Read more about acceldata-airflow-sdk from [here](https://pypi.org/project/acceldata-airflow-sdk/)
 
 ## Create TorchClient
 
-While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is enabled. If we want we can disable that check by passing `do_version_check` as `False
+While creating a TorchClient connection to torch by default version compatibility checks between torch and sdk is disabled. If we want we can Enable that check by passing `do_version_check` as `True`
 
 
 ```python
 from acceldata-sdk.torch_client import TorchClient
 torchClient = TorchClient(
     url="https://torch.acceldata.local:5443",
     access_key="OY2VVIN2N6LJ",
@@ -438,14 +438,14 @@
             print("Policy execution encountered an error.")
 
 ```
 
 Version Log
 ==========
 
-3.3.0 (15/04/2024)
+3.4.0 (08/05/2024)
 -------------------
 - Acceldata airflow sdk - Wrapper on apache airflow
-- Acceldata airflow sdk provides support for observability of airflow dags in torch catalog. With the use of acceldata airflow SDK, user can e2e observability on airflow dag run in torch UI.
+- Acceldata airflow sdk provides support for observability of airflow dags in ADOC catalog. With the use of acceldata airflow SDK, user can e2e observability on airflow dag run in ADOC UI.
```

### Comparing `acceldata_airflow_sdk-3.3.0/acceldata_airflow_sdk.egg-info/SOURCES.txt` & `acceldata_airflow_sdk-3.4.0/acceldata_airflow_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/README.md` & `acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/README.md`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/listener/constants.py` & `acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/listener/events_listener.py` & `acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/events_listener.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/listener/utils.py` & `acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener/utils.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/adoc_listener_plugin/plugins/listener_plugin.py` & `acceldata_airflow_sdk-3.4.0/adoc_listener_plugin/plugins/listener_plugin.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt` & `acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.decorators.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt` & `acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.operators.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt` & `acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt` & `acceldata_airflow_sdk-3.4.0/docs/_build/html/_sources/torch_airflow_sdk.utils.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/docs/conf.py` & `acceldata_airflow_sdk-3.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/openlineage/airflow_local_settings.py` & `acceldata_airflow_sdk-3.4.0/openlineage/airflow_local_settings.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/openlineage/extractors/bigquery_insert_job_extractor.py` & `acceldata_airflow_sdk-3.4.0/openlineage/extractors/bigquery_insert_job_extractor.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/openlineage/extractors/gcs_bigquery_extractor.py` & `acceldata_airflow_sdk-3.4.0/openlineage/extractors/gcs_bigquery_extractor.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/openlineage/policy/config_helper.py` & `acceldata_airflow_sdk-3.4.0/openlineage/policy/config_helper.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/openlineage/tokenproviders/access_key_secret_token_provider.py` & `acceldata_airflow_sdk-3.4.0/openlineage/tokenproviders/access_key_secret_token_provider.py`

 * *Files identical despite different names*

### Comparing `acceldata_airflow_sdk-3.3.0/setup.py` & `acceldata_airflow_sdk-3.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: Apache Software License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='acceldata_airflow_sdk',
-  version='3.3.0',
+  version='3.4.0',
   description='Acceldata Airflow SDK.' + '\n\n' + open('README.txt').read(),
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type="text/markdown",
   url='',
   author='acceldata',
   author_email='apisupport@acceldata.io',
   license='MIT License',
```

