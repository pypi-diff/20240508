# Comparing `tmp/pipeline_telemetry-1.0.0.tar.gz` & `tmp/pipeline_telemetry-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_telemetry-1.0.0.tar", last modified: Wed May  8 13:22:19 2024, max compression
+gzip compressed data, was "pipeline_telemetry-1.0.1.tar", last modified: Wed May  8 14:08:46 2024, max compression
```

## Comparing `pipeline_telemetry-1.0.0.tar` & `pipeline_telemetry-1.0.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    43679 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.115273 pipeline_telemetry-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/adding telemetry.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/decorators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/process_type.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.115273 pipeline_telemetry-1.0.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/reference/pipeline_telemetry.rst
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/storage class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/telemetry aggregation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/telemetry counters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/telemetry mixin.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/telemetry object.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-08 13:22:19.131273 pipeline_telemetry-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.111273 pipeline_telemetry-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.115273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.119273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/mongo_aggregator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.119273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/data_classes/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/data_classes/telemetry_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14116 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.119273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/data_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/date_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/process_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/telemetry_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.119273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/mongo_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.123273 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/abstract_validator_instruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/entries_have_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/has_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/validate_entries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-08 13:22:19.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-08 13:22:19.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:22:19.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 13:22:19.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 13:22:19.000000 pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.123273 pipeline_telemetry-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_add_telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.123273 pipeline_telemetry-1.0.0/tests/test_aggregator/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_aggregator_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_daily_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_mongo_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_aggregator/test_partial_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_integration/test_int_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_integration/test_integration_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_process_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/tests/test_settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_settings/test_date_time_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_settings/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_settings_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/tests/test_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_storage/test_mongo_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_storage/test_sqllite_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_storage/test_storage_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_telemetry_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_telemetry_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/tests/test_telemetry_models/
--rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:19.127273 pipeline_telemetry-1.0.0/tests/test_validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_validators/test_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_validators/test_entries_have_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_validators/test_has_key_instruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-08 13:22:15.000000 pipeline_telemetry-1.0.0/tests/test_validators/test_validate_entries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.035305 pipeline_telemetry-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    43679 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-08 14:08:46.035305 pipeline_telemetry-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.019305 pipeline_telemetry-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/adding telemetry.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/process_type.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.019305 pipeline_telemetry-1.0.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/reference/pipeline_telemetry.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/storage class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/telemetry aggregation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/telemetry counters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/telemetry mixin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/telemetry object.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-08 14:08:46.035305 pipeline_telemetry-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.015305 pipeline_telemetry-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.023305 pipeline_telemetry-1.0.1/src/pipeline_telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.023305 pipeline_telemetry-1.0.1/src/pipeline_telemetry/aggregator/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/aggregator/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/aggregator/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/aggregator/mongo_aggregator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.023305 pipeline_telemetry-1.0.1/src/pipeline_telemetry/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/data_classes/telemetry_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14116 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.027305 pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/data_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/date_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/process_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/telemetry_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.027305 pipeline_telemetry-1.0.1/src/pipeline_telemetry/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/storage/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/storage/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/storage/mongo_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.027305 pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/abstract_validator_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/entries_have_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/has_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/validate_entries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.035305 pipeline_telemetry-1.0.1/src/pipeline_telemetry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-08 14:08:45.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-08 14:08:46.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:08:45.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 14:08:45.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 14:08:45.000000 pipeline_telemetry-1.0.1/src/pipeline_telemetry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.027305 pipeline_telemetry-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_add_telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.031305 pipeline_telemetry-1.0.1/tests/test_aggregator/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_aggregator/test_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_aggregator/test_aggregator_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_aggregator/test_daily_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_aggregator/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_aggregator/test_mongo_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_aggregator/test_partial_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.031305 pipeline_telemetry-1.0.1/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_integration/test_int_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_integration/test_integration_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_process_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.031305 pipeline_telemetry-1.0.1/tests/test_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_settings/test_date_time_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_settings/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_settings_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.031305 pipeline_telemetry-1.0.1/tests/test_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_storage/test_mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_storage/test_sqllite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_storage/test_storage_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_telemetry_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_telemetry_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.031305 pipeline_telemetry-1.0.1/tests/test_telemetry_models/
+-rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_telemetry_models/test_telemetry_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_telemetry_models/test_telemetry_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_telemetry_models/test_telemetry_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:46.031305 pipeline_telemetry-1.0.1/tests/test_validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_validators/test_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_validators/test_entries_have_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_validators/test_has_key_instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-08 14:08:42.000000 pipeline_telemetry-1.0.1/tests/test_validators/test_validate_entries.py
```

### Comparing `pipeline_telemetry-1.0.0/CHANGELOG.rst` & `pipeline_telemetry-1.0.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/CONTRIBUTING.rst` & `pipeline_telemetry-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/LICENSE` & `pipeline_telemetry-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/PKG-INFO` & `pipeline_telemetry-1.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-telemetry
-Version: 1.0.0
+Version: 1.0.1
 Summary: Measure your data pipelines with easy to use telemetry logic
 Home-page: https://github.com/MaartendeRuyter/pipeline-telemetry
 Author: Maarten de Ruyter
 Author-email: "Maarten de Ruyter" <maarten@geodatagarden.com>
 License: GNU
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Intended Audience :: Developers
@@ -16,119 +16,47 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: error-manager
 Requires-Dist: mongoengine
 Requires-Dist: jmespath
 
-========
-Overview
-========
+# Pipeline Telemetry
 
-.. start-badges
+**Pipeline Telemetry** makes it easy for project to generate store telemetry data from within your data pipelines.
 
-.. list-table::
-    :stub-columns: 1
+```python
 
-    * - docs
-      - |docs|
-    * - tests
-      - | |travis| |requires|
-        | |codecov|
-    * - package
-      - | |version| |wheel|
-        | |supported-versions|
-        | |supported-implementations|
-        | |commits-since|
-.. |docs| image:: https://readthedocs.org/projects/pipeline-telemetry/badge/?style=flat
-    :target: https://pipeline-telemetry.readthedocs.io/
-    :alt: Documentation Status
+    from counters import INVALID_DATA, PROCESSED_DATA_POINTS
 
-.. |travis| image:: https://api.travis-ci.com/MaartendeRuyter/pipeline-telemetry.svg?branch=master
-    :alt: Travis-CI Build Status
-    :target: https://travis-ci.com/github/MaartendeRuyter/pipeline-telemetry
 
-.. |requires| image:: https://requires.io/github/MaartendeRuyter/pipeline-telemetry/requirements.svg?branch=master
-    :alt: Requirements Status
-    :target: https://requires.io/github/MaartendeRuyter/pipeline-telemetry/requirements/?branch=master
+    def my_data_pipeline():
+        telemetry = Telemetry(**TELEMETRY_PARAMS)
 
-.. |codecov| image:: https://codecov.io/gh/MaartendeRuyter/pipeline-telemetry/branch/master/graphs/badge.svg?branch=master
-    :alt: Coverage Status
-    :target: https://codecov.io/github/MaartendeRuyter/pipeline-telemetry
+        from url in data_urls:
+            data = get_data_from_url(url)
+            telemetry.add_telemetry_counter(telemetry_counter=URL_RETRIEVALS)    # increase counter for retrieved URLS
+            if data.invalid:
+                telemetry.add_telemetry_counter(telemetry_counter=INVALID_DATA)  # increase counter for failed retrievals
+                continue
+            
+            processed_data_points = process_and_store_data(data)
+            telemetry.add_telemetry_counter(                                     # increase counter number of datapoints retrieved
+                telemetry_counter=PROCESSED_DATA_POINTS,
+                increment=len(processed_data_points))  
+        
+        telemetry.save_and_close()
+```
 
-.. |version| image:: https://img.shields.io/pypi/v/pipeline-telemetry.svg
-    :alt: PyPI Package latest release
-    :target: https://pypi.org/project/pipeline-telemetry
+In this example data is retrieved for a list of urls. Total retrievals, insuccesfull retrievals as well as number of processed datapoints are stored in the telemetry object.
+This allows you to closely monitor the quality and behavior of your datapipeline. For example all retrievals might be OK but if the number of processed datapoints suddenly drops there might be an issue with some the endpoints.
 
-.. |wheel| image:: https://img.shields.io/pypi/wheel/pipeline-telemetry.svg
-    :alt: PyPI Wheel
-    :target: https://pypi.org/project/pipeline-telemetry
 
-.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pipeline-telemetry.svg
-    :alt: Supported versions
-    :target: https://pypi.org/project/pipeline-telemetry
 
-.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pipeline-telemetry.svg
-    :alt: Supported implementations
-    :target: https://pypi.org/project/pipeline-telemetry
-
-.. |commits-since| image:: https://img.shields.io/github/commits-since/MaartendeRuyter/pipeline-telemetry/v0.0.1.svg
-    :alt: Commits since latest release
-    :target: https://github.com/MaartendeRuyter/pipeline-telemetry/compare/v0.0.1...master
-
-
-
-.. end-badges
-
-Create and store data pipeline telemetry data
-
-* Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
-
-Installing pipeline-telemetry
-=============================
-
-::
-
-    pip install pipeline-telemetry
-
-You can also install the in-development version with::
-
-    pip install https://github.com/MaartendeRuyter/pipeline-telemetry/archive/master.zip
-
-
-Documentation
-=============
-
-
-https://pipeline-telemetry.readthedocs.io/
-
-
-Testing
-=======
-
-To run all the tests run::
-
-    tox
-
-Note, to combine the coverage data from all the tox environments run:
-
-.. list-table::
-    :widths: 10 90
-    :stub-columns: 1
-
-    - - Windows
-      - ::
-
-            set PYTEST_ADDOPTS=--cov-append
-            tox
-
-    - - Other
-      - ::
-
-            PYTEST_ADDOPTS=--cov-append tox
+[![Supported Versions](https://img.shields.io/pypi/pyversions/pipeline-telemetry.svg)](https://pypi.org/project/pipeline-telemetry)
 
 
 Changelog
 =========
 1.0.0 (2024-05-08)
 -------------------
 * Added python 3.12 support
```

### Comparing `pipeline_telemetry-1.0.0/README.rst` & `pipeline_telemetry-1.0.1/docs/readme.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 .. list-table::
     :stub-columns: 1
 
     * - docs
       - |docs|
     * - tests
-      - | |travis| |requires|
-        | |codecov|
+      - |codecov|
     * - package
       - | |version| |wheel|
         | |supported-versions|
         | |supported-implementations|
         | |commits-since|
 .. |docs| image:: https://readthedocs.org/projects/pipeline-telemetry/badge/?style=flat
     :target: https://pipeline-telemetry.readthedocs.io/
@@ -50,15 +49,14 @@
     :target: https://pypi.org/project/pipeline-telemetry
 
 .. |commits-since| image:: https://img.shields.io/github/commits-since/MaartendeRuyter/pipeline-telemetry/v0.0.1.svg
     :alt: Commits since latest release
     :target: https://github.com/MaartendeRuyter/pipeline-telemetry/compare/v0.0.1...master
 
 
-
 .. end-badges
 
 Create and store data pipeline telemetry data
 
 * Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
 
 Installing pipeline-telemetry
@@ -99,7 +97,8 @@
             set PYTEST_ADDOPTS=--cov-append
             tox
 
     - - Other
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
+
```

### Comparing `pipeline_telemetry-1.0.0/docs/adding telemetry.rst` & `pipeline_telemetry-1.0.1/docs/adding telemetry.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/docs/conf.py` & `pipeline_telemetry-1.0.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "Pipeline Telemetry"
 year = "2024"
 author = "Maarten de Ruyter"
 copyright = "{0}, {1}".format(year, author)
-version = release = "1.0.0"
+version = release = "1.0.1"
 
 extensions = []
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 html_theme = "sphinx_rtd_theme"
```

### Comparing `pipeline_telemetry-1.0.0/docs/decorators.rst` & `pipeline_telemetry-1.0.1/docs/decorators.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/docs/process_type.rst` & `pipeline_telemetry-1.0.1/docs/process_type.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/docs/telemetry aggregation.rst` & `pipeline_telemetry-1.0.1/docs/telemetry aggregation.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/docs/telemetry counters.rst` & `pipeline_telemetry-1.0.1/docs/telemetry counters.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/docs/telemetry mixin.rst` & `pipeline_telemetry-1.0.1/docs/telemetry mixin.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/docs/telemetry object.rst` & `pipeline_telemetry-1.0.1/docs/telemetry object.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/docs/usage.rst` & `pipeline_telemetry-1.0.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/setup.cfg` & `pipeline_telemetry-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pipeline-telemetry
-version = 1.0.0
+version = 1.0.1
 description = Measure your data pipelines with easy to use telemetry logic
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/markdown
 url = https://github.com/MaartendeRuyter/pipeline-telemetry
 author = Maarten de Ruyter
 author_email = "Maarten de Ruyter" <maarten@geodatagarden.com>
 license = GNU
```

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/__init__.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/aggregator.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/helper.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/aggregator/helper.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/aggregator/mongo_aggregator.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/aggregator/mongo_aggregator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/data_classes/telemetry_models.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/data_classes/telemetry_models.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/decorator.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/decorator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/helper.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/helper.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/main.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/main.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/mixin.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/mixin.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/__init__.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/data_class.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/data_class.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/date_ranges.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/date_ranges.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/exceptions.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/process_type.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/process_type.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/settings.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/settings.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/settings/telemetry_errors.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/settings/telemetry_errors.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/generic.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/storage/generic.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/memory.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/storage/memory.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/mongo.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/storage/mongo_connection.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/storage/mongo_connection.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/abstract_validator_instruction.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/abstract_validator_instruction.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/dict_validator.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/dict_validator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/entries_have_key.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/entries_have_key.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/has_key.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/has_key.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry/validators/validate_entries.py` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry/validators/validate_entries.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/PKG-INFO` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-telemetry
-Version: 1.0.0
+Version: 1.0.1
 Summary: Measure your data pipelines with easy to use telemetry logic
 Home-page: https://github.com/MaartendeRuyter/pipeline-telemetry
 Author: Maarten de Ruyter
 Author-email: "Maarten de Ruyter" <maarten@geodatagarden.com>
 License: GNU
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Intended Audience :: Developers
@@ -16,119 +16,47 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: error-manager
 Requires-Dist: mongoengine
 Requires-Dist: jmespath
 
-========
-Overview
-========
+# Pipeline Telemetry
 
-.. start-badges
+**Pipeline Telemetry** makes it easy for project to generate store telemetry data from within your data pipelines.
 
-.. list-table::
-    :stub-columns: 1
+```python
 
-    * - docs
-      - |docs|
-    * - tests
-      - | |travis| |requires|
-        | |codecov|
-    * - package
-      - | |version| |wheel|
-        | |supported-versions|
-        | |supported-implementations|
-        | |commits-since|
-.. |docs| image:: https://readthedocs.org/projects/pipeline-telemetry/badge/?style=flat
-    :target: https://pipeline-telemetry.readthedocs.io/
-    :alt: Documentation Status
+    from counters import INVALID_DATA, PROCESSED_DATA_POINTS
 
-.. |travis| image:: https://api.travis-ci.com/MaartendeRuyter/pipeline-telemetry.svg?branch=master
-    :alt: Travis-CI Build Status
-    :target: https://travis-ci.com/github/MaartendeRuyter/pipeline-telemetry
 
-.. |requires| image:: https://requires.io/github/MaartendeRuyter/pipeline-telemetry/requirements.svg?branch=master
-    :alt: Requirements Status
-    :target: https://requires.io/github/MaartendeRuyter/pipeline-telemetry/requirements/?branch=master
+    def my_data_pipeline():
+        telemetry = Telemetry(**TELEMETRY_PARAMS)
 
-.. |codecov| image:: https://codecov.io/gh/MaartendeRuyter/pipeline-telemetry/branch/master/graphs/badge.svg?branch=master
-    :alt: Coverage Status
-    :target: https://codecov.io/github/MaartendeRuyter/pipeline-telemetry
+        from url in data_urls:
+            data = get_data_from_url(url)
+            telemetry.add_telemetry_counter(telemetry_counter=URL_RETRIEVALS)    # increase counter for retrieved URLS
+            if data.invalid:
+                telemetry.add_telemetry_counter(telemetry_counter=INVALID_DATA)  # increase counter for failed retrievals
+                continue
+            
+            processed_data_points = process_and_store_data(data)
+            telemetry.add_telemetry_counter(                                     # increase counter number of datapoints retrieved
+                telemetry_counter=PROCESSED_DATA_POINTS,
+                increment=len(processed_data_points))  
+        
+        telemetry.save_and_close()
+```
 
-.. |version| image:: https://img.shields.io/pypi/v/pipeline-telemetry.svg
-    :alt: PyPI Package latest release
-    :target: https://pypi.org/project/pipeline-telemetry
+In this example data is retrieved for a list of urls. Total retrievals, insuccesfull retrievals as well as number of processed datapoints are stored in the telemetry object.
+This allows you to closely monitor the quality and behavior of your datapipeline. For example all retrievals might be OK but if the number of processed datapoints suddenly drops there might be an issue with some the endpoints.
 
-.. |wheel| image:: https://img.shields.io/pypi/wheel/pipeline-telemetry.svg
-    :alt: PyPI Wheel
-    :target: https://pypi.org/project/pipeline-telemetry
 
-.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pipeline-telemetry.svg
-    :alt: Supported versions
-    :target: https://pypi.org/project/pipeline-telemetry
 
-.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pipeline-telemetry.svg
-    :alt: Supported implementations
-    :target: https://pypi.org/project/pipeline-telemetry
-
-.. |commits-since| image:: https://img.shields.io/github/commits-since/MaartendeRuyter/pipeline-telemetry/v0.0.1.svg
-    :alt: Commits since latest release
-    :target: https://github.com/MaartendeRuyter/pipeline-telemetry/compare/v0.0.1...master
-
-
-
-.. end-badges
-
-Create and store data pipeline telemetry data
-
-* Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
-
-Installing pipeline-telemetry
-=============================
-
-::
-
-    pip install pipeline-telemetry
-
-You can also install the in-development version with::
-
-    pip install https://github.com/MaartendeRuyter/pipeline-telemetry/archive/master.zip
-
-
-Documentation
-=============
-
-
-https://pipeline-telemetry.readthedocs.io/
-
-
-Testing
-=======
-
-To run all the tests run::
-
-    tox
-
-Note, to combine the coverage data from all the tox environments run:
-
-.. list-table::
-    :widths: 10 90
-    :stub-columns: 1
-
-    - - Windows
-      - ::
-
-            set PYTEST_ADDOPTS=--cov-append
-            tox
-
-    - - Other
-      - ::
-
-            PYTEST_ADDOPTS=--cov-append tox
+[![Supported Versions](https://img.shields.io/pypi/pyversions/pipeline-telemetry.svg)](https://pypi.org/project/pipeline-telemetry)
 
 
 Changelog
 =========
 1.0.0 (2024-05-08)
 -------------------
 * Added python 3.12 support
```

### Comparing `pipeline_telemetry-1.0.0/src/pipeline_telemetry.egg-info/SOURCES.txt` & `pipeline_telemetry-1.0.1/src/pipeline_telemetry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_add_telemetry.py` & `pipeline_telemetry-1.0.1/tests/test_add_telemetry.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_aggregator/test_aggregator.py` & `pipeline_telemetry-1.0.1/tests/test_aggregator/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_aggregator/test_aggregator_data.py` & `pipeline_telemetry-1.0.1/tests/test_aggregator/test_aggregator_data.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_aggregator/test_daily_aggregator.py` & `pipeline_telemetry-1.0.1/tests/test_aggregator/test_daily_aggregator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_aggregator/test_helper.py` & `pipeline_telemetry-1.0.1/tests/test_aggregator/test_helper.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_aggregator/test_mongo_aggregator.py` & `pipeline_telemetry-1.0.1/tests/test_aggregator/test_mongo_aggregator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_aggregator/test_partial_aggregator.py` & `pipeline_telemetry-1.0.1/tests/test_aggregator/test_partial_aggregator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_data.py` & `pipeline_telemetry-1.0.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_decorator.py` & `pipeline_telemetry-1.0.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_helpers.py` & `pipeline_telemetry-1.0.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_integration/test_int_telemetry.py` & `pipeline_telemetry-1.0.1/tests/test_integration/test_int_telemetry.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_integration/test_integration_data.py` & `pipeline_telemetry-1.0.1/tests/test_integration/test_integration_data.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_mixin.py` & `pipeline_telemetry-1.0.1/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_process_types.py` & `pipeline_telemetry-1.0.1/tests/test_process_types.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_settings/test_date_time_ranges.py` & `pipeline_telemetry-1.0.1/tests/test_settings/test_date_time_ranges.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_settings/test_exceptions.py` & `pipeline_telemetry-1.0.1/tests/test_settings/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_storage/test_mongo_storage.py` & `pipeline_telemetry-1.0.1/tests/test_storage/test_mongo_storage.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_storage/test_sqllite_storage.py` & `pipeline_telemetry-1.0.1/tests/test_storage/test_sqllite_storage.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_telemetry_class_methods.py` & `pipeline_telemetry-1.0.1/tests/test_telemetry_class_methods.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_telemetry_counter.py` & `pipeline_telemetry-1.0.1/tests/test_telemetry_counter.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_class.py` & `pipeline_telemetry-1.0.1/tests/test_telemetry_models/test_telemetry_class.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_data.py` & `pipeline_telemetry-1.0.1/tests/test_telemetry_models/test_telemetry_data.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_telemetry_models/test_telemetry_model.py` & `pipeline_telemetry-1.0.1/tests/test_telemetry_models/test_telemetry_model.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_validators/test_dict_validator.py` & `pipeline_telemetry-1.0.1/tests/test_validators/test_dict_validator.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_validators/test_entries_have_key.py` & `pipeline_telemetry-1.0.1/tests/test_validators/test_entries_have_key.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_validators/test_has_key_instruction.py` & `pipeline_telemetry-1.0.1/tests/test_validators/test_has_key_instruction.py`

 * *Files identical despite different names*

### Comparing `pipeline_telemetry-1.0.0/tests/test_validators/test_validate_entries.py` & `pipeline_telemetry-1.0.1/tests/test_validators/test_validate_entries.py`

 * *Files identical despite different names*

